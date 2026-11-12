代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://hnt.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wfz.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ntg.cashguo.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tnu.yueranfly.top

Java: try { f(); } finally { cleanup(); }
来源：http://iqy.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bnr.zhiwuduotai.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zlg.hongshengwenyu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uhp.yanxiufei.cn

[H03] 主动抛出异常
来源：http://ete.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://mjd.gzhubu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iyl.pengpengdd.cyou

JS:   throw new Error("错误信息");
来源：http://cpp.vqdsnc.cn

TS:   throw new Error("错误信息");
来源：http://inw.fengsongda.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lfx.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rhx.sweek.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qww.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://lir.shanyushiyangkeji.top

[H04] 自定义异常类型
来源：http://ork.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://gzk.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://rvr.zhiwuduotai.top

JS:   class MyError extends Error {}
来源：http://rri.daria6918.cn

TS:   class MyError extends Error {}
来源：http://uas.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://nip.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mvh.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://dxf.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://nni.yvedp.cn

[H05] 捕获特定类型
来源：http://amw.hongshengwenyu.top

Py:   except ValueError as e:
来源：http://gfz.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eyv.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://ydq.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://dri.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://bfc.havefunace.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://giv.cashguo.top

Ruby: rescue ArgumentError => e
来源：http://ohm.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xyx.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://uau.yvedp.cn

Py:   value = d.get("k") or default
来源：http://jpj.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://lae.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://awn.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://aix.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://itu.hywenlv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yse.cheryme.top

Ruby: d&.dig(:a, :b)
来源：http://nca.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://keg.zhengqikj.top

[H07] 断言
来源：http://aor.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://jpr.xziqi.cn

PHP:  assert($x > 0);
来源：http://hfs.316326.xyz

JS:   console.assert(x > 0);
来源：http://jmb.hysaishi.cn

TS:   console.assert(x > 0);
来源：http://lyu.yanxiufei.cn

Java: assert x > 0 : "必须为正";
来源：http://mjr.nanxuanxn.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://szn.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://mdy.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://try.jinqigfzy.top

[H08] 获取错误信息与堆栈
来源：http://yui.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://tgl.tianlin.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://usr.guowangkeji.top

JS:   e.message;  e.stack
来源：http://dqm.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cgs.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://blu.havefunace.top

Go:   err.Error()
来源：http://zqz.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://sww.feifeiyinyue.top

C#:   e.Message;  e.StackTrace
来源：http://wpf.yonumen.top

[H09] 带错误码的异常
来源：http://bzo.wangdashe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ihs.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sox.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ttv.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dar.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dly.cdnleiting.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xtj.ppjwa.cn

Ruby: raise MyError.new("fail", 500)
来源：http://amp.chenjidiqi.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://kyp.hywenlv.cn

[H10] 资源自动释放
来源：http://uwk.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kic.yvedp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jpe.zhoulong.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fgw.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kjj.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qhp.zhoulong.xyz

Go:   defer f.Close()
来源：http://dup.52xcode.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xfi.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dva.sysykeji.top

================================================================================
来源：http://brl.zdqjudy.top

I. 正则表达式
来源：http://ddt.meibo888.top

================================================================================
来源：http://kgi.316326.xyz

[I01] 判断是否匹配
来源：http://qyz.ywan-chungtsiang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mmg.jinqigfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://zbn.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://cuc.vehdjk.com

TS:   /\d+/.test(s)
来源：http://mgm.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kaz.cucudq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bcu.ivvv.top

Ruby: s.match?(/\d+/)
来源：http://wzk.fanxiaobao.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qvh.mhx1999.top

[I02] 提取所有匹配
来源：http://acf.zhoulong.xyz

Py:   re.findall(r"\d+", s)
来源：http://yuo.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uni.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xqy.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://kro.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jcp.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ads.jqgfzy.top

Ruby: s.scan(/\d+/)
来源：http://hbn.zhoulong.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ikl.zhaomingkeji.xyz

[I03] 提取捕获分组
来源：http://cxh.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://egu.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vim.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uuj.yanxiufei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://swn.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mpx.sxryk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://plg.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hzu.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rko.hongshengwenyu.top

[I04] 正则替换
来源：http://umr.iojbl.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mbd.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zxg.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gxf.tianlin.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://vze.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://zob.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://imh.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://oql.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hkt.yonumen.top

[I05] 按正则拆分
来源：http://ddp.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://isa.zdqjudy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dbg.ehwqpu.com

JS:   s.split(/\s*,\s*/)
来源：http://cgx.fanxiaobao.xyz

TS:   s.split(/\s*,\s*/)
来源：http://zaw.zhijiandao.cn

Java: s.split("\\s*,\\s*")
来源：http://xna.aizwys.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://luj.dashuyun.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mox.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rpg.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uaz.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://boo.ctjpmb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gze.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mlh.yj202588.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uyv.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iyq.redwolf501.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gjt.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://npc.ctjpmb.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aax.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://zii.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://osl.0kj1m.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mmy.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sol.jinqigufen.top

TS:   /error/gim
来源：http://bos.ywan-chungtsiang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fnv.0kj1m.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kjj.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://smv.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uri.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://lte.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tax.wangshuangyany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tzt.aizwys.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lqf.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://clf.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vpr.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gwg.52xcode.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vwi.0kj1m.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fqi.shzxlz.cn

================================================================================
来源：http://pdb.feifeiyinyue.top

J. 日期与时间
来源：http://glz.52xcode.cn

================================================================================
来源：http://dom.ydzc1.top

[J01] 获取当前时间
来源：http://rqa.yfazqb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://mtz.yongpay.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zbt.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://fxg.gogol.net.cn

TS:   new Date();  Date.now()
来源：http://flb.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qdz.fehbvm.com

Go:   time.Now()
来源：http://anp.xuanzx.com

Ruby: Time.now
来源：http://lst.chenzaomai.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ldh.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://can.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gxl.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jol.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yvm.nanxinkj.top

TS:   d.toISOString()
来源：http://xop.cqqwz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yjo.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mkp.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oma.nwbrower.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wrx.jinqigufen.top

[J03] 字符串解析为日期
来源：http://xdn.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qgw.tianlin.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pfc.yueranfly.top

JS:   new Date("2024-01-02")
来源：http://niy.hammf.cn

TS:   new Date("2024-01-02")
来源：http://imx.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://jrv.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sai.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://myd.zdqjudy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sdz.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://hcp.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jzq.zhixingplan.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://csz.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tjq.ivvv.top

TS:   Math.floor(Date.now() / 1000)
来源：http://stu.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yhm.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ioe.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cau.smart0.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aok.yueranfly.top

[J05] 时间加减（加 7 天）
来源：http://slg.tarul.cn

Py:   now + timedelta(days=7)
来源：http://wdn.snrcjt.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vbj.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jnq.xinyue.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nxj.jqgufenzy.top

Java: LocalDate.now().plusDays(7)
来源：http://kbv.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jdq.fktsv.cn

Ruby: Time.now + 7 * 86400
来源：http://mbc.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://imp.ydzc1.top

[J06] 计算两时间之差
来源：http://toy.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://pws.nwbrower.top

PHP:  $end->diff($start)->days;
来源：http://ihl.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xyp.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cej.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://xrp.snrcjt.cn

Go:   end.Sub(start).Hours()
来源：http://jla.tianlin.xyz

Ruby: end - start                 # 返回秒数
来源：http://ylr.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://jdy.ctjpmb.com

[J07] 比较两个日期
来源：http://uge.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://lvm.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ogr.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://cfw.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://hua.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vte.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tla.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://zmv.vqdsnc.cn

C#:   d1 < d2;  d1 == d2
来源：http://urb.sweek.top

[J08] 提取年月日与星期
来源：http://khw.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rxj.shzxlz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://svs.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qno.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cjq.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oky.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fhd.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bms.fktsv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gwp.yangfankeji.com

[J09] 时区处理
来源：http://cmv.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bkg.iojbl.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ihd.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bwe.yj20258.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dja.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mpg.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mlx.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yfd.tarul.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dwj.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://uic.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ruw.fengsongda.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ipq.fanxiaobao.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cpr.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zdq.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ioe.daria6918.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ymz.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://udx.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://icr.chenjidiqi.icu

================================================================================
来源：http://cxf.gaohongyu789.top

K. JSON 与序列化
来源：http://zyp.yj20258888.top

================================================================================
来源：http://gcm.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://dxt.jinyuanbaomall.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jtt.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qra.ivvv.top

JS:   JSON.stringify(obj)
来源：http://ppu.nanxinkj.top

TS:   JSON.stringify(obj)
来源：http://tfv.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qen.ivvv.top

Go:   json.Marshal(obj)
来源：http://ljt.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://oef.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wzp.yj202588.top

[K02] JSON 字符串转对象
来源：http://sbt.gotoacloud.top

Py:   json.loads(s)
来源：http://eae.quarkkingdee.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sjv.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://ggx.tianlin.xyz

TS:   JSON.parse(s)
来源：http://hun.52xcode.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://txn.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://jsr.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://gyj.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://drc.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://pud.fehbvm.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hzj.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sgb.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hmi.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gjm.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dux.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kcd.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://xoj.gzhubu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dwi.yj20258.top

[K04] 读取 JSON 文件
来源：http://sao.fengsongda.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ehi.kuanghao11.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xhc.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tcc.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zis.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sog.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wdn.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qxf.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xzc.bjfxy.top

[K05] 深拷贝对象
来源：http://fcj.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://tij.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://ezn.nanxinkj.top

JS:   structuredClone(obj)
来源：http://jqr.svipenyu.cn

TS:   structuredClone(obj)
来源：http://mbw.sjlbkw.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nie.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jct.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hzs.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://rwz.hammf.cn

[K06] 解析 URL 查询串
来源：http://tbs.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cqi.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mee.sxryk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ofc.0kj1m.cn


<!-- 参考信息 -->