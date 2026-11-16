代发 wailian999

TS:   throw new Error("错误信息");
来源：http://vxu.xuanzx.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://mtg.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vhs.yongpay.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vnu.tanke756.top

C#:   throw new ArgumentException("错误信息");
来源：http://zke.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://rwl.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://yna.nwbrower.top

PHP:  class MyError extends RuntimeException {}
来源：http://plp.hesvh.cn

JS:   class MyError extends Error {}
来源：http://fsf.bbcook.cn

TS:   class MyError extends Error {}
来源：http://caz.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://pge.bbcook.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://owi.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://liy.chenlongwang.top

C#:   class MyException : Exception {}
来源：http://jrq.feifeiyinyue.top

[H05] 捕获特定类型
来源：http://dhs.fehbvm.com

Py:   except ValueError as e:
来源：http://irl.mhx1999.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zzs.snrcjt.cn

JS:   if (e instanceof TypeError) {}
来源：http://jpc.ehwqpu.com

TS:   if (e instanceof TypeError) {}
来源：http://znp.tian-w.cn

Java: catch (IOException | SQLException e) {}
来源：http://tap.havefunace.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hvd.sweek.top

Ruby: rescue ArgumentError => e
来源：http://iab.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rfs.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://mcn.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://aae.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://xdj.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hcr.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://ahf.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hho.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://scc.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://yqn.gotoacloud.top

C#:   obj?.A?.B ?? default
来源：http://cuv.sysykeji.top

[H07] 断言
来源：http://rmd.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://hhh.hcnkem.com

PHP:  assert($x > 0);
来源：http://xab.wangshuangyany.cn

JS:   console.assert(x > 0);
来源：http://uxn.bjfxy.top

TS:   console.assert(x > 0);
来源：http://hih.0kj1m.cn

Java: assert x > 0 : "必须为正";
来源：http://grn.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cnv.birdmap.top

Ruby: raise "必须为正" unless x > 0
来源：http://lcd.fengsongda.top

C#:   Debug.Assert(x > 0);
来源：http://igd.yfazqb.com

[H08] 获取错误信息与堆栈
来源：http://qix.pycfn.com

Py:   str(e);  traceback.format_exc()
来源：http://cri.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cik.daria6918.cn

JS:   e.message;  e.stack
来源：http://ddb.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://pqk.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gai.yj202588.top

Go:   err.Error()
来源：http://mft.nwbrower.top

Ruby: e.message;  e.backtrace
来源：http://nxm.sxryk.cn

C#:   e.Message;  e.StackTrace
来源：http://ahq.zhoulong.xyz

[H09] 带错误码的异常
来源：http://egu.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pnl.jqgfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tcs.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sqr.epnwcf.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jdq.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lwv.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://apl.9152youxi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hmv.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://usd.cucudq.cn

[H10] 资源自动释放
来源：http://wvd.yuxming.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wco.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fna.fanxiaobao.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zdl.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://car.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nen.vqdsnc.cn

Go:   defer f.Close()
来源：http://eis.cashguo.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qki.jinyuanbaomall.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hkw.cqqwz.cn

================================================================================
来源：http://olf.xingfuxueyuan.xyz

I. 正则表达式
来源：http://mam.tian-w.cn

================================================================================
来源：http://obn.jianghu66.top

[I01] 判断是否匹配
来源：http://aks.fktsv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lmf.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://blg.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://atd.yuxming.cn

TS:   /\d+/.test(s)
来源：http://yjm.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://heo.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://shd.yonumen.top

Ruby: s.match?(/\d+/)
来源：http://xnk.tianlin.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nfw.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://xon.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://qpu.wangshuangyany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iyh.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nhj.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://dbx.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hhs.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://max.zhoulong.xyz

Ruby: s.scan(/\d+/)
来源：http://cxr.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lvg.birdmap.top

[I03] 提取捕获分组
来源：http://rai.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sxb.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fek.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vkt.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nmk.jiagoushi.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jwm.hongshengwenyu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://apz.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aij.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wyx.shanyushiyangtech.top

[I04] 正则替换
来源：http://otq.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ydp.52xcode.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tdk.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xtw.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://lkx.birdmap.top

Java: s.replaceAll("\\d+", "#")
来源：http://bjy.iojbl.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://goe.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://smg.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nit.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://qqh.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qlg.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dsz.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://nmv.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://xnp.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://jkw.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tjx.cqqwz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ypp.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ehs.hongshengwenyu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wgo.jinqigufen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hfp.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ort.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bew.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://emt.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cbs.yfazqb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vkv.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mij.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://isv.xylfe.cn

[I07] 忽略大小写与多行模式
来源：http://ghp.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nwo.cucudq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lti.xinyue.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pgf.dashuyun.cn

TS:   /error/gim
来源：http://hbv.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xqb.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qzk.hnqzz.top

Ruby: s.scan(/error/i)
来源：http://ikt.gogol.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rrl.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://sif.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mgz.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qjl.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://glh.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eai.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ydb.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://afx.ydjk.org.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rcp.nanxinkj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sws.wangshuangyany.cn

================================================================================
来源：http://ujx.wangshuangyany.cn

J. 日期与时间
来源：http://tgv.chenlongwang.top

================================================================================
来源：http://sqe.daria6918.cn

[J01] 获取当前时间
来源：http://qib.0kj1m.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nfm.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zvb.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://qlt.hcnkem.com

TS:   new Date();  Date.now()
来源：http://cbg.jlsjyb.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://now.jyoumei.cn

Go:   time.Now()
来源：http://jue.xinyue.icu

Ruby: Time.now
来源：http://msm.shanyushiyangtech.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hms.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://ipv.chenlongwang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mgk.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qdf.jyoumei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jwv.guannengcc.top

TS:   d.toISOString()
来源：http://xnv.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gkf.yj20258.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://izf.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dlf.chenzaomai.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qtx.hfpthk.cn

[J03] 字符串解析为日期
来源：http://pne.0kj1m.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tda.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gtg.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://mcw.ivvv.top

TS:   new Date("2024-01-02")
来源：http://aza.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://yyc.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bic.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://yhf.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yza.jianghu66.top

[J04] 时间戳与日期互转
来源：http://bio.xziqi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ior.chenzaomai.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://igd.52xcode.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bit.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zds.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://llx.zdqjudy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://saw.xinyue.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tqt.gaohongyu789.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jlg.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://cdm.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://dvs.jqgufenzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://oia.wangdashe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltr.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://klr.nwbrower.top

Java: LocalDate.now().plusDays(7)
来源：http://jxc.jiagoushi.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://btb.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://iyl.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://bxr.cucudq.cn

[J06] 计算两时间之差
来源：http://jkd.sufxvd.cn

Py:   (end - start).total_seconds()
来源：http://iqr.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://uys.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://guc.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lxv.shanyushiyangtech.top

Java: Duration.between(start, end).toSeconds()
来源：http://rgj.yongpay.top

Go:   end.Sub(start).Hours()
来源：http://wdh.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://ewh.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://dcl.epnwcf.com

[J07] 比较两个日期
来源：http://xep.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://vel.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nir.c1oappe.top

JS:   d1.getTime() < d2.getTime()
来源：http://qpy.vehdjk.com

TS:   d1.getTime() < d2.getTime()
来源：http://orb.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cat.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aif.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://jbn.jinqigufen.top

C#:   d1 < d2;  d1 == d2
来源：http://gzh.aibaodan.cn

[J08] 提取年月日与星期
来源：http://fas.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qlt.gogol.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pha.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hfn.sjlbkw.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rmt.ydjk.org.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mki.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mhj.yueranfly.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uds.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uql.yangfankeji.com

[J09] 时区处理
来源：http://mor.zhongyouzk.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://svs.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dmp.zhixingplan.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bbu.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bkr.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vqm.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eka.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ybj.daria6918.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mdk.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://vxm.yueranfly.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kpw.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wog.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jdi.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oac.0kj1m.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://edz.shanyushiyangtech.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wzm.meibo888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xzh.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://avr.ppjwa.cn

================================================================================
来源：http://ify.chenlongwang.top

K. JSON 与序列化
来源：http://zux.zhoulong.xyz

================================================================================
来源：http://idz.sweek.top

[K01] 对象转 JSON 字符串
来源：http://ecp.jyoumei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pck.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ujv.haohaochexian.top

JS:   JSON.stringify(obj)
来源：http://zkz.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://xnk.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bdd.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://vkp.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://rad.andypj.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://mpv.yj20258888.top

[K02] JSON 字符串转对象
来源：http://vcx.9152youxi.cn

Py:   json.loads(s)
来源：http://gpi.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aqx.xuetiantiany.cn

JS:   JSON.parse(s)
来源：http://san.tianlin.xyz

TS:   JSON.parse(s)
来源：http://tuk.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xar.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://lih.yvedp.cn

Ruby: JSON.parse(s)
来源：http://buz.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qju.haohaochexian.top

[K03] JSON 美化输出（带缩进）
来源：http://toi.nanxuanxn.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mct.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hpk.hammf.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ajj.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lfp.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lgs.c1oappe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lls.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://qzr.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cje.iojbl.cn

[K04] 读取 JSON 文件
来源：http://imd.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lpj.jinqigufen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://die.nwbrower.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lpi.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://whb.gotoacloud.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pzj.zdbjq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fau.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vly.jinyuanbaomall.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qps.guowangkeji.top

[K05] 深拷贝对象
来源：http://ywp.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://fjn.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://pdi.daxiang520.top

JS:   structuredClone(obj)
来源：http://fvj.9152youxi.cn

TS:   structuredClone(obj)
来源：http://sai.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://buz.tanke756.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oud.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vxn.hcnkem.com

C#:   // 序列化往返，或自定义 Clone
来源：http://bhg.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://ilz.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kcu.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mrl.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rhn.hysaishi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://akd.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fjt.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rcu.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bpn.hywenlv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zaa.zhaomingkeji.xyz

[K07] 进制转换
来源：http://dtr.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kup.jqgfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sze.yj20258.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qwo.xuetiantiany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zpj.yuanzhike.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zht.zhengqikj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://czp.yonumen.top


<!-- 参考信息 -->