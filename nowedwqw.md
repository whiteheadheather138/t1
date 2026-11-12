代发 wailian999

[H03] 主动抛出异常
来源：http://ouh.xinyue.icu

Py:   raise ValueError("错误信息")
来源：http://tfs.tian-w.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ptt.andypj.xyz

JS:   throw new Error("错误信息");
来源：http://yds.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://ghm.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://unp.mhx1999.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uog.shangyingyoupin.top

Ruby: raise ArgumentError, "错误信息"
来源：http://emh.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://iwa.uphjek.com

[H04] 自定义异常类型
来源：http://opv.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://udt.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://ntq.bbcook.cn

JS:   class MyError extends Error {}
来源：http://thr.fengsongda.top

TS:   class MyError extends Error {}
来源：http://rkk.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://iff.wangshuangyany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ziq.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://vrz.birdmap.top

C#:   class MyException : Exception {}
来源：http://fdx.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://nnc.tian-w.cn

Py:   except ValueError as e:
来源：http://ddk.shanyushiyangtech.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fry.sxryk.cn

JS:   if (e instanceof TypeError) {}
来源：http://lhw.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://nax.fanxiaobao.xyz

Java: catch (IOException | SQLException e) {}
来源：http://prj.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cbw.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://ily.jinghuilouyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qje.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://sni.fktsv.cn

Py:   value = d.get("k") or default
来源：http://ucr.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://zwq.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://utm.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xxe.haohaochexian.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xmc.hfpthk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fuf.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://ykc.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://gdz.zdqjudy.top

[H07] 断言
来源：http://mbr.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://kko.kuanghao11.cn

PHP:  assert($x > 0);
来源：http://epf.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://lqv.shuidangran.top

TS:   console.assert(x > 0);
来源：http://bsf.hcnkem.com

Java: assert x > 0 : "必须为正";
来源：http://fgh.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uxv.wangshuangyany.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gkd.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://bgj.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://jxq.shzxlz.cn

Py:   str(e);  traceback.format_exc()
来源：http://ffm.dianchejie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lsg.yonumen.top

JS:   e.message;  e.stack
来源：http://and.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rfn.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kpm.tarul.cn

Go:   err.Error()
来源：http://ysy.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://eaz.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://jcu.andypj.xyz

[H09] 带错误码的异常
来源：http://hec.jinqigfzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iyn.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rth.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rhh.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xkx.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pdd.vehdjk.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pzy.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://vwb.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://amw.daria6918.cn

[H10] 资源自动释放
来源：http://tfv.yuanzhike.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cqk.ybcxt.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qbs.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lfc.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wwt.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wqw.tarul.cn

Go:   defer f.Close()
来源：http://ute.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fqx.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wup.chenjidiqi.icu

================================================================================
来源：http://gge.yonumen.top

I. 正则表达式
来源：http://ugt.fanxiaobao.xyz

================================================================================
来源：http://uce.uphjek.com

[I01] 判断是否匹配
来源：http://qbt.bjfxy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rzk.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://deq.yanxiufei.cn

JS:   /\d+/.test(s)
来源：http://oki.ywan-chungtsiang.top

TS:   /\d+/.test(s)
来源：http://gyx.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jjm.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nfx.quarkkingdee.top

Ruby: s.match?(/\d+/)
来源：http://fgy.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qal.uphjek.com

[I02] 提取所有匹配
来源：http://cfx.yfazqb.com

Py:   re.findall(r"\d+", s)
来源：http://kmh.jinyuanbaomall.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vrq.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oht.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://vdw.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lyx.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sey.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://yqw.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ssc.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://uyt.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wrm.nanxinkj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tkx.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://weq.chenzaomai.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tgk.uphjek.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iwn.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kpy.c1oappe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kir.wangdashe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wnq.bjfxy.top

[I04] 正则替换
来源：http://bhy.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://egt.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gml.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lrl.316326.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://nqz.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://upy.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://inv.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hpd.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hrb.yuanzhike.top

[I05] 按正则拆分
来源：http://isz.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jcd.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vxf.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://hgu.yj202588.top

TS:   s.split(/\s*,\s*/)
来源：http://uve.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://qxn.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gut.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wpo.zhiwuduotai.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zqv.snrcjt.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jbl.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kkf.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://grm.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dya.fehbvm.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://frg.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bbm.9152youxi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hpj.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://utp.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zzd.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://dfb.ydzc1.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dyx.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gsf.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uqz.fengsongda.top

TS:   /error/gim
来源：http://wxb.0kj1m.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blf.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wzx.iojbl.cn

Ruby: s.scan(/error/i)
来源：http://mba.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uff.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://odq.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://smw.shanyushiyangtech.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bqt.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mwb.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fqd.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qgl.316326.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jty.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jww.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jdt.zhoulong.xyz

================================================================================
来源：http://mlb.fktsv.cn

J. 日期与时间
来源：http://jvk.yvedp.cn

================================================================================
来源：http://jlb.yongpay.top

[J01] 获取当前时间
来源：http://phc.hnxiangtu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ctj.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qva.yuxming.cn

JS:   new Date();  Date.now()
来源：http://kfb.guannengcc.top

TS:   new Date();  Date.now()
来源：http://glc.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vgj.gotoacloud.top

Go:   time.Now()
来源：http://wzq.tarul.cn

Ruby: Time.now
来源：http://pir.fktsv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nth.gogol.net.cn

[J02] 格式化输出
来源：http://ddm.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tvr.sxryk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://myw.vehdjk.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ikt.hywenlv.cn

TS:   d.toISOString()
来源：http://yoi.iojbl.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://egp.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dsb.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dnp.xylfe.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ulv.jlsjyb.cn

[J03] 字符串解析为日期
来源：http://ckf.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://auk.zhoulong.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jmw.shanyushiyangkeji.top

JS:   new Date("2024-01-02")
来源：http://ejz.yfazqb.com

TS:   new Date("2024-01-02")
来源：http://amt.sjlbkw.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jgn.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ury.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://xwk.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wtd.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://osi.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rty.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jky.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fpe.nanxinkj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fbv.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vki.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vxy.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wmu.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://scb.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://gew.shanyushiyangtech.top

Py:   now + timedelta(days=7)
来源：http://ccw.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qsb.bjfxy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ljh.smart0.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uxw.shuidangran.top

Java: LocalDate.now().plusDays(7)
来源：http://ubp.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dxm.zhaomingkeji.xyz

Ruby: Time.now + 7 * 86400
来源：http://cyg.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://xhj.0kj1m.cn

[J06] 计算两时间之差
来源：http://dim.0kj1m.cn

Py:   (end - start).total_seconds()
来源：http://zoh.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://fkf.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wwf.hysaishi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://weg.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pnn.tian-w.cn

Go:   end.Sub(start).Hours()
来源：http://gty.gotoacloud.top

Ruby: end - start                 # 返回秒数
来源：http://ydu.jqgufenzy.top

C#:   (end - start).TotalSeconds
来源：http://iln.uphjek.com

[J07] 比较两个日期
来源：http://ydy.hnxiangtu.top

Py:   d1 < d2;  d1 == d2
来源：http://jdq.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ccw.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://now.fanxiaobao.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://pjf.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rpt.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rwm.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://uml.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://sox.jlsjyb.cn

[J08] 提取年月日与星期
来源：http://hbh.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ino.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kif.zhoulong.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bwe.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fqi.yangfankeji.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tcd.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://znj.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zzm.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yeh.fanxiaobao.xyz

[J09] 时区处理
来源：http://fgg.dianchejie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://obq.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vcm.jinqigfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lon.fehbvm.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nur.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ies.xingfuxueyuan.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bhx.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rly.chenjidiqi.icu

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eie.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://bua.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rfb.hongshengwenyu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jal.ehwqpu.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jrl.xuanzx.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vcb.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vta.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wbp.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mpx.sweek.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jzh.zhixingplan.top

================================================================================
来源：http://pmf.nanxinkj.top

K. JSON 与序列化
来源：http://tkn.shuidangran.top

================================================================================
来源：http://xtd.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://dve.tarul.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lym.birdmap.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ksy.shzxlz.cn

JS:   JSON.stringify(obj)
来源：http://nnc.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://jaj.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tvv.tanke756.top

Go:   json.Marshal(obj)
来源：http://opb.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://ngd.0kj1m.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dyk.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://ncn.havefunace.top

Py:   json.loads(s)
来源：http://xyr.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sws.c1oappe.top

JS:   JSON.parse(s)
来源：http://yrq.jinyuanbaomall.cn

TS:   JSON.parse(s)
来源：http://orp.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mbx.hesvh.cn

Go:   json.Unmarshal(data, &v)
来源：http://prx.daxiang520.top

Ruby: JSON.parse(s)
来源：http://zhs.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://enz.jinqigfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://ife.xinyue.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aca.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vil.svipenyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qge.hcnkem.com

TS:   JSON.stringify(obj, null, 2)
来源：http://gnj.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gcr.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qmm.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://bst.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qpu.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://bqe.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kls.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://skw.fehbvm.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zlo.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wvc.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rig.xziqi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ujy.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://czn.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fne.tarul.cn

[K05] 深拷贝对象
来源：http://wxd.xylfe.cn

Py:   copy.deepcopy(obj)
来源：http://yus.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://rxk.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://qco.jinqigfzy.top

TS:   structuredClone(obj)
来源：http://cle.zdqjudy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mza.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uye.uphjek.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uyk.yj20258.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tnl.chenzaomai.com

[K06] 解析 URL 查询串
来源：http://myt.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bft.birdmap.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zrq.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mjz.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yya.vehdjk.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eyn.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qyu.zdqjudy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iop.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://doc.dashuyun.cn

[K07] 进制转换
来源：http://ogu.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mld.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cvn.hongshengwenyu.top


<!-- 参考信息 -->