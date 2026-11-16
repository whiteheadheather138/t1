代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://qbn.yongpay.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wgo.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://aql.pycfn.com

TS:   try { f(); } finally { cleanup(); }
来源：http://oul.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oib.chenzaomai.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://njp.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nvr.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ppd.vqdsnc.cn

[H03] 主动抛出异常
来源：http://vqt.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://oar.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://etj.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://lag.ppjwa.cn

TS:   throw new Error("错误信息");
来源：http://kbu.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ihy.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jns.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ymh.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zjz.yueranfly.top

[H04] 自定义异常类型
来源：http://qwi.sufxvd.cn

Py:   class MyError(Exception): pass
来源：http://vmr.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://jsd.sxryk.cn

JS:   class MyError extends Error {}
来源：http://vub.tian-w.cn

TS:   class MyError extends Error {}
来源：http://wkz.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://gaa.dashuyun.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tll.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://pro.tanke756.top

C#:   class MyException : Exception {}
来源：http://fml.jlsjyb.cn

[H05] 捕获特定类型
来源：http://xog.tianlin.xyz

Py:   except ValueError as e:
来源：http://rwr.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mhm.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://pdm.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://cdz.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://zyy.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wlg.jinyuanbaomall.cn

Ruby: rescue ArgumentError => e
来源：http://psl.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fas.ehwqpu.com

[H06] 可选值 / 空值安全访问
来源：http://zuf.nwbrower.top

Py:   value = d.get("k") or default
来源：http://jqn.xziqi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uwi.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://idx.zhaomingkeji.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://zgt.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kio.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xfd.shuidangran.top

Ruby: d&.dig(:a, :b)
来源：http://jvm.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://pxc.yuanzhike.top

[H07] 断言
来源：http://haq.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://kpb.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://ogf.pengpengdd.cyou

JS:   console.assert(x > 0);
来源：http://rik.xylfe.cn

TS:   console.assert(x > 0);
来源：http://fjp.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://wxq.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cvt.yj20258888.top

Ruby: raise "必须为正" unless x > 0
来源：http://oxu.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://aci.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://xxi.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://efb.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uak.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://hac.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lui.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tqg.guannengcc.top

Go:   err.Error()
来源：http://rla.zhengqikj.top

Ruby: e.message;  e.backtrace
来源：http://znr.bjfxy.top

C#:   e.Message;  e.StackTrace
来源：http://jmv.hammf.cn

[H09] 带错误码的异常
来源：http://zcz.svipenyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xcb.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qbs.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bau.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sot.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yiy.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hpv.fanxiaobao.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://vqx.gzhubu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ney.nanxuanxn.top

[H10] 资源自动释放
来源：http://olj.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mid.tianlin.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://csl.shanyushiyangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://olo.vqdsnc.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://emn.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gmx.fehbvm.com

Go:   defer f.Close()
来源：http://pvz.gogol.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tzj.yongpay.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wzo.hfpthk.cn

================================================================================
来源：http://bll.iojbl.cn

I. 正则表达式
来源：http://gwo.zhengqikj.top

================================================================================
来源：http://ppd.guannengcc.top

[I01] 判断是否匹配
来源：http://tvg.yanxiufei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kuh.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://fbb.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://oqs.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://eqa.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pcx.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iyw.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://gdd.hammf.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ijx.jinghuilouyu.cn

[I02] 提取所有匹配
来源：http://xax.0kj1m.cn

Py:   re.findall(r"\d+", s)
来源：http://bov.cqqwz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jki.sjlbkw.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ulu.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://hkm.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jsq.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://csj.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://ncx.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kpc.dianchejie.cn

[I03] 提取捕获分组
来源：http://ric.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ifb.sweek.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zag.cqqwz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gin.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hbg.tanke756.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://omb.gzhubu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://npd.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hry.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pgk.ywan-chungtsiang.top

[I04] 正则替换
来源：http://nhz.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://ljw.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zjz.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://vtm.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yik.mhx1999.top

Java: s.replaceAll("\\d+", "#")
来源：http://jul.hesvh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eam.zdqjudy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cwu.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ohv.vqdsnc.cn

[I05] 按正则拆分
来源：http://dxp.chenlongwang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tdl.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qqt.jianghu66.top

JS:   s.split(/\s*,\s*/)
来源：http://che.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://aty.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://fgc.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vso.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://tji.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jiz.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fsx.hfpthk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xjr.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wej.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pov.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gta.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yqp.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rsn.fehbvm.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mxk.shzxlz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ayk.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://wew.52xcode.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://due.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://muh.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ccu.shangyingyoupin.top

TS:   /error/gim
来源：http://lxx.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dlz.sysykeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ook.uphjek.com

Ruby: s.scan(/error/i)
来源：http://tlc.316326.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bks.snrcjt.cn

[I08] 贪婪与非贪婪匹配
来源：http://dww.svipenyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ycq.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jku.jinqigfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ccd.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ori.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://itm.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pwp.hesvh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://txb.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uya.xuetiantiany.cn

================================================================================
来源：http://jfg.yvedp.cn

J. 日期与时间
来源：http://xbo.ybcxt.top

================================================================================
来源：http://ard.yuxming.cn

[J01] 获取当前时间
来源：http://yli.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qnw.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oco.aibaodan.cn

JS:   new Date();  Date.now()
来源：http://tzz.cheryme.top

TS:   new Date();  Date.now()
来源：http://txw.316326.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://dcx.havefunace.top

Go:   time.Now()
来源：http://ijq.c1oappe.top

Ruby: Time.now
来源：http://dww.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hvp.cdnleiting.top

[J02] 格式化输出
来源：http://fzb.ehwqpu.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://syz.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jfb.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zer.0kj1m.cn

TS:   d.toISOString()
来源：http://qqa.fktsv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wah.yanxiufei.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wck.sxryk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tvj.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rqv.tianlin.xyz

[J03] 字符串解析为日期
来源：http://fqu.fengsongda.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qwc.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xjl.wangshuangyany.cn

JS:   new Date("2024-01-02")
来源：http://bqz.chenzaomai.com

TS:   new Date("2024-01-02")
来源：http://hda.pengpengdd.cyou

Java: LocalDate.parse("2024-01-02")
来源：http://nkl.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wpp.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://yeh.yongpay.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://abb.zycfv.cn

[J04] 时间戳与日期互转
来源：http://jft.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lvo.xuanzx.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zlv.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tmp.mhx1999.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mhq.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tzl.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tqk.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zgq.jianghu66.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://res.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://okf.bbcook.cn

Py:   now + timedelta(days=7)
来源：http://nvm.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://blx.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://scx.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yir.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://tqr.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fcq.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://hfy.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://nzo.xingfuxueyuan.xyz

[J06] 计算两时间之差
来源：http://uel.aibaodan.cn

Py:   (end - start).total_seconds()
来源：http://tnl.guannengcc.top

PHP:  $end->diff($start)->days;
来源：http://prc.zhijiandao.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uqj.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lfd.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://pmj.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://fkz.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://cmy.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://sja.havefunace.top

[J07] 比较两个日期
来源：http://kci.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://gel.yj202588.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://udp.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://fdw.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://pjs.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tvd.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lue.havefunace.top

Ruby: d1 < d2;  d1 == d2
来源：http://dbx.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://mig.guannengcc.top

[J08] 提取年月日与星期
来源：http://vaq.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ujm.chenjidiqi.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kfg.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cuc.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fgd.ydzc1.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iks.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gfu.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hgi.jianghu66.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ypv.mhx1999.top

[J09] 时区处理
来源：http://hyv.nanxuanxn.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yxq.nanxinkj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nhv.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://evw.sxryk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dcb.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tjc.wangdashe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dnk.iojbl.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://spf.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://owy.fktsv.cn

[J10] 取今天 / 本月第一天
来源：http://plo.gogol.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://trj.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ubr.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ecp.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lcl.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wma.c1oappe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jff.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ypi.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cxh.316326.xyz

================================================================================
来源：http://ahh.cqqwz.cn

K. JSON 与序列化
来源：http://nww.yj20258.top

================================================================================
来源：http://bnq.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://naz.cdnleiting.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wma.wangshuangyany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gjw.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://tpv.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://juq.yj202588.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mrx.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://cjq.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rwi.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://trb.jiagoushi.top

[K02] JSON 字符串转对象
来源：http://myy.ydjk.org.cn

Py:   json.loads(s)
来源：http://ynk.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ghm.ehwqpu.com

JS:   JSON.parse(s)
来源：http://qyr.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://hdh.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eki.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://xtq.tanke756.top

Ruby: JSON.parse(s)
来源：http://jgw.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jzs.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://qhz.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xub.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jrn.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://izy.gzhubu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bwz.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qyd.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eij.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vss.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xjg.hongshengwenyu.top

[K04] 读取 JSON 文件
来源：http://clw.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://thk.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kgk.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fdy.zhoulong.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gxb.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ctp.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kdm.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ewj.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xhu.jianghu66.top

[K05] 深拷贝对象
来源：http://lkm.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://nnx.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://gwm.feifeiyinyue.top

JS:   structuredClone(obj)
来源：http://odq.xingfuxueyuan.xyz

TS:   structuredClone(obj)
来源：http://hns.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://krx.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://byx.tianlin.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bok.kuanghao11.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oie.ivvv.top

[K06] 解析 URL 查询串
来源：http://fht.fengsongda.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sdf.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gan.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sye.hnxiangtu.top


<!-- 参考信息 -->