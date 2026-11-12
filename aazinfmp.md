代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://fmm.andypj.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://tqk.hesvh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wwe.meibo888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gfs.yvedp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xlb.ydzc1.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jec.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://hxi.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qay.hesvh.cn

[H03] 主动抛出异常
来源：http://gzd.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://cdk.yj202588.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xcp.fzhhl.top

JS:   throw new Error("错误信息");
来源：http://bqj.vehdjk.com

TS:   throw new Error("错误信息");
来源：http://phq.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ins.zhijiandao.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oxo.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fzl.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://guw.bjfxy.top

[H04] 自定义异常类型
来源：http://bxp.hywenlv.cn

Py:   class MyError(Exception): pass
来源：http://wag.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://maj.fktsv.cn

JS:   class MyError extends Error {}
来源：http://waj.c1oappe.top

TS:   class MyError extends Error {}
来源：http://hxo.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://hgf.ydzc1.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vve.yuxming.cn

Ruby: class MyError < StandardError; end
来源：http://mcs.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://obp.hnxiangtu.top

[H05] 捕获特定类型
来源：http://zzi.nanxuanxn.top

Py:   except ValueError as e:
来源：http://txc.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pzf.zdbjq.cn

JS:   if (e instanceof TypeError) {}
来源：http://wpj.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://gwn.fengsongda.top

Java: catch (IOException | SQLException e) {}
来源：http://dus.tarul.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jmg.snrcjt.cn

Ruby: rescue ArgumentError => e
来源：http://idj.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dcg.jinqigfzy.top

[H06] 可选值 / 空值安全访问
来源：http://ywa.gzhubu.top

Py:   value = d.get("k") or default
来源：http://tqc.ctjpmb.com

PHP:  $v = $d["k"] ?? null;
来源：http://dvc.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://zoa.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aes.hfpthk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ntv.fehbvm.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ltg.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://wsz.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://rpn.yangfankeji.com

[H07] 断言
来源：http://tdl.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://kbf.uphjek.com

PHP:  assert($x > 0);
来源：http://gbi.jinqigfzy.top

JS:   console.assert(x > 0);
来源：http://htc.hammf.cn

TS:   console.assert(x > 0);
来源：http://ogg.fengsongda.top

Java: assert x > 0 : "必须为正";
来源：http://jdm.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gdd.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://bgw.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://bhh.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://erj.gogol.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://cal.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://scs.vqdsnc.cn

JS:   e.message;  e.stack
来源：http://fri.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xrd.fzhhl.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pgc.shzxlz.cn

Go:   err.Error()
来源：http://phc.ehwqpu.com

Ruby: e.message;  e.backtrace
来源：http://iab.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://pel.birdmap.top

[H09] 带错误码的异常
来源：http://hao.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zkv.chenlongwang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://njf.gaohongyu789.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rcr.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qos.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ljo.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zxz.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://how.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ywv.yj20258.top

[H10] 资源自动释放
来源：http://hwv.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://xxs.chenjidiqi.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rci.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yua.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nod.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fmh.shzxlz.cn

Go:   defer f.Close()
来源：http://wsu.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uvh.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oca.tianlin.xyz

================================================================================
来源：http://ubt.xinyue.icu

I. 正则表达式
来源：http://ppb.xingfuxueyuan.xyz

================================================================================
来源：http://tpt.gzhubu.top

[I01] 判断是否匹配
来源：http://zlm.tianlin.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tei.fengsongda.top

PHP:  preg_match('/\d+/', $s);
来源：http://bal.svipenyu.cn

JS:   /\d+/.test(s)
来源：http://hor.gotoacloud.top

TS:   /\d+/.test(s)
来源：http://odc.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vlo.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pct.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://qqs.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rpz.andypj.xyz

[I02] 提取所有匹配
来源：http://vck.nanxinkj.top

Py:   re.findall(r"\d+", s)
来源：http://dja.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vpa.chenjidiqi.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jwj.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://mrc.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jtf.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ulw.gotoacloud.top

Ruby: s.scan(/\d+/)
来源：http://dod.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eeo.ctjpmb.com

[I03] 提取捕获分组
来源：http://gct.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://abq.jqgfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rng.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lhr.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bre.dashuyun.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hle.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gjl.zdqjudy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pea.svipenyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://spw.aizwys.cn

[I04] 正则替换
来源：http://lhk.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wfs.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fsp.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://vbd.zhoulong.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://nfa.tanke756.top

Java: s.replaceAll("\\d+", "#")
来源：http://wgl.hfpthk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nkl.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rtz.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vcr.pengpengdd.cyou

[I05] 按正则拆分
来源：http://zdq.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pnp.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zvm.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://kxe.52xcode.cn

TS:   s.split(/\s*,\s*/)
来源：http://bvj.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://rau.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mtd.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://ywc.zhoulong.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xzd.andypj.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vtr.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ieh.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yyh.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://asx.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jyo.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rzy.jlsjyb.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xqp.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hjc.ppjwa.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wsg.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://rgw.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mbu.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bfs.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xyq.jlsjyb.cn

TS:   /error/gim
来源：http://jjl.yuanzhike.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://guv.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dtk.52xcode.cn

Ruby: s.scan(/error/i)
来源：http://ktn.yfazqb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://thz.hongshengwenyu.top

[I08] 贪婪与非贪婪匹配
来源：http://dzy.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://atn.xylfe.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xpx.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ojn.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bfz.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://par.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zbb.wangshuangyany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eax.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jkg.cashguo.top

================================================================================
来源：http://xmz.ctjpmb.com

J. 日期与时间
来源：http://edi.hcnkem.com

================================================================================
来源：http://hyd.meibo888.top

[J01] 获取当前时间
来源：http://znl.zdbjq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://czd.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cze.vehdjk.com

JS:   new Date();  Date.now()
来源：http://zwq.guannengcc.top

TS:   new Date();  Date.now()
来源：http://xlx.jyoumei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bug.mhx1999.top

Go:   time.Now()
来源：http://fjk.yj202588.top

Ruby: Time.now
来源：http://knu.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://orn.dashuyun.cn

[J02] 格式化输出
来源：http://sbf.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://krb.smart0.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qay.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jgp.9152youxi.cn

TS:   d.toISOString()
来源：http://ijk.shangyingyoupin.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://run.9152youxi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://goo.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yyq.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yqv.tarul.cn

[J03] 字符串解析为日期
来源：http://yen.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dke.yj20258.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://grd.zhijiandao.cn

JS:   new Date("2024-01-02")
来源：http://qfk.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://leo.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xec.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vnh.yonumen.top

Ruby: Date.parse("2024-01-02")
来源：http://niv.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://luf.9152youxi.cn

[J04] 时间戳与日期互转
来源：http://tsx.c1oappe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nyl.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xix.jqgufenzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mva.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vbp.jyoumei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xgc.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tyu.jinqigfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sil.zhixingplan.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hnj.zhongyouzk.top

[J05] 时间加减（加 7 天）
来源：http://tsg.yongpay.top

Py:   now + timedelta(days=7)
来源：http://omw.sxryk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ayt.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hpz.52xcode.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pkh.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://wwo.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yjg.xuanzx.com

Ruby: Time.now + 7 * 86400
来源：http://qla.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ced.ydjk.org.cn

[J06] 计算两时间之差
来源：http://yiz.ctjpmb.com

Py:   (end - start).total_seconds()
来源：http://yrm.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://iul.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jim.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lsm.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://doi.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://rff.zdbjq.cn

Ruby: end - start                 # 返回秒数
来源：http://uvu.fehbvm.com

C#:   (end - start).TotalSeconds
来源：http://qdc.pengpengdd.cyou

[J07] 比较两个日期
来源：http://gxk.chenjidiqi.icu

Py:   d1 < d2;  d1 == d2
来源：http://xax.fengsongda.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ysj.sxryk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://eru.iojbl.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hsd.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xft.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://imv.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://aoy.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://xyv.zycfv.cn

[J08] 提取年月日与星期
来源：http://vyc.aizwys.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cqn.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uan.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://spt.wangshuangyany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mtj.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rbj.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ltl.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tax.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fhv.xziqi.cn

[J09] 时区处理
来源：http://udf.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jbq.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rbf.zhixingplan.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://veh.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://myd.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tjt.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zcf.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bgh.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gco.yuxming.cn

[J10] 取今天 / 本月第一天
来源：http://tsd.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bsb.52xcode.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://efs.gzhubu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mrr.wangshuangyany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pjc.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uhv.jiagoushi.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hjh.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zuo.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dlv.hcnkem.com

================================================================================
来源：http://bbf.ydzc1.top

K. JSON 与序列化
来源：http://mrf.cheryme.top

================================================================================
来源：http://mre.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://mot.yonumen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nei.daxiang520.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dhe.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://cjg.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://iqa.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jzn.yuxming.cn

Go:   json.Marshal(obj)
来源：http://qey.sweek.top

Ruby: obj.to_json                                     // require "json"
来源：http://ouw.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bzu.yj20258.top

[K02] JSON 字符串转对象
来源：http://dwg.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://ext.guowangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zta.snrcjt.cn

JS:   JSON.parse(s)
来源：http://qjp.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://zxc.yj20258.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uji.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ezg.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://kqf.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xqf.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://snx.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://atk.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ygy.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qhe.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://avc.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://juo.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vkk.ppjwa.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qlb.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kmi.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://ntd.daxiang520.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hvf.andypj.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xdf.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pbj.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ddl.sjlbkw.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ojw.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qsc.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://jia.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tcf.ehwqpu.com

[K05] 深拷贝对象
来源：http://ycw.ywan-chungtsiang.top

Py:   copy.deepcopy(obj)
来源：http://zmy.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://xjp.ywan-chungtsiang.top

JS:   structuredClone(obj)
来源：http://ndx.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://eex.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://seu.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ssd.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ckf.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://puo.ydzc1.top

[K06] 解析 URL 查询串
来源：http://jep.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mlg.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nod.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kbs.shzxlz.cn


<!-- 参考信息 -->