var inProgress, path, loadStylesheet, installedCssChunks, __webpack_modules__ = {
        80885: (e, t, n) => {
                var i = n(28506)
                  , r = "chrome-extension://__MSG_@@extension_id__/"
                  , s = "moz-extension://__MSG_@@extension_id__/"
                  , o = "safari-web-extension://__MSG_@@extension_id__/"
                  , a = self.GR_RESOURCE_ROOT || r
                  , c = self.GR_RESOURCE_ROOT || s
                  , l = self.GR_RESOURCE_ROOT || o;
                e.exports = {
                        __css: i.toString().replace(new RegExp(r,"g"), a).replace(new RegExp(s,"g"), c).replace(new RegExp(o,"g"), l),
                        ...i.locals
                }
        }
        ,
        26620: (e, t) => {
                Object.defineProperty(t, "__esModule", {
                        value: !0
                }),
                t.config = void 0;
                var n = {
                        prod: "grammarly.com",
                        preprod: "ppgr.io",
                        qa: "qagr.io"
                };
                t.config = function(e) {
                        var t = n[e];
                        return {
                                url: {
                                        properties: "https://properties." + t,
                                        treatment: "https://treatment." + t,
                                        gates: "https://gates." + t
                                }
                        }
                }
        }
        ,
        22407: (e, t) => {
                Object.defineProperty(t, "__esModule", {
                        value: !0
                }),
                t.NOT_ASSIGNED = t.Experiment = void 0;
                var n = function() {
                        function e(e, t) {
                                void 0 === t && (t = []),
                                this.name = e,
                                this._experiences = t
                        }
                        return Object.defineProperty(e.prototype, "experiences", {
                                get: function() {
                                        return Object.fromEntries(this._experiences.map((function(e) {
                                                return [e, e]
                                        }
                                        )))
                                },
                                enumerable: !1,
                                configurable: !0
                        }),
                        Object.defineProperty(e.prototype, "experiencesArray", {
                                get: function() {
                                        return this._experiences
                                },
                                enumerable: !1,
                                configurable: !0
                        }),
                        e
                }();
                t.Experiment = n,
                t.NOT_ASSIGNED = "NOT_ASSIGNED"
        }
        ,
        29427: function(e, t, n) {
                var i = this && this.__awaiter || function(e, t, n, i) {
                        return new (n || (n = Promise))((function(r, s) {
                                function o(e) {
                                        try {
                                                c(i.next(e))
                                        } catch (e) {
                                                s(e)
                                        }
                                }
                                function a(e) {
                                        try {
                                                c(i.throw(e))
                                        } catch (e) {
                                                s(e)
                                        }
                                }
                                function c(e) {
                                        var t;
                                        e.done ? r(e.value) : (t = e.value,
                                        t instanceof n ? t : new n((function(e) {
                                                e(t)
                                        }
                                        ))).then(o, a)
                                }
                                c((i = i.apply(e, t || [])).next())
                        }
                        ))
                }
                  , r = this && this.__generator || function(e, t) {
                        var n, i, r, s, o = {
                                label: 0,
                                sent: function() {
                                        if (1 & r[0])
                                                throw r[1];
                                        return r[1]
                                },
                                trys: [],
                                ops: []
                        };
                        return s = {
                                next: a(0),
                                throw: a(1),
                                return: a(2)
                        },
                        "function" == typeof Symbol && (s[Symbol.iterator] = function() {
                                return this
                        }
                        ),
                        s;
                        function a(s) {
                                return function(a) {
                                        return function(s) {
                                                if (n)
                                                        throw new TypeError("Generator is already executing.");
                                                for (; o; )
                                                        try {
                                                                if (n = 1,
                                                                i && (r = 2 & s[0] ? i.return : s[0] ? i.throw || ((r = i.return) && r.call(i),
                                                                0) : i.next) && !(r = r.call(i, s[1])).done)
                                                                        return r;
                                                                switch (i = 0,
                                                                r && (s = [2 & s[0], r.value]),
                                                                s[0]) {
                                                                case 0:
                                                                case 1:
                                                                        r = s;
                                                                        break;
                                                                case 4:
                                                                        return o.label++,
                                                                        {
                                                                                value: s[1],
                                                                                done: !1
                                                                        };
                                                                case 5:
                                                                        o.label++,
                                                                        i = s[1],
                                                                        s = [0];
                                                                        continue;
                                                                case 7:
                                                                        s = o.ops.pop(),
                                                                        o.trys.pop();
                                                                        continue;
                                                                default:
                                                                        if (!(r = o.trys,
                                                                        (r = r.length > 0 && r[r.length - 1]) || 6 !== s[0] && 2 !== s[0])) {
                                                                                o = 0;
                                                                                continue
                                                                        }
                                                                        if (3 === s[0] && (!r || s[1] > r[0] && s[1] < r[3])) {
                                                                                o.label = s[1];
                                                                                break
                                                                        }
                                                                        if (6 === s[0] && o.label < r[1]) {
                                                                                o.label = r[1],
                                                                                r = s;
                                                                                break
                                                                        }
                                                                        if (r && o.label < r[2]) {
                                                                                o.label = r[2],
                                                                                o.ops.push(s);
                                                                                break
                                                                        }
                                                                        r[2] && o.ops.pop(),
                                                                        o.trys.pop();
                                                                        continue
                                                                }
                                                                s = t.call(e, o)
                                                        } catch (e) {
                                                                s = [6, e],
                                                                i = 0
                                                        } finally {
                                                                n = r = 0
                                                        }
                                                if (5 & s[0])
                                                        throw s[1];
                                                return {
                                                        value: s[0] ? s[1] : void 0,
                                                        done: !0
                                                }
                                        }([s, a])
                                }
                        }
                }
                ;
                Object.defineProperty(t, "__esModule", {
                        value: !0
                }),
                t.ExperimentClient = void 0;
                var s = n(22407)
                  , o = n(22388)
                  , a = n(94248)
                  , c = n(53555)
                  , l = function(e, t, n, l, u) {
                        var d = this;
                        void 0 === u && (u = {}),
                        this._treatmentService = e,
                        this._experiments = t,
                        this._gatesService = n,
                        this._gates = l,
                        this._config = u,
                        this._experimentTreatments = new Map,
                        this._gateTreatments = new Map,
                        this._initialFetched = !1,
                        this.setPrefetchedTreatments = function(e) {
                                if (d._startRefreshIfNeeded(),
                                !c.validateTreatmentsWithType(e))
                                        throw new Error("Not valid treatments");
                                d._updateTreatmentForExpAndGates(e)
                        }
                        ,
                        this._updateTreatmentForExpAndGates = function(e) {
                                d._treatmentService.refresh && d._treatmentService.refresh(),
                                d._experimentTreatments = new Map(e.filter((function(e) {
                                        return e.type === o.ExperimentType.experiment
                                }
                                )).map((function(e) {
                                        return [e.experimentName, e]
                                }
                                ))),
                                d._gateTreatments = new Map(e.filter((function(e) {
                                        return e.type === o.ExperimentType.gate
                                }
                                )).map((function(e) {
                                        return [e.experimentName, e]
                                }
                                )))
                        }
                        ,
                        this.fetchTreatments = function(e) {
                                return void 0 === e && (e = {}),
                                i(d, void 0, void 0, (function() {
                                        return r(this, (function(t) {
                                                switch (t.label) {
                                                case 0:
                                                        return this._startRefreshIfNeeded(),
                                                        [4, this._fetchTreatments(e.clearCacheOnError)];
                                                case 1:
                                                        return t.sent(),
                                                        [2]
                                                }
                                        }
                                        ))
                                }
                                ))
                        }
                        ,
                        this._fetchTreatments = function(e) {
                                return i(d, void 0, void 0, (function() {
                                        var t, n, i, s, o, a, c;
                                        return r(this, (function(r) {
                                                switch (r.label) {
                                                case 0:
                                                        t = null,
                                                        n = null,
                                                        r.label = 1;
                                                case 1:
                                                        return r.trys.push([1, 3, , 4]),
                                                        i = this._experiments.concat(this._gates),
                                                        [4, this._treatmentService.getTreatment(i.map((function(e) {
                                                                return e.name
                                                        }
                                                        )))];
                                                case 2:
                                                        return t = r.sent(),
                                                        [3, 4];
                                                case 3:
                                                        return s = r.sent(),
                                                        n = s,
                                                        e && this._experimentTreatments.clear(),
                                                        [3, 4];
                                                case 4:
                                                        if (t)
                                                                return this._updateTreatmentForExpAndGates(t),
                                                                [2];
                                                        o = null,
                                                        a = null,
                                                        r.label = 5;
                                                case 5:
                                                        return r.trys.push([5, 7, , 8]),
                                                        [4, this._gatesService.getTreatment(this._gates.map((function(e) {
                                                                return e.name
                                                        }
                                                        )))];
                                                case 6:
                                                        return o = r.sent(),
                                                        [3, 8];
                                                case 7:
                                                        return c = r.sent(),
                                                        a = c,
                                                        e && this._gateTreatments.clear(),
                                                        [3, 8];
                                                case 8:
                                                        if (o && (this._gateTreatments = new Map(o.map((function(e) {
                                                                return [e.experimentName, e]
                                                        }
                                                        )))),
                                                        a || n)
                                                                throw a || n;
                                                        return [2]
                                                }
                                        }
                                        ))
                                }
                                ))
                        }
                        ,
                        this._startRefreshIfNeeded = function() {
                                d._initialFetched || (d._config.ttl && (d._refreshTreatment = setInterval((function() {
                                        return i(d, void 0, void 0, (function() {
                                                var e, t = this;
                                                return r(this, (function(n) {
                                                        switch (n.label) {
                                                        case 0:
                                                                return e = function() {
                                                                        return i(t, void 0, void 0, (function() {
                                                                                return r(this, (function(e) {
                                                                                        switch (e.label) {
                                                                                        case 0:
                                                                                                return e.trys.push([0, 2, , 3]),
                                                                                                [4, this._fetchTreatments()];
                                                                                        case 1:
                                                                                        case 2:
                                                                                                return e.sent(),
                                                                                                [3, 3];
                                                                                        case 3:
                                                                                                return [2]
                                                                                        }
                                                                                }
                                                                                ))
                                                                        }
                                                                        ))
                                                                }
                                                                ,
                                                                this._config.ttl && this._config.useRefreshJitter ? (this._delayedRefreshTreatment = setTimeout(e, .1 * this._config.ttl * Math.random()),
                                                                [3, 3]) : [3, 1];
                                                        case 1:
                                                                return [4, e()];
                                                        case 2:
                                                                n.sent(),
                                                                n.label = 3;
                                                        case 3:
                                                                return [2]
                                                        }
                                                }
                                                ))
                                        }
                                        ))
                                }
                                ), d._config.ttl)),
                                d._initialFetched = !0)
                        }
                        ,
                        this.dispose = function() {
                                d._refreshTreatment && clearInterval(d._refreshTreatment),
                                d._delayedRefreshTreatment && clearTimeout(d._delayedRefreshTreatment)
                        }
                        ,
                        this.getTreatment = function(e) {
                                var t = d.peekTreatment(e);
                                return null !== t && d.logTreatment(e, t).catch((function() {}
                                )),
                                t
                        }
                        ,
                        this.getTreatmentManakin = function(e) {
                                var t = d.getTreatment(e);
                                return t === s.NOT_ASSIGNED ? null : t
                        }
                        ,
                        this.peekTreatment = function(e) {
                                var t = d._experimentTreatments.get(e.name) || d._gateTreatments.get(e.name)
                                  , n = null == t ? void 0 : t.groupName;
                                if (0 === e.experiencesArray.length || a.getExperienceName(null != n ? n : "") === s.NOT_ASSIGNED)
                                        return a.getExperienceName(null != n ? n : "");
                                if (n) {
                                        var i = e.experiencesArray.find((function(e) {
                                                return a.getGroupNames(e).includes(n)
                                        }
                                        ));
                                        if (i)
                                                return i
                                }
                                return null
                        }
                        ,
                        this.peekTreatmentManakin = function(e) {
                                var t = d.peekTreatment(e);
                                return t === s.NOT_ASSIGNED ? null : t
                        }
                        ,
                        this.logTreatment = function(e, t) {
                                if (d._config.ssrDisableLogging)
                                        return Promise.resolve();
                                var n = d._experimentTreatments.get(e.name) || d._gateTreatments.get(e.name);
                                if (!n || a.getExperienceName(n.groupName) !== t)
                                        throw new Error("Cannot find associated treatment");
                                return (void 0 !== n.needLog ? n.needLog : n.type !== o.ExperimentType.gate) ? d._treatmentService.logTreatment(n) : Promise.resolve()
                        }
                        ,
                        this.isGateEnabled = function(e) {
                                return d._getExperienceOfEnabledGate(e.name) === e.experience
                        }
                        ,
                        this._getExperienceOfEnabledGate = function(e) {
                                var t = d._gateTreatments.get(e);
                                return t ? a.getExperienceName(t.groupName) : null
                        }
                        ,
                        this.getDynamicConfiguration = function(e) {
                                var t = d._experimentTreatments.get(e.name) || d._gateTreatments.get(e.name);
                                return t && t.dynamicConfiguration ? t.dynamicConfiguration : null
                        }
                };
                t.ExperimentClient = l
        },
        22388: (e, t) => {
                Object.defineProperty(t, "__esModule", {
                        value: !0
                }),
                t.ExperimentType = void 0,
                function(e) {
                        e.experiment = "experiment",
                        e.gate = "gate"
                }(t.ExperimentType || (t.ExperimentType = {}))
        }
        ,
        49892: (e, t) => {
                Object.defineProperty(t, "__esModule", {
                        value: !0
                }),
                t.Gate = void 0;
                var n = function(e, t) {
                        void 0 === t && (t = "enabled"),
                        this.name = e,
                        this.experience = t
                };
                t.Gate = n
        }
        ,
        15392: function(e, t, n) {
                var i = this && this.__awaiter || function(e, t, n, i) {
                        return new (n || (n = Promise))((function(r, s) {
                                function o(e) {
                                        try {
                                                c(i.next(e))
                                        } catch (e) {
                                                s(e)
                                        }
                                }
                                function a(e) {
                                        try {
                                                c(i.throw(e))
                                        } catch (e) {
                                                s(e)
                                        }
                                }
                                function c(e) {
                                        var t;
                                        e.done ? r(e.value) : (t = e.value,
                                        t instanceof n ? t : new n((function(e) {
                                                e(t)
                                        }
                                        ))).then(o, a)
                                }
                                c((i = i.apply(e, t || [])).next())
                        }
                        ))
                }
                  , r = this && this.__generator || function(e, t) {
                        var n, i, r, s, o = {
                                label: 0,
                                sent: function() {
                                        if (1 & r[0])
                                                throw r[1];
                                        return r[1]
                                },
                                trys: [],
                                ops: []
                        };
                        return s = {
                                next: a(0),
                                throw: a(1),
                                return: a(2)
                        },
                        "function" == typeof Symbol && (s[Symbol.iterator] = function() {
                                return this
                        }
                        ),
                        s;
                        function a(s) {
                                return function(a) {
                                        return function(s) {
                                                if (n)
                                                        throw new TypeError("Generator is already executing.");
                                                for (; o; )
                                                        try {
                                                                if (n = 1,
                                                                i && (r = 2 & s[0] ? i.return : s[0] ? i.throw || ((r = i.return) && r.call(i),
                                                                0) : i.next) && !(r = r.call(i, s[1])).done)
                                                                        return r;
                                                                switch (i = 0,
                                                                r && (s = [2 & s[0], r.value]),
                                                                s[0]) {
                                                                case 0:
                                                                case 1:
                                                                        r = s;
                                                                        break;
                                                                case 4:
                                                                        return o.label++,
                                                                        {
                                                                                value: s[1],
                                                                                done: !1
                                                                        };
                                                                case 5:
                                                                        o.label++,
                                                                        i = s[1],
                                                                        s = [0];
                                                                        continue;
                                                                case 7:
                                                                        s = o.ops.pop(),
                                                                        o.trys.pop();
                                                                        continue;
                                                                default:
                                                                        if (!(r = o.trys,
                                                                        (r = r.length > 0 && r[r.length - 1]) || 6 !== s[0] && 2 !== s[0])) {
                                                                                o = 0;
                                                                                continue
                                                                        }
                                                                        if (3 === s[0] && (!r || s[1] > r[0] && s[1] < r[3])) {
                                                                                o.label = s[1];
                                                                                break
                                                                        }
                                                                        if (6 === s[0] && o.label < r[1]) {
                                                                                o.label = r[1],
                                                                                r = s;
                                                                                break
                                                                        }
                                                                        if (r && o.label < r[2]) {
                                                                                o.label = r[2],
                                                                                o.ops.push(s);
                                                                                break
                                                                        }
                                                                        r[2] && o.ops.pop(),
                                                                        o.trys.pop();
                                                                        continue
                                                                }
                                                                s = t.call(e, o)
                                                        } catch (e) {
                                                                s = [6, e],
                                                                i = 0
                                                        } finally {
                                                                n = r = 0
                                                        }
                                                if (5 & s[0])
                                                        throw s[1];
                                                return {
                                                        value: s[0] ? s[1] : void 0,
                                                        done: !0
                                                }
                                        }([s, a])
                                }
                        }
                }
                ;
                Object.defineProperty(t, "__esModule", {
                        value: !0
                }),
                t.GatesService = void 0;
                var s = n(26620)
                  , o = n(5230)
                  , a = n(53555)
                  , c = function() {
                        function e(e, t, n) {
                                this.type = "gate",
                                this._httpClient = new o.HttpClient(e,t),
                                this._gatesUrl = s.config(n).url.gates + "/gates/get"
                        }
                        return e.prototype.getTreatment = function(e) {
                                return i(this, void 0, void 0, (function() {
                                        var t;
                                        return r(this, (function(n) {
                                                switch (n.label) {
                                                case 0:
                                                        return [4, this._httpClient.post(this._gatesUrl, e)];
                                                case 1:
                                                        if (t = n.sent(),
                                                        a.validateTreatmentsWithType(t))
                                                                return [2, t];
                                                        throw new Error("Did not get valid gate treatments")
                                                }
                                        }
                                        ))
                                }
                                ))
                        }
                        ,
                        e
                }();
                t.GatesService = c
        },
        5230: function(e, t) {
                var n = this && this.__assign || function() {
                        return n = Object.assign || function(e) {
                                for (var t, n = 1, i = arguments.length; n < i; n++)
                                        for (var r in t = arguments[n])
                                                Object.prototype.hasOwnProperty.call(t, r) && (e[r] = t[r]);
                                return e
                        }
                        ,
                        n.apply(this, arguments)
                }
                  , i = this && this.__awaiter || function(e, t, n, i) {
                        return new (n || (n = Promise))((function(r, s) {
                                function o(e) {
                                        try {
                                                c(i.next(e))
                                        } catch (e) {
                                                s(e)
                                        }
                                }
                                function a(e) {
                                        try {
                                                c(i.throw(e))
                                        } catch (e) {
                                                s(e)
                                        }
                                }
                                function c(e) {
                                        var t;
                                        e.done ? r(e.value) : (t = e.value,
                                        t instanceof n ? t : new n((function(e) {
                                                e(t)
                                        }
                                        ))).then(o, a)
                                }
                                c((i = i.apply(e, t || [])).next())
                        }
                        ))
                }
                  , r = this && this.__generator || function(e, t) {
                        var n, i, r, s, o = {
                                label: 0,
                                sent: function() {
                                        if (1 & r[0])
                                                throw r[1];
                                        return r[1]
                                },
                                trys: [],
                                ops: []
                        };
                        return s = {
                                next: a(0),
                                throw: a(1),
                                return: a(2)
                        },
                        "function" == typeof Symbol && (s[Symbol.iterator] = function() {
                                return this
                        }
                        ),
                        s;
                        function a(s) {
                                return function(a) {
                                        return function(s) {
                                                if (n)
                                                        throw new TypeError("Generator is already executing.");
                                                for (; o; )
                                                        try {
                                                                if (n = 1,
                                                                i && (r = 2 & s[0] ? i.return : s[0] ? i.throw || ((r = i.return) && r.call(i),
                                                                0) : i.next) && !(r = r.call(i, s[1])).done)
                                                                        return r;
                                                                switch (i = 0,
                                                                r && (s = [2 & s[0], r.value]),
                                                                s[0]) {
                                                                case 0:
                                                                case 1:
                                                                        r = s;
                                                                        break;
                                                                case 4:
                                                                        return o.label++,
                                                                        {
                                                                                value: s[1],
                                                                                done: !1
                                                                        };
                                                                case 5:
                                                                        o.label++,
                                                                        i = s[1],
                                                                        s = [0];
                                                                        continue;
                                                                case 7:
                                                                        s = o.ops.pop(),
                                                                        o.trys.pop();
                                                                        continue;
                                                                default:
                                                                        if (!(r = o.trys,
                                                                        (r = r.length > 0 && r[r.length - 1]) || 6 !== s[0] && 2 !== s[0])) {
                                                                                o = 0;
                                                                                continue
                                                                        }
                                                                        if (3 === s[0] && (!r || s[1] > r[0] && s[1] < r[3])) {
                                                                                o.label = s[1];
                                                                                break
                                                                        }
                                                                        if (6 === s[0] && o.label < r[1]) {
                                                                                o.label = r[1],
                                                                                r = s;
                                                                                break
                                                                        }
                                                                        if (r && o.label < r[2]) {
                                                                                o.label = r[2],
                                                                                o.ops.push(s);
                                                                                break
                                                                        }
                                                                        r[2] && o.ops.pop(),
                                                                        o.trys.pop();
                                                                        continue
                                                                }
                                                                s = t.call(e, o)
                                                        } catch (e) {
                                                                s = [6, e],
                                                                i = 0
                                                        } finally {
                                                                n = r = 0
                                                        }
                                                if (5 & s[0])
                                                        throw s[1];
                                                return {
                                                        value: s[0] ? s[1] : void 0,
                                                        done: !0
                                                }
                                        }([s, a])
                                }
                        }
                }
                ;
                Object.defineProperty(t, "__esModule", {
                        value: !0
                }),
                t.HttpClient = void 0;
                var s = function() {
                        function e(e, t) {
                                var n = this;
                                this._fetch = e,
                                this._config = t,
                                this._fetchWithTimeout = this._config.timeout ? function() {
                                        for (var e = [], t = 0; t < arguments.length; t++)
                                                e[t] = arguments[t];
                                        return Promise.race([n._fetch.apply(n, e), new Promise((function(e, t) {
                                                return setTimeout((function() {
                                                        return t(new Error("Timeout"))
                                                }
                                                ), n._config.timeout)
                                        }
                                        ))])
                                }
                                : this._fetch
                        }
                        return e.prototype.get = function(e) {
                                return i(this, void 0, void 0, (function() {
                                        var t, n;
                                        return r(this, (function(i) {
                                                switch (i.label) {
                                                case 0:
                                                        return [4, this._getHeaders()];
                                                case 1:
                                                        return t = i.sent(),
                                                        [4, this._fetchWithTimeout(e, {
                                                                credentials: "include",
                                                                mode: "cors",
                                                                headers: t
                                                        })];
                                                case 2:
                                                        return n = i.sent(),
                                                        [2, this._parseResponse(n)]
                                                }
                                        }
                                        ))
                                }
                                ))
                        }
                        ,
                        e.prototype.post = function(e, t) {
                                return i(this, void 0, void 0, (function() {
                                        var i, s;
                                        return r(this, (function(r) {
                                                switch (r.label) {
                                                case 0:
                                                        return [4, this._getHeaders()];
                                                case 1:
                                                        return i = r.sent(),
                                                        [4, this._fetchWithTimeout(e, {
                                                                method: "POST",
                                                                credentials: "include",
                                                                mode: "cors",
                                                                headers: n(n({}, i), {
                                                                        "Content-Type": "application/json"
                                                                }),
                                                                body: JSON.stringify(t)
                                                        })];
                                                case 2:
                                                        return s = r.sent(),
                                                        [2, this._parseResponse(s)]
                                                }
                                        }
                                        ))
                                }
                                ))
                        }
                        ,
                        e.prototype._filterHeaders = function(e) {
                                var t = {};
                                return Object.entries(e).forEach((function(e) {
                                        var n = e[0]
                                          , i = e[1];
                                        i && (t[n] = i)
                                }
                                )),
                                t
                        }
                        ,
                        e.prototype._getHeaders = function() {
                                return i(this, void 0, void 0, (function() {
                                        var e;
                                        return r(this, (function(t) {
                                                switch (t.label) {
                                                case 0:
                                                        return this._config.getApplicationHeaders ? (e = this._filterHeaders,
                                                        [4, this._config.getApplicationHeaders()]) : [3, 2];
                                                case 1:
                                                        return [2, e.apply(this, [t.sent()])];
                                                case 2:
                                                        throw new Error("Cannot get application headers")
                                                }
                                        }
                                        ))
                                }
                                ))
                        }
                        ,
                        e.prototype._parseResponse = function(e) {
                                if (!e.ok)
                                        throw new Error("Network response was not ok, status " + e.status);
                                return "application/json" === e.headers.get("Content-Type") ? e.json() : e.text()
                        }
                        ,
                        e
                }();
                t.HttpClient = s
        },
        19917: (e, t, n) => {
                t.Cc = void 0;
                var i = n(29427);
                var r = n(93703);
                var s = n(15392);
                var o = n(22271);
                var a = n(22407);
                var c = n(49892);
                Object.defineProperty(t, "Cc", {
                        enumerable: !0,
                        get: function() {
                                return c.Gate
                        }
                });
                var l = n(22388)
        }
        ,
        22271: (e, t, n) => {
                Object.defineProperty(t, "__esModule", {
                        value: !0
                }),
                t.PropertiesClient = void 0;
                var i = n(26620)
                  , r = n(5230)
                  , s = function() {
                        function e(e, t, n) {
                                this._propertiesUrl = i.config(t).url.properties + "/properties",
                                this._httpClient = new r.HttpClient(e,n)
                        }
                        return e.prototype.getAll = function() {
                                return this._httpClient.get(this._propertiesUrl)
                        }
                        ,
                        e.prototype.getOne = function(e) {
                                var t = this._propertiesUrl + "/" + e;
                                return this._httpClient.get(t)
                        }
                        ,
                        e.prototype.set = function(e) {
                                return this._httpClient.post(this._propertiesUrl, e)
                        }
                        ,
                        e
                }();
                t.PropertiesClient = s
        }
        ,
        94248: (e, t) => {
                Object.defineProperty(t, "__esModule", {
                        value: !0
                }),
                t.getGroupNames = t.getExperienceName = void 0;
                t.getExperienceName = function(e) {
                        return e.endsWith("_1") || e.endsWith("_2") ? e.slice(0, -2) : null
                }
                ;
                t.getGroupNames = function(e) {
                        return [e + "_1", e + "_2"]
                }
        }
        ,
        53555: (e, t) => {
                Object.defineProperty(t, "__esModule", {
                        value: !0
                }),
                t.validateTreatmentsWithType = void 0;
                var n = function(e) {
                        return "string" == typeof e
                };
                t.validateTreatmentsWithType = function(e) {
                        return Array.isArray(e) && e.reduce((function(e, t) {
                                return e && (n((i = t).experimentName) && n(i.groupName) && n(i.experimentId) && n(i.type));
                                var i
                        }
                        ), !0)
                }
        }
        ,
        93703: function(e, t, n) {
                var i = this && this.__awaiter || function(e, t, n, i) {
                        return new (n || (n = Promise))((function(r, s) {
                                function o(e) {
                                        try {
                                                c(i.next(e))
                                        } catch (e) {
                                                s(e)
                                        }
                                }
                                function a(e) {
                                        try {
                                                c(i.throw(e))
                                        } catch (e) {
                                                s(e)
                                        }
                                }
                                function c(e) {
                                        var t;
                                        e.done ? r(e.value) : (t = e.value,
                                        t instanceof n ? t : new n((function(e) {
                                                e(t)
                                        }
                                        ))).then(o, a)
                                }
                                c((i = i.apply(e, t || [])).next())
                        }
                        ))
                }
                  , r = this && this.__generator || function(e, t) {
                        var n, i, r, s, o = {
                                label: 0,
                                sent: function() {
                                        if (1 & r[0])
                                                throw r[1];
                                        return r[1]

