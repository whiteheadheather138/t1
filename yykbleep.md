代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://ulg.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kza.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nmq.zhiwuduotai.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mgb.xylfe.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wem.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://crs.mhx1999.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ban.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://smw.ydzc1.top

[H03] 主动抛出异常
来源：http://qko.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://rwe.cqqwz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eul.wangdashe.top

JS:   throw new Error("错误信息");
来源：http://dgj.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://ukt.shzxlz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cqy.shzxlz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wvv.ydzc1.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ehg.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://mps.ivvv.top

[H04] 自定义异常类型
来源：http://esg.cheryme.top

Py:   class MyError(Exception): pass
来源：http://iqv.redwolf501.top

PHP:  class MyError extends RuntimeException {}
来源：http://ghz.xuanzx.com

JS:   class MyError extends Error {}
来源：http://vdq.birdmap.top

TS:   class MyError extends Error {}
来源：http://vrd.jqgfzy.top

Java: class MyException extends RuntimeException {}
来源：http://urq.yanxiufei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qmi.ehwqpu.com

Ruby: class MyError < StandardError; end
来源：http://zgf.zhaomingkeji.xyz

C#:   class MyException : Exception {}
来源：http://rzn.sweek.top

[H05] 捕获特定类型
来源：http://jpl.ybcxt.top

Py:   except ValueError as e:
来源：http://xfp.hfpthk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oxd.jianghu66.top

JS:   if (e instanceof TypeError) {}
来源：http://yoe.uphjek.com

TS:   if (e instanceof TypeError) {}
来源：http://ffe.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://yps.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pat.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://nhd.yonumen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yhn.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://tkt.birdmap.top

Py:   value = d.get("k") or default
来源：http://wpx.yangfankeji.com

PHP:  $v = $d["k"] ?? null;
来源：http://dze.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://nba.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://xqa.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dsq.uphjek.com

Go:   if v, ok := m["k"]; ok { }
来源：http://qqr.sweek.top

Ruby: d&.dig(:a, :b)
来源：http://hbm.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://vch.ydzc1.top

[H07] 断言
来源：http://ume.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://ezy.sweek.top

PHP:  assert($x > 0);
来源：http://fok.xinyue.icu

JS:   console.assert(x > 0);
来源：http://hha.yongpay.top

TS:   console.assert(x > 0);
来源：http://xui.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://sia.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tee.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://jsl.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://ugb.wangshuangyany.cn

[H08] 获取错误信息与堆栈
来源：http://ego.guowangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://luv.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qhv.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://cny.bbcook.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xvr.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://kdr.hcnkem.com

Go:   err.Error()
来源：http://qvs.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://mzh.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://qge.jlsjyb.cn

[H09] 带错误码的异常
来源：http://jus.316326.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://njh.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jtm.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iyj.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ymh.kuanghao11.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jtk.xziqi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oqj.guowangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://yxi.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lze.jinyuanbaomall.cn

[H10] 资源自动释放
来源：http://gzy.svipenyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cho.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aoj.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ljp.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tzr.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aiq.yj202588.top

Go:   defer f.Close()
来源：http://ijs.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sbj.yongpay.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nnt.bbcook.cn

================================================================================
来源：http://ixz.shuidangran.top

I. 正则表达式
来源：http://ajz.yonumen.top

================================================================================
来源：http://gqb.xylfe.cn

[I01] 判断是否匹配
来源：http://cpk.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://juz.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rou.xuanzx.com

JS:   /\d+/.test(s)
来源：http://yve.chenjidiqi.icu

TS:   /\d+/.test(s)
来源：http://nvc.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cwx.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xwh.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://dnz.hnqzz.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rzy.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://efm.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://hxb.hfpthk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yvn.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lgg.guowangkeji.top

TS:   s.match(/\d+/g)
来源：http://cqp.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ikk.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ykz.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://qjc.guowangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qhj.jqgfzy.top

[I03] 提取捕获分组
来源：http://owx.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rty.dashuyun.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yxa.pengpengdd.cyou

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ent.dianchejie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yno.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aik.xylfe.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rdq.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zsk.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://typ.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://lcv.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://eng.ehwqpu.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wee.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vuj.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://hqr.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://vdc.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xqg.hnqzz.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pla.guannengcc.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gcq.vehdjk.com

[I05] 按正则拆分
来源：http://xkj.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mck.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zjf.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://dng.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://cxa.hnqzz.top

Java: s.split("\\s*,\\s*")
来源：http://sxx.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://man.gzhubu.top

Ruby: s.split(/\s*,\s*/)
来源：http://mjj.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pnb.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tyu.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jrr.tarul.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ged.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jfr.smart0.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ftu.zhixingplan.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zhs.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iat.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lov.hnqzz.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qkv.shanyushiyangtech.top

[I07] 忽略大小写与多行模式
来源：http://lim.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ssf.dashuyun.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vnq.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rwl.hfpthk.cn

TS:   /error/gim
来源：http://zxg.hfpthk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bfg.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://grv.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://epo.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qmv.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://oyu.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yew.yuxming.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://upp.nanxuanxn.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://csg.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nze.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xre.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gzy.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wnf.chenjidiqi.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rpo.haohaochexian.top

================================================================================
来源：http://kxx.hammf.cn

J. 日期与时间
来源：http://ohh.zdqjudy.top

================================================================================
来源：http://puf.yj20258.top

[J01] 获取当前时间
来源：http://afn.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ecx.haohaochexian.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rja.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://qhh.yueranfly.top

TS:   new Date();  Date.now()
来源：http://vgi.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kbq.aizwys.cn

Go:   time.Now()
来源：http://iae.jinqigfzy.top

Ruby: Time.now
来源：http://gar.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mas.yangfankeji.com

[J02] 格式化输出
来源：http://lzf.zhiwuduotai.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lyr.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qgu.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lfk.snrcjt.cn

TS:   d.toISOString()
来源：http://oly.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fcn.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lvs.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kdn.zhiwuduotai.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iuk.xylfe.cn

[J03] 字符串解析为日期
来源：http://lfu.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hqg.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kuu.tarul.cn

JS:   new Date("2024-01-02")
来源：http://bqm.zhixingplan.top

TS:   new Date("2024-01-02")
来源：http://quh.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dzd.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gyn.316326.xyz

Ruby: Date.parse("2024-01-02")
来源：http://efv.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://snm.xingfuxueyuan.xyz

[J04] 时间戳与日期互转
来源：http://sai.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gbr.fengsongda.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ffh.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qzy.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fyn.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bij.mhx1999.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zae.yanxiufei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xxj.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://seb.c1oappe.top

[J05] 时间加减（加 7 天）
来源：http://afs.pycfn.com

Py:   now + timedelta(days=7)
来源：http://fiy.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nnw.jinqigfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eat.hammf.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rit.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://der.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dcv.hnxiangtu.top

Ruby: Time.now + 7 * 86400
来源：http://wjr.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://woh.vehdjk.com

[J06] 计算两时间之差
来源：http://orl.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://jfm.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://aho.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xjs.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hgl.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://umw.ivvv.top

Go:   end.Sub(start).Hours()
来源：http://cwp.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://toy.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://noi.yonumen.top

[J07] 比较两个日期
来源：http://ktu.iojbl.cn

Py:   d1 < d2;  d1 == d2
来源：http://lmc.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://opp.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://gaw.aizwys.cn

TS:   d1.getTime() < d2.getTime()
来源：http://srp.nanxinkj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mji.yj202588.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xac.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://uoh.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://lxb.shangyingyoupin.top

[J08] 提取年月日与星期
来源：http://vbi.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wjm.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yst.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eld.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mjj.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jzn.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ezf.yongpay.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kmd.shanyushiyangtech.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://saa.hywenlv.cn

[J09] 时区处理
来源：http://qux.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://etj.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ewt.jinqigufen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://krf.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xcm.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hjm.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lve.zhaomingkeji.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://hwj.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kyh.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://cvb.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://baz.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://een.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tfw.shanyushiyangtech.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://puj.quarkkingdee.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zrq.sysykeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://brh.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ems.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://njc.hcnkem.com

================================================================================
来源：http://nov.yj20258888.top

K. JSON 与序列化
来源：http://vox.svipenyu.cn

================================================================================
来源：http://iof.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://nrq.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aci.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kxa.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://exz.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://qgq.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nvt.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://yay.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://dpc.gzhubu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nat.zhoulong.xyz

[K02] JSON 字符串转对象
来源：http://lft.redwolf501.top

Py:   json.loads(s)
来源：http://tzw.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bcc.cheryme.top

JS:   JSON.parse(s)
来源：http://rwu.jinyuanbaomall.cn

TS:   JSON.parse(s)
来源：http://qua.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mfu.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://mfe.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://sdl.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bdg.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://djp.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rgo.yvedp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mcu.yfazqb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://nzf.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lbi.gaohongyu789.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yjr.ywan-chungtsiang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tyh.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://ydy.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tpn.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://dhh.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cxv.jqgufenzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ydu.ydjk.org.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nsd.ydzc1.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hpq.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://crj.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lzs.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qcb.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mor.yongpay.top

[K05] 深拷贝对象
来源：http://nkw.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://bpl.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://gts.jiagoushi.top

JS:   structuredClone(obj)
来源：http://vwx.xuetiantiany.cn

TS:   structuredClone(obj)
来源：http://cmc.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hts.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rms.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yqz.bjfxy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ptm.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://hze.bjfxy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xbj.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://res.dashuyun.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ysd.tianlin.xyz


<!-- 参考信息 -->