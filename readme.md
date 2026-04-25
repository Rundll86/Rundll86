# The world

slogan: **Hello Internet!!!**

There is FallingShrimp.

- I'm a senior high school student.
- I'm a **full stack web app** & **2D game** developer.

## Languages

```plain
· TypeScript/JavaScript - Frontend/Backend
· Rust/C#               - Game develop (Unity & Godot.NET & WebAssembly)
· GDScript/Python       - Game develop & Chore scripts
```

And my featuring language **FallingAnchor**... Its journey is still long.

## Frameworks

```plain
· Webpack/tsup    - Frontend
· Hono.js/Flask   - Backend
· Tauri           - Cross-platform framework
· Unity/Godot.NET - Game engine

And my featuring...

· Nine9           - Reactive UI framework
· NDDrone-SDK     - Fly the mind.
```

## Falling... Maybe

```fallinganchor
# This a state-safe scripting language.

hook "stdout";
hook "math" pullout seed;

class FallingShrimp {
    slot String name = "FallingShrimp"; # reactive data slot
    slot Int age = 17;
    sync String id = this.name + (this.age -> String); # computed data & type casting

    define operator init() {
        # watch state update (or a reactive expression)
        watch (this.age):
            # after dependencies update
            after > (Int newAge, Int oldAge) => {
                stdout.write("Age %scraesed!" % newAge > oldAge ? "in" : "de");
                stdout.write("New id: %s" % this.id);
            }
            # before dependencies update
            before > (Int _n, Int _o) => {} # arrow functions: mark as a function without side effects
        
        stdout.write("%s was born." % this.name);
    }

    define Null advance(Int amount) { # define functions: mark as a function with side effects
        this.age += amount;
    }
    define Boolean playGame() {
        if (seed() < 0.5) {
            this.advance(1);
            return true;
        } else {
            return false;
        }
    }
}
```
