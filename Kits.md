
##TACO Kits

Your Apache Cordova apps rely heavily on platforms and plugins in order to function properly. In a perfect world, migrating to a new version of Cordova should be easy. Everything that worked in your app before the upgrade still works. The hope is that everything now works a little bit better and maybe even a little bit faster. Unfortunately, things don’t always work out that nicely in reality. Getting the right versions of plugins and platforms is often a delicate balancing act. Plugins and platforms that work in one version of Cordova may not work properly in another. Because of this complexity, many of you have told us that you would prefer sticking with your current version of Cordova – even if a newer and better version exists.

We don’t have a perfect solution for this just yet. We have our best people working on it! In the interim, what we do have is something known as **Kits**. A Kit is a validated combination of platforms, build tools, and plug-ins that give you a working snapshot of everything for a particular Cordova version:

![TACO Kits in action!](https://raw.githubusercontent.com/Microsoft/TACO-Site-Private/master/src/assets/images/docs/tacokit.PNG?token=AEBP_F02HKD8b514FN27UCH8oMdqM-I_ks5V8hbEwA==)

Think of a Kit as a safety blanket. With Kits, you don’t have to go through the mess of download stats, star ratings and open issues to know which components are both stable and compatible with your app. We've taken care of figuring that out for you.

By default, projects you create with TACO are based on a Kit tied to Cordova 5.1.1. You can inspect the version of the components that make up this Kit, move to a new Kit, or choose to bypass Kits altogether and just work with a CLI version directly. To access all of the functionality Kits bring to the table, simply type **taco kit help**.

##Common Kit Operations
The following are some examples of operations you may perform with Kits:

   * List the validated set of Cordova CLI, platforms and plugins for tacokit@2.0.0

        <pre><code>
        taco kit list --kit tacokit@2.0.0
        </pre></code>

   * Update the current project to a Kit project targeting tacokit@2.0.0

        <pre><code>
        taco kit select --kit tacokit@2.0.0
        </pre></code>

   * Update the current project to a CLI project targeting Cordova CLI v5.2.0

        <pre><code>
        taco kit select --cli 5.2.0
        </pre></code>

