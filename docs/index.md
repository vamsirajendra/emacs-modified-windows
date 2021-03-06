# Presentation

> Important change in the distribution: Emacs is now a 64-bit build!

Emacs Modified for Windows is a 64-bit (x64) distribution of
[GNU Emacs](https://www.gnu.org/software/emacs/) **25.2** (released
April 21, 2017) bundled with a few select packages for LaTeX users and
R developers.

The additions to stock Emacs are the following:

- [ESS](http://ess.r-project.org) 16.10;
- [AUCTeX](http://www.gnu.org/software/auctex/) 11.90;
- [org](http://orgmode.org/) 9.0.7;
- [polymode](https://github.com/vitoshka/polymode) 2017-03-07;
- [markdown-mode.el](http://jblevins.org/projects/markdown-mode/) 2.2;
- [psvn.el](http://svn.apache.org/viewvc/subversion/trunk/contrib/client-side/emacs/) r1573006, an interface for the version control system
  [Subversion](http://subversion.tigris.org) modified to include Andre
  Colomb's and Koji Nakamaru's
  [combined patches](http://mail-archives.apache.org/mod_mbox//subversion-dev/201208.mbox/raw/%3c503B958F.6010906@schickhardt.org%3e/1/4)
  to support Subversion 1.7;
- [Aspell](http://aspell.net/) 0.50.3;
- English, French, German and Spanish
  [dictionaries](http://aspell.net/win32) for Aspell;
- [framepop.el](http://bazaar.launchpad.net/~vcs-imports/emacs-goodies-el/trunk/view/head:/elisp/emacs-goodies-el/framepop.el)
  to open temporary buffers in a separate frame;
- [default.el]({{ site.github.repository_url }}/tags/v25.2-modified-3/default.el)
  and
  [site-start.el]({{ site.github.repository_url }}/tags/v25.2-modified-3/site-start.el),
  configuration files to make everything work.

The distribution is based on the release version of
[emacs-w64](https://sourceforge.net/projects/emacsbinw64/), a native
64-bit distribution of GNU Emacs for Windows compiled with optimization and
providing support for PNG, JPEG, TIFF, GIF and SVG images, XML2 and GnuTLS.

## Latest release

Version 25.2-modified-3
([Release notes]({{ site.github.repository_url }}/releases/tag/v25.2-modified-3/))

## System requirements

This distribution requires a 64-Bit version of Microsoft Windows.

If you are still running a 32-bit version of Windows you need to install the
32-bit build. The last such version of the distribution was
[25.2-modified-2]({{ site.github.releases_url }}/tag/v25.2-modified-2/).


# Installation

Start the installation wizard and follow the instructions on screen.


# Images and preview-latex mode

This version of Emacs bundles the libraries needed to display images
in formats XPM, PNG, JPEG, TIFF, GIF and SVG supported on Windows
since Emacs version 22.1. Among other things, this means that the
toolbar displays in color, that the ESS toolbar displays correctly and
that the preview-latex mode of
[AUCTeX](http://www.gnu.org/software/auctex/) works 11.90 its full
extent. However, the latter requires to separately install
[Ghostscript](http://www.cs.wisc.edu/~ghost/ "Ghostscript/view
utilities") and to make sure that the file `gswin32c.exe` or
`gswin64c.exe` is in a folder along the `PATH` environment variable.


# Unix applications

Emacs sometimes uses external applications that are standard on Unix but
not available on Windows (for example: `diff`, `gzip`). When needed,
install the applications from the
[ezwinports](http://sourceforge.net/projects/ezwinports/) project. To
make sure Emacs can find the applications, include the folder where they
are installed to the `PATH` environment variable. *(With thanks to
Laurent Pantera for the hint.)*


# Also available

[Emacs Modified for macOS](https://{{ site.github.owner_name }}.{{ site.github.pages_hostname }}/emacs-modified-macos/).
