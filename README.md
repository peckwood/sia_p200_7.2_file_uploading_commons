### File Uploading using <u>Commons</u>MultipartResolver, configured with <u>AbstractAnnotationConfigDispatcherServletInitializer</u>

#### Significant configuration files:

- ~~spittr.config.SpittrWebAppInitializer~~
- spittr.config.WebConfig
  - sets the location of temp upload folder to *D:/d/data/temp/upload*
  - registers multipartResolver bean

#### Other significant files

- <u>pom.xml</u> (added dependency for commons-fileupload)
- /main/webapp/WEB-INF/views/registerForm.jsp
  - form enctype attribute
  - file input
- spittr.web.FileUploadController

This project only works on Servlet 3.0 supported servers because I didn't not use web.xml configuration, but it can support Servlet 2.5 if we use web.xml configuration, it can start based on the project `sia_p197_7.1.3_declaring_DispatcherServlet_in_servlet2.5_web.xml`.