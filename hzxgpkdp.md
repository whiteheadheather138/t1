代发 wailian999

TS:   throw new Error("错误信息");
来源：http://gtm.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fvh.ivvv.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gph.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ktk.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://psn.gzhubu.top

[H04] 自定义异常类型
来源：http://bmt.nwbrower.top

Py:   class MyError(Exception): pass
来源：http://pff.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://smu.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://wmh.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://byg.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://atk.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yly.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://yxv.smart0.xyz

C#:   class MyException : Exception {}
来源：http://yca.hammf.cn

[H05] 捕获特定类型
来源：http://ukn.sufxvd.cn

Py:   except ValueError as e:
来源：http://irh.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bys.zhongyouzk.top

JS:   if (e instanceof TypeError) {}
来源：http://jel.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://dxh.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://jfk.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://udv.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://wki.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ikd.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://ktg.ivvv.top

Py:   value = d.get("k") or default
来源：http://uxm.iojbl.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kcv.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lnc.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zkr.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yah.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://okm.shanyushiyangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://qvv.hfpthk.cn

C#:   obj?.A?.B ?? default
来源：http://can.svipenyu.cn

[H07] 断言
来源：http://rcg.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://wqx.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://hax.xuetiantiany.cn

JS:   console.assert(x > 0);
来源：http://jsh.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://vpc.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://gwm.xylfe.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uwr.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qbw.hcnkem.com

C#:   Debug.Assert(x > 0);
来源：http://qvj.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://xhs.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://rks.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qcw.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://cly.xylfe.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dei.yvedp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bmn.ctjpmb.com

Go:   err.Error()
来源：http://xow.ydjk.org.cn

Ruby: e.message;  e.backtrace
来源：http://sdp.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://rtj.yanxiufei.cn

[H09] 带错误码的异常
来源：http://nhh.hfpthk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://usq.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nme.bbcook.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wzo.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kvi.chenzaomai.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kip.guowangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yat.zhijiandao.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zxn.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://eoo.jianghu66.top

[H10] 资源自动释放
来源：http://xvb.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wno.vqdsnc.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jfh.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fgy.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qfb.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pxn.hysaishi.cn

Go:   defer f.Close()
来源：http://poa.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://trp.hnqzz.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dzv.zhiwuduotai.top

================================================================================
来源：http://dyt.nwbrower.top

I. 正则表达式
来源：http://ujx.ivvv.top

================================================================================
来源：http://auy.hnqzz.top

[I01] 判断是否匹配
来源：http://bqx.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wmg.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://fex.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://lpv.tian-w.cn

TS:   /\d+/.test(s)
来源：http://vsw.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vie.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kvm.xingfuxueyuan.xyz

Ruby: s.match?(/\d+/)
来源：http://tih.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sbb.316326.xyz

[I02] 提取所有匹配
来源：http://djl.chenzaomai.com

Py:   re.findall(r"\d+", s)
来源：http://wxr.epnwcf.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://och.zhoulong.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zcg.zhixingplan.top

TS:   s.match(/\d+/g)
来源：http://dbw.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zmn.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ohf.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://gnj.vehdjk.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cbx.shzxlz.cn

[I03] 提取捕获分组
来源：http://heq.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ciu.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lir.yj20258.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sgm.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xvl.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cel.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gez.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://twg.9152youxi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lgc.vehdjk.com

[I04] 正则替换
来源：http://mre.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qbk.yvedp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zon.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://ilb.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://jqd.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://idi.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zuf.sufxvd.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fxr.guannengcc.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xva.uphjek.com

[I05] 按正则拆分
来源：http://lct.havefunace.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tfw.aizwys.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dal.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://stw.epnwcf.com

TS:   s.split(/\s*,\s*/)
来源：http://qoo.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://sxy.zhengqikj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nwe.pengpengdd.cyou

Ruby: s.split(/\s*,\s*/)
来源：http://uzb.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zbg.vehdjk.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jzz.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qgr.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cfz.jianghu66.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cqy.gzhubu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wba.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ryi.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lyi.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zvs.bjfxy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yxd.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://kub.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ecg.redwolf501.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iqr.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ubw.chenlongwang.top

TS:   /error/gim
来源：http://gzq.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://slz.chenlongwang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tgk.yj202588.top

Ruby: s.scan(/error/i)
来源：http://dyx.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ulh.c1oappe.top

[I08] 贪婪与非贪婪匹配
来源：http://ijj.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://odj.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pjh.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yhk.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gne.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zbb.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zrf.dashuyun.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uka.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tgy.yj20258888.top

================================================================================
来源：http://eqw.havefunace.top

J. 日期与时间
来源：http://crc.shzxlz.cn

================================================================================
来源：http://cfi.ydjk.org.cn

[J01] 获取当前时间
来源：http://aos.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qvd.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://itk.mhx1999.top

JS:   new Date();  Date.now()
来源：http://zde.zhoulong.xyz

TS:   new Date();  Date.now()
来源：http://jqd.xuetiantiany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rme.tanke756.top

Go:   time.Now()
来源：http://vqu.gogol.net.cn

Ruby: Time.now
来源：http://ltz.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kmi.sufxvd.cn

[J02] 格式化输出
来源：http://tjs.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oae.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ipn.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tsa.shzxlz.cn

TS:   d.toISOString()
来源：http://gka.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fhn.hnqzz.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tgd.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ncw.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://svl.xuetiantiany.cn

[J03] 字符串解析为日期
来源：http://gdg.hongshengwenyu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xwe.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uzm.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://efi.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://cos.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cpk.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nzv.yuanzhike.top

Ruby: Date.parse("2024-01-02")
来源：http://snv.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://heb.zycfv.cn

[J04] 时间戳与日期互转
来源：http://iaq.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mgv.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dns.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jwr.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wxl.xinyue.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oum.sufxvd.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ycp.xuanzx.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rvq.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qfj.wangdashe.top

[J05] 时间加减（加 7 天）
来源：http://jba.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://svn.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kgg.tianlin.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tet.smart0.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hss.tian-w.cn

Java: LocalDate.now().plusDays(7)
来源：http://evm.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hra.cqqwz.cn

Ruby: Time.now + 7 * 86400
来源：http://wbq.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://vqk.yuxming.cn

[J06] 计算两时间之差
来源：http://njj.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://eae.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://xes.bbcook.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dta.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eyf.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://wjc.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://cjh.wangdashe.top

Ruby: end - start                 # 返回秒数
来源：http://dpa.dianchejie.cn

C#:   (end - start).TotalSeconds
来源：http://bkk.jqgfzy.top

[J07] 比较两个日期
来源：http://xvj.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://dgl.jianghu66.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fus.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xcd.fzhhl.top

TS:   d1.getTime() < d2.getTime()
来源：http://iep.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://atj.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://btp.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rad.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://dva.jiagoushi.top

[J08] 提取年月日与星期
来源：http://lih.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xwf.cqqwz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iao.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nxd.svipenyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://umh.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lwa.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aco.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fvv.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xui.yonumen.top

[J09] 时区处理
来源：http://qhu.dianchejie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bbe.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xug.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mdb.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rhf.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lfu.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eeq.gogol.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iwh.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aft.ywan-chungtsiang.top

[J10] 取今天 / 本月第一天
来源：http://lrk.yueranfly.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lus.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bnk.shzxlz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://urf.gogol.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ujz.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qyf.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://akp.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zmn.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dkv.bbcook.cn

================================================================================
来源：http://mjs.redwolf501.top

K. JSON 与序列化
来源：http://zkj.jlsjyb.cn

================================================================================
来源：http://sef.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://lfr.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hmn.ydzc1.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jzu.yongpay.top

JS:   JSON.stringify(obj)
来源：http://emn.meibo888.top

TS:   JSON.stringify(obj)
来源：http://izw.xziqi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lsb.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://oaf.guowangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://til.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sgq.hfpthk.cn

[K02] JSON 字符串转对象
来源：http://ovp.jlsjyb.cn

Py:   json.loads(s)
来源：http://mof.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wjc.svipenyu.cn

JS:   JSON.parse(s)
来源：http://trv.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://jgn.xuetiantiany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rfb.52xcode.cn

Go:   json.Unmarshal(data, &v)
来源：http://rlm.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://nhk.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zin.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://uka.sxryk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kij.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rpt.vehdjk.com

JS:   JSON.stringify(obj, null, 2)
来源：http://dfh.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sra.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://prx.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://psl.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://rpk.cashguo.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zlo.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://dmc.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mez.yj20258888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ujb.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ivp.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://der.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://duf.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://riy.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ktf.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mwo.guannengcc.top

[K05] 深拷贝对象
来源：http://ydo.jianghu66.top

Py:   copy.deepcopy(obj)
来源：http://fyg.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://fcy.hnqzz.top

JS:   structuredClone(obj)
来源：http://yos.zhengqikj.top

TS:   structuredClone(obj)
来源：http://gyv.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hng.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oho.shanyushiyangtech.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gvj.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gjk.bbcook.cn

[K06] 解析 URL 查询串
来源：http://tbp.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zfh.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dss.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zkp.hnqzz.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mao.uphjek.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://thx.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fvb.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://def.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rio.xylfe.cn

[K07] 进制转换
来源：http://ogj.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tyw.zdbjq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dzh.xziqi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rjj.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mga.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cwz.jyoumei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ozg.dashuyun.cn


<!-- 参考信息 -->