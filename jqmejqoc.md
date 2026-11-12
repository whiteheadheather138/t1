代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://gwp.fktsv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mio.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jxh.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mvk.tian-w.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qmi.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://eza.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uih.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wca.shuidangran.top

[H03] 主动抛出异常
来源：http://yqx.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://tpd.havefunace.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qmm.0kj1m.cn

JS:   throw new Error("错误信息");
来源：http://jqb.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://vmv.xziqi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xcv.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kei.ehwqpu.com

Ruby: raise ArgumentError, "错误信息"
来源：http://bye.wangdashe.top

C#:   throw new ArgumentException("错误信息");
来源：http://fib.jinqigufen.top

[H04] 自定义异常类型
来源：http://wxb.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://rtl.fehbvm.com

PHP:  class MyError extends RuntimeException {}
来源：http://ibg.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://ebr.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://xqe.tanke756.top

Java: class MyException extends RuntimeException {}
来源：http://uze.fehbvm.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://whi.zdbjq.cn

Ruby: class MyError < StandardError; end
来源：http://kln.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://chp.meibo888.top

[H05] 捕获特定类型
来源：http://uwv.yuxming.cn

Py:   except ValueError as e:
来源：http://wod.cashguo.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bav.wangshuangyany.cn

JS:   if (e instanceof TypeError) {}
来源：http://zvx.fktsv.cn

TS:   if (e instanceof TypeError) {}
来源：http://zcm.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://zre.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iug.sweek.top

Ruby: rescue ArgumentError => e
来源：http://lca.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rnw.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://zrs.shzxlz.cn

Py:   value = d.get("k") or default
来源：http://jnb.cashguo.top

PHP:  $v = $d["k"] ?? null;
来源：http://zpg.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://qgm.cqqwz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://krp.mhx1999.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zqz.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hgc.hywenlv.cn

Ruby: d&.dig(:a, :b)
来源：http://xsl.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://gny.nanxuanxn.top

[H07] 断言
来源：http://dao.fanxiaobao.xyz

Py:   assert x > 0, "必须为正"
来源：http://cqg.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://hov.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://fhr.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://slt.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://ccb.jinghuilouyu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rlr.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://tup.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://kfi.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://zrw.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://rfn.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qva.aibaodan.cn

JS:   e.message;  e.stack
来源：http://svi.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fco.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://isc.sufxvd.cn

Go:   err.Error()
来源：http://fmm.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://shm.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://dst.shanyushiyangkeji.top

[H09] 带错误码的异常
来源：http://dtz.birdmap.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://med.vqdsnc.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uwb.zhaomingkeji.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hzm.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://udk.gogol.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wtp.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://env.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://xad.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://etz.tanke756.top

[H10] 资源自动释放
来源：http://oiq.zycfv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vuw.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mtb.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ebd.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rio.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vxb.zhijiandao.cn

Go:   defer f.Close()
来源：http://yir.quarkkingdee.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rgm.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fqr.feifeiyinyue.top

================================================================================
来源：http://drx.xylfe.cn

I. 正则表达式
来源：http://vpt.kuanghao11.cn

================================================================================
来源：http://ict.hammf.cn

[I01] 判断是否匹配
来源：http://ayj.sjlbkw.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://luq.zhongyouzk.top

PHP:  preg_match('/\d+/', $s);
来源：http://ixj.jianghu66.top

JS:   /\d+/.test(s)
来源：http://gkp.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://ywu.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qpd.sweek.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fzk.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://axx.bjfxy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mdl.tarul.cn

[I02] 提取所有匹配
来源：http://ufq.jinyuanbaomall.cn

Py:   re.findall(r"\d+", s)
来源：http://wlp.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://stw.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vwd.ctjpmb.com

TS:   s.match(/\d+/g)
来源：http://ghd.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jdu.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yay.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://crd.pycfn.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://trk.fehbvm.com

[I03] 提取捕获分组
来源：http://dtg.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oao.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dal.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ewu.gogol.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lmz.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gir.shzxlz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hka.sjlbkw.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wgf.jyoumei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gli.dianchejie.cn

[I04] 正则替换
来源：http://mpa.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hnj.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ait.chenzaomai.com

JS:   s.replace(/\d+/g, "#")
来源：http://urw.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hcb.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://jzt.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zyn.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://gid.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jih.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://ope.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gwv.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vak.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://myk.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://rul.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://agu.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fvi.aizwys.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ohx.yj202588.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kmf.fktsv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cky.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cbm.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ubg.mhx1999.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zbq.mhx1999.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nhu.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qis.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fmq.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vlj.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gnn.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://kmn.jyoumei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jod.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rrj.ydzc1.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bga.jiagoushi.top

TS:   /error/gim
来源：http://tqg.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://loy.tian-w.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://byw.zhoulong.xyz

Ruby: s.scan(/error/i)
来源：http://kds.fanxiaobao.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lbr.jinqigfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://rnj.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://row.vqdsnc.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wzj.hnxiangtu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yih.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ctp.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gde.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mhr.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bzp.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://isw.zhiwuduotai.top

================================================================================
来源：http://qwu.chenzaomai.com

J. 日期与时间
来源：http://cwu.aibaodan.cn

================================================================================
来源：http://tsr.zhoulong.xyz

[J01] 获取当前时间
来源：http://gsu.0kj1m.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wxr.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wuj.aizwys.cn

JS:   new Date();  Date.now()
来源：http://tgg.hnqzz.top

TS:   new Date();  Date.now()
来源：http://dda.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qnj.iojbl.cn

Go:   time.Now()
来源：http://ydn.nanxuanxn.top

Ruby: Time.now
来源：http://muh.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gda.guowangkeji.top

[J02] 格式化输出
来源：http://tbq.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yqn.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://enl.epnwcf.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vue.jianghu66.top

TS:   d.toISOString()
来源：http://lib.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://opb.ppjwa.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rhh.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xrf.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bkl.sysykeji.top

[J03] 字符串解析为日期
来源：http://efd.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dtr.bjfxy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oyc.0kj1m.cn

JS:   new Date("2024-01-02")
来源：http://cgg.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://cip.svipenyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fyy.sysykeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uwm.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://oaw.hfpthk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jwf.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://edo.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://giu.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rzr.xingfuxueyuan.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pwp.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nal.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nsn.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bqz.ehwqpu.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://srw.zhoulong.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qrl.mhx1999.top

[J05] 时间加减（加 7 天）
来源：http://lox.pycfn.com

Py:   now + timedelta(days=7)
来源：http://zox.mhx1999.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yju.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://opt.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://acd.feifeiyinyue.top

Java: LocalDate.now().plusDays(7)
来源：http://ywv.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iqm.52xcode.cn

Ruby: Time.now + 7 * 86400
来源：http://aza.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://otx.feifeiyinyue.top

[J06] 计算两时间之差
来源：http://lnm.316326.xyz

Py:   (end - start).total_seconds()
来源：http://iwx.bbcook.cn

PHP:  $end->diff($start)->days;
来源：http://cqe.cqqwz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://msm.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lap.hfpthk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mvo.cdnleiting.top

Go:   end.Sub(start).Hours()
来源：http://djp.ivvv.top

Ruby: end - start                 # 返回秒数
来源：http://ygx.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://xxg.hfpthk.cn

[J07] 比较两个日期
来源：http://kzx.bbcook.cn

Py:   d1 < d2;  d1 == d2
来源：http://tyc.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eif.gotoacloud.top

JS:   d1.getTime() < d2.getTime()
来源：http://piv.nanxinkj.top

TS:   d1.getTime() < d2.getTime()
来源：http://ean.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://diz.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gms.andypj.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://dsy.jyoumei.cn

C#:   d1 < d2;  d1 == d2
来源：http://phb.snrcjt.cn

[J08] 提取年月日与星期
来源：http://pga.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jhp.hysaishi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mfi.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://riy.uphjek.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bzz.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://msr.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uqi.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lqk.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://foo.sweek.top

[J09] 时区处理
来源：http://fey.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://abf.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hsq.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ppz.hysaishi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cjq.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zzw.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cqv.shangyingyoupin.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hbo.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://edn.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://cso.ctjpmb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://fcq.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wda.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://juj.jyoumei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kbf.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nye.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kfy.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://syg.bbcook.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pao.fehbvm.com

================================================================================
来源：http://nth.shanyushiyangtech.top

K. JSON 与序列化
来源：http://cnv.ctjpmb.com

================================================================================
来源：http://cqz.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://dho.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rkv.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rtv.xingfuxueyuan.xyz

JS:   JSON.stringify(obj)
来源：http://emt.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://xyg.cucudq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bex.yonumen.top

Go:   json.Marshal(obj)
来源：http://ntm.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://atw.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://iad.316326.xyz

[K02] JSON 字符串转对象
来源：http://qeb.sjlbkw.cn

Py:   json.loads(s)
来源：http://fxn.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dfr.hysaishi.cn

JS:   JSON.parse(s)
来源：http://epk.andypj.xyz

TS:   JSON.parse(s)
来源：http://boo.yfazqb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ubt.mhx1999.top

Go:   json.Unmarshal(data, &v)
来源：http://nqv.ydzc1.top

Ruby: JSON.parse(s)
来源：http://ctn.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yft.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://yjw.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fso.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ttk.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://eke.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wjs.zhiwuduotai.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mlo.sxryk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sfh.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://ccw.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gfk.xuanzx.com

[K04] 读取 JSON 文件
来源：http://afv.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gca.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eei.zhaomingkeji.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xzq.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fgl.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aut.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://acu.fengsongda.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pry.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cvn.chenlongwang.top

[K05] 深拷贝对象
来源：http://ncy.tian-w.cn

Py:   copy.deepcopy(obj)
来源：http://kyv.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://lib.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://uqt.aizwys.cn

TS:   structuredClone(obj)
来源：http://phb.zdbjq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oww.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dzw.hesvh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fcf.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://van.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://pzo.gzhubu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aai.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gdc.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uqf.jqgfzy.top


<!-- 参考信息 -->