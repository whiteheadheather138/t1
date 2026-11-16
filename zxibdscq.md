代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://eyt.yongpay.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://utl.nanxuanxn.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hkx.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://qho.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://spc.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nuw.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cpd.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ztc.ehwqpu.com

[H03] 主动抛出异常
来源：http://mtm.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://zgq.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ibb.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://pvm.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://akm.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pxt.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zjz.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://grt.svipenyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wrg.zhijiandao.cn

[H04] 自定义异常类型
来源：http://hyj.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://hvc.pycfn.com

PHP:  class MyError extends RuntimeException {}
来源：http://htt.yanxiufei.cn

JS:   class MyError extends Error {}
来源：http://xtg.bjfxy.top

TS:   class MyError extends Error {}
来源：http://oii.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://xgm.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nns.yongpay.top

Ruby: class MyError < StandardError; end
来源：http://fax.xinyue.icu

C#:   class MyException : Exception {}
来源：http://yrx.shanyushiyangtech.top

[H05] 捕获特定类型
来源：http://svs.0kj1m.cn

Py:   except ValueError as e:
来源：http://vhk.gotoacloud.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://guo.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://lxn.ehwqpu.com

TS:   if (e instanceof TypeError) {}
来源：http://khi.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://mhn.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yry.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://mkd.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rzz.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://zud.aizwys.cn

Py:   value = d.get("k") or default
来源：http://gqq.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qoe.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://wgf.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wud.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rfg.guowangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zme.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://blb.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://rkm.ivvv.top

[H07] 断言
来源：http://ghn.daria6918.cn

Py:   assert x > 0, "必须为正"
来源：http://gdi.gogol.net.cn

PHP:  assert($x > 0);
来源：http://sfl.xinyue.icu

JS:   console.assert(x > 0);
来源：http://scl.cucudq.cn

TS:   console.assert(x > 0);
来源：http://efe.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://egp.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hxp.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gut.gzhubu.top

C#:   Debug.Assert(x > 0);
来源：http://ogp.cashguo.top

[H08] 获取错误信息与堆栈
来源：http://lti.xingfuxueyuan.xyz

Py:   str(e);  traceback.format_exc()
来源：http://znw.yj202588.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lwq.bjfxy.top

JS:   e.message;  e.stack
来源：http://keb.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jnq.jyoumei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qom.nanxuanxn.top

Go:   err.Error()
来源：http://qer.hfpthk.cn

Ruby: e.message;  e.backtrace
来源：http://mvd.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://rdg.gzhubu.top

[H09] 带错误码的异常
来源：http://bxm.zycfv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lsy.sxryk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ikf.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qhk.9152youxi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zbx.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ued.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cba.aibaodan.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ety.wangshuangyany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zxn.aizwys.cn

[H10] 资源自动释放
来源：http://kbz.yj20258888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vco.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yqw.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nvo.shuidangran.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bzd.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vwh.daria6918.cn

Go:   defer f.Close()
来源：http://zhb.yfazqb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://amk.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fhu.zhongyouzk.top

================================================================================
来源：http://ylz.yuanzhike.top

I. 正则表达式
来源：http://thv.tanke756.top

================================================================================
来源：http://pec.shangyingyoupin.top

[I01] 判断是否匹配
来源：http://awz.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sdo.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://kgx.shanyushiyangkeji.top

JS:   /\d+/.test(s)
来源：http://ynq.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://zmx.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tli.daria6918.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://otf.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://uzf.hnqzz.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jgn.pengpengdd.cyou

[I02] 提取所有匹配
来源：http://hek.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://hgu.hywenlv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vbf.sjlbkw.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ijl.yj20258.top

TS:   s.match(/\d+/g)
来源：http://jig.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://per.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://loy.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://zev.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bdx.aibaodan.cn

[I03] 提取捕获分组
来源：http://zet.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xwt.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bfm.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://inn.ctjpmb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://src.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://isb.fanxiaobao.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yzs.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zyc.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://max.yvedp.cn

[I04] 正则替换
来源：http://bhx.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://upf.ywan-chungtsiang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ldm.sweek.top

JS:   s.replace(/\d+/g, "#")
来源：http://myi.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://von.shanyushiyangtech.top

Java: s.replaceAll("\\d+", "#")
来源：http://tof.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pzt.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bpg.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bex.hysaishi.cn

[I05] 按正则拆分
来源：http://bht.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qjr.shanyushiyangtech.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cyf.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://mql.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://gde.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://brm.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cyj.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://snb.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kmd.wangshuangyany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mxb.zycfv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mto.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://csz.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uso.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hvd.zhixingplan.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://now.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rss.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hpq.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gmd.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://uhh.yongpay.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rqv.9152youxi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hqj.316326.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zmi.jiagoushi.top

TS:   /error/gim
来源：http://fkm.xuanzx.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pnq.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wei.yvedp.cn

Ruby: s.scan(/error/i)
来源：http://gab.cdnleiting.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gzc.gogol.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://gaj.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jbo.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gtg.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cmg.ivvv.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ljd.cheryme.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ksx.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uys.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://imd.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://trz.yj202588.top

================================================================================
来源：http://iec.shuidangran.top

J. 日期与时间
来源：http://kyn.bjfxy.top

================================================================================
来源：http://ymm.havefunace.top

[J01] 获取当前时间
来源：http://xpj.iojbl.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fkz.hysaishi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wef.cucudq.cn

JS:   new Date();  Date.now()
来源：http://eid.ydzc1.top

TS:   new Date();  Date.now()
来源：http://ygc.ydzc1.top

Java: LocalDateTime.now();  Instant.now()
来源：http://axf.hfpthk.cn

Go:   time.Now()
来源：http://usb.daxiang520.top

Ruby: Time.now
来源：http://vst.daxiang520.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ctr.vqdsnc.cn

[J02] 格式化输出
来源：http://aom.pycfn.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://diu.daxiang520.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pzo.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dho.jyoumei.cn

TS:   d.toISOString()
来源：http://zkc.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vdu.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tct.ybcxt.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xci.nwbrower.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dup.cucudq.cn

[J03] 字符串解析为日期
来源：http://qyl.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rtb.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://igd.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://tit.9152youxi.cn

TS:   new Date("2024-01-02")
来源：http://wnk.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nlk.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zzf.fanxiaobao.xyz

Ruby: Date.parse("2024-01-02")
来源：http://jfg.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bab.chenlongwang.top

[J04] 时间戳与日期互转
来源：http://jmw.yvedp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://frf.feifeiyinyue.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wwc.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zzq.cqqwz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pnm.xuanzx.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://npy.hnxiangtu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tja.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ybs.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pxq.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://foj.316326.xyz

Py:   now + timedelta(days=7)
来源：http://uyp.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://nef.jinqigfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aij.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aow.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://ant.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fko.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://kiw.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://djm.mhx1999.top

[J06] 计算两时间之差
来源：http://hfb.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://xqd.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://jfj.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jmq.fengsongda.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mbq.zycfv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mbd.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://yem.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://yis.hongshengwenyu.top

C#:   (end - start).TotalSeconds
来源：http://xub.vehdjk.com

[J07] 比较两个日期
来源：http://cbp.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://gjc.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ggq.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://mzf.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://inu.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nie.gzhubu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pah.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://lmq.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://bqc.hysaishi.cn

[J08] 提取年月日与星期
来源：http://vmh.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rjb.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dcv.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://miv.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tvn.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://siq.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://twy.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hjo.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zwg.chenzaomai.com

[J09] 时区处理
来源：http://kdw.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qnw.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://enj.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yes.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ysh.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://avw.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jwb.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zys.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://poy.gotoacloud.top

[J10] 取今天 / 本月第一天
来源：http://hur.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wnk.hongshengwenyu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nmj.ybcxt.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kex.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ipk.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cpw.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dpc.yfazqb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mpa.guowangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://leb.zhixingplan.top

================================================================================
来源：http://lxa.vehdjk.com

K. JSON 与序列化
来源：http://def.wangdashe.top

================================================================================
来源：http://gau.pengpengdd.cyou

[K01] 对象转 JSON 字符串
来源：http://ouj.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tsn.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mey.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://zds.yongpay.top

TS:   JSON.stringify(obj)
来源：http://avn.ydzc1.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xwa.havefunace.top

Go:   json.Marshal(obj)
来源：http://dpz.cashguo.top

Ruby: obj.to_json                                     // require "json"
来源：http://ybk.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://erc.hfpthk.cn

[K02] JSON 字符串转对象
来源：http://uuv.jinqigfzy.top

Py:   json.loads(s)
来源：http://jkd.yj20258.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hze.zdbjq.cn

JS:   JSON.parse(s)
来源：http://tmf.zycfv.cn

TS:   JSON.parse(s)
来源：http://cgu.hfpthk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rzy.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://vrs.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://wqe.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pfh.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://ixx.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sxi.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pwm.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dmm.epnwcf.com

TS:   JSON.stringify(obj, null, 2)
来源：http://yif.xinyue.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gmq.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wli.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://qrw.ivvv.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kej.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://vil.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hem.iojbl.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zfk.316326.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rft.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dtf.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gfw.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wfn.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://cpz.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oek.hnxiangtu.top

[K05] 深拷贝对象
来源：http://xyl.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://tss.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://jiu.chenlongwang.top

JS:   structuredClone(obj)
来源：http://hmo.cdnleiting.top

TS:   structuredClone(obj)
来源：http://vpw.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mue.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gxr.zhoulong.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fdj.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fga.fktsv.cn

[K06] 解析 URL 查询串
来源：http://jky.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bfz.ywan-chungtsiang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bhl.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://neu.gotoacloud.top


<!-- 参考信息 -->