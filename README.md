# Christie's StyleGuide
This repo is used for working with the SCSS files for Christies.com.
The majority of this code is based on a styleguide provided by a collaboration of designer and developer. The visual stylegguide can be found on frontify:
[https://app.frontify.com/d/YOJshoa2gxNy/christie-s-style-guide](https://app.frontify.com/d/YOJshoa2gxNy/christie-s-style-guide)

<<<<<<< HEAD
##GRID
---
Naming Convention based on Bootstrap 3 (excluding xs).

*"X" represents the number of columns*

| Breakpoint        | Class Prefix           |
| ------------- |:-------------:| -----:|
| 0-767      | col-sm-X |
| 768-1023      | col-md-X      |
| 1024-1279 | col-lg-X      |
| 1280+ | col-xl-X      |

###Pulling and Pushing columns
- Pulling a column means giving it white space on the right side of the column.
- Pushing a column means giving it white space on the left side of the column.

| Breakpoint        | Class Prefix (Pull)  | Class Prefix (Pull) |
| ------------- |:-------------:| -----:|
| 0-767  | col-sm-pull-X | col-sm-push-X |
| 768-1023  | col-md-pull-X  | col-md-push-X |
| 1024-1279 | col-lg-pull-X  | col-lg-push-X |
| 1280+ | col-xl-pull-X  | col-cl-push-X |


---

##Responsive Utilities
---
The purpose these responsive uilities is to hide/show elements in specific breakpoints. Using a class for a single breapoint means all the other breakpoints will be `display:none`.

**Examples**
- Using `.visible-sm-block` means the element will be visible ONLY on the small breakpoint. 
- Using `.visibile-sm-block .visible-xl-inline` means the element will be visible on the small breakpoint as a block, hidden on medium and large and visible as inline on xl

**Options for showing/hiding are:**
- block
- inline-block
- inline
- print-block
- print-inline
- print-inline-block


| Breakpoint        | Class Prefix           |
| ------------- |:-------------:| -----:|
| 0-767      | visible-sm-X |
| 768-1023      | visible-md-X      |
| 1024-1279 | visible-lg-X      |
| 1280+ | visible-xl-X      |

In the same way you show an element in a specific breakpoint, you can also hide an element in a specific breakpoint.

**Examples**
- Using `.hidden-sm` means the element will be hidden ONLY on the small breakpoint. 
- Using `.hidden-sm .hidden-xl` means the element will be hidden on the small breakpoint and the xl breakpoint, but visible on the medium and large breakpoint.

| Breakpoint        | Class           |
| ------------- |:-------------:| -----:|
| 0-767      | hidden-sm |
| 768-1023      | hidden-md      |
| 1024-1279 | hidden-lg      |
| 1280+ | hidden-xl      |


###Hiding elements when printing
Using `.hidden-print` will hide any element from being printed

###Showing elements ONLY when printing
| Value        | Class           |
| ------------- |:-------------:| -----:|
| display:block      | visible-print-block |
| display:inline-block      | visible-print-inline-block      |
| display:inline | visible-print-inline      |

=======
>>>>>>> broken-nav
## CSS on Dev ##
**Compile to Dev:**

    \\10.100.1.214\d$\christies\websites\sitecore\dev\build\css

**Compile to dev files:**

- styles.css
- styles.css.map



## CSS on Stage ##
When it's time to move to stage, there are two options:

1. You can copy files from dev to stage
2. You can re-compile files directly to stage

The path to copy or compile to is:

    \\cmwscriis01u\websites\sitecore\Build\css

Regardless of the option you choose, stage should always have minified files:

- styles.min.css
- styles.min.css.map

## Grunt ##
There is a grunt file included in this repo. You don't HAVE to use it, but it's there for your convenience. If you're not familiar with Grunt, but have your own way of compiling SCSS files into CSS, you can do so that way, too. 
