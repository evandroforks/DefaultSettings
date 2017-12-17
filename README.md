
# Default Settings


What is does?

It does nothing, except require the dependency `0_settings_loader`.
<br>


What it is necessary?

Because the standard `Package Control` is uninstalling the `0_settings_loader` if it is required
by the default `Package`.
<br>


Why it is uninstalling?

Because when Sublime Text starts,
`Package Control` runs a called `Package Clean Up` which uninstalls all dependencies which are not
required by the installed packages, except the default packages and the installed dependencies.

Therefore,
if a dependency or a default package, requires dependencies,
its dependencies are going to be uninstalled as soon as package control starts up.

