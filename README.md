# Tailwind CSS Gradient and Shadow Rendering Issue

This repository demonstrates a subtle rendering bug that can occur when using Tailwind CSS gradients and shadows together. The shadow sometimes appears behind the gradient instead of on top, likely due to stacking context issues.

**Bug:**
The `shadow-lg` class renders below the gradient, resulting in an incorrect visual appearance.

**Solution:**
The order of classes matters.  Adjusting the order to place `shadow-lg` before the gradient classes will solve the issue in most cases. For more complex scenarios, a different approach may be required, such as using `z-index` to explicitly manage stacking.