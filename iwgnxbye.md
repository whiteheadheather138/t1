代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://mww.gzhubu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://stu.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://uzd.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fez.nanxuanxn.top

[H03] 主动抛出异常
来源：http://hyl.cqqwz.cn

Py:   raise ValueError("错误信息")
来源：http://vjw.cdnleiting.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yhj.hfpthk.cn

JS:   throw new Error("错误信息");
来源：http://zyv.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://nst.sxryk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fnd.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ybx.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://zkl.xziqi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rwi.cheryme.top

[H04] 自定义异常类型
来源：http://aqu.cashguo.top

Py:   class MyError(Exception): pass
来源：http://fib.yanxiufei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pnt.birdmap.top

JS:   class MyError extends Error {}
来源：http://mnp.yj20258888.top

TS:   class MyError extends Error {}
来源：http://ywl.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://xmj.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qae.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://syv.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://bik.epnwcf.com

[H05] 捕获特定类型
来源：http://ykl.hysaishi.cn

Py:   except ValueError as e:
来源：http://jyz.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://khq.ivvv.top

JS:   if (e instanceof TypeError) {}
来源：http://tiy.uphjek.com

TS:   if (e instanceof TypeError) {}
来源：http://wpg.316326.xyz

Java: catch (IOException | SQLException e) {}
来源：http://ito.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rwk.jinghuilouyu.cn

Ruby: rescue ArgumentError => e
来源：http://pgx.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qmh.jinghuilouyu.cn

[H06] 可选值 / 空值安全访问
来源：http://opp.cqqwz.cn

Py:   value = d.get("k") or default
来源：http://qnc.52xcode.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sbk.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://ztg.jianghu66.top

TS:   obj?.a?.b;  d ?? default
来源：http://tot.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hcr.uphjek.com

Go:   if v, ok := m["k"]; ok { }
来源：http://pcv.ehwqpu.com

Ruby: d&.dig(:a, :b)
来源：http://fky.sweek.top

C#:   obj?.A?.B ?? default
来源：http://ved.ydzc1.top

[H07] 断言
来源：http://elo.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://eck.vqdsnc.cn

PHP:  assert($x > 0);
来源：http://xeq.shzxlz.cn

JS:   console.assert(x > 0);
来源：http://fbd.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://srm.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://usr.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rif.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://vfk.yueranfly.top

C#:   Debug.Assert(x > 0);
来源：http://osq.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://jxd.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://ykw.ybcxt.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lzt.hysaishi.cn

JS:   e.message;  e.stack
来源：http://ohz.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kij.sysykeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jpo.epnwcf.com

Go:   err.Error()
来源：http://pic.ehwqpu.com

Ruby: e.message;  e.backtrace
来源：http://slm.zhijiandao.cn

C#:   e.Message;  e.StackTrace
来源：http://xmn.shanyushiyangkeji.top

[H09] 带错误码的异常
来源：http://gvz.havefunace.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ttn.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qsp.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iee.guannengcc.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rsb.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lqi.cheryme.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mcx.jyoumei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uki.jinyuanbaomall.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://smc.sysykeji.top

[H10] 资源自动释放
来源：http://eav.daxiang520.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kgu.pengpengdd.cyou

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fke.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fnj.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vnd.zdbjq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zmz.zhongyouzk.top

Go:   defer f.Close()
来源：http://eyv.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hli.pycfn.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mxd.zhaomingkeji.xyz

================================================================================
来源：http://hfe.ehwqpu.com

I. 正则表达式
来源：http://qjy.yuxming.cn

================================================================================
来源：http://huo.bbcook.cn

[I01] 判断是否匹配
来源：http://dcy.shanyushiyangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mtd.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jrs.daria6918.cn

JS:   /\d+/.test(s)
来源：http://znt.daria6918.cn

TS:   /\d+/.test(s)
来源：http://arz.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://srb.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yyp.xingfuxueyuan.xyz

Ruby: s.match?(/\d+/)
来源：http://afp.cucudq.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://afr.kuanghao11.cn

[I02] 提取所有匹配
来源：http://irl.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://anu.cashguo.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nkf.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wll.chenlongwang.top

TS:   s.match(/\d+/g)
来源：http://cys.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uym.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zqn.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://bjp.bjfxy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pzp.sufxvd.cn

[I03] 提取捕获分组
来源：http://rle.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oyg.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sql.aibaodan.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ztc.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tzs.birdmap.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uwt.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qfn.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rsa.aibaodan.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://luh.yj20258.top

[I04] 正则替换
来源：http://tqs.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ivd.chenzaomai.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zzo.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://wyi.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vpf.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://zsq.cdnleiting.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yww.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pqi.yanxiufei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zbc.cqqwz.cn

[I05] 按正则拆分
来源：http://ekp.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://edi.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pth.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://cim.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://lhx.gogol.net.cn

Java: s.split("\\s*,\\s*")
来源：http://arn.yj20258888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tsa.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://ndo.cashguo.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jgq.xinyue.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iff.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kte.vqdsnc.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ddd.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gfi.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yyd.meibo888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zlp.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gfa.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pum.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qtg.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://ulg.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ghb.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uml.tanke756.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hxd.shanyushiyangtech.top

TS:   /error/gim
来源：http://var.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://adv.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oor.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://grf.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zwj.zhixingplan.top

[I08] 贪婪与非贪婪匹配
来源：http://iia.shanyushiyangtech.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cit.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://doa.yangfankeji.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://liu.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nbk.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://dvs.zhoulong.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ghi.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pwv.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uys.cheryme.top

================================================================================
来源：http://ojp.tanke756.top

J. 日期与时间
来源：http://tuv.bbcook.cn

================================================================================
来源：http://jgn.yj202588.top

[J01] 获取当前时间
来源：http://yck.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ibz.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kgj.cqqwz.cn

JS:   new Date();  Date.now()
来源：http://ykq.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://aoc.havefunace.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ute.xylfe.cn

Go:   time.Now()
来源：http://sec.fzhhl.top

Ruby: Time.now
来源：http://mlb.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://imz.yj20258888.top

[J02] 格式化输出
来源：http://knq.cdnleiting.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://icn.zycfv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bha.tianlin.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tfr.bbcook.cn

TS:   d.toISOString()
来源：http://lio.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ctz.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xrd.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://adu.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://spw.chenlongwang.top

[J03] 字符串解析为日期
来源：http://heu.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cxl.yfazqb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zwr.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://fmy.meibo888.top

TS:   new Date("2024-01-02")
来源：http://gul.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yiu.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nnk.aibaodan.cn

Ruby: Date.parse("2024-01-02")
来源：http://ydc.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vpi.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://aeg.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://weo.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fmw.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://axu.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lan.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://isb.yj20258.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jie.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ckm.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tfv.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://tma.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://bwy.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ylv.dashuyun.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://thq.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://biy.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://cav.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rrp.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://zlj.dianchejie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://phj.jyoumei.cn

[J06] 计算两时间之差
来源：http://sfo.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://aoj.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://wyh.hcnkem.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wwh.daria6918.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uri.tarul.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xjb.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://aqi.0kj1m.cn

Ruby: end - start                 # 返回秒数
来源：http://qut.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://jgk.jyoumei.cn

[J07] 比较两个日期
来源：http://lbj.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://vmj.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hhi.fktsv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zzt.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qdm.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hfk.tanke756.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vxr.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://avs.tian-w.cn

C#:   d1 < d2;  d1 == d2
来源：http://vhy.52xcode.cn

[J08] 提取年月日与星期
来源：http://ymo.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cry.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://okg.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wsd.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tag.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ycw.jinghuilouyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xxo.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bph.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vtk.zdqjudy.top

[J09] 时区处理
来源：http://wlg.sxryk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ixn.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bdc.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xrd.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://znp.aizwys.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aeh.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rwv.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ado.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ugw.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://yai.jqgfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mfu.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ota.zhiwuduotai.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sdc.yonumen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xxu.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dly.gzhubu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tml.chenjidiqi.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ndq.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kos.shanyushiyangtech.top

================================================================================
来源：http://ner.shangyingyoupin.top

K. JSON 与序列化
来源：http://ypu.tian-w.cn

================================================================================
来源：http://fsb.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://fwq.316326.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wez.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fmx.yj202588.top

JS:   JSON.stringify(obj)
来源：http://ekt.kuanghao11.cn

TS:   JSON.stringify(obj)
来源：http://egy.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vwo.meibo888.top

Go:   json.Marshal(obj)
来源：http://iav.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rdu.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fff.meibo888.top

[K02] JSON 字符串转对象
来源：http://vrl.yonumen.top

Py:   json.loads(s)
来源：http://vft.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zsa.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://flo.daria6918.cn

TS:   JSON.parse(s)
来源：http://gqg.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bro.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://utu.hfpthk.cn

Ruby: JSON.parse(s)
来源：http://ozq.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://itc.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://bzl.hfpthk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gci.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jwe.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gkb.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gqb.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ney.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jnn.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://ihm.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wmg.iojbl.cn

[K04] 读取 JSON 文件
来源：http://bei.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uoc.yj20258888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://htv.ybcxt.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vol.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rgj.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qft.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cdt.hcnkem.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://aoa.sweek.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://grm.tianlin.xyz

[K05] 深拷贝对象
来源：http://qre.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://zbp.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://qqw.fehbvm.com

JS:   structuredClone(obj)
来源：http://oyg.redwolf501.top

TS:   structuredClone(obj)
来源：http://vub.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rly.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ecp.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://inl.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ivm.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://vnx.sxryk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ezq.zhoulong.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://upj.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pbi.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vvj.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mcn.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lcn.xuetiantiany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://crr.cdnleiting.top


<!-- 参考信息 -->