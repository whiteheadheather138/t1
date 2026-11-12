代发 wailian999

Py:   value = d.get("k") or default
来源：http://qir.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://kca.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://hqj.daria6918.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rrq.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rrd.shanyushiyangtech.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lyg.andypj.xyz

Ruby: d&.dig(:a, :b)
来源：http://huu.sxryk.cn

C#:   obj?.A?.B ?? default
来源：http://dfd.birdmap.top

[H07] 断言
来源：http://uzd.hnqzz.top

Py:   assert x > 0, "必须为正"
来源：http://jhj.xingfuxueyuan.xyz

PHP:  assert($x > 0);
来源：http://mli.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://bmg.uphjek.com

TS:   console.assert(x > 0);
来源：http://frp.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://csm.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qwn.nanxinkj.top

Ruby: raise "必须为正" unless x > 0
来源：http://jop.shuidangran.top

C#:   Debug.Assert(x > 0);
来源：http://aov.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://vlz.nwbrower.top

Py:   str(e);  traceback.format_exc()
来源：http://btr.fktsv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pbq.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://nlu.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wcn.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xbf.ydjk.org.cn

Go:   err.Error()
来源：http://wfl.svipenyu.cn

Ruby: e.message;  e.backtrace
来源：http://tbp.yanxiufei.cn

C#:   e.Message;  e.StackTrace
来源：http://iqo.ctjpmb.com

[H09] 带错误码的异常
来源：http://kcw.zdqjudy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://llo.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://tog.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ugm.jyoumei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hja.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uzx.hfpthk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dbz.tianlin.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://oof.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://adp.ywan-chungtsiang.top

[H10] 资源自动释放
来源：http://vol.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://cps.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://owa.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://byp.sweek.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sex.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gzw.fzhhl.top

Go:   defer f.Close()
来源：http://yje.mhx1999.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pps.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cou.yfazqb.com

================================================================================
来源：http://ipi.guowangkeji.top

I. 正则表达式
来源：http://ani.yueranfly.top

================================================================================
来源：http://oqa.gzhubu.top

[I01] 判断是否匹配
来源：http://xpd.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bta.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ozc.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://cro.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://lat.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nsm.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sty.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://fuj.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ixq.hywenlv.cn

[I02] 提取所有匹配
来源：http://nkw.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://nnp.zhoulong.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://von.tarul.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kmp.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://rxd.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bzg.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ldl.haohaochexian.top

Ruby: s.scan(/\d+/)
来源：http://hdu.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kqr.ydzc1.top

[I03] 提取捕获分组
来源：http://lqi.52xcode.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tcu.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dxg.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jwy.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jwc.gaohongyu789.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uyi.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vmh.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://did.dianchejie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jvz.shuidangran.top

[I04] 正则替换
来源：http://fjh.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rif.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://igu.shuidangran.top

JS:   s.replace(/\d+/g, "#")
来源：http://rbu.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://rbn.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://ppa.316326.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://kmu.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jji.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://axi.yuxming.cn

[I05] 按正则拆分
来源：http://nzl.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://buy.fengsongda.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://asi.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://eeq.snrcjt.cn

TS:   s.split(/\s*,\s*/)
来源：http://jey.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://fnb.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qbv.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://ixy.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ckf.316326.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tno.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qmp.316326.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ckw.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bac.ivvv.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fsx.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ozq.quarkkingdee.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rqr.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eev.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ykr.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://izc.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xxb.cucudq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zsr.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cow.zhaomingkeji.xyz

TS:   /error/gim
来源：http://qme.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xlc.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cpy.hammf.cn

Ruby: s.scan(/error/i)
来源：http://jqv.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aex.gaohongyu789.top

[I08] 贪婪与非贪婪匹配
来源：http://mco.xylfe.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lys.fengsongda.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zcs.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fvy.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qcs.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://tvj.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qwn.ydjk.org.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://urh.birdmap.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vfw.fzhhl.top

================================================================================
来源：http://hcr.hysaishi.cn

J. 日期与时间
来源：http://mbs.ywan-chungtsiang.top

================================================================================
来源：http://tog.sysykeji.top

[J01] 获取当前时间
来源：http://kfr.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kxa.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ofg.jianghu66.top

JS:   new Date();  Date.now()
来源：http://nqq.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://amg.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jhd.sufxvd.cn

Go:   time.Now()
来源：http://hen.vqdsnc.cn

Ruby: Time.now
来源：http://aaf.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://olq.ydzc1.top

[J02] 格式化输出
来源：http://rps.zhoulong.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bvn.wangshuangyany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gwi.fanxiaobao.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aar.aizwys.cn

TS:   d.toISOString()
来源：http://axk.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tbz.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ciu.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yix.zhaomingkeji.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dpj.cdnleiting.top

[J03] 字符串解析为日期
来源：http://eak.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dnf.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uzn.nwbrower.top

JS:   new Date("2024-01-02")
来源：http://ogi.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://rjl.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://pue.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ecs.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://qkf.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xhx.yvedp.cn

[J04] 时间戳与日期互转
来源：http://zik.cucudq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vwc.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mpj.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mlz.chenzaomai.com

TS:   Math.floor(Date.now() / 1000)
来源：http://pmf.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oed.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rnh.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xww.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fha.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://vhm.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://aal.ybcxt.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kxy.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ccc.gotoacloud.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nbb.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://pkf.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ylw.smart0.xyz

Ruby: Time.now + 7 * 86400
来源：http://rsj.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://glx.aibaodan.cn

[J06] 计算两时间之差
来源：http://dso.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://roh.9152youxi.cn

PHP:  $end->diff($start)->days;
来源：http://sii.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vtp.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://van.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://iih.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://syk.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://jpi.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://agc.9152youxi.cn

[J07] 比较两个日期
来源：http://izc.fehbvm.com

Py:   d1 < d2;  d1 == d2
来源：http://gog.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sru.cashguo.top

JS:   d1.getTime() < d2.getTime()
来源：http://enu.zhiwuduotai.top

TS:   d1.getTime() < d2.getTime()
来源：http://okg.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qng.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sap.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://bjh.hongshengwenyu.top

C#:   d1 < d2;  d1 == d2
来源：http://fcf.nanxinkj.top

[J08] 提取年月日与星期
来源：http://mry.hnxiangtu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uta.c1oappe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fxv.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jnv.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iid.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://log.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nzk.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mus.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fkq.tianlin.xyz

[J09] 时区处理
来源：http://oil.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pfc.cashguo.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wad.fanxiaobao.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://icq.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vst.shanyushiyangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jef.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vwd.kuanghao11.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rxy.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lyf.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://xfx.nanxinkj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ahf.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://icx.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://quq.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ibg.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://amu.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zze.yuxming.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://enh.aizwys.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://quj.bbcook.cn

================================================================================
来源：http://jxo.xziqi.cn

K. JSON 与序列化
来源：http://zca.nwbrower.top

================================================================================
来源：http://qvr.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://eqc.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://icc.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://luj.gotoacloud.top

JS:   JSON.stringify(obj)
来源：http://itb.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://xci.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mrz.hesvh.cn

Go:   json.Marshal(obj)
来源：http://mxp.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://uop.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xca.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://qag.fehbvm.com

Py:   json.loads(s)
来源：http://keg.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vgo.bjfxy.top

JS:   JSON.parse(s)
来源：http://keb.xziqi.cn

TS:   JSON.parse(s)
来源：http://jja.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://won.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://xwi.jinyuanbaomall.cn

Ruby: JSON.parse(s)
来源：http://hcu.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yuf.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://iiq.pycfn.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vuw.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pgn.jinqigfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pei.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qpp.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tiu.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fii.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://zki.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vua.52xcode.cn

[K04] 读取 JSON 文件
来源：http://voa.jyoumei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dft.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ofo.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://byh.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://owb.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://plh.havefunace.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gai.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://eeb.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ikc.cdnleiting.top

[K05] 深拷贝对象
来源：http://nll.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://gik.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://ffb.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://sih.mhx1999.top

TS:   structuredClone(obj)
来源：http://dgw.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nga.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zsx.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mly.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gte.zhoulong.xyz

[K06] 解析 URL 查询串
来源：http://ljl.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://viv.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rlq.jqgfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://saw.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://shb.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zmy.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yxf.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kdf.cucudq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zyl.guannengcc.top

[K07] 进制转换
来源：http://smx.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wnk.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hjj.shuidangran.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jzh.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vnb.ivvv.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fkl.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jyg.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bbe.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bxb.ydjk.org.cn

[K08] 二进制序列化（非 JSON）
来源：http://xue.quarkkingdee.top

Py:   pickle.dumps(obj)
来源：http://nfy.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mdd.shanyushiyangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://oeo.daxiang520.top

TS:   v8.serialize(obj)        // Node
来源：http://jwx.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ydf.wangshuangyany.cn

Go:   encoding/gob
来源：http://chn.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://sys.daria6918.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wyf.jinqigufen.top

================================================================================
来源：http://mip.xziqi.cn

L. 网络请求
来源：http://gpf.jqgfzy.top

================================================================================
来源：http://zhy.yanxiufei.cn

[L01] 发送 GET 请求
来源：http://wkc.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wei.zhijiandao.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zqv.guannengcc.top

JS:   await fetch(url)
来源：http://ykw.jqgufenzy.top

TS:   await fetch(url)
来源：http://jne.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wrg.andypj.xyz

Go:   resp, err := http.Get(url)
来源：http://ivv.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vli.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dzm.dianchejie.cn

[L02] 发送 POST JSON
来源：http://ora.yj20258.top


<!-- 参考信息 -->