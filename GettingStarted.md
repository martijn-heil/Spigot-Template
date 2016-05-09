1. You should define a Intellij path variable called `SPIGOT_DEVSERVER` and set it's value to the server root of your
Spigot development server.
You can configure Intellij IDEA path variables at `File > Settings > Appearance & Behaviour > Path Variables`

2. Your server jar should be called `spigot.jar`

3. You should use the default directory structure for the Spigot server.

4. You should define a profile in your maven `settings.xml` like this:

```
<profiles>
    ...
    <profile>
        <id>spigotdev</id>
        <properties>
            <spigot-devserver-root>/path/to/spigot/devserver/root</spigot-devserver-root>
        </properties>
    </profile>
    ...
</profiles>
```
And make sure it is active,
```
<activeProfiles>
    ...
    <activeProfile>spigotdev</activeProfile>
    ...
</activeProfiles>
```