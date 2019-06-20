//<![CDATA[
$(document)['ready'](function() {
    $('#main-menu')['each'](function() {
        var _0x9631x2 = $(this)['find']('.LinkList ul > li')['children']('a'),
            _0x9631x3 = _0x9631x2['length'];
        for (var _0x9631x4 = 0; _0x9631x4 < _0x9631x3; _0x9631x4++) {
            var _0x9631x5 = _0x9631x2['eq'](_0x9631x4),
                _0x9631x6 = _0x9631x5['text']();
            if (_0x9631x6['charAt'](0) !== '_') {
                var _0x9631x7 = _0x9631x2['eq'](_0x9631x4 + 1),
                    _0x9631x8 = _0x9631x7['text']();
                if (_0x9631x8['charAt'](0) === '_') {
                    var _0x9631x9 = _0x9631x5['parent']();
                    _0x9631x9['append']('<ul class="sub-menu m-sub"/>')
                }
            };
            if (_0x9631x6['charAt'](0) === '_') {
                _0x9631x5['text'](_0x9631x6['replace']('_', ''));
                _0x9631x5['parent']()['appendTo'](_0x9631x9['children']('.sub-menu'))
            }
        };
        for (var _0x9631x4 = 0; _0x9631x4 < _0x9631x3; _0x9631x4++) {
            var _0x9631xa = _0x9631x2['eq'](_0x9631x4),
                _0x9631xb = _0x9631xa['text']();
            if (_0x9631xb['charAt'](0) !== '_') {
                var _0x9631xc = _0x9631x2['eq'](_0x9631x4 + 1),
                    _0x9631xd = _0x9631xc['text']();
                if (_0x9631xd['charAt'](0) === '_') {
                    var _0x9631xe = _0x9631xa['parent']();
                    _0x9631xe['append']('<ul class="sub-menu2 m-sub"/>')
                }
            };
            if (_0x9631xb['charAt'](0) === '_') {
                _0x9631xa['text'](_0x9631xb['replace']('_', ''));
                _0x9631xa['parent']()['appendTo'](_0x9631xe['children']('.sub-menu2'))
            }
        };
        $('#main-menu ul li ul')['parent']('li')['addClass']('has-sub');
        $('#main-menu .widget')['addClass']('show-menu')
    });
    $('#main-menu-nav')['clone']()['appendTo']('.mobile-menu');
    $('.mobile-menu .has-sub')['append']('<div class="submenu-toggle"/>');
    $('.slide-menu-toggle, .overlay')['on']('click', function() {
        $('body')['toggleClass']('nav-active');
        $('.overlay')['fadeToggle'](170)
    });
    $('.mobile-menu ul li .submenu-toggle')['on']('click', function(_0x9631xf) {
        if ($(this)['parent']()['hasClass']('has-sub')) {
            _0x9631xf['preventDefault']();
            if (!$(this)['parent']()['hasClass']('show')) {
                $(this)['parent']()['addClass']('show')['children']('.m-sub')['slideToggle'](170)
            } else {
                $(this)['parent']()['removeClass']('show')['find']('> .m-sub')['slideToggle'](170)
            }
        }
    });
    $('.show-search, .show-mobile-search')['on']('click', function() {
        $('#nav-search, .mobile-search-form')['fadeIn'](250)['find']('input')['focus']()
    });
    $('.hide-search, .hide-mobile-search')['on']('click', function() {
        $('#nav-search, .mobile-search-form')['fadeOut'](250)['find']('input')['blur']()
    });
    $('.Label a, a.b-label')['attr']('href', function(_0x9631xf, _0x9631x10) {
        return _0x9631x10['replace'](_0x9631x10, _0x9631x10 + '?&max-results=' + postPerPage)
    });
    $('.avatar-image-container img')['attr']('src', function(_0x9631xf, _0x9631x4) {
        _0x9631x4 = _0x9631x4['replace']('/s35-c/', '/s45-c/');
        _0x9631x4 = _0x9631x4['replace']('//img1.blogblog.com/img/blank.gif', '//4.bp.blogspot.com/-uCjYgVFIh70/VuOLn-mL7PI/AAAAAAAADUs/Kcu9wJbv790hIo83rI_s7lLW3zkLY01EA/s55-r/avatar.png');
        return _0x9631x4
    });
    $('.index-post .post-image-link img')['attr']('src', function(_0x9631xf, _0x9631x4) {
        _0x9631x4 = _0x9631x4['replace']('https://4.bp.blogspot.com/-O3EpVMWcoKw/WxY6-6I4--I/AAAAAAAAB2s/KzC0FqUQtkMdw7VzT6oOR_8vbZO6EJc-ACK4BGAYYCw/w680/nth.png', noThumbnail);
        return _0x9631x4
    });
    $('.author-description a')['each'](function() {
        $(this)['attr']('target', '_blank')
    });
    $('.post-nav')['each'](function() {
        var _0x9631x11 = $('a.prev-post-link')['attr']('href'),
            _0x9631x12 = $('a.next-post-link')['attr']('href');
        $['ajax']({
            url: _0x9631x11,
            type: 'get',
            success: function(_0x9631x13) {
                var _0x9631x14 = $(_0x9631x13)['find']('.blog-post h1.post-title')['text']();
                $('.post-prev a .post-nav-inner p')['text'](_0x9631x14)
            }
        });
        $['ajax']({
            url: _0x9631x12,
            type: 'get',
            success: function(_0x9631x15) {
                var _0x9631x14 = $(_0x9631x15)['find']('.blog-post h1.post-title')['text']();
                $('.post-next a .post-nav-inner p')['text'](_0x9631x14)
            }
        })
    });
    $('.post-body strike')['each'](function() {
        var _0x9631xf = $(this),
            _0x9631x16 = _0x9631xf['text']();
        if (_0x9631x16['match']('left-sidebar')) {
            _0x9631xf['replaceWith']('<style>.item #main-wrapper{float:right;padding:0 0 0 25px}.item #sidebar-wrapper{float:left}</style>')
        };
        if (_0x9631x16['match']('right-sidebar')) {
            _0x9631xf['replaceWith']('<style>.item #main-wrapper{float:left;padding:0 25px 0 0}.item #sidebar-wrapper{float:right}</style>')
        };
        if (_0x9631x16['match']('full-width')) {
            _0x9631xf['replaceWith']('<style>.item #main-wrapper{width:100%;padding:0}.item #sidebar-wrapper{display:none}</style>')
        }
    });
    $('#main-wrapper, #sidebar-wrapper')['each'](function() {
        if (fixedSidebar == true) {
            $(this)['theiaStickySidebar']({
                additionalMarginTop: 25,
                additionalMarginBottom: 25
            })
        }
    });
    $('.back-top')['each'](function() {
        var _0x9631xf = $(this);
        $(window)['on']('scroll', function() {
            $(this)['scrollTop']() >= 100 ? _0x9631xf['fadeIn'](250) : _0x9631xf['fadeOut'](250)
        }), _0x9631xf['click'](function() {
            $('html, body')['animate']({
                scrollTop: 0
            }, 500)
        })
    });
    $('#main-menu #main-menu-nav li')['each'](function() {
        var _0x9631x17 = $(this),
            _0x9631x18 = _0x9631x17['find']('a')['attr']('href')['trim'](),
            _0x9631xf = _0x9631x17,
            _0x9631x16 = _0x9631x18['toLowerCase'](),
            _0x9631x19 = _0x9631x18['split']('/'),
            _0x9631x1a = _0x9631x19[0];
        _0x9631x2e(_0x9631xf, _0x9631x16, 5, _0x9631x1a)
    });
    $('#hot-section .widget-content')['each'](function() {
        var _0x9631xf = $(this),
            _0x9631x18 = _0x9631xf['text']()['trim'](),
            _0x9631x16 = _0x9631x18['toLowerCase'](),
            _0x9631x19 = _0x9631x18['split']('/'),
            _0x9631x1a = _0x9631x19[0];
        _0x9631x2e(_0x9631xf, _0x9631x16, 6, _0x9631x1a)
    });
    $('.featured-posts .widget-content')['each'](function() {
        var _0x9631xf = $(this),
            _0x9631x18 = _0x9631xf['text']()['trim'](),
            _0x9631x16 = _0x9631x18['toLowerCase'](),
            _0x9631x19 = _0x9631x18['split']('/'),
            _0x9631x1b = _0x9631x19[0],
            _0x9631x1a = _0x9631x19[1];
        _0x9631x2e(_0x9631xf, _0x9631x16, _0x9631x1b, _0x9631x1a)
    });
    $('.common-widget .widget-content')['each'](function() {
        var _0x9631xf = $(this),
            _0x9631x18 = _0x9631xf['text']()['trim'](),
            _0x9631x16 = _0x9631x18['toLowerCase'](),
            _0x9631x19 = _0x9631x18['split']('/'),
            _0x9631x1b = _0x9631x19[0],
            _0x9631x1a = _0x9631x19[1];
        _0x9631x2e(_0x9631xf, _0x9631x16, _0x9631x1b, _0x9631x1a)
    });
    $('.related-ready')['each'](function() {
        var _0x9631xf = $(this),
            _0x9631x1a = _0x9631xf['find']('.related-tag')['data']('label');
        _0x9631x2e(_0x9631xf, 'related', 3, _0x9631x1a)
    });

    function _0x9631x1c(_0x9631x1d, _0x9631x4) {
        for (var _0x9631x1e = 0; _0x9631x1e < _0x9631x1d[_0x9631x4]['link']['length']; _0x9631x1e++) {
            if (_0x9631x1d[_0x9631x4]['link'][_0x9631x1e]['rel'] == 'alternate') {
                var _0x9631x1f = _0x9631x1d[_0x9631x4]['link'][_0x9631x1e]['href'];
                break
            }
        };
        return _0x9631x1f
    }

    function _0x9631x20(_0x9631x1d, _0x9631x4, _0x9631x1f, _0x9631x21) {
        var _0x9631x22 = _0x9631x1d[_0x9631x4]['title']['$t'],
            _0x9631x23 = '<a href="' + _0x9631x1f + '"><span class="title-text">' + _0x9631x22 + '</span>' + _0x9631x21 + '</a>';
        return _0x9631x23
    }

    function _0x9631x24(_0x9631x1d, _0x9631x4) {
        var _0x9631x25 = _0x9631x1d[_0x9631x4]['published']['$t'],
            _0x9631x26 = _0x9631x25['substring'](0, 4),
            _0x9631x27 = _0x9631x25['substring'](5, 7),
            _0x9631x28 = _0x9631x25['substring'](8, 10),
            _0x9631x29 = monthFormat[parseInt(_0x9631x27, 10) - 1] + ' ' + _0x9631x28 + ', ' + _0x9631x26,
            _0x9631x23 = '<span class="post-date">' + _0x9631x29 + '</span>';
        return _0x9631x23
    }

    function _0x9631x2a(_0x9631x1d, _0x9631x4) {
        var _0x9631x22 = _0x9631x1d[_0x9631x4]['title']['$t'],
            _0x9631x2b = _0x9631x1d[_0x9631x4]['content']['$t'],
            _0x9631x2c = $('<div>')['html'](_0x9631x2b);
        if ('media$thumbnail' in _0x9631x1d[_0x9631x4]) {
            var _0x9631x2d = _0x9631x1d[_0x9631x4]['media$thumbnail']['url']['replace']('/s72-c', '/w72')
        } else {
            if (_0x9631x2b['indexOf']('<img') > -1) {
                _0x9631x2d = _0x9631x2c['find']('img:first')['attr']('src')
            } else {
                _0x9631x2d = noThumbnail
            }
        };
        var _0x9631x23 = '<img class="post-thumb" alt="' + _0x9631x22 + '" src="' + _0x9631x2d + '"/>';
        return _0x9631x23
    }

    function _0x9631x2e(_0x9631xf, _0x9631x16, _0x9631x1b, _0x9631x1a) {
        if (_0x9631x16['match']('hot-default') || _0x9631x16['match']('hot-colored') || _0x9631x16['match']('col-left') || _0x9631x16['match']('col-right') || _0x9631x16['match']('feat-list') || _0x9631x16['match']('post-list') || _0x9631x16['match']('related')) {
            var _0x9631x2f = '';
            if (_0x9631x1a == 'recent') {
                _0x9631x2f = '/feeds/posts/default?alt=json-in-script&max-results=' + _0x9631x1b
            } else {
                if (_0x9631x1a == 'random') {
                    var _0x9631x30 = Math['floor'](Math['random']() * _0x9631x1b) + 1;
                    _0x9631x2f = '/feeds/posts/default?max-results=' + _0x9631x1b + '&start-index=' + _0x9631x30 + '&alt=json-in-script'
                } else {
                    _0x9631x2f = '/feeds/posts/default/-/' + _0x9631x1a + '?alt=json-in-script&max-results=' + _0x9631x1b
                }
            };
            $['ajax']({
                url: _0x9631x2f,
                type: 'get',
                dataType: 'jsonp',
                beforeSend: function() {
                    if (_0x9631x16['match']('hot-default') || _0x9631x16['match']('hot-colored')) {
                        _0x9631xf['html']('<div class="hot-loader"/>')['parent']()['addClass']('show-hot')
                    }
                },
                success: function(_0x9631x31) {
                    if (_0x9631x16['match']('hot-default')) {
                        var _0x9631x32 = '<ul class="hot-posts">'
                    } else {
                        if (_0x9631x16['match']('hot-colored')) {
                            var _0x9631x32 = '<ul class="hot-posts hot-posts-color">'
                        } else {
                            if (_0x9631x16['match']('col-right') || _0x9631x16['match']('col-left')) {
                                var _0x9631x32 = '<ul class="feat-col feat-x1">'
                            } else {
                                if (_0x9631x16['match']('feat-list')) {
                                    var _0x9631x32 = '<ul class="feat-list feat-x1">'
                                } else {
                                    if (_0x9631x16['match']('post-list')) {
                                        var _0x9631x32 = '<ul class="custom-widget feat-x1">'
                                    } else {
                                        if (_0x9631x16['match']('related')) {
                                            var _0x9631x32 = '<ul class="related-posts feat-x1">'
                                        }
                                    }
                                }
                            }
                        }
                    };
                    var _0x9631x33 = _0x9631x31['feed']['entry'];
                    if (_0x9631x33 != undefined) {
                        for (var _0x9631x4 = 0, _0x9631x1d = _0x9631x33; _0x9631x4 < _0x9631x1d['length']; _0x9631x4++) {
                            var _0x9631x1f = _0x9631x1c(_0x9631x1d, _0x9631x4),
                                _0x9631x34 = _0x9631x2a(_0x9631x1d, _0x9631x4),
                                _0x9631x21 = _0x9631x24(_0x9631x1d, _0x9631x4),
                                _0x9631x14 = _0x9631x20(_0x9631x1d, _0x9631x4, _0x9631x1f, _0x9631x21);
                            var _0x9631x35 = '';
                            if (_0x9631x16['match']('hot-default') || _0x9631x16['match']('hot-colored')) {
                                _0x9631x35 += '<li class="hot-item item-' + _0x9631x4 + '"><div class="hot-item-inner"><a class="post-image-link" href="' + _0x9631x1f + '">' + _0x9631x34 + '</a><div class="post-info"><h2 class="post-title">' + _0x9631x14 + '</h2></div></div></li>'
                            } else {
                                if (_0x9631x16['match']('col-left') || _0x9631x16['match']('col-right') || _0x9631x16['match']('feat-list') || _0x9631x16['match']('post-list') || _0x9631x16['match']('related')) {
                                    _0x9631x35 += '<li class="feat-item item-' + _0x9631x4 + '"><a class="post-image-link" href="' + _0x9631x1f + '">' + _0x9631x34 + '</a><div class="post-info"><h2 class="post-title">' + _0x9631x14 + '</h2></div></li>'
                                }
                            };
                            _0x9631x32 += _0x9631x35
                        };
                        _0x9631x32 += '</ul>'
                    } else {
                        _0x9631x32 = '<ul class="no-posts">Error: No Posts Found <i class="fa fa-frown-o"/></ul>'
                    };
                    if (_0x9631x16['match']('hot-default') || _0x9631x16['match']('hot-colored')) {
                        _0x9631xf['html'](_0x9631x32)['parent']()['addClass']('show-hot')
                    } else {
                        if (_0x9631x16['match']('feat-list') || _0x9631x16['match']('col-left') || _0x9631x16['match']('col-right')) {
                            _0x9631xf['parent']()['find']('.widget-title')['append']('<a class="view-all" href="/search/label/' + _0x9631x1a + '?&max-results=' + postPerPage + '">' + messages['viewAll'] + '</a>');
                            if (_0x9631x16['match']('col-left') || _0x9631x16['match']('col-right')) {
                                if (_0x9631x16['match']('col-right')) {
                                    _0x9631xf['parent']()['addClass']('col-right')
                                };
                                _0x9631xf['parent']()['addClass']('col-width')
                            };
                            _0x9631xf['html'](_0x9631x32)['parent']()['addClass']('show-widget')
                        } else {
                            if (_0x9631x16['match']('related')) {
                                _0x9631xf['html'](_0x9631x32)['parent']()['addClass']('show-related')
                            } else {
                                _0x9631xf['html'](_0x9631x32)
                            }
                        }
                    }
                }
            })
        }
    }
    $('.blog-post-comments')['each'](function() {
        var _0x9631x36 = commentsSystem,
            _0x9631x37 = disqus_blogger_current_url,
            _0x9631x38 = '<div id="disqus_thread"/>',
            _0x9631x39 = $(location)['attr']('href'),
            _0x9631x3a = '<div class="fb-comments" data-width="100%" data-href="' + _0x9631x39 + '" data-numposts="5"></div>',
            _0x9631x3b = 'comments-system-' + _0x9631x36;
        if (_0x9631x36 == 'blogger') {
            $(this)['addClass'](_0x9631x3b)['show']()
        } else {
            if (_0x9631x36 == 'disqus') {
                (function() {
                    var _0x9631x3c = document['createElement']('script');
                    _0x9631x3c['type'] = 'text/javascript';
                    _0x9631x3c['async'] = true;
                    _0x9631x3c['src'] = '//' + disqusShortname + '.disqus.com/embed.js';
                    (document['getElementsByTagName']('head')[0] || document['getElementsByTagName']('body')[0])['appendChild'](_0x9631x3c)
                })();
                $('#comments, #gpluscomments')['remove']();
                $(this)['append'](_0x9631x38)['addClass'](_0x9631x3b)['show']()
            } else {
                if (_0x9631x36 == 'facebook') {
                    $('#comments, #gpluscomments')['remove']();
                    $(this)['append'](_0x9631x3a)['addClass'](_0x9631x3b)['show']()
                } else {
                    if (_0x9631x36 == 'hide') {
                        $(this)['hide']()
                    } else {
                        $(this)['addClass']('comments-system-default')['show']()
                    }
                }
            }
        }
    })
})
//]]>
