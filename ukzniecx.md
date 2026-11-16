代发 wailian999

TS:   throw new Error("错误信息");
来源：http://uxy.yuanzhike.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ylw.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vpl.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://aad.bbcook.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bqo.yfazqb.com

[H04] 自定义异常类型
来源：http://xyc.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://tsf.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://vcn.aibaodan.cn

JS:   class MyError extends Error {}
来源：http://ikb.sjlbkw.cn

TS:   class MyError extends Error {}
来源：http://oxk.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://qgv.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gcw.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://zaj.cashguo.top

C#:   class MyException : Exception {}
来源：http://jcu.fktsv.cn

[H05] 捕获特定类型
来源：http://odh.yuxming.cn

Py:   except ValueError as e:
来源：http://qqe.yvedp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ynz.ydjk.org.cn

JS:   if (e instanceof TypeError) {}
来源：http://ygq.guowangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://twn.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://oms.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wfh.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://lrc.yfazqb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wrl.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://xeb.sysykeji.top

Py:   value = d.get("k") or default
来源：http://vks.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mma.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://sjx.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://qdq.feifeiyinyue.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xqp.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vql.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://ghn.fktsv.cn

C#:   obj?.A?.B ?? default
来源：http://yyt.fengsongda.top

[H07] 断言
来源：http://epk.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://epl.dashuyun.cn

PHP:  assert($x > 0);
来源：http://ofv.nanxuanxn.top

JS:   console.assert(x > 0);
来源：http://tuw.haohaochexian.top

TS:   console.assert(x > 0);
来源：http://wme.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://wlx.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vmb.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zdm.sjlbkw.cn

C#:   Debug.Assert(x > 0);
来源：http://mjt.guowangkeji.top

[H08] 获取错误信息与堆栈
来源：http://eka.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://myj.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uhb.fzhhl.top

JS:   e.message;  e.stack
来源：http://qwh.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dmw.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://auc.ydzc1.top

Go:   err.Error()
来源：http://tjl.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://jfx.tianlin.xyz

C#:   e.Message;  e.StackTrace
来源：http://pie.jinqigfzy.top

[H09] 带错误码的异常
来源：http://fqv.zycfv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xxi.hysaishi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fnh.yj20258.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wzd.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://otn.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xab.sxryk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xkt.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://vwx.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wgc.yj20258888.top

[H10] 资源自动释放
来源：http://zcj.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://isb.xylfe.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jen.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uyi.ehwqpu.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tel.gogol.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wng.zhiwuduotai.top

Go:   defer f.Close()
来源：http://egm.shangyingyoupin.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kpx.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kbu.shanyushiyangkeji.top

================================================================================
来源：http://apx.xziqi.cn

I. 正则表达式
来源：http://lvd.sufxvd.cn

================================================================================
来源：http://zkq.hongshengwenyu.top

[I01] 判断是否匹配
来源：http://vas.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eyi.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://rqg.zhixingplan.top

JS:   /\d+/.test(s)
来源：http://kme.kuanghao11.cn

TS:   /\d+/.test(s)
来源：http://cle.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xqu.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dmw.hfpthk.cn

Ruby: s.match?(/\d+/)
来源：http://ivx.sysykeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://prz.yj20258888.top

[I02] 提取所有匹配
来源：http://kgo.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://faf.zhoulong.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bec.chenlongwang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iro.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://ren.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://axy.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dhs.hcnkem.com

Ruby: s.scan(/\d+/)
来源：http://lle.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nzk.zhoulong.xyz

[I03] 提取捕获分组
来源：http://nmp.chenlongwang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://juy.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qvx.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hks.chenlongwang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qqd.xziqi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qqb.sxryk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://suo.zdqjudy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ceg.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tml.zhixingplan.top

[I04] 正则替换
来源：http://ael.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://khh.xinyue.icu

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://huj.gogol.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tzz.daria6918.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hgn.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://xtt.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://aub.yj20258.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uba.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pwi.feifeiyinyue.top

[I05] 按正则拆分
来源：http://ziq.fanxiaobao.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://byc.shuidangran.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fsi.havefunace.top

JS:   s.split(/\s*,\s*/)
来源：http://sjf.316326.xyz

TS:   s.split(/\s*,\s*/)
来源：http://efg.hnqzz.top

Java: s.split("\\s*,\\s*")
来源：http://mro.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tzg.wangshuangyany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xrw.hcnkem.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sia.snrcjt.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mgb.yj20258.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nvp.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lkg.yj20258.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gqb.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wnn.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tgy.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ffk.guannengcc.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qlp.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dfs.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://whb.quarkkingdee.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tlt.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://shi.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://azp.zhongyouzk.top

TS:   /error/gim
来源：http://hyc.sysykeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mba.epnwcf.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mwd.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://jcm.zhiwuduotai.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://frk.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://svb.ehwqpu.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eey.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xxi.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://csc.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wdr.hesvh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zzi.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lbo.wangdashe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qmn.tian-w.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dvx.sweek.top

================================================================================
来源：http://dqj.ywan-chungtsiang.top

J. 日期与时间
来源：http://rvw.gotoacloud.top

================================================================================
来源：http://vpb.0kj1m.cn

[J01] 获取当前时间
来源：http://rgz.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://noa.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tfw.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://kyt.yj20258.top

TS:   new Date();  Date.now()
来源：http://pnn.yonumen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wjx.yvedp.cn

Go:   time.Now()
来源：http://xlm.feifeiyinyue.top

Ruby: Time.now
来源：http://doy.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://axp.nanxinkj.top

[J02] 格式化输出
来源：http://nnl.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hej.cqqwz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hqd.yj20258.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kwb.zhiwuduotai.top

TS:   d.toISOString()
来源：http://ppj.tian-w.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ddv.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oow.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ikv.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lnv.nwbrower.top

[J03] 字符串解析为日期
来源：http://ncn.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mws.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oor.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://evd.guannengcc.top

TS:   new Date("2024-01-02")
来源：http://yhs.tanke756.top

Java: LocalDate.parse("2024-01-02")
来源：http://mxm.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gmo.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://mll.yj20258888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mqb.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://arz.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fvm.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cqw.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dnn.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bxy.zdbjq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bdy.kuanghao11.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lky.tanke756.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nfp.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ynk.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://hao.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://lln.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jgl.quarkkingdee.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://owk.wangdashe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dvb.yvedp.cn

Java: LocalDate.now().plusDays(7)
来源：http://vwo.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tyr.nwbrower.top

Ruby: Time.now + 7 * 86400
来源：http://mtf.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://wom.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://hgm.quarkkingdee.top

Py:   (end - start).total_seconds()
来源：http://lnk.yj20258888.top

PHP:  $end->diff($start)->days;
来源：http://bsq.hammf.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oii.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tpt.shanyushiyangtech.top

Java: Duration.between(start, end).toSeconds()
来源：http://ign.52xcode.cn

Go:   end.Sub(start).Hours()
来源：http://xvi.zycfv.cn

Ruby: end - start                 # 返回秒数
来源：http://hra.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://epv.fktsv.cn

[J07] 比较两个日期
来源：http://myn.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://tlt.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dss.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yth.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://axt.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://six.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kyn.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jdn.jinqigfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://cty.xuanzx.com

[J08] 提取年月日与星期
来源：http://cwd.zhaomingkeji.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ufq.hysaishi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://smq.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dcf.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wia.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mms.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bie.ydzc1.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xup.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fkw.quarkkingdee.top

[J09] 时区处理
来源：http://oxn.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ial.fktsv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://foc.jinyuanbaomall.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nuz.gaohongyu789.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lko.ppjwa.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fqw.jiagoushi.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xmw.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ici.cdnleiting.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mue.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://zsr.aibaodan.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zpw.zdbjq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dvx.dashuyun.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hsu.redwolf501.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://npb.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qrl.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lme.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xrz.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ijm.zdqjudy.top

================================================================================
来源：http://ytq.zdqjudy.top

K. JSON 与序列化
来源：http://vqb.haohaochexian.top

================================================================================
来源：http://pzb.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://dui.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tjc.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xyq.shangyingyoupin.top

JS:   JSON.stringify(obj)
来源：http://jwm.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://soh.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iru.cucudq.cn

Go:   json.Marshal(obj)
来源：http://wio.yj202588.top

Ruby: obj.to_json                                     // require "json"
来源：http://rul.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ycu.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://kfk.zhongyouzk.top

Py:   json.loads(s)
来源：http://ivv.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gbg.316326.xyz

JS:   JSON.parse(s)
来源：http://gmo.yvedp.cn

TS:   JSON.parse(s)
来源：http://ijp.ydjk.org.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hcr.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://for.ivvv.top

Ruby: JSON.parse(s)
来源：http://jkh.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dxw.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://fst.chenlongwang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lrw.sysykeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oqb.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://wfy.hysaishi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kce.shanyushiyangtech.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nzn.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aeb.shangyingyoupin.top

Ruby: JSON.pretty_generate(obj)
来源：http://fmy.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://csx.haohaochexian.top

[K04] 读取 JSON 文件
来源：http://whe.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aok.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bxr.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gwr.hysaishi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aws.hongshengwenyu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ioa.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pgk.haohaochexian.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jzh.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ocq.ctjpmb.com

[K05] 深拷贝对象
来源：http://jon.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://xxe.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://tdt.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://jyr.haohaochexian.top

TS:   structuredClone(obj)
来源：http://knc.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bxm.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cai.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://doz.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://jax.redwolf501.top

[K06] 解析 URL 查询串
来源：http://wyw.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fqf.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pvu.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fnw.pycfn.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rgb.ehwqpu.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nnp.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://svk.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gcn.snrcjt.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nye.xziqi.cn

[K07] 进制转换
来源：http://nfa.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cst.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lox.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ies.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mod.hcnkem.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tzn.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ybz.sjlbkw.cn


<!-- 参考信息 -->