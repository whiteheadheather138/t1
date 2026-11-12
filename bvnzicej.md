代发 wailian999

TS:   throw new Error("错误信息");
来源：http://psf.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tms.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uxh.epnwcf.com

Ruby: raise ArgumentError, "错误信息"
来源：http://jaq.cashguo.top

C#:   throw new ArgumentException("错误信息");
来源：http://dbz.316326.xyz

[H04] 自定义异常类型
来源：http://xhc.daria6918.cn

Py:   class MyError(Exception): pass
来源：http://awp.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://ujp.cheryme.top

JS:   class MyError extends Error {}
来源：http://cgt.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://hqx.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://rrk.cheryme.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cxg.yj20258888.top

Ruby: class MyError < StandardError; end
来源：http://xqw.xziqi.cn

C#:   class MyException : Exception {}
来源：http://yld.havefunace.top

[H05] 捕获特定类型
来源：http://zdn.hongshengwenyu.top

Py:   except ValueError as e:
来源：http://pid.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://taj.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://tbg.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://aes.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://gox.haohaochexian.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kwc.tianlin.xyz

Ruby: rescue ArgumentError => e
来源：http://neg.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ixb.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://dtg.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://pxh.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://cox.ydjk.org.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ixr.fzhhl.top

TS:   obj?.a?.b;  d ?? default
来源：http://tzx.jyoumei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ssb.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://oec.dianchejie.cn

Ruby: d&.dig(:a, :b)
来源：http://jmj.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://rcc.gzhubu.top

[H07] 断言
来源：http://yyb.yonumen.top

Py:   assert x > 0, "必须为正"
来源：http://dtg.sysykeji.top

PHP:  assert($x > 0);
来源：http://gff.bjfxy.top

JS:   console.assert(x > 0);
来源：http://icc.yueranfly.top

TS:   console.assert(x > 0);
来源：http://yxz.ehwqpu.com

Java: assert x > 0 : "必须为正";
来源：http://hkk.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baw.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kss.316326.xyz

C#:   Debug.Assert(x > 0);
来源：http://hbu.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://qic.cdnleiting.top

Py:   str(e);  traceback.format_exc()
来源：http://znr.birdmap.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jbu.hysaishi.cn

JS:   e.message;  e.stack
来源：http://rwd.ydjk.org.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eys.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xjj.ehwqpu.com

Go:   err.Error()
来源：http://sjb.guowangkeji.top

Ruby: e.message;  e.backtrace
来源：http://usn.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://gdt.yanxiufei.cn

[H09] 带错误码的异常
来源：http://fly.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cbe.cheryme.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ysd.cucudq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iug.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bkr.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://loe.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tlg.gzhubu.top

Ruby: raise MyError.new("fail", 500)
来源：http://spa.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qbs.shzxlz.cn

[H10] 资源自动释放
来源：http://qpu.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zwb.feifeiyinyue.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rbj.zdqjudy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ivz.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oct.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zvd.bjfxy.top

Go:   defer f.Close()
来源：http://xqd.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jsc.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eiy.zhiwuduotai.top

================================================================================
来源：http://khf.jianghu66.top

I. 正则表达式
来源：http://ffg.iojbl.cn

================================================================================
来源：http://cqy.havefunace.top

[I01] 判断是否匹配
来源：http://emk.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jcg.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oyf.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://ryw.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://ghh.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://err.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xby.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://cqw.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kdr.hongshengwenyu.top

[I02] 提取所有匹配
来源：http://bnv.smart0.xyz

Py:   re.findall(r"\d+", s)
来源：http://gxg.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nbp.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hae.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://yec.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nrp.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kdl.fengsongda.top

Ruby: s.scan(/\d+/)
来源：http://diy.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aun.shanyushiyangtech.top

[I03] 提取捕获分组
来源：http://usa.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yqv.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://enk.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gia.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uuw.hammf.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xyr.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fba.svipenyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://amb.xingfuxueyuan.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zbq.daxiang520.top

[I04] 正则替换
来源：http://zmw.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qmr.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tsx.vqdsnc.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bpt.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://mhp.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://dba.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cgo.yj20258.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ylw.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kru.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://ghv.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ejj.shanyushiyangtech.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fsu.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://hhy.havefunace.top

TS:   s.split(/\s*,\s*/)
来源：http://zen.cashguo.top

Java: s.split("\\s*,\\s*")
来源：http://vzm.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kag.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://tdh.tian-w.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ccr.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sxn.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gns.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hsc.cashguo.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://esd.cashguo.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xuz.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://scf.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jdt.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kip.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rgb.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://dne.jiagoushi.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gia.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qin.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oim.zhengqikj.top

TS:   /error/gim
来源：http://epp.jyoumei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fjk.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ovg.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://pup.haohaochexian.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bgp.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://zjs.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ifa.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xno.bjfxy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tvc.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dbe.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://abw.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qag.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wfl.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fri.meibo888.top

================================================================================
来源：http://dsn.jinqigfzy.top

J. 日期与时间
来源：http://omr.chenzaomai.com

================================================================================
来源：http://jbo.bjfxy.top

[J01] 获取当前时间
来源：http://lhu.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fjk.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zqk.c1oappe.top

JS:   new Date();  Date.now()
来源：http://myo.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://nfr.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zms.zhoulong.xyz

Go:   time.Now()
来源：http://emj.tarul.cn

Ruby: Time.now
来源：http://hxs.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mtf.316326.xyz

[J02] 格式化输出
来源：http://bqi.bjfxy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ekv.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hcz.aibaodan.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kjw.jiagoushi.top

TS:   d.toISOString()
来源：http://osn.gzhubu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lwo.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hsx.vqdsnc.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://znc.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://spt.zdqjudy.top

[J03] 字符串解析为日期
来源：http://cks.guowangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ish.zhoulong.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wfr.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://jny.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://mge.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wtk.nanxuanxn.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gik.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://cbq.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ixg.gotoacloud.top

[J04] 时间戳与日期互转
来源：http://nog.ctjpmb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://btq.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ybr.chenjidiqi.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ohw.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://szz.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xpb.birdmap.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iix.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://itu.pengpengdd.cyou

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vci.fengsongda.top

[J05] 时间加减（加 7 天）
来源：http://lkw.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://wzu.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://jgp.bjfxy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://van.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ask.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://qum.tanke756.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cnf.yj20258.top

Ruby: Time.now + 7 * 86400
来源：http://pac.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ywj.ppjwa.cn

[J06] 计算两时间之差
来源：http://iak.ppjwa.cn

Py:   (end - start).total_seconds()
来源：http://dvo.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://eys.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gnx.kuanghao11.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jic.meibo888.top

Java: Duration.between(start, end).toSeconds()
来源：http://vvr.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://wwd.ivvv.top

Ruby: end - start                 # 返回秒数
来源：http://ffs.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://twq.jinyuanbaomall.cn

[J07] 比较两个日期
来源：http://dsy.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://qje.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kty.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://zlw.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://mzf.nanxuanxn.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pgg.daxiang520.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://alo.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://sod.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ijh.yj202588.top

[J08] 提取年月日与星期
来源：http://nyd.zhaomingkeji.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://snu.xuanzx.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uoz.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ayl.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bxp.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ulc.dashuyun.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://grr.cdnleiting.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iqq.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qmd.guannengcc.top

[J09] 时区处理
来源：http://ayu.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jih.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nsz.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nvs.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ohx.xziqi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nvc.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ean.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pru.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xeq.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://tpb.yj202588.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dup.zycfv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fha.zhongyouzk.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zlt.vqdsnc.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pli.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kgn.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ysz.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wtj.andypj.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fmh.cucudq.cn

================================================================================
来源：http://wvw.yfazqb.com

K. JSON 与序列化
来源：http://lfb.chenzaomai.com

================================================================================
来源：http://hgz.uphjek.com

[K01] 对象转 JSON 字符串
来源：http://eon.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ubn.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uyu.uphjek.com

JS:   JSON.stringify(obj)
来源：http://mux.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://ivh.jqgfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://grv.xingfuxueyuan.xyz

Go:   json.Marshal(obj)
来源：http://epd.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://vkp.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vqf.hcnkem.com

[K02] JSON 字符串转对象
来源：http://lms.xylfe.cn

Py:   json.loads(s)
来源：http://jln.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yvl.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://rvh.daxiang520.top

TS:   JSON.parse(s)
来源：http://uud.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gxe.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://gku.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://tyj.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jfc.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://str.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cgp.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ddz.zdqjudy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uuu.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qbw.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hzd.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://luk.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lms.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tli.xuanzx.com

[K04] 读取 JSON 文件
来源：http://slz.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://otb.yj20258.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hor.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mza.yueranfly.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dvx.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://soq.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zvv.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gew.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hzo.ydjk.org.cn

[K05] 深拷贝对象
来源：http://zzh.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://zyz.andypj.xyz

PHP:  unserialize(serialize($obj));
来源：http://ank.tanke756.top

JS:   structuredClone(obj)
来源：http://rmi.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://whw.0kj1m.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dan.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ygt.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wyq.xinyue.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://hhj.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://vjg.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ces.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oja.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ted.nwbrower.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blq.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zmf.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://otg.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fin.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fmr.epnwcf.com

[K07] 进制转换
来源：http://eze.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qib.daria6918.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dxk.ybcxt.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xvs.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kie.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xjx.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wsj.xinyue.icu


<!-- 参考信息 -->