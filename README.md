# Kdenlive

See: <https://flathub.org/apps/org.kde.kdenlive>

**Temporary fix for popup menus in Qt6 under Gnome with mutter and wayland** [Bug 508321](https://bugs.kde.org/show_bug.cgi?id=508321)

## Requirements
```flatpak install org.kde.Sdk```
```flatpak install org.freedesktop.Sdk.Extension.llvm19```

## Build
```flatpak-builder --force-clean --repo=repo ./flatpak-buildir org.kde.kdenlive.json```

For ```flatpak>=1.4.2``` use ```org.kde.kdenlive.orig.json```

## Create package
```flatpak build-bundle ./repo kdenlive.flatpak org.kde.kdenlive stable --runtime-repo=https://flathub.org/repo/flathub.flatpakrepo```

## Install
```flatpak --user install ./kdenlive.flatpak```
