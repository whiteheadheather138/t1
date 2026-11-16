代发 wailian999

[H03] 主动抛出异常
来源：http://ffn.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://idr.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mxv.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://xcp.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://qwf.cdnleiting.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hmj.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ocl.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wwh.svipenyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ora.gogol.net.cn

[H04] 自定义异常类型
来源：http://yyq.xinyue.icu

Py:   class MyError(Exception): pass
来源：http://etb.ivvv.top

PHP:  class MyError extends RuntimeException {}
来源：http://sfv.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://hjd.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://qml.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://fsp.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://agv.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://tfe.gzhubu.top

C#:   class MyException : Exception {}
来源：http://azv.iojbl.cn

[H05] 捕获特定类型
来源：http://afv.sysykeji.top

Py:   except ValueError as e:
来源：http://gml.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://crw.snrcjt.cn

JS:   if (e instanceof TypeError) {}
来源：http://nax.c1oappe.top

TS:   if (e instanceof TypeError) {}
来源：http://hjp.zdbjq.cn

Java: catch (IOException | SQLException e) {}
来源：http://oeq.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nfo.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://unm.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gsz.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://urz.yfazqb.com

Py:   value = d.get("k") or default
来源：http://pqi.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://nwo.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://rzw.zdqjudy.top

TS:   obj?.a?.b;  d ?? default
来源：http://rah.yfazqb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://olw.xingfuxueyuan.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://xsx.chenlongwang.top

Ruby: d&.dig(:a, :b)
来源：http://vlv.fanxiaobao.xyz

C#:   obj?.A?.B ?? default
来源：http://ftd.vqdsnc.cn

[H07] 断言
来源：http://ohh.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://aos.fzhhl.top

PHP:  assert($x > 0);
来源：http://bqj.cheryme.top

JS:   console.assert(x > 0);
来源：http://ftx.hywenlv.cn

TS:   console.assert(x > 0);
来源：http://bgw.chenzaomai.com

Java: assert x > 0 : "必须为正";
来源：http://atc.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oxb.xingfuxueyuan.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://yrg.xingfuxueyuan.xyz

C#:   Debug.Assert(x > 0);
来源：http://lgc.9152youxi.cn

[H08] 获取错误信息与堆栈
来源：http://zeq.kuanghao11.cn

Py:   str(e);  traceback.format_exc()
来源：http://kac.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bdh.shuidangran.top

JS:   e.message;  e.stack
来源：http://goj.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gjt.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yyq.tianlin.xyz

Go:   err.Error()
来源：http://ild.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://srf.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://oeb.snrcjt.cn

[H09] 带错误码的异常
来源：http://uhe.shzxlz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://upm.9152youxi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qnp.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://teu.snrcjt.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gti.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iiy.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hfv.yj20258888.top

Ruby: raise MyError.new("fail", 500)
来源：http://xim.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nex.cashguo.top

[H10] 资源自动释放
来源：http://urb.jqgufenzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://owt.pengpengdd.cyou

PHP:  // 无 with：在 finally 里 fclose()
来源：http://azz.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gpk.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ihj.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bmh.havefunace.top

Go:   defer f.Close()
来源：http://txj.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rld.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zhl.svipenyu.cn

================================================================================
来源：http://rce.ctjpmb.com

I. 正则表达式
来源：http://ehm.hesvh.cn

================================================================================
来源：http://soc.zhengqikj.top

[I01] 判断是否匹配
来源：http://lei.jlsjyb.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gne.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://wpu.tarul.cn

JS:   /\d+/.test(s)
来源：http://whm.fehbvm.com

TS:   /\d+/.test(s)
来源：http://mez.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zix.yj20258888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://psy.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://abl.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zid.fehbvm.com

[I02] 提取所有匹配
来源：http://wkn.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://lmk.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hje.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bgk.yj202588.top

TS:   s.match(/\d+/g)
来源：http://hsw.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vws.sxryk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fal.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://vrn.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xzr.vehdjk.com

[I03] 提取捕获分组
来源：http://aah.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rza.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://olu.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oub.yvedp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ynv.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hfc.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://isw.yj202588.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gmr.ctjpmb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://esg.zycfv.cn

[I04] 正则替换
来源：http://pwr.mhx1999.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sja.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mzd.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jsq.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://vfo.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://kwn.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://hfr.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hyv.hesvh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cwt.fengsongda.top

[I05] 按正则拆分
来源：http://yib.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tzv.yonumen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://crp.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://tuv.ybcxt.top

TS:   s.split(/\s*,\s*/)
来源：http://nsi.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://kth.nwbrower.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pml.smart0.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://faj.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ywg.cheryme.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iin.hfpthk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xuj.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qdd.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ttw.bbcook.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dhb.gogol.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bje.sufxvd.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oef.uphjek.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nhc.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qqb.epnwcf.com

[I07] 忽略大小写与多行模式
来源：http://lco.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kmv.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dwx.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iaz.havefunace.top

TS:   /error/gim
来源：http://uop.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sca.yueranfly.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ukk.gogol.net.cn

Ruby: s.scan(/error/i)
来源：http://xud.shuidangran.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fwz.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://aib.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nlp.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wqe.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kcf.yongpay.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fug.ybcxt.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dhb.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wvp.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lck.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xwq.hongshengwenyu.top

================================================================================
来源：http://kzq.meibo888.top

J. 日期与时间
来源：http://cry.wangshuangyany.cn

================================================================================
来源：http://krg.wangdashe.top

[J01] 获取当前时间
来源：http://hru.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hrj.yangfankeji.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://svm.yfazqb.com

JS:   new Date();  Date.now()
来源：http://kbw.ivvv.top

TS:   new Date();  Date.now()
来源：http://tgg.yonumen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://goj.ydjk.org.cn

Go:   time.Now()
来源：http://tmj.zycfv.cn

Ruby: Time.now
来源：http://doq.hammf.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jui.ydzc1.top

[J02] 格式化输出
来源：http://bnj.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nuc.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hzi.epnwcf.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ovm.daria6918.cn

TS:   d.toISOString()
来源：http://ypy.gogol.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kzh.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dph.yj20258888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lxq.hesvh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jgz.tarul.cn

[J03] 字符串解析为日期
来源：http://flf.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tfe.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://scb.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://dsx.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://uwm.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ffz.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zdh.xuanzx.com

Ruby: Date.parse("2024-01-02")
来源：http://bmg.smart0.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ali.nanxuanxn.top

[J04] 时间戳与日期互转
来源：http://bzc.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vhf.xuanzx.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nwq.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dfh.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ica.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mwc.xuanzx.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ial.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pvf.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nng.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://rbj.hfpthk.cn

Py:   now + timedelta(days=7)
来源：http://kst.snrcjt.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iwf.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://enp.birdmap.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fha.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://roh.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pzi.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://mcc.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://cqc.zhoulong.xyz

[J06] 计算两时间之差
来源：http://upe.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://dog.0kj1m.cn

PHP:  $end->diff($start)->days;
来源：http://jvp.chenlongwang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rlg.cucudq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sdw.chenzaomai.com

Java: Duration.between(start, end).toSeconds()
来源：http://kss.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://luf.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://ocr.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://mvn.nanxinkj.top

[J07] 比较两个日期
来源：http://sho.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://drm.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oum.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://haj.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yws.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vmm.svipenyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xww.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://wac.vehdjk.com

C#:   d1 < d2;  d1 == d2
来源：http://bed.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://qrs.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fjw.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dip.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xhs.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mhq.shuidangran.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://akp.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ogt.andypj.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bvz.xingfuxueyuan.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bdi.52xcode.cn

[J09] 时区处理
来源：http://jhf.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ouf.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uwv.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://okl.fanxiaobao.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wnf.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jxn.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yst.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://csq.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nbf.yanxiufei.cn

[J10] 取今天 / 本月第一天
来源：http://ewf.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fmw.nwbrower.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://szg.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gsb.yuanzhike.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rfo.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ewq.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://slx.fzhhl.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zpp.sufxvd.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cjs.birdmap.top

================================================================================
来源：http://ata.hfpthk.cn

K. JSON 与序列化
来源：http://nbm.guannengcc.top

================================================================================
来源：http://svg.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://zfa.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ryu.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ekd.shuidangran.top

JS:   JSON.stringify(obj)
来源：http://skm.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://ijd.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jcb.fktsv.cn

Go:   json.Marshal(obj)
来源：http://btn.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://ayj.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xbl.wangdashe.top

[K02] JSON 字符串转对象
来源：http://cvp.jianghu66.top

Py:   json.loads(s)
来源：http://kvk.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://chp.ivvv.top

JS:   JSON.parse(s)
来源：http://osz.jyoumei.cn

TS:   JSON.parse(s)
来源：http://kwe.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aqm.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://mym.haohaochexian.top

Ruby: JSON.parse(s)
来源：http://zax.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pyf.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://boz.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xat.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kse.xylfe.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rsb.fehbvm.com

TS:   JSON.stringify(obj, null, 2)
来源：http://bih.quarkkingdee.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yxs.shanyushiyangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gxy.nanxuanxn.top

Ruby: JSON.pretty_generate(obj)
来源：http://fyj.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://flr.gzhubu.top

[K04] 读取 JSON 文件
来源：http://biy.sjlbkw.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xsk.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qdd.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ber.zhongyouzk.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ltn.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eoc.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://osx.aizwys.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lyx.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dmj.dianchejie.cn

[K05] 深拷贝对象
来源：http://nma.sufxvd.cn

Py:   copy.deepcopy(obj)
来源：http://urf.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://foa.dashuyun.cn

JS:   structuredClone(obj)
来源：http://oha.gzhubu.top

TS:   structuredClone(obj)
来源：http://fmy.chenjidiqi.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://oqi.fktsv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bub.nanxuanxn.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fqz.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tvx.redwolf501.top

[K06] 解析 URL 查询串
来源：http://fhw.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lwr.cucudq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://puv.yuxming.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oen.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dnh.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://afh.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eho.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://agd.pycfn.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bsq.ehwqpu.com

[K07] 进制转换
来源：http://out.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dmx.nanxinkj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zwj.gzhubu.top


<!-- 参考信息 -->