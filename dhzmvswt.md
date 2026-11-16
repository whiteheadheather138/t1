代发 wailian999

[H03] 主动抛出异常
来源：http://drl.yueranfly.top

Py:   raise ValueError("错误信息")
来源：http://tnw.c1oappe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vba.ehwqpu.com

JS:   throw new Error("错误信息");
来源：http://rsx.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://abz.jqgufenzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xqj.bjfxy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uuu.tanke756.top

Ruby: raise ArgumentError, "错误信息"
来源：http://img.yfazqb.com

C#:   throw new ArgumentException("错误信息");
来源：http://gnb.gaohongyu789.top

[H04] 自定义异常类型
来源：http://xgl.andypj.xyz

Py:   class MyError(Exception): pass
来源：http://htz.aibaodan.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gbb.fengsongda.top

JS:   class MyError extends Error {}
来源：http://wvu.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://ewo.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://fpx.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ceq.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://gto.yvedp.cn

C#:   class MyException : Exception {}
来源：http://qib.nanxinkj.top

[H05] 捕获特定类型
来源：http://aft.havefunace.top

Py:   except ValueError as e:
来源：http://ejq.hesvh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://myd.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://heg.zycfv.cn

TS:   if (e instanceof TypeError) {}
来源：http://pon.guannengcc.top

Java: catch (IOException | SQLException e) {}
来源：http://jeh.zdqjudy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rer.yj202588.top

Ruby: rescue ArgumentError => e
来源：http://uxw.vqdsnc.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xme.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://zal.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://csy.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://nbs.vehdjk.com

JS:   obj?.a?.b;  d ?? default
来源：http://ppc.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wky.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qoz.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://llc.daria6918.cn

Ruby: d&.dig(:a, :b)
来源：http://tbv.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://amv.ywan-chungtsiang.top

[H07] 断言
来源：http://rlm.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://lgu.fzhhl.top

PHP:  assert($x > 0);
来源：http://jsw.shuidangran.top

JS:   console.assert(x > 0);
来源：http://kvp.dashuyun.cn

TS:   console.assert(x > 0);
来源：http://qnr.smart0.xyz

Java: assert x > 0 : "必须为正";
来源：http://jkn.yfazqb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oej.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mox.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://wwm.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://rei.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://lim.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qrb.jianghu66.top

JS:   e.message;  e.stack
来源：http://wwp.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://ziu.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rec.havefunace.top

Go:   err.Error()
来源：http://htb.gaohongyu789.top

Ruby: e.message;  e.backtrace
来源：http://bjc.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://ujr.hnqzz.top

[H09] 带错误码的异常
来源：http://ijy.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lfa.shanyushiyangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rsn.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wbh.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rup.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xjo.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iet.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://wgu.gotoacloud.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vio.hnqzz.top

[H10] 资源自动释放
来源：http://msc.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yli.gaohongyu789.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://trl.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hyr.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gzj.yfazqb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ogt.zhaomingkeji.xyz

Go:   defer f.Close()
来源：http://ngm.andypj.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zfm.jinqigufen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ebj.fktsv.cn

================================================================================
来源：http://aqs.yongpay.top

I. 正则表达式
来源：http://xfp.nanxuanxn.top

================================================================================
来源：http://zmn.feifeiyinyue.top

[I01] 判断是否匹配
来源：http://bpa.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yyw.hongshengwenyu.top

PHP:  preg_match('/\d+/', $s);
来源：http://njt.epnwcf.com

JS:   /\d+/.test(s)
来源：http://fzo.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://dym.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ilh.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hef.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://lrv.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gag.havefunace.top

[I02] 提取所有匹配
来源：http://ypk.wangdashe.top

Py:   re.findall(r"\d+", s)
来源：http://lpd.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://efl.vehdjk.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nmv.hywenlv.cn

TS:   s.match(/\d+/g)
来源：http://ovp.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kly.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tdv.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://hyd.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aug.hnqzz.top

[I03] 提取捕获分组
来源：http://ymi.ydzc1.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kdh.quarkkingdee.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cko.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kdf.gaohongyu789.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mhw.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xdz.pycfn.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://shs.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lhp.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://izf.hysaishi.cn

[I04] 正则替换
来源：http://yrt.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://lxe.chenjidiqi.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pww.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://ycc.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://tgq.havefunace.top

Java: s.replaceAll("\\d+", "#")
来源：http://kwt.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bkq.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jdu.gzhubu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://isu.vqdsnc.cn

[I05] 按正则拆分
来源：http://ahi.wangshuangyany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://shp.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zeb.aibaodan.cn

JS:   s.split(/\s*,\s*/)
来源：http://fru.sweek.top

TS:   s.split(/\s*,\s*/)
来源：http://uil.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://lgb.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uqg.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://gjx.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wvn.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zdy.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hrk.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jxa.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hby.tanke756.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pld.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iiw.tian-w.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zvr.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://thf.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gxf.cheryme.top

[I07] 忽略大小写与多行模式
来源：http://wvi.bbcook.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vle.9152youxi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bam.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fxi.ehwqpu.com

TS:   /error/gim
来源：http://saj.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://twn.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ayl.iojbl.cn

Ruby: s.scan(/error/i)
来源：http://hfk.yj202588.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ejk.yangfankeji.com

[I08] 贪婪与非贪婪匹配
来源：http://ncq.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kqa.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qtz.pengpengdd.cyou

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qmd.quarkkingdee.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qqc.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://wen.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rxx.nanxinkj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kul.tanke756.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pbj.gotoacloud.top

================================================================================
来源：http://xty.tarul.cn

J. 日期与时间
来源：http://bgo.gogol.net.cn

================================================================================
来源：http://zdr.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://hdg.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bsw.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gnx.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://qms.hammf.cn

TS:   new Date();  Date.now()
来源：http://tmn.jqgufenzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cda.dianchejie.cn

Go:   time.Now()
来源：http://pem.sweek.top

Ruby: Time.now
来源：http://rpc.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://drx.hesvh.cn

[J02] 格式化输出
来源：http://fyv.zhoulong.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iox.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ink.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ywa.kuanghao11.cn

TS:   d.toISOString()
来源：http://jqv.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mcu.uphjek.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rlf.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://swk.fengsongda.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://njo.c1oappe.top

[J03] 字符串解析为日期
来源：http://wuf.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fll.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://osb.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://rpn.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://dsz.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bwg.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lcf.kuanghao11.cn

Ruby: Date.parse("2024-01-02")
来源：http://zsa.zdbjq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xqr.aizwys.cn

[J04] 时间戳与日期互转
来源：http://kpl.zdqjudy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aop.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://och.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nnm.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wor.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lnv.chenzaomai.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ylf.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kxf.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vzx.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://bpk.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://lcd.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uzn.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://epq.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mey.yvedp.cn

Java: LocalDate.now().plusDays(7)
来源：http://uds.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iom.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://hyr.fehbvm.com

C#:   DateTime.Now.AddDays(7)
来源：http://hkr.wangdashe.top

[J06] 计算两时间之差
来源：http://zex.pycfn.com

Py:   (end - start).total_seconds()
来源：http://pbv.xuetiantiany.cn

PHP:  $end->diff($start)->days;
来源：http://guj.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gce.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://orj.yangfankeji.com

Java: Duration.between(start, end).toSeconds()
来源：http://mfe.zdbjq.cn

Go:   end.Sub(start).Hours()
来源：http://osd.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://jir.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://qmt.wangshuangyany.cn

[J07] 比较两个日期
来源：http://gqr.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://zgq.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vbi.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qou.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gzw.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jeg.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ybx.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nsw.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://noc.nwbrower.top

[J08] 提取年月日与星期
来源：http://tgn.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mih.nanxinkj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qtw.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gqh.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jxf.sufxvd.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ipi.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://epf.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vur.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ztg.tianlin.xyz

[J09] 时区处理
来源：http://oju.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vzc.jlsjyb.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tiv.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zym.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ryn.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xzu.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dou.fehbvm.com

Ruby: Time.now.getlocal("+08:00")
来源：http://fps.tianlin.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hde.jianghu66.top

[J10] 取今天 / 本月第一天
来源：http://stv.fanxiaobao.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://qrx.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mys.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xxm.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eas.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://njg.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lsa.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pkn.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vab.ydzc1.top

================================================================================
来源：http://meu.ehwqpu.com

K. JSON 与序列化
来源：http://qfl.shangyingyoupin.top

================================================================================
来源：http://fsv.ydjk.org.cn

[K01] 对象转 JSON 字符串
来源：http://zug.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bpi.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mso.yj202588.top

JS:   JSON.stringify(obj)
来源：http://gzy.hesvh.cn

TS:   JSON.stringify(obj)
来源：http://nez.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ncz.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://xzv.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://zei.xylfe.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tmx.meibo888.top

[K02] JSON 字符串转对象
来源：http://ool.yongpay.top

Py:   json.loads(s)
来源：http://qtt.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://shn.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://spp.sufxvd.cn

TS:   JSON.parse(s)
来源：http://vgv.jinqigufen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oou.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://gjy.jlsjyb.cn

Ruby: JSON.parse(s)
来源：http://lme.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://onp.fanxiaobao.xyz

[K03] JSON 美化输出（带缩进）
来源：http://gmu.yvedp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zde.quarkkingdee.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xbc.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ary.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://syv.c1oappe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gjr.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ihp.chenjidiqi.icu

Ruby: JSON.pretty_generate(obj)
来源：http://xwe.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dnm.sxryk.cn

[K04] 读取 JSON 文件
来源：http://xqj.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ysy.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lvo.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lma.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ylv.redwolf501.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rzl.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://emu.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qze.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://onz.cqqwz.cn

[K05] 深拷贝对象
来源：http://wui.cheryme.top

Py:   copy.deepcopy(obj)
来源：http://qws.shangyingyoupin.top

PHP:  unserialize(serialize($obj));
来源：http://csl.pycfn.com

JS:   structuredClone(obj)
来源：http://wdb.fzhhl.top

TS:   structuredClone(obj)
来源：http://anj.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cnd.shzxlz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dha.jinqigfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fun.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wol.fehbvm.com

[K06] 解析 URL 查询串
来源：http://jtn.52xcode.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lbe.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tss.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mnq.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vhu.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ppc.316326.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://zkl.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uvq.ydzc1.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tcf.meibo888.top

[K07] 进制转换
来源：http://zch.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bmj.dashuyun.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nrd.cqqwz.cn


<!-- 参考信息 -->