# Grid based framework
> This assignment consists of building a grid-based framework (similar to bootstrap) that includes some basic functionality necessary to build a website.

This is our grid framework and it's based on a twelve-column system and it has its own offset system. All of the columns are set with margins and each column represents a fraction of the container's total width.

## Getting Started

Each one of the grid properties is specified with the different `@media screen` breakpoints which are:
- *Small* (**-sm**): for screens smaller than 720px width.
- *Medium* (**-md**): for screens with at least 720px width or more.
- *Large* (**-lg**): for screens with at least 1024px width or more.

The sufixes mentioned above are used within the classes for the rest of the grid. They go after the rule and before the size. For example:
```
<div class="container">
    <div class="row">
        <div class="col-sm-12 col-md-6">
            'Content in the first column goes here'
        </div>
        <div class="col-sm-12 col-md-6">
            'Content in the second column goes here'
        </div>
    </div>
    <div class="row">
        ...
    </div>
</div>
```

In the previous example we are setting the `<div>` element width to fill the container but then changing it to half width once you reach the medium breakpoint (`min-width: 720px`).

The first element class is the **container**. It will take the whole page width until it reaches the specified breakpoint, then it will keep that width for bigger viewports. This **container** has a special property called **-fluid** which makes the container take the viewport width at all times.

The possible classes for this container are:
- ***container***
    - **-fluid**

The grid can be created by nesting **columns** inside **row** elements. For the columns all the possible classes are:
- ***col***
    - **-sm** Or **-md** Or **-lg** *(optional)*
        - **-0**
        - **-1**
        - **-2**
        - **-3**
        - **-4**
        - **-5**
        - **-6**
        - **-7**
        - **-8**
        - **-9**
        - **-10**
        - **-11**
        - **-12**

The offset property takes works by taking the space of a column with the specified size moving everything else to the right. Its clases are similar to the ones used for **columns**:
- ***offset***
    - **-sm** Or **-md** Or **-lg** *(optional)*
        - **-0**
        - **-1**
        - **-2**
        - **-3**
        - **-4**
        - **-5**
        - **-6**
        - **-7**
        - **-8**
        - **-9**
        - **-10**
        - **-11**
        - **-12**

## Built With

* [VS Code](https://code.visualstudio.com/) - The code editor used

## Authors

* **Jaak Kivinukk** - *Initial work* - [Jaakal](https://github.com/Jaakal)
* **Diego Luna Granados** - *Initial work* - [SlowKingV](https://github.com/SlowKingV)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
