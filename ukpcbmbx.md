代发 wailian999

TS:   throw new Error("错误信息");
来源：http://giq.52xcode.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yqn.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pfd.hesvh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hng.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://olg.hysaishi.cn

[H04] 自定义异常类型
来源：http://emk.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://ifk.vehdjk.com

PHP:  class MyError extends RuntimeException {}
来源：http://rfn.ydzc1.top

JS:   class MyError extends Error {}
来源：http://jhz.52xcode.cn

TS:   class MyError extends Error {}
来源：http://ieu.zhixingplan.top

Java: class MyException extends RuntimeException {}
来源：http://sgb.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hwc.daria6918.cn

Ruby: class MyError < StandardError; end
来源：http://nvr.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://iiv.meibo888.top

[H05] 捕获特定类型
来源：http://lzv.zhijiandao.cn

Py:   except ValueError as e:
来源：http://ugb.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cjy.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://cci.cashguo.top

TS:   if (e instanceof TypeError) {}
来源：http://hxl.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://nws.svipenyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://poi.hongshengwenyu.top

Ruby: rescue ArgumentError => e
来源：http://kfv.quarkkingdee.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oom.aibaodan.cn

[H06] 可选值 / 空值安全访问
来源：http://xfy.daxiang520.top

Py:   value = d.get("k") or default
来源：http://rtu.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mvl.zdqjudy.top

JS:   obj?.a?.b;  d ?? default
来源：http://vbw.gaohongyu789.top

TS:   obj?.a?.b;  d ?? default
来源：http://eii.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wjr.316326.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://wge.xinyue.icu

Ruby: d&.dig(:a, :b)
来源：http://fep.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://bgz.kuanghao11.cn

[H07] 断言
来源：http://dun.zhixingplan.top

Py:   assert x > 0, "必须为正"
来源：http://zus.52xcode.cn

PHP:  assert($x > 0);
来源：http://jsv.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://nuj.tanke756.top

TS:   console.assert(x > 0);
来源：http://jxe.gotoacloud.top

Java: assert x > 0 : "必须为正";
来源：http://ofx.vqdsnc.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zjt.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bnq.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://ouq.jlsjyb.cn

[H08] 获取错误信息与堆栈
来源：http://nle.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://ypf.fzhhl.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ooj.yanxiufei.cn

JS:   e.message;  e.stack
来源：http://ccw.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wqa.mhx1999.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ngu.hysaishi.cn

Go:   err.Error()
来源：http://rfs.gzhubu.top

Ruby: e.message;  e.backtrace
来源：http://ene.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://rji.ivvv.top

[H09] 带错误码的异常
来源：http://vis.nwbrower.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bvr.nwbrower.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jhe.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oqc.andypj.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ulj.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dkj.shanyushiyangtech.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://biy.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://nrq.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kyq.cashguo.top

[H10] 资源自动释放
来源：http://pzj.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lku.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ggq.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hvi.sweek.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zuh.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qbn.ydjk.org.cn

Go:   defer f.Close()
来源：http://hjm.yonumen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nlr.dashuyun.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zri.yangfankeji.com

================================================================================
来源：http://dyv.gaohongyu789.top

I. 正则表达式
来源：http://kzd.fzhhl.top

================================================================================
来源：http://vxh.cdnleiting.top

[I01] 判断是否匹配
来源：http://wsg.tianlin.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ipx.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://elw.andypj.xyz

JS:   /\d+/.test(s)
来源：http://ndn.zdbjq.cn

TS:   /\d+/.test(s)
来源：http://zqq.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iig.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://odc.tanke756.top

Ruby: s.match?(/\d+/)
来源：http://gya.sjlbkw.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vnl.pycfn.com

[I02] 提取所有匹配
来源：http://lke.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://bty.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yek.chenlongwang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ise.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://kzx.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vpl.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uxa.shangyingyoupin.top

Ruby: s.scan(/\d+/)
来源：http://kii.yongpay.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wcs.daria6918.cn

[I03] 提取捕获分组
来源：http://yor.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://red.dianchejie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iju.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qwh.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jbt.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zpb.jinqigfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fld.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ioa.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sbg.sjlbkw.cn

[I04] 正则替换
来源：http://vtn.ppjwa.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mhk.fktsv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jvi.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nig.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yql.zhixingplan.top

Java: s.replaceAll("\\d+", "#")
来源：http://yeu.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://efe.sufxvd.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jzo.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xke.daria6918.cn

[I05] 按正则拆分
来源：http://osl.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xzs.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sqd.tarul.cn

JS:   s.split(/\s*,\s*/)
来源：http://dnn.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://roo.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://zdf.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pok.sufxvd.cn

Ruby: s.split(/\s*,\s*/)
来源：http://way.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ydk.chenlongwang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fjp.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ikc.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nig.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tvt.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://alp.fengsongda.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bnp.vehdjk.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nqt.wangdashe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://npy.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mnv.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://kmv.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bpj.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ijb.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vql.wangshuangyany.cn

TS:   /error/gim
来源：http://mfe.sweek.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xgd.smart0.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://skz.kuanghao11.cn

Ruby: s.scan(/error/i)
来源：http://kfi.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hiq.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://qjo.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hfj.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eab.yuanzhike.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rop.pycfn.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://stk.yuxming.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://knd.yueranfly.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://onm.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eyg.gotoacloud.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://man.ydzc1.top

================================================================================
来源：http://apa.yueranfly.top

J. 日期与时间
来源：http://kxs.hysaishi.cn

================================================================================
来源：http://yus.chenzaomai.com

[J01] 获取当前时间
来源：http://vjb.ctjpmb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://rvf.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dly.jinyuanbaomall.cn

JS:   new Date();  Date.now()
来源：http://xhw.yj20258.top

TS:   new Date();  Date.now()
来源：http://vbi.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pov.zycfv.cn

Go:   time.Now()
来源：http://nnp.dashuyun.cn

Ruby: Time.now
来源：http://gmx.sjlbkw.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sux.yj20258.top

[J02] 格式化输出
来源：http://fsd.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ccx.jinqigfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://whx.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vpw.daria6918.cn

TS:   d.toISOString()
来源：http://tbk.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://plq.chenlongwang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bri.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xcg.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wlu.sxryk.cn

[J03] 字符串解析为日期
来源：http://qcy.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gbd.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tah.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://lao.yongpay.top

TS:   new Date("2024-01-02")
来源：http://clb.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://wwv.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rhk.zhixingplan.top

Ruby: Date.parse("2024-01-02")
来源：http://eoc.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jvt.sweek.top

[J04] 时间戳与日期互转
来源：http://dsn.tian-w.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eof.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mct.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sap.jqgfzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ggt.yj20258888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mgg.birdmap.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dkw.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aby.hnxiangtu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ggp.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://rss.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://ibd.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sxd.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rbh.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mmc.sjlbkw.cn

Java: LocalDate.now().plusDays(7)
来源：http://uab.yj20258.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zej.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://peg.ydzc1.top

C#:   DateTime.Now.AddDays(7)
来源：http://ugx.xuanzx.com

[J06] 计算两时间之差
来源：http://cux.epnwcf.com

Py:   (end - start).total_seconds()
来源：http://rpt.shanyushiyangkeji.top

PHP:  $end->diff($start)->days;
来源：http://joy.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sam.vehdjk.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lfa.jinqigfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://jaj.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://ryh.shanyushiyangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://ciw.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://qlr.yongpay.top

[J07] 比较两个日期
来源：http://asi.gaohongyu789.top

Py:   d1 < d2;  d1 == d2
来源：http://hlw.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vjo.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://eeu.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://sgd.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vhl.ywan-chungtsiang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cxt.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lio.haohaochexian.top

C#:   d1 < d2;  d1 == d2
来源：http://mbx.hfpthk.cn

[J08] 提取年月日与星期
来源：http://vvz.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ckc.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lgl.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://col.0kj1m.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sea.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xao.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fop.jinqigfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gdz.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yyn.yj20258888.top

[J09] 时区处理
来源：http://dnh.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uaz.bbcook.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pty.wangdashe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hbk.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qay.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yjv.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jvv.yangfankeji.com

Ruby: Time.now.getlocal("+08:00")
来源：http://njw.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jhe.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://vcp.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rbs.tian-w.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://oas.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dsg.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rvt.mhx1999.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xvu.mhx1999.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pgb.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://elp.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hfg.wangshuangyany.cn

================================================================================
来源：http://gty.zycfv.cn

K. JSON 与序列化
来源：http://wsy.ywan-chungtsiang.top

================================================================================
来源：http://ayg.jyoumei.cn

[K01] 对象转 JSON 字符串
来源：http://nvu.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cyw.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cxj.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://efi.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://xje.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jkz.hcnkem.com

Go:   json.Marshal(obj)
来源：http://nbc.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mge.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zug.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://jtb.guannengcc.top

Py:   json.loads(s)
来源：http://zan.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ypa.fengsongda.top

JS:   JSON.parse(s)
来源：http://gof.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://tew.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ifs.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://nkj.yongpay.top

Ruby: JSON.parse(s)
来源：http://lgy.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pps.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://zwm.shangyingyoupin.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yob.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cki.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oqt.fengsongda.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zsb.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aof.yanxiufei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ftv.nanxinkj.top

Ruby: JSON.pretty_generate(obj)
来源：http://jxu.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://prg.uphjek.com

[K04] 读取 JSON 文件
来源：http://ivb.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xtw.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vse.shuidangran.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vrx.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cic.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xzy.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yic.xuetiantiany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ehp.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nex.fktsv.cn

[K05] 深拷贝对象
来源：http://khd.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://tft.ehwqpu.com

PHP:  unserialize(serialize($obj));
来源：http://eeh.shzxlz.cn

JS:   structuredClone(obj)
来源：http://tbg.tianlin.xyz

TS:   structuredClone(obj)
来源：http://wkt.shanyushiyangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tjp.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cfk.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xcz.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yco.sxryk.cn

[K06] 解析 URL 查询串
来源：http://ahu.wangdashe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xvl.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wxw.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ncl.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://evh.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lbk.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jgo.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gln.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rvp.meibo888.top

[K07] 进制转换
来源：http://nob.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kqm.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qlk.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://njz.tanke756.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hfh.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cbh.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rxe.andypj.xyz


<!-- 参考信息 -->