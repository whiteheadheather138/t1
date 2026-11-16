代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://iau.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://idx.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qrt.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uoi.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://mal.zhijiandao.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xtg.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hfs.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hzl.shanyushiyangkeji.top

[H03] 主动抛出异常
来源：http://sjr.hywenlv.cn

Py:   raise ValueError("错误信息")
来源：http://ejs.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mqs.yj20258.top

JS:   throw new Error("错误信息");
来源：http://yhs.ivvv.top

TS:   throw new Error("错误信息");
来源：http://dtr.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fna.iojbl.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kvm.pengpengdd.cyou

Ruby: raise ArgumentError, "错误信息"
来源：http://zir.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://wcs.vehdjk.com

[H04] 自定义异常类型
来源：http://tcg.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://lbn.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ahh.ydzc1.top

JS:   class MyError extends Error {}
来源：http://jiu.sysykeji.top

TS:   class MyError extends Error {}
来源：http://tjx.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://xre.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zzq.hfpthk.cn

Ruby: class MyError < StandardError; end
来源：http://yjt.aizwys.cn

C#:   class MyException : Exception {}
来源：http://jde.pengpengdd.cyou

[H05] 捕获特定类型
来源：http://enz.kuanghao11.cn

Py:   except ValueError as e:
来源：http://eto.sjlbkw.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dnc.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://xfp.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://hlb.hongshengwenyu.top

Java: catch (IOException | SQLException e) {}
来源：http://zka.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rvk.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://azk.quarkkingdee.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oje.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://ryx.nwbrower.top

Py:   value = d.get("k") or default
来源：http://kmo.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://llt.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://ohv.yongpay.top

TS:   obj?.a?.b;  d ?? default
来源：http://xrw.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gyu.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ixq.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://nws.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://wft.ydzc1.top

[H07] 断言
来源：http://spv.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://hxt.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://aub.aizwys.cn

JS:   console.assert(x > 0);
来源：http://ibr.guannengcc.top

TS:   console.assert(x > 0);
来源：http://mlo.hnxiangtu.top

Java: assert x > 0 : "必须为正";
来源：http://sqp.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fkl.smart0.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://udj.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://yoy.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://vyn.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://abm.hammf.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fgf.nanxinkj.top

JS:   e.message;  e.stack
来源：http://ixn.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lus.52xcode.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bst.pycfn.com

Go:   err.Error()
来源：http://sig.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://fyx.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://qic.hywenlv.cn

[H09] 带错误码的异常
来源：http://mya.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xfc.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fer.snrcjt.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mfx.smart0.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://htn.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://esx.shzxlz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lwt.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://wqp.birdmap.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ckg.9152youxi.cn

[H10] 资源自动释放
来源：http://hdr.feifeiyinyue.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wha.ydjk.org.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gql.yfazqb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sba.sysykeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dns.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kap.9152youxi.cn

Go:   defer f.Close()
来源：http://mbj.wangdashe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jqn.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wbh.fehbvm.com

================================================================================
来源：http://tyg.ywan-chungtsiang.top

I. 正则表达式
来源：http://pna.cqqwz.cn

================================================================================
来源：http://fvw.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://hto.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kxf.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hoz.shangyingyoupin.top

JS:   /\d+/.test(s)
来源：http://btu.jinyuanbaomall.cn

TS:   /\d+/.test(s)
来源：http://zlw.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ujd.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kna.9152youxi.cn

Ruby: s.match?(/\d+/)
来源：http://skt.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oki.xuanzx.com

[I02] 提取所有匹配
来源：http://ljy.meibo888.top

Py:   re.findall(r"\d+", s)
来源：http://uxw.hnxiangtu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://twn.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jeg.pycfn.com

TS:   s.match(/\d+/g)
来源：http://dha.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lqn.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jzp.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://qga.fktsv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qvg.hesvh.cn

[I03] 提取捕获分组
来源：http://mvw.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hie.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vpj.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dmt.gzhubu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ztu.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bip.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zkh.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://erq.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jtj.yuanzhike.top

[I04] 正则替换
来源：http://umw.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vgl.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ihm.hammf.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dcz.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://fmq.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://ppb.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hwx.cashguo.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dnt.tian-w.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zco.hongshengwenyu.top

[I05] 按正则拆分
来源：http://hlx.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://drx.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vux.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://swv.daxiang520.top

TS:   s.split(/\s*,\s*/)
来源：http://azr.nanxinkj.top

Java: s.split("\\s*,\\s*")
来源：http://iwn.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kol.nanxuanxn.top

Ruby: s.split(/\s*,\s*/)
来源：http://vfd.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lxq.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://crt.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sye.wangdashe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vvo.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xdz.tian-w.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jeg.cdnleiting.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wen.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sje.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iky.sweek.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://owv.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://eaj.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gyc.shuidangran.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://krr.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hqm.jyoumei.cn

TS:   /error/gim
来源：http://npx.xziqi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aft.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gwk.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://hqk.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ean.tanke756.top

[I08] 贪婪与非贪婪匹配
来源：http://ffy.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mvf.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mua.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rhx.tian-w.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hug.cheryme.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nhv.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oqj.316326.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ugj.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wsa.nanxinkj.top

================================================================================
来源：http://ihf.nanxuanxn.top

J. 日期与时间
来源：http://nfe.jianghu66.top

================================================================================
来源：http://klq.xylfe.cn

[J01] 获取当前时间
来源：http://pwp.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gyc.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://svo.ydzc1.top

JS:   new Date();  Date.now()
来源：http://cnh.mhx1999.top

TS:   new Date();  Date.now()
来源：http://und.sufxvd.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nnl.gaohongyu789.top

Go:   time.Now()
来源：http://tvq.52xcode.cn

Ruby: Time.now
来源：http://ato.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dhq.zhiwuduotai.top

[J02] 格式化输出
来源：http://vyr.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aos.smart0.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bbu.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gvl.sjlbkw.cn

TS:   d.toISOString()
来源：http://kjw.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xed.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fea.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tvw.snrcjt.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ccz.c1oappe.top

[J03] 字符串解析为日期
来源：http://ktt.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://chc.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xfp.feifeiyinyue.top

JS:   new Date("2024-01-02")
来源：http://ovw.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://ijj.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hkv.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ama.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://skh.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rlr.yongpay.top

[J04] 时间戳与日期互转
来源：http://ewq.zycfv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://glw.hfpthk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yqz.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rqq.nanxinkj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ovo.yuxming.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://suy.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qzw.cashguo.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wnl.snrcjt.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qui.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://afi.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://ght.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wcs.redwolf501.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xlx.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qbe.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://aju.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jbm.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://egy.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://omn.havefunace.top

[J06] 计算两时间之差
来源：http://gpn.meibo888.top

Py:   (end - start).total_seconds()
来源：http://sqn.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://tlt.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xho.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://brn.hfpthk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wyx.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://kvx.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://qcp.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://hqa.0kj1m.cn

[J07] 比较两个日期
来源：http://qup.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://ama.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kcv.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://vdf.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bjt.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zee.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://amk.xylfe.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bwy.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://jbv.zhaomingkeji.xyz

[J08] 提取年月日与星期
来源：http://yql.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pwm.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hqm.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oam.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cfp.xylfe.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mab.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pnh.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lok.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jga.ywan-chungtsiang.top

[J09] 时区处理
来源：http://gxt.shuidangran.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nsv.sysykeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nhv.hammf.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kkn.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://juh.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gcl.zdqjudy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qms.gzhubu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://oat.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tms.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://cjt.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yyj.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://anr.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jwb.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wmf.cqqwz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://agu.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zwm.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ped.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mhu.chenjidiqi.icu

================================================================================
来源：http://nxh.yj20258888.top

K. JSON 与序列化
来源：http://oaz.shanyushiyangtech.top

================================================================================
来源：http://xee.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://bkq.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://urb.shzxlz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://deb.wangshuangyany.cn

JS:   JSON.stringify(obj)
来源：http://czc.xylfe.cn

TS:   JSON.stringify(obj)
来源：http://pwo.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://unl.meibo888.top

Go:   json.Marshal(obj)
来源：http://yri.316326.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://hgy.hysaishi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gre.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://ucw.bbcook.cn

Py:   json.loads(s)
来源：http://vwm.sxryk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uyl.zdqjudy.top

JS:   JSON.parse(s)
来源：http://wao.sxryk.cn

TS:   JSON.parse(s)
来源：http://mga.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hvx.quarkkingdee.top

Go:   json.Unmarshal(data, &v)
来源：http://ttx.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://rdh.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rkc.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://kev.shangyingyoupin.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gxv.sxryk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rgd.hnxiangtu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bih.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bmc.gotoacloud.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kef.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fre.yfazqb.com

Ruby: JSON.pretty_generate(obj)
来源：http://gqo.mhx1999.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xfo.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://ywb.dianchejie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pme.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ppo.9152youxi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cpk.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ssd.sufxvd.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vxy.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uov.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://dog.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ruh.haohaochexian.top

[K05] 深拷贝对象
来源：http://exu.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://hlf.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://ojt.nwbrower.top

JS:   structuredClone(obj)
来源：http://psa.daria6918.cn

TS:   structuredClone(obj)
来源：http://xvo.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hit.yuxming.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mww.cucudq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vzd.bjfxy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eeu.zycfv.cn

[K06] 解析 URL 查询串
来源：http://vor.smart0.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cas.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qqz.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tgl.quarkkingdee.top


<!-- 参考信息 -->