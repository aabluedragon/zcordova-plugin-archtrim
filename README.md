# zcordova-plugin-archtrim

The plugin helps solve app submission validation errors such as:
> ERROR ITMS-90087: "Unsupported Architectures. The executable for YourApp.app/Frameworks/SomeThing.framework contains unsupported architectures '[x86_64, i386]'."

It adds a hook that adds a "Run Script" build phase to your Xcode project.
The run script is credited to Daniel Kennet and can be found in http://ikennd.ac/blog/2015/02/stripping-unwanted-architectures-from-dynamic-libraries-in-xcode

The plugin name starts with the 'z' character intentionally, to have it's hook run last during 'after_platform_add'.
