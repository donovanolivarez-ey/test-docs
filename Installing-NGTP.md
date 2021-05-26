# Setting up NGTP
## Understanding the NGTP layout
As mentioned earlier, Next Gen Testing Platform is a modular test harness: it needs the following to function:
* Atleast 1 core library (etaf-core-library, etl-core-libraries etc)
* The corresponding step-definitions library (etaf-step-definitions, etl-step-definitions etc)
* And the cherry-on-top, the actual test automation framework which in itself is essentially a shell which needs its above libraries to be fully-functional. There are different libraries for doing different things with this framework. Namely,
- etaf-step-definitions: Provides all the reusable steps needed for functional, UI and system testing of web applications
  - etaf-core-libraries: Provides the capabilities required by etaf-step-definitions to enable Web app testing
- etl-step-definitions: Provides all the reusable steps needed for data and ETL testing
  - etl-core-libraries: Provides the capabilities required by etl-step-definitions to enable data and ETL testing

and many more. Please refer the [wiki](List-of-NGTP-libraries) links for other such component libraries.

To configure your project to consume these libraries you need to add either the library dependencies to your pom.xml and cofiguring your maven settings.xml or, their library jars directly to your project and adding it to your pom.xml. This is what will be covered in the next sections.

But once completed your pom.xml will essentially contain these

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque imperdiet a enim vel semper. Mauris at justo a magna mattis ultricies sed sit amet tortor. Nulla facilisi. Donec ac ipsum a ante tincidunt semper at id risus. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Quisque luctus rutrum sem eget euismod. In placerat facilisis enim eu fermentum. Praesent cursus bibendum nunc, non tristique massa suscipit et. Nullam nunc elit, sagittis tincidunt pretium eu, molestie nec augue. Duis nec risus sed nulla lobortis viverra sed non magna. Donec finibus tortor sed efficitur luctus. Nullam aliquam venenatis sapien, nec vulputate ipsum aliquet et. Quisque sit amet nulla a purus mattis vehicula.

Interdum et malesuada fames ac ante ipsum primis in faucibus. Vivamus posuere vitae lectus at elementum. Fusce et diam justo. Maecenas sem massa, condimentum non dui eu, aliquet pulvinar purus. Duis sagittis, est a lacinia vulputate, lacus risus porttitor ex, ut fermentum eros enim a leo. Curabitur sagittis urna vitae nunc dapibus, semper efficitur libero congue. In pretium eleifend neque, a viverra velit eleifend a. Fusce dapibus volutpat magna, pharetra ultrices sem rhoncus quis. Aliquam erat volutpat. Curabitur id leo nulla. Sed pulvinar bibendum nulla ac tristique. Duis lobortis, felis vel facilisis egestas, tellus ligula finibus ex, vel sodales diam sem sit amet dui.

Mauris imperdiet justo ligula, vitae tempor risus viverra eget. Morbi tempus auctor arcu in finibus. Aliquam dignissim in dolor id laoreet. Nam fringilla dictum tellus. Cras non ornare massa, pharetra ultricies massa. Interdum et malesuada fames ac ante ipsum primis in faucibus. Vestibulum varius in risus sit amet scelerisque. Quisque eleifend sit amet leo at euismod. Proin mollis est fringilla sem imperdiet egestas. Sed aliquam id arcu vel pretium. Proin non hendrerit lacus. Nulla egestas enim quam, eget lacinia dui sagittis ut. Integer et lorem vel sapien ultrices convallis.

In placerat velit sed faucibus pulvinar. Ut hendrerit elit ut iaculis rhoncus. Pellentesque varius id diam nec congue. Donec eu gravida quam, sed eleifend mauris. Vivamus sed nibh lorem. Suspendisse sollicitudin lectus eu accumsan euismod. Aliquam et sollicitudin odio, a blandit metus.

***
