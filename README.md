# Tailwind CSS Class Compilation Issue

This repository demonstrates a common issue when using Tailwind CSS: classes defined in components not being picked up by the build process.

## Problem

Tailwind CSS uses the `content` array in your `tailwind.config.js` file to scan for classes used in your project. If this array doesn't include the paths to your component files, Tailwind won't detect your custom classes and won't generate the corresponding CSS.

This leads to your custom classes not being applied to your elements.

## Solution

Ensure the `content` array in `tailwind.config.js` correctly includes all directories and files containing your components.  You'll need to update this array any time you add or move component files.