代发 wailian999

TS:   throw new Error("错误信息");
来源：http://lgd.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bnp.zhiwuduotai.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hza.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://brq.xinyue.icu

C#:   throw new ArgumentException("错误信息");
来源：http://bqf.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://css.zhengqikj.top

Py:   class MyError(Exception): pass
来源：http://ktv.jianghu66.top

PHP:  class MyError extends RuntimeException {}
来源：http://xso.uphjek.com

JS:   class MyError extends Error {}
来源：http://mje.havefunace.top

TS:   class MyError extends Error {}
来源：http://ksa.shanyushiyangtech.top

Java: class MyException extends RuntimeException {}
来源：http://owp.fktsv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yfj.tian-w.cn

Ruby: class MyError < StandardError; end
来源：http://duf.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://uke.yanxiufei.cn

[H05] 捕获特定类型
来源：http://wza.nanxinkj.top

Py:   except ValueError as e:
来源：http://jha.hcnkem.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pbz.hammf.cn

JS:   if (e instanceof TypeError) {}
来源：http://nbf.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://ozo.guowangkeji.top

Java: catch (IOException | SQLException e) {}
来源：http://fcb.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ezc.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://vqw.yvedp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://niw.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://vkd.ydjk.org.cn

Py:   value = d.get("k") or default
来源：http://dgf.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://qjm.andypj.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://iaa.gzhubu.top

TS:   obj?.a?.b;  d ?? default
来源：http://wle.c1oappe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://npz.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ffe.cucudq.cn

Ruby: d&.dig(:a, :b)
来源：http://vij.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://edw.xingfuxueyuan.xyz

[H07] 断言
来源：http://qhp.chenzaomai.com

Py:   assert x > 0, "必须为正"
来源：http://yqd.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://byv.nanxuanxn.top

JS:   console.assert(x > 0);
来源：http://xoq.yj20258888.top

TS:   console.assert(x > 0);
来源：http://vgm.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://wog.gotoacloud.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://brs.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wvt.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://iro.bbcook.cn

[H08] 获取错误信息与堆栈
来源：http://qah.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://kmu.ppjwa.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kbi.yfazqb.com

JS:   e.message;  e.stack
来源：http://xqd.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oqp.ppjwa.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yks.jinqigufen.top

Go:   err.Error()
来源：http://chh.hesvh.cn

Ruby: e.message;  e.backtrace
来源：http://jjm.jyoumei.cn

C#:   e.Message;  e.StackTrace
来源：http://mvy.haohaochexian.top

[H09] 带错误码的异常
来源：http://coh.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pge.zhiwuduotai.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qrp.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pcg.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jqw.cdnleiting.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mfr.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eym.mhx1999.top

Ruby: raise MyError.new("fail", 500)
来源：http://vve.ydjk.org.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uld.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://uky.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ewq.jinqigufen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://njv.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tyf.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vkm.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nti.cashguo.top

Go:   defer f.Close()
来源：http://aat.wangdashe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ubg.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mvx.yuanzhike.top

================================================================================
来源：http://bai.ydzc1.top

I. 正则表达式
来源：http://puo.feifeiyinyue.top

================================================================================
来源：http://kdy.epnwcf.com

[I01] 判断是否匹配
来源：http://jjj.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://viz.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://jcy.52xcode.cn

JS:   /\d+/.test(s)
来源：http://jir.nwbrower.top

TS:   /\d+/.test(s)
来源：http://tjp.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jpe.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ayz.yonumen.top

Ruby: s.match?(/\d+/)
来源：http://rsh.ivvv.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eau.hywenlv.cn

[I02] 提取所有匹配
来源：http://dgg.cucudq.cn

Py:   re.findall(r"\d+", s)
来源：http://pho.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mfe.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vtx.aizwys.cn

TS:   s.match(/\d+/g)
来源：http://udk.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gjc.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cbk.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://ffm.ydzc1.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jfl.vehdjk.com

[I03] 提取捕获分组
来源：http://all.xylfe.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://syv.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pot.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://trv.sysykeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zxz.andypj.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ndv.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wpf.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uyi.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jyy.ywan-chungtsiang.top

[I04] 正则替换
来源：http://avg.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://iwt.zdbjq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kks.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://wes.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://ewg.iojbl.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gto.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xro.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zxg.hcnkem.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://igt.ydjk.org.cn

[I05] 按正则拆分
来源：http://ztw.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://lvy.yonumen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pgy.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://tkr.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://imv.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://gmg.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://guw.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://pmt.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qxp.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qnp.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vew.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zre.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://chf.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://abe.yvedp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yza.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://juk.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cbd.dianchejie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fkp.yueranfly.top

[I07] 忽略大小写与多行模式
来源：http://syt.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bbm.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gxo.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sso.c1oappe.top

TS:   /error/gim
来源：http://swb.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://poh.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rvg.tarul.cn

Ruby: s.scan(/error/i)
来源：http://aph.aizwys.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zrt.tian-w.cn

[I08] 贪婪与非贪婪匹配
来源：http://bsf.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nyo.yongpay.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rwb.zhixingplan.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://igl.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yfx.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hpv.yueranfly.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qdr.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nto.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pjr.shangyingyoupin.top

================================================================================
来源：http://lrn.jinqigufen.top

J. 日期与时间
来源：http://hnm.meibo888.top

================================================================================
来源：http://wft.hnxiangtu.top

[J01] 获取当前时间
来源：http://vmq.meibo888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://uzz.fzhhl.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://knp.ivvv.top

JS:   new Date();  Date.now()
来源：http://lgi.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://mny.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sqp.shanyushiyangkeji.top

Go:   time.Now()
来源：http://cxh.fanxiaobao.xyz

Ruby: Time.now
来源：http://eps.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hap.daxiang520.top

[J02] 格式化输出
来源：http://mmi.havefunace.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dro.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vno.ivvv.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kad.pengpengdd.cyou

TS:   d.toISOString()
来源：http://kec.chenjidiqi.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tqi.snrcjt.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rjp.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rmq.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uct.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://psd.yuxming.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xii.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xku.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://xvs.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://omz.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://ymr.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://afx.hfpthk.cn

Ruby: Date.parse("2024-01-02")
来源：http://xpn.hfpthk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lfc.haohaochexian.top

[J04] 时间戳与日期互转
来源：http://dze.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bqe.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wei.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jrx.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ebl.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dox.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mnd.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tfn.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mcs.yuxming.cn

[J05] 时间加减（加 7 天）
来源：http://brp.yj202588.top

Py:   now + timedelta(days=7)
来源：http://mzu.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cup.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nzv.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xhm.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://uif.hywenlv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nyk.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://pka.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cwp.iojbl.cn

[J06] 计算两时间之差
来源：http://buo.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://kfd.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://mzv.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nhh.fengsongda.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pwx.chenzaomai.com

Java: Duration.between(start, end).toSeconds()
来源：http://neo.hongshengwenyu.top

Go:   end.Sub(start).Hours()
来源：http://esr.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://fpq.bbcook.cn

C#:   (end - start).TotalSeconds
来源：http://ayr.zhoulong.xyz

[J07] 比较两个日期
来源：http://mhj.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://bno.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qvt.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://zxq.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pbc.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vao.sjlbkw.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eky.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://shr.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://ogi.ydjk.org.cn

[J08] 提取年月日与星期
来源：http://xlw.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dla.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zup.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://elt.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vid.yangfankeji.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eil.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gdd.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ulz.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zgn.cucudq.cn

[J09] 时区处理
来源：http://jqz.sxryk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mgo.mhx1999.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ukb.redwolf501.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mvl.jqgfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jvm.bjfxy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wlt.tanke756.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://okk.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xyu.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hvc.tanke756.top

[J10] 取今天 / 本月第一天
来源：http://tiq.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pvt.iojbl.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iyv.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gyn.zhongyouzk.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uaz.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://keu.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://emt.gaohongyu789.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dwn.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aat.ctjpmb.com

================================================================================
来源：http://ryi.guowangkeji.top

K. JSON 与序列化
来源：http://doi.yj20258888.top

================================================================================
来源：http://eqj.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://ojc.feifeiyinyue.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lpf.ctjpmb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fmq.birdmap.top

JS:   JSON.stringify(obj)
来源：http://wge.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://goa.sweek.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://osq.cashguo.top

Go:   json.Marshal(obj)
来源：http://kot.ivvv.top

Ruby: obj.to_json                                     // require "json"
来源：http://slj.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qio.pengpengdd.cyou

[K02] JSON 字符串转对象
来源：http://aru.hnqzz.top

Py:   json.loads(s)
来源：http://baz.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tua.0kj1m.cn

JS:   JSON.parse(s)
来源：http://nsv.ctjpmb.com

TS:   JSON.parse(s)
来源：http://gex.hongshengwenyu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://snf.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://zsu.meibo888.top

Ruby: JSON.parse(s)
来源：http://dnz.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mve.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://llm.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qlu.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qnp.tarul.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://voa.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://oqi.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tgu.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vsj.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://tqp.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dyo.yongpay.top

[K04] 读取 JSON 文件
来源：http://whl.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uvv.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ome.vehdjk.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ych.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hti.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cvj.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qzf.zhaomingkeji.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://nnx.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fen.birdmap.top

[K05] 深拷贝对象
来源：http://amb.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://hdd.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://uue.guowangkeji.top

JS:   structuredClone(obj)
来源：http://yaj.ctjpmb.com

TS:   structuredClone(obj)
来源：http://mfk.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gjt.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bbo.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ula.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://scr.cqqwz.cn

[K06] 解析 URL 查询串
来源：http://qno.ehwqpu.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gha.zhoulong.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://axq.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nfk.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sth.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sgt.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://phe.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rxs.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rqb.svipenyu.cn

[K07] 进制转换
来源：http://fly.jqgfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nlo.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cts.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qny.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ygs.epnwcf.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yuj.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zmp.hcnkem.com


<!-- 参考信息 -->