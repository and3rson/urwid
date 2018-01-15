# 1.4.0-beta1 release notes

  - **Andrew Dunai**

    *Mon, 15 Jan 2018 02:06:09 +0200*%nn    `f48671b306c896583bff23cb0fdfe7a055d6b05d`

        Added contributors list.


  - **Andrew Dunai**

    *Wed, 10 Jan 2018 14:56:32 +0200*%nn    `a2919015de2f016339cc7c5face9aecdc97cdb40`

        Merge pull request #271 from federicotdn/master

        Create the EventLoop abstract class, add documentation
        for signal handling

  - **Federico T**

    *Mon, 8 Jan 2018 18:18:38 -0300*%nn    `b309279e6e3bf17a7f742d8d6e81d22c2a8169cd`

        Create the EventLoop abstract class, add documentation
        for signal handling, use Python .gitignore provided by
        GitHub


  - **Andrew Dunai**

    *Sun, 7 Jan 2018 02:31:03 +0200*%nn    `1704e374ba55e6fdfe8d68870bd1781ce8afedcd`

        Merge pull request #270 from federicotdn/master

        Allow Screen class to set signal handlers using a
        function provided by the event loop

  - **Andrew Dunai**

    *Sun, 7 Jan 2018 02:24:25 +0200*%nn    `9c3d68da020b028a55d38b1061db8aacae74ba89`

        Merge pull request #151 from inducer/master

        Fix default screen size on raw display

  - **Andrew Dunai**

    *Sun, 7 Jan 2018 02:22:31 +0200*%nn    `53b5d29c2614ef0f428fd23fa4c3153bde19475e`

        Merge pull request #124 from
        KennethNielsen/graph-example-python3-fix

        Python3 fix in graph example

  - **Andrew Dunai**

    *Sun, 7 Jan 2018 02:15:55 +0200*%nn    `cd1b0b86c8c74c480e47370d03067ef4c8140ac4`

        Merge pull request #222 from
        aleufroy/221_fix_fds_release_by_raw_display

        fix: raw display should release file descriptors (issue
        #221)

  - **Andrew Dunai**

    *Sun, 7 Jan 2018 02:09:53 +0200*%nn    `eeec0d3a82f7b02c0cc03d278bc26bb985eddb47`

        Merge pull request #215 from
        abadger/linebox-can-omit-sides

        Additional linebox functionality

  - **Toshio Kuratomi**

    *Sat, 6 Jan 2018 15:59:19 -0800*%nn    `7f4060cd5cb5645153a211d3169b9f7e585586ae`

        Correct problem with defining no left line character
        breaking later widget layout


  - **Federico T**

    *Fri, 5 Jan 2018 01:49:21 -0300*%nn    `626deb940841f57d331e5a9d2f023f3461c97cb7`

        Screen class now sets signal handlers using a function
        provided by the event loop

        The Screen class used to set signal handlers using the
        signal() function from the signal standard library
        module.  This commit changes this behaviour so that the
        Screen class now uses a function provided by the active
        event loop to set signal event handlers.  This allows us
        to use GLib specific signal handling functions when
        using the GLib event loop.


  - **Andrew Dunai**

    *Thu, 4 Jan 2018 17:51:29 +0200*%nn    `6608ee2c9932d264abd1171468d833b7a4082e13`

        Update README.rst

  - **Andrew Dunai**

    *Thu, 4 Jan 2018 17:45:16 +0200*%nn    `1bf2fb7458286d2faa5413e7614a9f4731ecc8db`

        Issue & pull request templates.


  - **Andrew Dunai**

    *Thu, 4 Jan 2018 14:02:37 +0200*%nn    `3f3bff6607dfcffcdd1dee42f521287de9f8e3f7`

        Merge pull request #113 from dnaeon/doc-typos

        Typo fixes

  - **Andrew Dunai**

    *Thu, 4 Jan 2018 13:59:50 +0200*%nn    `1495adb2b666d2e0a6d1b3ed543dd6aefc449833`

        Merge pull request #175 from rr-/patch-1

        Correct error messages in Filler

  - **Andrew Dunai**

    *Thu, 4 Jan 2018 13:56:40 +0200*%nn    `cf0307c500e1d575fec5fc5a37e4ff4e69972b92`

        Python dual support (#266)

        * WIP

        * Metaclasses

        * String literal fixes

        * Remove 2to3 and make tests compatible with both Python
        2 & 3

        * Removed debug code.

        * Added tests for ProgressBar

        * Fixed examples.

        * future division & font literals fix

        * Cleaner fonts initialization.


  - **Andrew Dunai**

    *Thu, 4 Jan 2018 13:55:43 +0200*%nn    `2496a176c00eab88492f1566f2a89c58be4e15d9`

        Merge pull request #269 from
        rndusr/feature/listbox-home-end

        Feature/listbox home end

  - **Andrew Dunai**

    *Thu, 4 Jan 2018 11:06:46 +0200*%nn    `2c63148dc756168e085074bded033dfc0eae1699`

        Merge pull request #176 from rr-/patch-2

        Correct Edit documentation

  - **Toshio Kuratomi**

    *Sat, 21 Jan 2017 13:33:35 -0800*%nn    `7ce9d0d1c3205c771ef799f02add867f37326041`

        Additional listbox functionality

        * Add title_align as a new keyword argument to construct
        a ListBox.  It
         allows justifying a ListBox to the left or right in
        addition to
         centering it.  This can be useful for constructing
        columns out of
         ListBoxes.
        * Implement borderless sides.  If a ListBox is created
        with lines or
         corners set to the empty string then do not create a
        border element
         for them. This allows adjoining list boxes to share a
        single border,
         or two ListBoxes to seamlessly merge into one another.

        Fixes #211


  - **Andrew Dunai**

    *Wed, 3 Jan 2018 16:50:30 +0200*%nn    `2920475c0068d40cadd31d58650d9cfd7a1c2394`

        Merge pull request #214 from
        abadger/fix-edit-change-signal

        Emit postchange after text is updated

  - **Random User**

    *Wed, 3 Jan 2018 13:40:16 +0100*%nn    `f4204cf0e3b66ff9d215e668d3ef151b33ca878f`

        Merge branch 'feature/listbox-home-end'


  - **Andrew Dunai**

    *Wed, 3 Jan 2018 00:08:20 +0200*%nn    `6f94735e10ad10f5c750566382be97c4c9c11738`

        Merge pull request #239 from geier/strikethrough

        [RFC] New foreground setting "strikethrough"

  - **Christian Geier**

    *Wed, 31 May 2017 00:41:26 +0200*%nn    `6933bedd953cdaa2ffafa800cccb23eff8177393`

        Support for new foreground setting "strikethrough"

        If you are unsure if your terminal supports this, try
        the following:

        echo -e "\e[9mstrikethrough\e[0m"


  - **Andrew Dunai**

    *Tue, 2 Jan 2018 17:32:26 +0200*%nn    `ab6bfbcaf0ff2326e3392d7895fb1aaee5bbb167`

        Merge pull request #220 from jwilk-forks/master

        Fix typos

  - **Andrew Dunai**

    *Tue, 2 Jan 2018 15:03:13 +0200*%nn    `8ba8d0bec070180c459679e7c84f0d174235061f`

        Added .tox to ignore.


  - **Andrew Dunai**

    *Tue, 2 Jan 2018 14:47:51 +0200*%nn    `70781ad8fa79cc1bfcb8caf446ee0162ca2880c0`

        Added coveralls dependency


  - **Andrew Dunai**

    *Tue, 2 Jan 2018 14:44:12 +0200*%nn    `a36a1f4fbcc7afe7a6ad878004e969dd5ad54c64`

        Tox + Travis


  - **Andrew Dunai**

    *Tue, 2 Jan 2018 14:40:02 +0200*%nn    `5d179614b558e48a3fe1704f005ad5b3e47b3d67`

        Refactoring tox.ini


  - **Andrew Dunai**

    *Tue, 2 Jan 2018 14:37:02 +0200*%nn    `3409aa26e159be1d5315fabd977f69c7b73cd704`

        Added tox to simplify local testing.


  - **Andrew Dunai**

    *Tue, 2 Jan 2018 14:16:09 +0200*%nn    `69a6fe7da1dd543337f5aeef53b34d933bed3b69`

        Coveragerc


  - **Andrew Dunai**

    *Tue, 2 Jan 2018 14:12:29 +0200*%nn    `40cd687b25a818b264a155561e545456d4b5beae`

        Updated coverage command


  - **Andrew Dunai**

    *Tue, 2 Jan 2018 14:10:44 +0200*%nn    `fe2ac25272e8cc94b2f79364cbffa444caead2ed`

        Fixed typo in coverage badge URL.


  - **Andrew Dunai**

    *Tue, 2 Jan 2018 14:09:37 +0200*%nn    `268975b5b0145400f75615a78835f8441ab635ca`

        Added coverage + coveralls


  - **Andrew Dunai**

    *Tue, 2 Jan 2018 13:44:48 +0200*%nn    `0e1e6a8225af12865b74871ca17505c10644be82`

        Merge pull request #255 from geier/blink

        Mention blink and italics attributes in manual.

  - **Andrew Dunai**

    *Tue, 2 Jan 2018 13:43:41 +0200*%nn    `877128f956e10a0f746483f1dadaf3e8a2fa1a58`

        Merge pull request #260 from larsks/feature/py3

        python 3 compatibility changes

  - **xndcn**

    *Tue, 2 Jan 2018 19:39:18 +0800*%nn    `f5be3db8aba792307bb8a35aeba0b5e391268f41`

        ListBox: Modify inside docs of `keypress` method. (#257)

        Since from f5f6711 now `page up` and `page down` will be
        also handled by widget in focus, so the documents inside
        the `keypress` method have to be modified to avoid
        confusing.

  - **Andrew Dunai**

    *Tue, 2 Jan 2018 13:35:01 +0200*%nn    `86eb95edd5345435658ef7e62f9a6ce248aa3ba4`

        Fixed issue with Unicode characters in ProgressBar
        (#261)

        * Fixed issue with unicode characters in ProgressBar

        * Fixed Travis build - replaced deprecated
        3.2_with_system_site_packages with
        3.4_with_system_site_packages.

        * Fixed typo.

        * Fixing build for Python 3.2

        * Fix for Python 3.2 & tornado/twisted

        * Setup script update in regards to #216

        * Travis fix

        * Dependencies for Travis

        * Removed Python 3.2 from Travis dependency list as
        deprecated

        * Regression fix.

        * Removed bogus lines.

        * Docs.


  - **Ian Ward**

    *Mon, 1 Jan 2018 14:00:06 +0800*%nn    `a38178441f35cd0c23654896378823a62c874535`

        Urwid is looking for new maintainers

  - **Lars Kellogg-Stedman**

    *Sat, 23 Dec 2017 08:11:05 -0500*%nn    `31e9c2732721f0bc1aa27b74f065491e660898c8`

        python 3 compatibility changes

        this updates the syntax in many of the examples so that
        they run under both python 2 and python 3.


  - **Christian Geier**

    *Tue, 26 Sep 2017 23:30:28 +0200*%nn    `609d9527dddda0102306a5b6724c38c04a74779a`

        Mention blink and italics attributes in manual.


  - **Ian Ward**

    *Tue, 22 Aug 2017 14:32:39 -0400*%nn    `c29b072e1f6df12e237a1294e249943222879536`

        Merge pull request #243 from Sjc1000/master

        Fixed Terminal widget crashes with Python3

  - **Ian Ward**

    *Tue, 22 Aug 2017 14:31:25 -0400*%nn    `1a6772e426d0201920a1542a5d88bfbd289374f2`

        Merge pull request #249 from Lothiraldan/cleaning

        Small style cleaning of ParentNode.set_child_node

  - **Ian Ward**

    *Tue, 22 Aug 2017 14:30:46 -0400*%nn    `09d1107ea7106f4f2b18cbe20a8b28e4618edeeb`

        Merge pull request #248 from waveform80/master

        Fix #246, fix #234

  - **Boris Feld**

    *Mon, 21 Aug 2017 20:55:52 +0200*%nn    `4ccbb3c4679904348852a9ab68277636be6d5ecd`

        Small style cleaning of ParentNode.set_child_node


  - **Dave Jones**

    *Sun, 20 Aug 2017 20:26:44 +0100*%nn    `6f9d01e527a69eb8ea58277b3e9488c96d76c8dc`

        Fix #246, fix #234

        Adjusts the internal representation of an alarm in
        SelectEventLoop to include a "tie-break" value prior to
        the callback (as recommended in the heapq documentation)
        to prevent TypeError when comparing two different
        callbacks. Also tweaks SelectEventLoop to use
        heapq.heappop instead of list.pop for retrieving the
        next alarm, to maintain the heap structure of the alarm
        list.


  - **Ian Ward**

    *Wed, 26 Jul 2017 19:53:12 -0400*%nn    `f406b0eb410ad3a732e28e613860dab4ac269c15`

        Merge pull request #244 from mobyte0/master

        fixed docstring typo

  - **mobyte0**

    *Wed, 26 Jul 2017 12:36:42 -0400*%nn    `2e6395d4e35807273dae0de11bc75259dcdb5671`

        fixed docstring typo


  - **Sjc1000**

    *Tue, 18 Jul 2017 10:20:52 +1000*%nn    `d32f8643b543c590ecd8bbd12433205f5ef35ee3`

        Fixed Terminal widget crashes with Python3


  - **Ian Ward**

    *Tue, 4 Jul 2017 08:46:45 -0400*%nn    `b44ce386c981c7e7ff344db3973d3c69a8244a56`

        Merge pull request #237 from floppym/test-vterm-EINTR

        test_vterm: handle EINTR when reading from pipe

  - **Ian Ward**

    *Mon, 26 Jun 2017 13:54:52 -0400*%nn    `fa86c560d390253de77a96767006e0fd3d3ad7e6`

        Merge pull request #241 from mimi1vx/patch-1

        Update travis to check python 3.6

  - **Ondřej Súkup**

    *Mon, 26 Jun 2017 19:22:45 +0200*%nn    `4e2af0433a8b633d2c5f6f714396ba42e3cc1e9d`

        Update travis to check python 3.6

        python-2.6 is out of support and some distributions
        moving to python-3.6

  - **Ian Ward**

    *Wed, 7 Jun 2017 20:23:34 -0400*%nn    `949f4ec91a0a4700c9784dc6e382e02e23a807f7`

        Merge pull request #238 from mwhudson/issue-164

        fix test_remove_watch_file flakiness

  - **Michael Hudson-Doyle**

    *Wed, 7 Jun 2017 13:52:17 -0700*%nn    `4b0ed8b6030450e6d99909a7c683e9642e546387`

        fix test_remove_watch_file flakiness

        pass a known-good file descriptor to watch_file rather
        than hard-coding 5

        Fixes #164


  - **Mike Gilbert**

    *Sat, 3 Jun 2017 14:53:51 -0400*%nn    `f68f2cf089cfd5ec45863baf59a91d5aeb0cf5c3`

        test_vterm: handle EINTR when reading from pipe

        Fixes: https://github.com/urwid/urwid/issues/230


  - **Ian Ward**

    *Wed, 24 May 2017 12:44:47 -0400*%nn    `e06c76d0ad59bb34180e28deafd07c87fdc9066c`

        Merge pull request #207 from
        zrax/SimpleFocusListWalker_modified

        Fix missing `modified` signal in SimpleFocusListWalker

  - **Ian Ward**

    *Wed, 17 May 2017 08:17:26 -0400*%nn    `f5f671158a4006e45f47b84c0c6baaa56b7a43b8`

        Merge pull request #233 from
        rndusr/feature/listbox-forward-page-updown

        ListBox: Offer page up/down keys to focused widget

  - **Random User**

    *Wed, 17 May 2017 13:57:47 +0200*%nn    `a5109c3f1118f6f5a640983cae3d4344c4c9986a`

        ListBox: Offer page up/down keys to focused widget

        Child widgets of ListBoxes get all keys before ListBox
        uses them, including
        'page up' and 'page down'.


  - **Random User**

    *Sat, 29 Apr 2017 15:54:50 +0200*%nn    `b06439fa83624ff6523e37e4a85ee9e6dce43256`

        Add support for keys 'home' and 'end' to ListBox

        Pressing 'home' moves the focus to the first position,
        'end' moves focus to the last position.


  - **Ian Ward**

    *Mon, 24 Apr 2017 11:10:18 -0400*%nn    `c56f1f45bcbf963d977019455156372e4124e6db`

        Merge pull request #228 from
        rndusr/dont-use-pollinglistwalker

        Default to SimpleListWalker when setting ListBox.body

  - **Random User**

    *Mon, 24 Apr 2017 16:43:51 +0200*%nn    `e3db663643ae97866c1f790fa3c5397fb160af38`

        Default to SimpleListWalker when setting ListBox.body

        PollingListWalker is deprecated.


  - **Ian Ward**

    *Tue, 11 Apr 2017 07:56:14 -0400*%nn    `b099582caed8ce75aaba8d9198e76fedc64f8916`

        Merge pull request #219 from tonycpsu/master

        Workaround to get Travis working again.

  - **Alain Leufroy**

    *Thu, 16 Mar 2017 10:53:10 +0100*%nn    `95e3b328c637367176e53440a4f5cfac6efb0718`

        fix: raw display should release file descriptors (issue
        #221)

        `raw_display.Screen.hook_event_loop` does not fill
        `self._current_event_loop_handles` with handled file
        descriptors. So, `raw_display.Screen.hook_event_loop`
        can not release then.


  - **Jakub Wilk**

    *Tue, 28 Feb 2017 00:35:45 +0100*%nn    `f19850d0a005bf6f6313d22ee6a9df709ec6777b`

        Fix typos


  - **Tony Cebzanov**

    *Wed, 22 Feb 2017 20:33:47 -0500*%nn    `cf177d07be7767b5eb5f1588ad95925da8ba1b27`

        Workaround to get Travis working again.

        * The Travis environment "2.7_with_system_site_packages"
        has Python 2.7.3
         installed, but recent updates to twisted require an
        update to 2.7.9.
        * Explicitly pointing at twisted==16.6.0 when testing
        Python 2.7 seems to fix
         the problem.


  - **Ian Ward**

    *Wed, 22 Feb 2017 16:30:09 -0500*%nn    `fa4ca85f12092cd11a5e118053b4a9dd1bbb058b`

        Merge pull request #218 from EdwardBetts/master

        correct spelling mistakes

  - **Edward Betts**

    *Wed, 22 Feb 2017 08:04:17 +0000*%nn    `f72c4dc7685889ba8f3234048e79084da89d5a0a`

        correct spelling mistakes


  - **Toshio Kuratomi**

    *Sat, 21 Jan 2017 18:12:52 -0800*%nn    `2dcc541c0130d3ed3854c60ff30381fcc3406349`

        checkbox and radiobutton also needs to have a postchange
        event

        Just like Edit() boxes, CheckBox and RadioButton need to
        have an event emitted after the change has been
        commited.  This allows us to modify the state after it
        occurs.  (If the event only fires before the state is
        actually changed, the event handler cannot change the
        state because the emitter will change it to what they
        were going to after the event handler has finished.


  - **Toshio Kuratomi**

    *Sat, 21 Jan 2017 14:47:14 -0800*%nn    `4f85c63becc3267241b5940b32ed586a4da304a9`

        Implement postchange signal for Edit widget.

        The Edit widget in 1.3.0 has a "change" signal which
        fires before the edit_text is updated.  This means that
        change signal handlers cannot update the edit_text; the
        text is updated by the signal emitter after the change
        handler has finished running.  To remedy this, in a
        backwards compatible way, create a second signal,
        "postchange" which fires after edit_text has been
        changed.  "postchange" sends the widget's old text value
        as a parameter so that change handlers can use the
        former value if needed (for instance, to revert a change
        because the new_text was invalid)


  - **Toshio Kuratomi**

    *Sat, 21 Jan 2017 13:03:40 -0800*%nn    `cad6c144bf9940aa672611a36f2174655c579af7`

        Do not emit change until after text is updated

        Sometimes an Edit's change handler wants to edit the
        text that has just been entered.  For instance, if the
        handler does validation, it may want to immediately
        highlight or prevent invalid entries from being shown.
        This is not possible if the change signal is emitted
        before the internal text data is updated as the update
        will overwrite anything that the change handler
        performed.  Emitting the change event after the update
        has been performed allows for changes to be made.

        Fixes #212


  - **Ian Ward**

    *Wed, 21 Dec 2016 10:44:29 -0500*%nn    `fee50e77e85fb0fc5f7d664ae13c0e139d711a00`

        Merge pull request #210 from
        rndusr/listbox-body-property

        Make ListBox.body an invalidating property

  - **Random User**

    *Wed, 21 Dec 2016 14:22:49 +0100*%nn    `e47c6b27ee2ed2d290ab31ac415ff3b84fbfee6a`

        Use internal '_body' attribute instead of new 'body'
        property

        This should be slightly more efficient.


  - **Random User**

    *Wed, 21 Dec 2016 14:19:46 +0100*%nn    `926546596d36b5961fe709fc9afbfd4d8bbbf348`

        Make ListBox.body a property

        This lets us automatically call _invalidate() each time
        the list box's body is set.


  - **Michael Hansen**

    *Fri, 11 Nov 2016 14:39:01 -0800*%nn    `18eb5db0355ec46ecbf7be9b2c1ef642c9fb72d2`

        Fix missing `modified` signal in SimpleFocusListWalker


  - **Ian Ward**

    *Tue, 16 Aug 2016 13:56:09 -0400*%nn    `dc8e8b3fdb0bed9fe6cf8781b4c0b1396b7d406f`

        Merge pull request #201 from marlox-ouda/master

        fix iterator in WidgetContainerListContentsMixin

  - **Marlox**

    *Tue, 16 Aug 2016 19:33:34 +0200*%nn    `159d7dcd1d264f7dae2241e993833673d2f3dcbf`

        Merge branch 'master' of https://github.com/urwid/urwid


  - **Ian Ward**

    *Tue, 16 Aug 2016 07:31:38 -0400*%nn    `8facdd93f83c5cdc323d570eee4dee9ab7de0b07`

        Merge pull request #202 from marlox-ouda/fix-travis

         Fix travis

  - **Marlox**

    *Tue, 16 Aug 2016 07:13:42 +0200*%nn    `f7c6370667a3e3784c2a4eb5a318964ce848c177`

        .travis.yml: Fix 3.2 tests (again shell escape bug)


  - **Marlox**

    *Tue, 16 Aug 2016 06:51:32 +0200*%nn    `942c6cc46ea0495f58b273d9281911583d737f39`

        Revert ".travis.yml: removing '--use-mirrors' option in
        'pip install'"

        This reverts commit
        bc4aecc71708c406c1d59a035002929b8360b643.

        Travis fix is done in fix-travis branch I prefer to mix
        it and do not mix the issues.


  - **Marlox**

    *Tue, 16 Aug 2016 06:42:29 +0200*%nn    `60741af8cbb8ff11b2cc6d09c6e5fdf0ff9d7b72`

        setup.py: show that python version 3.5 is supported


  - **Marlox**

    *Tue, 16 Aug 2016 06:33:06 +0200*%nn    `7ac208ecd9e89e12d3f02c87d100f2484c1f005b`

        .travis.yml: Add support of python version 3.5 in
        travis. Same dependancies of python versions 3.3 and 3.4
        are used.


  - **Marlox**

    *Tue, 16 Aug 2016 06:22:11 +0200*%nn    `1cf11493419672326013d312624b10f6915ea193`

        .travis.yml: Fix 3.2 tests by imposing tornado<=4.3.0
        with python 3.2 see
        https://allmychanges.com/p/python/tornado 4.4.0 and
        4.3.0
         4.3.0 is the last version of tornado that supports
        python 3.2


  - **Marlox**

    *Tue, 16 Aug 2016 06:03:05 +0200*%nn    `bb0472aae2352dc76cfdfccad501c9d9673b3aba`

        Add support of python version 3.4 in travis. Same
        dependancy of python version 3.3 is used.


  - **Marlox**

    *Tue, 16 Aug 2016 05:45:12 +0200*%nn    `a58d0e1c50459d27db03dab927c3437b08842735`

        .travis.yml: removing '--use-mirrors' option in 'pip
        install' see: https://pip.pypa.io/en/stable/news version
        7.0.0
        -> remove of the deprecated [...] --use-mirrors [...]
        options


  - **Marlox**

    *Tue, 16 Aug 2016 05:33:20 +0200*%nn    `bc4aecc71708c406c1d59a035002929b8360b643`

        .travis.yml: removing '--use-mirrors' option in 'pip
        install'

        see: https://pip.pypa.io/en/stable/news version 7.0.0
         -> remove of the deprecated [...] --use-mirrors [...]
        options


  - **Marlox**

    *Mon, 15 Aug 2016 13:03:15 +0200*%nn    `982726ef8f48a1dc156b6b7caf7296d1c596530e`

        fix iterator in WidgetContainerListContentsMixin
         (x)range is an iterable
         __iterator__ should return an iterator (iter(iterable))


  - **Ian Ward**

    *Thu, 9 Jun 2016 11:05:34 -0400*%nn    `9a29c4ebd521ae0a3759d72b2ac330d7912289ef`

        Merge pull request #122 from ids1024/master

        Implement italics support

  - **Ian Ward**

    *Fri, 27 May 2016 07:08:57 -0400*%nn    `b91f12e3f9ffdf9eb594d634449c50b7ba0712f8`

        Merge pull request #191 from jwilk/string-formatting

        Fix string formatting error

  - **Jakub Wilk**

    *Fri, 27 May 2016 00:00:35 +0200*%nn    `68794d192c39cda419b31bfa4af37f26f1bf3ea3`

        Fix string formatting error


  - **Ian Ward**

    *Thu, 28 Apr 2016 09:08:30 -0400*%nn    `d72c1545f0d66bb0a9dac863a58a0d135098b5b2`

        fix subscribe link


  - **Marcin Kurczewski**

    *Sun, 14 Feb 2016 14:56:07 +0100*%nn    `84257ce849ca6ef36736ce4f35951a6787ac5a00`

        Correct Edit documentation

        There were missing doc comments for a few basic
        properties, + the text about `edit_text` property being
        a read-only property was a lie.

  - **Marcin Kurczewski**

    *Sun, 14 Feb 2016 13:43:17 +0100*%nn    `8bb2e7f058579366781cd5664de5f8949e14b5c4`

        Correct error messages in Decoration

        The error message talks about conditions for `fixed
        bottom` argument to be valid, when the argument is set
        to `fixed top`. This doesn't seem right.

  - **Ian Ward**

    *Fri, 12 Feb 2016 08:23:58 -0500*%nn    `5c7bff3d381e855b483b7b65688ce2d4f53cdd1b`

        Merge pull request #174 from aszlig/vterm-fix-nul

        vterm: Fix handling of NUL characters

  - **aszlig**

    *Thu, 11 Feb 2016 03:14:07 +0100*%nn    `701138a380fac06023e5915448af92ba13614cb9`

        vterm: Fix handling of NUL characters

        According to the VT100 programmers manual, the NUL
        character has to be ignored (at least on our side,
        because we are not a printer):

        http://vt100.net/docs/tp83/appendixb.html

        According to the bug reporter the VMS console driver
        inserts NUL characters after line feeds and our
        implementation prints those as "?".

        Tested against Python 2.7, 3.2, 3.3, 3.4 and 3.5.

        Signed-off-by: aszlig <aszlig@redmoonstudios.org>
        Reported-by: Robert Urban <urban@unix-beratung.de>


  - **Ian Ward**

    *Sat, 6 Feb 2016 13:55:22 -0500*%nn    `c6d79bfe0ecd7dac2873e906f62a977dc41b19bd`

        Merge pull request #173 from mgk/master

        fix #172 - html_fragment errors on Python 3.4

  - **Michael Keirnan**

    *Fri, 5 Feb 2016 23:23:40 -0500*%nn    `88f7e520b3e0a1fa2f820ff02a0b679e54457da0`

        fix #172 - html_fragment errors on Python 3.4


  - **Ian Ward**

    *Tue, 29 Dec 2015 21:44:26 -0500*%nn    `35cfcf387fe4c78d3f0cc7338f882f61a8d2254f`

        Merge pull request #167 from techtonik/patch-1

        indexcontent.html: Fix links after move to urwid/urwid

  - **anatoly techtonik**

    *Wed, 30 Dec 2015 01:30:24 +0300*%nn    `ce530761558874965f6c12b0199a551195982d9d`

        .travis.yml: Quote version specifier for Twisted

  - **anatoly techtonik**

    *Wed, 30 Dec 2015 01:22:49 +0300*%nn    `e048a539a5e7109f4eec878e7ddace8fd645faa7`

        .travis.yml: Another try to fix tests on Twisted

        Wrong cause

  - **anatoly techtonik**

    *Wed, 30 Dec 2015 01:15:36 +0300*%nn    `592909621ec9f265acc137e81401ce3922efd029`

        .travis.yml: Try to fix tests on Twisted

        Twisted 15.4 is the last with Python 2.6 support

  - **anatoly techtonik**

    *Wed, 30 Dec 2015 01:03:17 +0300*%nn    `d0a12c8cf00d5af7c97312a66e43a70b45f1d103`

        .travis.yml: Attempt to fix failing build

        Build: https://travis-ci.org/urwid/urwid/jobs/99337959
        Fix: https://github.com/travis-ci/travis-ci/issues/5221

  - **anatoly techtonik**

    *Wed, 30 Dec 2015 00:59:27 +0300*%nn    `933c97e8980bfcbdf185dea72774356e0b7da406`

        Merge pull request #1 from techtonik/master

        .travis.yml: Fix links after move to urwid/urwid

  - **anatoly techtonik**

    *Wed, 30 Dec 2015 00:54:38 +0300*%nn    `5b2cab2a652df0fe45c53053cdb3551665f3655b`

        .travis.yml: Fix links after move to urwid/urwid

  - **anatoly techtonik**

    *Tue, 29 Dec 2015 22:23:58 +0300*%nn    `22f4c91429aca4fbf7b1b99f0e14d8c96bb02036`

        indexcontent.html: Fix links after move to urwid/urwid

  - **Ian Ward**

    *Sat, 19 Dec 2015 15:01:42 -0500*%nn    `ff20bde4fc23cc8533d94d442818ae73f3666ae1`

        new mailing list location


  - **Ian Ward**

    *Sun, 1 Nov 2015 19:32:17 -0500*%nn    `3e8ad9ed8799ef3ccc37e9b77c002990c11ad985`

        Merge pull request #142 from grzaks/master

        fix for issue #141

  - **Ian Ward**

    *Sun, 1 Nov 2015 19:30:40 -0500*%nn    `1af52f86dd32da343fe6284c02ba2fae6e69ba2d`

        Merge pull request #158 from benjamin9999/fbterm

        256-color support for fbterm

  - **Benjamin Yates**

    *Sun, 18 Oct 2015 09:45:49 -0400*%nn    `9c734df4335f6f4e111d696109648e0cefa8542f`

        Add 256-color support for fbterm

        fbterm supports an analog of xterm's 256 color method,
        but due to overlap in the control codes, it uses
        different escape sequences. Since urwid doesn't use
        terminfo, it has to be coded in the raw_display
        directly.

        The call to register_palette_entry() during __init__ was
        moved because it now relies on the self.term attribute,
        and was previously being invoked before the class was
        fully initialized.


  - **Benjamin Yates**

    *Sun, 18 Oct 2015 09:43:24 -0400*%nn    `183cfa59045bf549be52fdce0e62b1520438ba52`

        Store envron's TERM value as a Screen attribute


  - **Andreas Klöckner**

    *Tue, 15 Sep 2015 03:07:45 -0500*%nn    `6120a99b8ca28c790d5c79e8c6154786a53c8dbf`

        Fix default screen size on raw display

  - **Grzegorz Aksamit**

    *Sat, 18 Jul 2015 00:12:55 +0200*%nn    `f520e211dd8c1d99a78d8419745d603a5f03c7ad`

        fix for issue #141


  - **Kenneth Nielsen**

    *Mon, 27 Apr 2015 08:52:25 +0200*%nn    `ccb5e8c1d9c1cf1baccee0278a5baa9763afbc4b`

        Python3 fix in graph example


  - **Ian D. Scott**

    *Sun, 19 Apr 2015 10:50:49 -0700*%nn    `3ed95e411c071665b980990a75e507c5fa5de07e`

        Implement italics support


  - **Marin Atanasov Nikolov**

    *Tue, 24 Feb 2015 14:05:16 +0200*%nn    `7dea88aa72e4ee25f7b548e47249f75efa4a01ca`

        Typo fixes


Output generated by:

    git log --pretty="  - **%aN**%n%n    *%aD*%%nn    \`%H\`%n%n%w(64,8,8)%B%n" release-1.3.1..HEAD > CHANGELOG.md

