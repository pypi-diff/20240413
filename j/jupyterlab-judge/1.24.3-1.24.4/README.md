# Comparing `tmp/jupyterlab_judge-1.24.3.tar.gz` & `tmp/jupyterlab_judge-1.24.4.tar.gz`

## Comparing `jupyterlab_judge-1.24.3.tar` & `jupyterlab_judge-1.24.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/.copier-answers.yml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/.yarnrc.yml
--rw-r--r--   0        0        0     8518 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/CHANGELOG.md
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/babel.config.js
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/conftest.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jest.config.js
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/setup.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/tsconfig.test.json
--rw-r--r--   0        0        0   435917 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/yarn.lock
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyter-config/nb-config/jupyterlab_judge.json
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyter-config/server-config/jupyterlab_judge.json
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/_version.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/handlers.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/yjudge.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/package.json
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/schemas/jupyterlab-judge/plugin.json
--rw-r--r--   0        0        0    14975 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js.LICENSE.txt
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js
--rw-r--r--   0        0        0     6939 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js
--rw-r--r--   0        0        0    54375 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js
--rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js
--rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js
--rw-r--r--   0        0        0  4279528 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js.LICENSE.txt
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js
--rw-r--r--   0        0        0    33287 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/960.abc3ea48609d1283cc0f.js
--rw-r--r--   0        0        0    10420 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/remoteEntry.c7382fcadc5b0c3a8903.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/style.js
--rw-r--r--   0        0        0    38387 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json
--rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/tests/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/jupyterlab_judge/tests/test_handlers.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/schema/plugin.json
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/commands.ts
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/constants.ts
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/handler.ts
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/index.ts
--rw-r--r--   0        0        0    16041 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/model.ts
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/tokens.ts
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/toolbar.tsx
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/__tests__/jupyterlab_judge.spec.ts
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/components/SubmissionArea.tsx
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/components/SubmissionControl.tsx
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/components/SubmissionItem.tsx
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/components/SubmissionItemStatus.tsx
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/components/SubmissionItemWait.tsx
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/components/SubmissionItemWaitStatus.tsx
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/components/SubmissionList.tsx
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/components/index.ts
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/problemProvider/HardCodedProblemProvider.ts
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/problemProvider/index.ts
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/problemProvider/problemProvider.ts
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/widgets/JudgeOutputArea.ts
--rw-r--r--   0        0        0    22457 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/widgets/JudgePanel.ts
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/widgets/JudgeProblemPanel.ts
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/widgets/JudgeSubmissionArea.tsx
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/widgets/JudgeTerminal.ts
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/src/widgets/index.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/style/index.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/style/judgeOutputArea.css
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/style/judgePanel.css
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/style/judgeTerminal.css
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/ui-tests/yarn.lock
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/ui-tests/tests/jupyterlab_judge.spec.ts
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/LICENSE
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/README.md
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/pyproject.toml
--rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.3/PKG-INFO
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/.copier-answers.yml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/.yarnrc.yml
+-rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/CHANGELOG.md
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/babel.config.js
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/conftest.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jest.config.js
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/setup.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/tsconfig.test.json
+-rw-r--r--   0        0        0   435917 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/yarn.lock
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyter-config/nb-config/jupyterlab_judge.json
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyter-config/server-config/jupyterlab_judge.json
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/_version.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/handlers.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/yjudge.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/package.json
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/schemas/jupyterlab-judge/plugin.json
+-rw-r--r--   0        0        0    14975 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js.LICENSE.txt
+-rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js
+-rw-r--r--   0        0        0     6939 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js
+-rw-r--r--   0        0        0    54375 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js
+-rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js
+-rw-r--r--   0        0        0     7287 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js
+-rw-r--r--   0        0        0  4279528 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js.LICENSE.txt
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js
+-rw-r--r--   0        0        0    33296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/960.376cb311c5431702de57.js
+-rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/remoteEntry.b81a0f7c77284e957c86.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/style.js
+-rw-r--r--   0        0        0    38387 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json
+-rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/tests/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/jupyterlab_judge/tests/test_handlers.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/schema/plugin.json
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/commands.ts
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/constants.ts
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/handler.ts
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/index.ts
+-rw-r--r--   0        0        0    16041 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/model.ts
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/tokens.ts
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/toolbar.tsx
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/__tests__/jupyterlab_judge.spec.ts
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionArea.tsx
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionControl.tsx
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionItem.tsx
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionItemStatus.tsx
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionItemWait.tsx
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionItemWaitStatus.tsx
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/SubmissionList.tsx
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/components/index.ts
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/problemProvider/HardCodedProblemProvider.ts
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/problemProvider/index.ts
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/problemProvider/problemProvider.ts
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/widgets/JudgeOutputArea.ts
+-rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/widgets/JudgePanel.ts
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/widgets/JudgeProblemPanel.ts
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/widgets/JudgeSubmissionArea.tsx
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/widgets/JudgeTerminal.ts
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/src/widgets/index.ts
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/style/index.js
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/style/judgeOutputArea.css
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/style/judgePanel.css
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/style/judgeTerminal.css
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/ui-tests/tests/jupyterlab_judge.spec.ts
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/LICENSE
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/README.md
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/pyproject.toml
+-rw-r--r--   0        0        0     9296 2020-02-02 00:00:00.000000 jupyterlab_judge-1.24.4/PKG-INFO
```

### Comparing `jupyterlab_judge-1.24.3/.copier-answers.yml` & `jupyterlab_judge-1.24.4/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/CHANGELOG.md` & `jupyterlab_judge-1.24.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.24.4
+
+([Full Changelog](https://github.com/team-monolith-product/jupyterlab-judge/compare/v1.24.3...5364c40d9549fb4817110ffe9c841f46209c18ee))
+
+### Merged PRs
+
+- fix: rstrip new line [#58](https://github.com/team-monolith-product/jupyterlab-judge/pull/58) ([@a3626a](https://github.com/a3626a))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/team-monolith-product/jupyterlab-judge/graphs/contributors?from=2024-04-08&to=2024-04-13&type=c))
+
+[@a3626a](https://github.com/search?q=repo%3Ateam-monolith-product%2Fjupyterlab-judge+involves%3Aa3626a+updated%3A2024-04-08..2024-04-13&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.24.3
 
 ([Full Changelog](https://github.com/team-monolith-product/jupyterlab-judge/compare/v1.24.2...668b1d002a29e4df3e7d9edf181841088dd27f09))
 
 ### Merged PRs
 
 - fix: make prompt argument optional [#57](https://github.com/team-monolith-product/jupyterlab-judge/pull/57) ([@a3626a](https://github.com/a3626a))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/team-monolith-product/jupyterlab-judge/graphs/contributors?from=2024-04-08&to=2024-04-08&type=c))
 
 [@a3626a](https://github.com/search?q=repo%3Ateam-monolith-product%2Fjupyterlab-judge+involves%3Aa3626a+updated%3A2024-04-08..2024-04-08&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 1.24.2
 
 ([Full Changelog](https://github.com/team-monolith-product/jupyterlab-judge/compare/v1.24.1...bb8c572290dcd744d538cf09d98459c85bdbd4ac))
 
 ### Merged PRs
 
 - fix: add prompt parameter to input function [#56](https://github.com/team-monolith-product/jupyterlab-judge/pull/56) ([@a3626a](https://github.com/a3626a))
```

### Comparing `jupyterlab_judge-1.24.3/RELEASE.md` & `jupyterlab_judge-1.24.4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jest.config.js` & `jupyterlab_judge-1.24.4/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/package.json` & `jupyterlab_judge-1.24.4/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'1.24.4'"}*

```diff
@@ -231,9 +231,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.24.3"
+    "version": "1.24.4"
 }
```

### Comparing `jupyterlab_judge-1.24.3/tsconfig.json` & `jupyterlab_judge-1.24.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/yarn.lock` & `jupyterlab_judge-1.24.4/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/__init__.py` & `jupyterlab_judge-1.24.4/jupyterlab_judge/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/handlers.py` & `jupyterlab_judge-1.24.4/jupyterlab_judge/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/yjudge.py` & `jupyterlab_judge-1.24.4/jupyterlab_judge/yjudge.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/package.json` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9796666666666667%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b81a0f7c77284e957c86.js'}}",*

 * * "'version'": "'1.24.4'"}*

```diff
@@ -135,15 +135,15 @@
         "schema/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/team-monolith-product/jupyterlab-judge",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c7382fcadc5b0c3a8903.js",
+            "load": "static/remoteEntry.b81a0f7c77284e957c86.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_judge"
                 },
@@ -236,9 +236,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.24.3"
+    "version": "1.24.4"
 }
```

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/schemas/jupyterlab-judge/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'1.24.4'"}*

```diff
@@ -231,9 +231,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.24.3"
+    "version": "1.24.4"
 }
```

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/146.ffbfc6be3b1d44378330.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/378.2c7a4a82fbc8f09f2463.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/599.7e6937b28ad247ccde7c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/732.d368cf762f465d394900.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/747.2841a40cba671c554a8c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/767.69c7e698f115ea487665.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/860.fee57e15b3a40a2d65fa.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/893.389b596eee368876402a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/901.b84e014859b58a1fa86a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/917.ab3207654a9c812bc979.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/960.abc3ea48609d1283cc0f.js` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/960.376cb311c5431702de57.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -30,21 +30,21 @@
                 SubmissionListImpl: () => me,
                 SubmissionListSignalWrapper: () => ce,
                 default: () => Ne,
                 factoryContext: () => ve,
                 openOrCreateFromId: () => A,
                 transContext: () => we
             });
-            var n = s(8368),
-                o = s(9510),
-                i = s(5962),
-                r = s(3452),
-                a = s(3471),
-                d = s(1638),
-                l = s(1778),
+            var n = s(4072),
+                o = s(1464),
+                i = s(8937),
+                r = s(6805),
+                a = s(7594),
+                d = s(2294),
+                l = s(3195),
                 u = s(6029),
                 c = s.n(u);
             const m = "jupyterlab-judge",
                 h = ".jce-judge",
                 p = "jupyterlab-judge";
             var g;
             ! function(e) {
@@ -77,15 +77,15 @@
                         name: "save",
                         widget: t(e, s)
                     }]
                 }
             }(g || (g = {}));
             var _ = s(4882),
                 b = s(5536),
-                y = s(8048);
+                y = s(3413);
             class C extends _.Panel {
                 constructor(e, t) {
                     super(), this._model = e.model, this._trans = e.translator.load(m), this._markdownRenderer = t.createRenderer("text/markdown"), this._markdownRenderer.addClass("jp-JudgePanel-problem"), this.addWidget(this._markdownRenderer)
                 }
                 renderProblem() {
                     var e, t;
                     this._markdownRenderer.renderModel(new y.MimeModel({
@@ -297,15 +297,15 @@
                     }, this._submitted.emit({
                         widget: this,
                         submission: m,
                         problem: s
                     })
                 }
                 async runWithInput(e, t, s, n) {
-                    const o = `\nimport io\nimport base64\n\ndef input(prompt=None):  \t\n    r = JUDGE_INPUT_STRING_IO.${"one_line"===s.inputTransferType?"readline":"read"}()  \t\n    if not r:  \t\t\n        return ''\n    return r\n\nJUDGE_INPUT_STRING_IO = io.StringIO()\n`;
+                    const o = `\nimport io\nimport base64\n\ndef input(prompt=None):  \t\n    r = JUDGE_INPUT_STRING_IO.${"one_line"===s.inputTransferType?"readline":"read"}().rstrip('\\n')\n    if not r:  \t\t\n        return ''\n    return r\n\nJUDGE_INPUT_STRING_IO = io.StringIO()\n`;
                     await e.requestExecute({
                         code: o,
                         stop_on_error: !0
                     }, !0, {}).done;
                     const i = 1e6;
                     for (let t = 0; t < n.length; t += i) {
                         const s = n.slice(t, t + i),
@@ -381,18 +381,18 @@
                         content: t,
                         context: e,
                         commands: this._commands,
                         translator: this.translator
                     })
                 }
             }
-            var T, P = s(7217),
+            var T, P = s(2818),
                 F = s(8093),
                 N = s(4901),
-                J = s(2425);
+                J = s(7263);
             class M {
                 constructor(e, t) {
                     this._contentChanged = new N.Signal(this), this._stateChanged = new N.Signal(this), this._isDisposed = !1, this._dirty = !1, this._problemChanged = new N.Signal(this), this._submissionsChanged = new N.Signal(this), this._submissionStatus = {
                         type: "idle"
                     }, this._submissionStatusChanged = new N.Signal(this), this.sharedModel = new M.YJudge, this.sharedModel.changed.connect((async (e, t) => {
                         t.problemIdChange && (this._problem = await this._problemProvider.getProblem(t.problemIdChange), this._problemChanged.emit(this._problem)), t.stateChange && t.stateChange.forEach((e => {
                             "dirty" === e.name && (this.dirty = e.newValue)
@@ -712,17 +712,17 @@
                         };
                         return JSON.stringify(o)
                     }
                 }(M || (M = {})),
                 function(e) {
                     e.open = `${p}:plugin:open`, e.openOrCreateFromId = `${p}:plugin:open-or-create-from-id`, e.execute = `${p}:plugin:execute`, e.undo = `${p}:plugin:undo`, e.redo = `${p}:plugin:redo`, e.run = `${p}:plugin:run`, e.runAll = `${p}:plugin:run-all`
                 }(T || (T = {}));
-            var O = s(5326),
-                D = s(9557),
-                L = s(4008),
+            var O = s(2232),
+                D = s(797),
+                L = s(5099),
                 W = s(7930);
             const $ = new W.Token(`${p}:IProblemProvider`),
                 R = new W.Token(`${p}:IJudgePanelFactory`),
                 K = new W.Token(`${p}:IJudgeSubmissionAreaFactory`),
                 B = new W.Token(`${p}:IJudgeTerminalFactory`),
                 U = new W.Token(`${p}:ISubmissionListFactory`),
                 z = new W.Token(`${p}:IJudgeSignal`);
@@ -852,15 +852,15 @@
     cursor: not-allowed;
   }
 
   :not(:disabled):hover {
     background: var(--jp-brand-color0);
   }
 `;
-            var Z = s(6311);
+            var Z = s(8671);
 
             function ee(e) {
                 const t = (0, u.useContext)(we);
                 let s = "",
                     n = "";
                 switch (e.status) {
                     case "AC":
```

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/remoteEntry.c7382fcadc5b0c3a8903.js` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/remoteEntry.b81a0f7c77284e957c86.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -57,15 +57,15 @@
         732: "d368cf762f465d394900",
         747: "2841a40cba671c554a8c",
         767: "69c7e698f115ea487665",
         860: "fee57e15b3a40a2d65fa",
         893: "389b596eee368876402a",
         901: "b84e014859b58a1fa86a",
         917: "ab3207654a9c812bc979",
-        960: "abc3ea48609d1283cc0f"
+        960: "376cb311c5431702de57"
     } [e] + ".js?v=" + {
         29: "d2153138b471f40c1c27",
         146: "ffbfc6be3b1d44378330",
         316: "18d9e632074f3acc892c",
         378: "2c7a4a82fbc8f09f2463",
         505: "fe5d2436cfe6faec3918",
         599: "7e6937b28ad247ccde7c",
@@ -73,15 +73,15 @@
         732: "d368cf762f465d394900",
         747: "2841a40cba671c554a8c",
         767: "69c7e698f115ea487665",
         860: "fee57e15b3a40a2d65fa",
         893: "389b596eee368876402a",
         901: "b84e014859b58a1fa86a",
         917: "ab3207654a9c812bc979",
-        960: "abc3ea48609d1283cc0f"
+        960: "376cb311c5431702de57"
     } [e], T.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -133,15 +133,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (o[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (i("@emotion/react", "11.11.1", (() => Promise.all([T.e(146), T.e(29), T.e(599)]).then((() => () => T(917))))), i("@emotion/styled", "11.11.0", (() => Promise.all([T.e(29), T.e(505), T.e(378)]).then((() => () => T(4378))))), i("@team-monolith/cds", "1.0.1", (() => Promise.all([T.e(146), T.e(901), T.e(29), T.e(704), T.e(316)]).then((() => () => T(7210))))), i("jupyterlab-judge", "1.24.3", (() => Promise.all([T.e(29), T.e(960)]).then((() => () => T(960))))), i("react-query", "3.39.3", (() => Promise.all([T.e(767), T.e(29), T.e(704)]).then((() => () => T(8767)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@emotion/react", "11.11.1", (() => Promise.all([T.e(146), T.e(29), T.e(599)]).then((() => () => T(917))))), i("@emotion/styled", "11.11.0", (() => Promise.all([T.e(29), T.e(505), T.e(378)]).then((() => () => T(4378))))), i("@team-monolith/cds", "1.0.1", (() => Promise.all([T.e(146), T.e(901), T.e(29), T.e(704), T.e(316)]).then((() => () => T(7210))))), i("jupyterlab-judge", "1.24.4", (() => Promise.all([T.e(29), T.e(960)]).then((() => () => T(960))))), i("react-query", "3.39.3", (() => Promise.all([T.e(767), T.e(29), T.e(704)]).then((() => () => T(8767)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         T.g.importScripts && (e = T.g.location + "");
         var r = T.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -250,48 +250,48 @@
         var n = T.I(r);
         return n && n.then ? n.then(e.bind(e, r, T.S[r], t, a, o)) : e(r, T.S[r], t, a, o)
     })(((e, r, t, a) => r && T.o(r, t) ? h(i(r, t)) : a())), y = m(((e, r, t, a) => (l(e, t), h(s(r, t, a) || b(r, e, t, a) || i(r, t))))), g = m(((e, r, t, a) => (l(e, t), f(r, 0, t, a)))), j = m(((e, r, t, a, o) => {
         var n = r && T.o(r, t) && s(r, t, a);
         return n ? h(n) : o()
     })), P = {}, w = {
         6029: () => g("default", "react", [1, 18, 2, 0]),
-        1638: () => y("default", "@jupyterlab/docregistry", [1, 4, 1, 5]),
-        1778: () => y("default", "@jupyterlab/outputarea", [1, 4, 1, 5]),
-        2425: () => y("default", "@jupyterlab/cells", [1, 4, 1, 5]),
-        3452: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
-        3471: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 5]),
+        797: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 6]),
+        1464: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        2232: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 6]),
+        2294: () => y("default", "@jupyterlab/docregistry", [1, 4, 1, 6]),
+        2818: () => g("default", "@jupyterlab/services", [1, 7, 1, 6]),
+        3195: () => y("default", "@jupyterlab/outputarea", [1, 4, 1, 6]),
+        3413: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 6]),
         3848: () => j("default", "react-query", [2, 3, 39, 0], (() => Promise.all([T.e(767), T.e(704)]).then((() => () => T(8767))))),
-        4008: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 5]),
+        4072: () => g("default", "@jupyterlab/application", [1, 4, 1, 6]),
         4882: () => g("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         4901: () => g("default", "@lumino/signaling", [1, 2, 0, 0]),
-        5326: () => g("default", "@jupyterlab/docmanager", [1, 4, 1, 5]),
+        5099: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 6]),
         5536: () => j("default", "@team-monolith/cds", [1, 1, 0, 1], (() => Promise.all([T.e(146), T.e(901), T.e(704), T.e(316)]).then((() => () => T(7210))))),
-        5962: () => g("default", "@jupyterlab/translation", [1, 4, 1, 5]),
-        6311: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
-        7217: () => g("default", "@jupyterlab/services", [1, 7, 1, 5]),
+        6805: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
+        7263: () => y("default", "@jupyterlab/cells", [1, 4, 1, 6]),
+        7594: () => g("default", "@jupyterlab/codeeditor", [1, 4, 1, 6]),
         7930: () => g("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        8048: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 5]),
         8093: () => g("default", "@jupyter/ydoc", [1, 1, 1, 1]),
         8149: () => j("default", "@emotion/styled", [1, 11, 6, 0], (() => Promise.all([T.e(505), T.e(860)]).then((() => () => T(4378))))),
-        8368: () => g("default", "@jupyterlab/application", [1, 4, 1, 5]),
-        9510: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
-        9557: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 5]),
+        8671: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
+        8937: () => g("default", "@jupyterlab/translation", [1, 4, 1, 6]),
         799: () => j("default", "@emotion/react", [1, 11, 0, 0, , "rc", 0], (() => Promise.all([T.e(146), T.e(917)]).then((() => () => T(917))))),
         5211: () => v("default", "@emotion/react", (() => Promise.all([T.e(146), T.e(917)]).then((() => () => T(917))))),
         7704: () => g("default", "react-dom", [1, 18, 2, 0]),
         718: () => j("default", "@emotion/styled", [1, 11, 8, 1], (() => Promise.all([T.e(505), T.e(893)]).then((() => () => T(4378))))),
         2148: () => j("default", "@emotion/react", [1, 11, 4, 1], (() => T.e(732).then((() => () => T(917))))),
         8800: () => j("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([T.e(505), T.e(893)]).then((() => () => T(4378))))),
         9558: () => j("default", "@emotion/react", [1, 11, 8, 2], (() => T.e(732).then((() => () => T(917)))))
     }, S = {
         29: [6029],
         316: [718, 2148, 8800, 9558],
         505: [799, 5211],
         704: [7704],
-        960: [1638, 1778, 2425, 3452, 3471, 3848, 4008, 4882, 4901, 5326, 5536, 5962, 6311, 7217, 7930, 8048, 8093, 8149, 8368, 9510, 9557]
+        960: [797, 1464, 2232, 2294, 2818, 3195, 3413, 3848, 4072, 4882, 4901, 5099, 5536, 6805, 7263, 7594, 7930, 8093, 8149, 8671, 8937]
     }, T.f.consumes = (e, r) => {
         T.o(S, e) && S[e].forEach((e => {
             if (T.o(P, e)) return r.push(P[e]);
             var t = r => {
                     P[e] = 0, T.m[e] = t => {
                         delete T.c[e], t.exports = r()
                     }
```

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/labextension/static/third-party-licenses.json` & `jupyterlab_judge-1.24.4/jupyterlab_judge/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json` & `jupyterlab_judge-1.24.4/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po` & `jupyterlab_judge-1.24.4/jupyterlab_judge/locale/ko_KR/LC_MESSAGES/jupyterlab_judge.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/commands.ts` & `jupyterlab_judge-1.24.4/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/handler.ts` & `jupyterlab_judge-1.24.4/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/index.ts` & `jupyterlab_judge-1.24.4/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/model.ts` & `jupyterlab_judge-1.24.4/src/model.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/tokens.ts` & `jupyterlab_judge-1.24.4/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/toolbar.tsx` & `jupyterlab_judge-1.24.4/src/toolbar.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/components/SubmissionArea.tsx` & `jupyterlab_judge-1.24.4/src/components/SubmissionArea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/components/SubmissionControl.tsx` & `jupyterlab_judge-1.24.4/src/components/SubmissionControl.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/components/SubmissionItem.tsx` & `jupyterlab_judge-1.24.4/src/components/SubmissionItem.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/components/SubmissionItemStatus.tsx` & `jupyterlab_judge-1.24.4/src/components/SubmissionItemStatus.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/components/SubmissionItemWait.tsx` & `jupyterlab_judge-1.24.4/src/components/SubmissionItemWait.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/components/SubmissionItemWaitStatus.tsx` & `jupyterlab_judge-1.24.4/src/components/SubmissionItemWaitStatus.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/components/SubmissionList.tsx` & `jupyterlab_judge-1.24.4/src/components/SubmissionList.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/problemProvider/HardCodedProblemProvider.ts` & `jupyterlab_judge-1.24.4/src/problemProvider/HardCodedProblemProvider.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/problemProvider/problemProvider.ts` & `jupyterlab_judge-1.24.4/src/problemProvider/problemProvider.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/widgets/JudgeOutputArea.ts` & `jupyterlab_judge-1.24.4/src/widgets/JudgeOutputArea.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/widgets/JudgePanel.ts` & `jupyterlab_judge-1.24.4/src/widgets/JudgePanel.ts`

 * *Files 1% similar despite different names*

```diff
@@ -503,15 +503,15 @@
     const prepareInput = `
 import io
 import base64
 
 def input(prompt=None):  	
     r = JUDGE_INPUT_STRING_IO.${
       problem.inputTransferType === 'one_line' ? 'readline' : 'read'
-    }()  	
+    }().rstrip('\\n')
     if not r:  		
         return ''
     return r
 
 JUDGE_INPUT_STRING_IO = io.StringIO()
 `;
     await kernel.requestExecute(
```

### Comparing `jupyterlab_judge-1.24.3/src/widgets/JudgeProblemPanel.ts` & `jupyterlab_judge-1.24.4/src/widgets/JudgeProblemPanel.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/widgets/JudgeSubmissionArea.tsx` & `jupyterlab_judge-1.24.4/src/widgets/JudgeSubmissionArea.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/src/widgets/JudgeTerminal.ts` & `jupyterlab_judge-1.24.4/src/widgets/JudgeTerminal.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/style/judgePanel.css` & `jupyterlab_judge-1.24.4/style/judgePanel.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/style/judgeTerminal.css` & `jupyterlab_judge-1.24.4/style/judgeTerminal.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/ui-tests/README.md` & `jupyterlab_judge-1.24.4/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/ui-tests/tests/jupyterlab_judge.spec.ts` & `jupyterlab_judge-1.24.4/ui-tests/tests/jupyterlab_judge.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/.gitignore` & `jupyterlab_judge-1.24.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/LICENSE` & `jupyterlab_judge-1.24.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/README.md` & `jupyterlab_judge-1.24.4/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/pyproject.toml` & `jupyterlab_judge-1.24.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_judge-1.24.3/PKG-INFO` & `jupyterlab_judge-1.24.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab_judge
-Version: 1.24.3
+Version: 1.24.4
 Dynamic: Keywords
 Summary: A simple online judge for Jupyter Lab.
 Project-URL: Homepage, https://github.com/team-monolith-product/jupyterlab-judge
 Project-URL: Bug Tracker, https://github.com/team-monolith-product/jupyterlab-judge/issues
 Project-URL: Repository, https://github.com/team-monolith-product/jupyterlab-judge.git
 Author-email: ChangHwan Lee <lch@team-mono.com>
 License: BSD 3-Clause License
```

