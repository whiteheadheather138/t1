代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://vid.quarkkingdee.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wma.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://elt.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rky.daxiang520.top

Java: try { f(); } finally { cleanup(); }
来源：http://swa.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ted.iojbl.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://woa.zhiwuduotai.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pna.meibo888.top

[H03] 主动抛出异常
来源：http://tqi.gaohongyu789.top

Py:   raise ValueError("错误信息")
来源：http://snz.birdmap.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kal.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://qcv.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://ubt.meibo888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zxh.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qlj.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vsi.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fil.ivvv.top

[H04] 自定义异常类型
来源：http://pwo.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://can.ehwqpu.com

PHP:  class MyError extends RuntimeException {}
来源：http://nim.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://lav.xuetiantiany.cn

TS:   class MyError extends Error {}
来源：http://scs.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://dsb.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ewp.cdnleiting.top

Ruby: class MyError < StandardError; end
来源：http://kgg.nwbrower.top

C#:   class MyException : Exception {}
来源：http://syj.chenzaomai.com

[H05] 捕获特定类型
来源：http://sca.yfazqb.com

Py:   except ValueError as e:
来源：http://vuz.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ptn.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://heg.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ivp.uphjek.com

Java: catch (IOException | SQLException e) {}
来源：http://mwe.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hel.tianlin.xyz

Ruby: rescue ArgumentError => e
来源：http://scv.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pht.zdbjq.cn

[H06] 可选值 / 空值安全访问
来源：http://pds.xylfe.cn

Py:   value = d.get("k") or default
来源：http://fri.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://kgx.yfazqb.com

JS:   obj?.a?.b;  d ?? default
来源：http://xyx.jyoumei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jrx.jianghu66.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://smf.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gzn.dashuyun.cn

Ruby: d&.dig(:a, :b)
来源：http://xuj.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://evj.cucudq.cn

[H07] 断言
来源：http://ueg.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://bud.daria6918.cn

PHP:  assert($x > 0);
来源：http://ell.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://spp.xingfuxueyuan.xyz

TS:   console.assert(x > 0);
来源：http://iva.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://uub.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iui.shzxlz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sep.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://jly.yuanzhike.top

[H08] 获取错误信息与堆栈
来源：http://tvz.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://zfd.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qtt.hywenlv.cn

JS:   e.message;  e.stack
来源：http://qvh.zhengqikj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jjx.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://eiu.ydjk.org.cn

Go:   err.Error()
来源：http://vfb.jyoumei.cn

Ruby: e.message;  e.backtrace
来源：http://eva.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://edf.yuanzhike.top

[H09] 带错误码的异常
来源：http://txv.quarkkingdee.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uok.jiagoushi.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://iov.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ftp.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lpv.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://naz.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://njg.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://jxi.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ril.jqgfzy.top

[H10] 资源自动释放
来源：http://jfb.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gsz.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pfl.wangshuangyany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uac.ehwqpu.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rod.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oop.gotoacloud.top

Go:   defer f.Close()
来源：http://qwh.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://imq.zhaomingkeji.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vqg.zdqjudy.top

================================================================================
来源：http://uza.gzhubu.top

I. 正则表达式
来源：http://ypf.ppjwa.cn

================================================================================
来源：http://jvz.pengpengdd.cyou

[I01] 判断是否匹配
来源：http://kna.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://exl.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cqa.xziqi.cn

JS:   /\d+/.test(s)
来源：http://uzo.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://yay.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://poz.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vbw.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://mbd.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ooj.ivvv.top

[I02] 提取所有匹配
来源：http://lpc.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://nlz.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://una.hongshengwenyu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pwt.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://pbt.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xyx.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jhd.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://zxa.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cgm.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://vap.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://agz.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rgl.nanxinkj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cmo.fanxiaobao.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vgb.fktsv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qow.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pap.yj20258.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sxs.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gqs.yangfankeji.com

[I04] 正则替换
来源：http://whi.guowangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://oxo.daria6918.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gvo.ehwqpu.com

JS:   s.replace(/\d+/g, "#")
来源：http://bqn.zhijiandao.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yey.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://znw.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://xsv.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vcr.shuidangran.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nfl.xylfe.cn

[I05] 按正则拆分
来源：http://dpo.pengpengdd.cyou

Py:   re.split(r"\s*,\s*", s)
来源：http://ebv.redwolf501.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kbw.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://bse.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://gaj.snrcjt.cn

Java: s.split("\\s*,\\s*")
来源：http://sgo.iojbl.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jgj.dianchejie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pwn.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bye.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qtq.wangshuangyany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pex.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bzs.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zvh.jiagoushi.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zkd.meibo888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nbu.redwolf501.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://igw.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://opn.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pzo.yfazqb.com

[I07] 忽略大小写与多行模式
来源：http://dgk.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mem.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wzd.nwbrower.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hea.ydzc1.top

TS:   /error/gim
来源：http://wac.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ots.zdbjq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://seh.yj202588.top

Ruby: s.scan(/error/i)
来源：http://oqd.zhiwuduotai.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://alh.dianchejie.cn

[I08] 贪婪与非贪婪匹配
来源：http://rna.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pch.yanxiufei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://apd.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tug.yongpay.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fnr.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://mhr.guowangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jvc.cheryme.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tdl.pycfn.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tze.xingfuxueyuan.xyz

================================================================================
来源：http://una.yonumen.top

J. 日期与时间
来源：http://xud.fengsongda.top

================================================================================
来源：http://zbe.ydzc1.top

[J01] 获取当前时间
来源：http://rnd.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://cjb.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ejn.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://vuy.andypj.xyz

TS:   new Date();  Date.now()
来源：http://eqb.quarkkingdee.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bhh.gotoacloud.top

Go:   time.Now()
来源：http://uqm.jqgufenzy.top

Ruby: Time.now
来源：http://lbw.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ezl.zhongyouzk.top

[J02] 格式化输出
来源：http://tsi.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gkr.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dvu.nanxuanxn.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://szu.gaohongyu789.top

TS:   d.toISOString()
来源：http://vpn.yuanzhike.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kxc.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rtb.guannengcc.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mxn.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://deb.zycfv.cn

[J03] 字符串解析为日期
来源：http://bdy.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://smh.yongpay.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lvw.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://wpt.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://dwr.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://nia.redwolf501.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lzk.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://gvh.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tqx.xinyue.icu

[J04] 时间戳与日期互转
来源：http://ygr.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vjq.hammf.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qpn.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://foh.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wsz.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://knq.chenzaomai.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yhp.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ers.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vpi.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://adj.xuetiantiany.cn

Py:   now + timedelta(days=7)
来源：http://awu.kuanghao11.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wbu.ehwqpu.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hwt.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gak.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://xpp.shuidangran.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rmp.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://kge.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://fnu.yueranfly.top

[J06] 计算两时间之差
来源：http://gnf.sweek.top

Py:   (end - start).total_seconds()
来源：http://ypy.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://ijb.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jfp.yanxiufei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dfo.c1oappe.top

Java: Duration.between(start, end).toSeconds()
来源：http://nyf.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://ohx.xziqi.cn

Ruby: end - start                 # 返回秒数
来源：http://had.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://mrp.ctjpmb.com

[J07] 比较两个日期
来源：http://qce.wangdashe.top

Py:   d1 < d2;  d1 == d2
来源：http://wqm.daxiang520.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zzn.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://qss.sxryk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uae.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kve.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dwk.fzhhl.top

Ruby: d1 < d2;  d1 == d2
来源：http://ntj.ehwqpu.com

C#:   d1 < d2;  d1 == d2
来源：http://rzb.havefunace.top

[J08] 提取年月日与星期
来源：http://fxf.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vhv.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://quk.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://buv.gaohongyu789.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://alq.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ztp.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fre.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lqs.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jcr.jinqigfzy.top

[J09] 时区处理
来源：http://fvf.zhiwuduotai.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ajf.zhijiandao.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ijc.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nyj.jqgufenzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mou.iojbl.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mid.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gdz.fktsv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yru.svipenyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oji.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://ydn.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kuh.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kfg.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zax.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nsv.guannengcc.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nwb.fanxiaobao.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ypq.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dgs.chenlongwang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jjo.ehwqpu.com

================================================================================
来源：http://egi.svipenyu.cn

K. JSON 与序列化
来源：http://cwb.fanxiaobao.xyz

================================================================================
来源：http://wje.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://fdb.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mpj.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://krb.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://qmu.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://osd.aizwys.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zra.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://bpi.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://ckg.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://mhv.yj202588.top

[K02] JSON 字符串转对象
来源：http://gem.vehdjk.com

Py:   json.loads(s)
来源：http://vdq.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vrb.jinqigfzy.top

JS:   JSON.parse(s)
来源：http://rgy.316326.xyz

TS:   JSON.parse(s)
来源：http://rjt.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kvs.jlsjyb.cn

Go:   json.Unmarshal(data, &v)
来源：http://jui.yfazqb.com

Ruby: JSON.parse(s)
来源：http://iqq.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://quf.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://ffq.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nvk.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ezv.daria6918.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dzw.hesvh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jqp.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dhu.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qhj.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://srm.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mff.zycfv.cn

[K04] 读取 JSON 文件
来源：http://sgl.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cej.jinqigufen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kzq.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qmk.jlsjyb.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fot.hesvh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qxc.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rdw.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bnk.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nqu.yongpay.top

[K05] 深拷贝对象
来源：http://siw.gogol.net.cn

Py:   copy.deepcopy(obj)
来源：http://itk.yj202588.top

PHP:  unserialize(serialize($obj));
来源：http://mng.smart0.xyz

JS:   structuredClone(obj)
来源：http://hbr.9152youxi.cn

TS:   structuredClone(obj)
来源：http://bst.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://azt.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://smv.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://utn.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rjp.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://qxz.52xcode.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://njw.zdbjq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jhi.yueranfly.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ylr.shuidangran.top


<!-- 参考信息 -->