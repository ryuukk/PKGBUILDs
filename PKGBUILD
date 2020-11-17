# Maintainer: Fredrick Brennan <copypaste@kittens.ph>
# Maintainer: Andrew Bueide <abueide@protonmail.com>
# Maintainer: rouhannb <rouhannb@gmail.com>
# Contributor: Wilson E. Alvarez <wilson.e.alvarez1@gmail.com>
# Contributor: Benoit Favre <benoit.favre@gmail.com>
# Contributor: Alexander Rødseth <rodseth@gmail.com>
# Contributor: Kamil Biduś <kamil.bidus@gmail.com>

pkgname=aseprite
pkgver=1.2.25
pkgrel=1
pkgdesc='Create animated sprites and pixel art'
arch=('x86_64')
url="http://www.aseprite.org/"
license=('custom')
depends=('cmark' 'curl' 'giflib' 'zlib' 'libpng' 'tinyxml' 'freetype2' 'fontconfig' 'libxcursor'
         'hicolor-icon-theme')
makedepends=('cmake' 'ninja' 'git' 'python2' 'freeglut' 'xorgproto' 'libxi' 'harfbuzz-icu'
             'nettle')
conflicts=("aseprite-git" "aseprite-gpl" "skia-git")
source=("https://github.com/${pkgname}/${pkgname}/releases/download/v${pkgver}/${pkgname^}-\
v${pkgver}-Source.zip"
"${pkgname}.desktop"
"git+https://chromium.googlesource.com/chromium/tools/depot_tools.git"
"git+https://github.com/${pkgname}/skia.git#branch=${pkgname}-m81"
"${pkgname}-buildtools.tar.gz::https://chromium.googlesource.com/chromium/buildtools.git/+archive/\
505de88083136eefd056e5ee4ca0f01fe9b33de8.tar.gz"
"${pkgname}-common.tar.gz::https://skia.googlesource.com/common.git/+archive/\
9737551d7a52c3db3262db5856e6bcd62c462b92.tar.gz"
"${pkgname}-angle2.tar.gz::https://chromium.googlesource.com/angle/angle.git/+archive/\
ee07cb317579dfda40dabb5d6d9c209e0e9e0643.tar.gz"
"${pkgname}-dawn.tar.gz::https://dawn.googlesource.com/dawn.git/+archive/\
604072bc2ed01018eb03bcbbf9d94042f679af63.tar.gz"
"${pkgname}-dng_sdk.tar.gz::https://android.googlesource.com/platform/external/dng_sdk.git/\
+archive/c8d0c9b1d16bfda56f15165d39e0ffa360a11123.tar.gz"
"${pkgname}-egl-registry.tar.gz::https://skia.googlesource.com/external/github.com/KhronosGroup\
/EGL-Registry/+archive/a0bca08de07c7d7651047bedc0b653cfaaa4f2ae.tar.gz"
"${pkgname}-expat.tar.gz::https://android.googlesource.com/platform/external/expat.git/+archive/\
e5aa0a2cb0a5f759ef31c0819dc67d9b14246a4a.tar.gz"
"${pkgname}-freetype.tar.gz::https://skia.googlesource.com/third_party/freetype2.git/+archive/\
0a3d2bb99b45b72e1d45185ab054efa993d97210.tar.gz"
"${pkgname}-harfbuzz.tar.gz::https://chromium.googlesource.com/external/github.com/harfbuzz/\
harfbuzz.git/+archive/3a74ee528255cc027d84b204a87b5c25e47bff79.tar.gz"
"${pkgname}-icu.tar.gz::https://chromium.googlesource.com/chromium/deps/icu.git/+archive/\
dbd3825b31041d782c5b504c59dcfb5ac7dda08c.tar.gz"
"${pkgname}-imgui.tar.gz::https://skia.googlesource.com/external/github.com/ocornut/imgui.git\
/+archive/d38d7c6628bebd02692cfdd6fa76b4d992a35b75.tar.gz"
"${pkgname}-libgifcodec.tar.gz::https://skia.googlesource.com/libgifcodec/+archive/\
38d9c73f49b861bb4a9829371ac311544b120023.tar.gz"
"${pkgname}-libjpeg-turbo.tar.gz::https://skia.googlesource.com/external/github.com/libjpeg-turbo\
/libjpeg-turbo.git/+archive/574f3a772c96dc9db2c98ef24706feb3f6dbda9a.tar.gz"
"${pkgname}-libpng.tar.gz::https://skia.googlesource.com/third_party/libpng.git/+archive/\
386707c6d19b974ca2e3db7f5c61873813c6fe44.tar.gz"
"${pkgname}-libwebp.tar.gz::https://chromium.googlesource.com/webm/libwebp.git/+archive/\
0fe1a89dbf1930fc2554dbe76adad5d962054ead.tar.gz"
"${pkgname}-lua.tar.gz::https://skia.googlesource.com/external/github.com/lua/lua.git/+archive/\
e354c6355e7f48e087678ec49e340ca0696725b1.tar.gz"
"${pkgname}-microhttpd.tar.gz::https://android.googlesource.com/platform/external/libmicrohttpd\
/+archive/748945ec6f1c67b7efc934ab0808e1d32f2fb98d.tar.gz"
"${pkgname}-opencl-lib.tar.gz::https://skia.googlesource.com/external/github.com/GPUOpen-Tools/\
common-lib-amd-APPSDK-3.0/+archive/4e6d30e406d2e5a65e1d65e404fe6df5f772a32b.tar.gz"
"${pkgname}-opencl-registry.tar.gz::https://skia.googlesource.com/external/github.com/\
KhronosGroup/OpenCL-Registry/+archive/932ed55c85f887041291cef8019e54280c033c35.tar.gz"
"${pkgname}-opengl-registry.tar.gz::https://skia.googlesource.com/external/github.com/\
KhronosGroup/OpenGL-Registry/+archive/14b80ebeab022b2c78f84a573f01028c96075553.tar.gz"
"${pkgname}-piex.tar.gz::https://android.googlesource.com/platform/external/piex.git/+archive/\
bb217acdca1cc0c16b704669dd6f91a1b509c406.tar.gz"
"${pkgname}-sdl.tar.gz::https://skia.googlesource.com/third_party/sdl/+archive/\
5d7cfcca344034aff9327f77fc181ae3754e7a90.tar.gz"
"${pkgname}-sfntly.tar.gz::https://chromium.googlesource.com/external/github.com/googlei18n/\
sfntly.git/+archive/b55ff303ea2f9e26702b514cf6a3196a2e3e2974.tar.gz"
"${pkgname}-spirv-cross.tar.gz::https://chromium.googlesource.com/external/github.com/\
KhronosGroup/SPIRV-Cross/+archive/53ab2144b90abede33be5161aec5dfc94ddc3caf.tar.gz"
"${pkgname}-spirv-headers.tar.gz::https://skia.googlesource.com/external/github.com/KhronosGroup/\
SPIRV-Headers.git/+archive/29c11140baaf9f7fdaa39a583672c556bf1795a1.tar.gz"
"${pkgname}-spirv-tools.tar.gz::https://skia.googlesource.com/external/github.com/KhronosGroup\
/SPIRV-Tools.git/+archive/0c4feb643b89d1792b02f7cbef315e9d95633bd7.tar.gz"
"${pkgname}-swiftshader.tar.gz::https://swiftshader.googlesource.com/SwiftShader/+archive/\
430def835f9f85d52f4a96db9b715cd9a7403c9c.tar.gz"
"${pkgname}-wuffs.tar.gz::https://skia.googlesource.com/external/github.com/google/wuffs.git\
/+archive/4080840928c0b05a80cda0d14ac2e2615f679f1a.tar.gz"
"${pkgname}-zlib.tar.gz::https://chromium.googlesource.com/chromium/src/third_party/zlib/+archive/\
ea3ba903faac98b64b2bf8de5e98cd97b335a474.tar.gz"
"gn::https://chromium-gn.storage-download.googleapis.com/3523d50538357829725d4ed74b777a572ce0ac74"
)
_gitsrc=("${source[@]:4:29}")
noextract=("${_gitsrc[@]%%::*}")
sha256sums=('c5496ad159454b44e9b6c0f872553a192a7d20feeb6337a799c3f7009cdda558'
            'deaf646a615c79a4672b087562a09c44beef37e7acfc6f5f66a437d4f3b97a25'
            'SKIP'
            'SKIP'
            'ea9192b75031f9bb15b039ca1c3d07d6e9f00a9b1d49c0d15cdda6725e348139'
            'ad9dad8c9d083da0f6493bf13db8640243b0deeadf24c8114551259af3f16815'
            '8be8172d4e09e9457155df58288625e0bdb4dbc5da6f33a699969e0771c0d593'
            '5fbf372e9815fe998b28d33e6c592886b44681165a661a71b9402985b2b3d809'
            'db13bb99db626669b297293303e95eb8cb1f3ef7069266d06fe2ddbc228cd20e'
            'e113aba9898c65a2449f23f3c1fdfce24bdc117c33bd9e77748cd015513822d3'
            'c0cb6ceae0270384e9d3445e1047cc2c2587ec6434781c4e3079c7a7874665ba'
            '0ae3d6d84b249363cf62f0e829b2ec78f1188b02500f6a9327ad26b4b9b275e4'
            'af341d5d21fbbebf99f3b6da9ce4e211046b5d88fb3ec532299dfc1323cfe835'
            '29641c234faf498b0741d4b85c70dbf9fdbbb642064c16c1d4d38c496cb09c25'
            '66a5a43e1ca069e9882b1f9e5021d4a1ff816d29c69d51c0f5fdc06115441464'
            'c7a5154249cc1ca1921b09120ee79134b33904e528d9278e46fbc76bca64ecd3'
            'a7f6de90a69e54667bc36008977a95ef4e7334ecff6b0cd3ed2153e833979f1f'
            'da860b9869bd426f387dbf16037468faf8bb103f3fdf49a25d9e44e87e3bba30'
            'a1a1c7197cdf48ff747212db09da89ae0d35b52bdd7807b752f42ebfab801379'
            '51562cb62e51b908ff8f977a8e1406acd056adeeaa8f65579e06653758b7d1f1'
            'da5e2e2383ed6cb09e65735587a3c5f8314b6274613881d1dd6114a442e48f91'
            'd2707e5056b70ae89099194c4088a4322dc1d4ab54ae21864df419091647c243'
            'e1864950d9c198a1882a4ba3cca1f0920bbf81df536e71580252dcdb70a6d169'
            '67262e02cafa132a47294cf1f245c89510d5947d94ab2b7708cce7e0b1f63c26'
            '65b69bb157f329efaeb7871f285b6ed2fa666b2cf119eca3697c97e4ca720be2'
            '055a3d643bd95b997ff875a0a28b3f82c25e1e351cf6998cc4ba1bc6db0dbdce'
            '938322aa1cf6de836454e1bf13215173fd8eec3107cea56d647b44a09b14286e'
            'c46de3453d5dc5ff9af5d539b8faec948f9da9d5a94cd232f1f7ec6c71229311'
            '46a947e232322b40c3cf610fe87091857a70176fce702bdf9bc24b1b2659ce75'
            '39ccfa6dcdd024a374fe6406514b97d5788b97ed8f850d8f6b9403877e1acd7c'
            '484efea4dee57ecf432e64f704f5bf680c0567f2699719a96e4872ab3da5a780'
            'b4dd94e4fe7c86698abfa418f6ea2d2071ff20854baa51738057c6a855eab275'
            '17188c5b17b8fd3565afc4f0f21dc42ed93ae4a94f15a111d66b21f661211ce3'
            'c8c2d617f1a33d6eb27f25ebcc30bd8ba1e6a0aa980cada21dda2ad1401fa4a2')

prepare() {
  cd "${srcdir}"

  # Install skia deps (essentially runs git-sync-deps with the files already downloaded)
  mkdir --parents --verbose skia/third_party/externals

  for _dep in buildtools common
  do
    mkdir --parents --verbose "skia/${_dep}"
    tar --verbose --extract --file "${pkgname}-${_dep}.tar.gz" --directory "skia/${_dep}"
  done

  for _dep in angle2 dawn dng_sdk egl-registry expat freetype harfbuzz icu imgui opencl-registry \
              libjpeg-turbo libpng libwebp lua microhttpd opencl-lib opengl-registry piex \
              sdl sfntly spirv-cross spirv-headers spirv-tools swiftshader zlib wuffs
  do
    mkdir --parents --verbose "skia/third_party/externals/${_dep}"
    tar --verbose --extract --file "${pkgname}-${_dep}.tar.gz" --directory \
      "skia/third_party/externals/${_dep}"
  done

  chmod u=rwx,g=rx,o=rx --verbose gn
  mv --verbose gn skia/bin/gn
  cp --verbose skia/bin/gn skia/buildtools/linux64/gn

  mkdir --parents --verbose binsub
  ln --force --symbolic $(which python2) binsub/python
}

build() {
  cd "${srcdir}"

  # Build skia
  _skiapath="${srcdir}/binsub:${srcdir}/depot_tools:${PATH}"
  cd skia
  PATH="${_skiapath}" gn gen out/Release-x64 \
    --args="is_debug=false is_official_build=true skia_use_system_expat=false \
    skia_use_system_icu=false skia_use_system_libjpeg_turbo=false skia_use_system_libpng=false \
    skia_use_system_libwebp=false skia_use_system_zlib=false"
  PATH="${_skiapath}" ninja -C out/Release-x64 skia modules

  # Build aseprite
  cd "${srcdir}"
  mkdir --parents --verbose build && cd build

  cmake \
    -DWITH_WEBP_SUPPORT=ON \
    -DUSE_SHARED_CURL=ON \
    -DUSE_SHARED_GIFLIB=ON \
    -DUSE_SHARED_HARFBUZZ=ON \
    -DUSE_SHARED_ZLIB=ON \
    -DUSE_SHARED_LIBPNG=ON \
    -DUSE_SHARED_TINYXML=ON \
    -DUSE_SHARED_CMARK=ON \
    -DENABLE_UPDATER=OFF \
    -DUSE_SHARED_FREETYPE=ON \
    -DCMAKE_INSTALL_PREFIX=/usr \
    -DCMAKE_BUILD_TYPE=Release \
    -DLAF_BACKEND=skia \
    -DSKIA_DIR="${srcdir}/skia" \
    -DSKIA_LIBRARY_DIR="${srcdir}/skia/out/Release-x64" \
    -DSKIA_LIBRARY="${srcdir}/skia/out/Release-x64/libskia.a" \
    -G Ninja \
    ..

  ninja aseprite
}

package() {
  cd "${srcdir}"/build

  install -D --verbose "bin/${pkgname}" "${pkgdir}/usr/bin/${pkgname}"

  # Aseprite, by default, doesn't install a few files on its own. So, they are installed manually.

  install --directory --verbose "${pkgdir}/usr/share/${pkgname}/data"
  cp --recursive --verbose 'bin/data' "${pkgdir}/usr/share/${pkgname}"

  install --directory --verbose "${pkgdir}/usr/share/doc/${pkgname}"
  cp --recursive --verbose '../docs' "${pkgdir}/usr/share/doc/${pkgname}"
  install --mode=644 --verbose 'bin/data/EULA.txt' "${pkgdir}/usr/share/doc/${pkgname}"
  install --mode=644 --verbose '../README.md' "${pkgdir}/usr/share/doc/${pkgname}"

  install -D --mode=644 --verbose "../${pkgname}.desktop" \
    "${pkgdir}/usr/share/applications/${pkgname}.desktop"

  for _size in 32 48 64
  do
    install -D --mode=644 --verbose "../data/icons/ase${_size}.png" \
      "${pkgdir}/usr/share/icons/hicolor/${_size}x${_size}/apps/${pkgname}.png"
  done

  install -D --mode=644 --verbose --target-directory "${pkgdir}/usr/share/licenses/${pkgname}" \
    'bin/data/EULA.txt'
  install --mode=644 --verbose '../docs/LICENSES.md' "${pkgdir}/usr/share/licenses/${pkgname}"
}

# vim:set ts=2 sw=2 et:
