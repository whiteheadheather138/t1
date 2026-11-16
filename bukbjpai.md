代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xwt.smart0.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://och.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xfu.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://iup.redwolf501.top

Py:   try: f()⏎finally: cleanup()
来源：http://kum.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ryl.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nze.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ekp.ydjk.org.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kls.fanxiaobao.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://naj.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gxd.tian-w.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uzp.yj20258888.top

[H03] 主动抛出异常
来源：http://ffg.dashuyun.cn

Py:   raise ValueError("错误信息")
来源：http://nxx.jlsjyb.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jyv.xuanzx.com

JS:   throw new Error("错误信息");
来源：http://oqy.yj202588.top

TS:   throw new Error("错误信息");
来源：http://aoc.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dgb.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pjy.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lxq.chenjidiqi.icu

C#:   throw new ArgumentException("错误信息");
来源：http://mss.tanke756.top

[H04] 自定义异常类型
来源：http://rzj.nwbrower.top

Py:   class MyError(Exception): pass
来源：http://xsu.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://kdd.epnwcf.com

JS:   class MyError extends Error {}
来源：http://mbr.gogol.net.cn

TS:   class MyError extends Error {}
来源：http://rjs.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://brd.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bjx.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://vkz.feifeiyinyue.top

C#:   class MyException : Exception {}
来源：http://jft.ydjk.org.cn

[H05] 捕获特定类型
来源：http://bdy.fzhhl.top

Py:   except ValueError as e:
来源：http://oet.epnwcf.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ytl.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://wjk.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://pqc.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://ish.jinqigfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xbz.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://hoy.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://siq.kuanghao11.cn

[H06] 可选值 / 空值安全访问
来源：http://jsd.yuxming.cn

Py:   value = d.get("k") or default
来源：http://ydz.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hom.jinqigfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://ief.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://ntl.zdqjudy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zel.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xvm.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://xca.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://rwz.dashuyun.cn

[H07] 断言
来源：http://dkn.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://mbc.shuidangran.top

PHP:  assert($x > 0);
来源：http://cqg.zhixingplan.top

JS:   console.assert(x > 0);
来源：http://nrc.52xcode.cn

TS:   console.assert(x > 0);
来源：http://okp.yanxiufei.cn

Java: assert x > 0 : "必须为正";
来源：http://rff.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rar.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://drw.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://kuq.gogol.net.cn

[H08] 获取错误信息与堆栈
来源：http://khp.fzhhl.top

Py:   str(e);  traceback.format_exc()
来源：http://cwy.jiagoushi.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hon.pycfn.com

JS:   e.message;  e.stack
来源：http://uep.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ncp.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://npd.aizwys.cn

Go:   err.Error()
来源：http://uux.tianlin.xyz

Ruby: e.message;  e.backtrace
来源：http://xqm.quarkkingdee.top

C#:   e.Message;  e.StackTrace
来源：http://jpz.gogol.net.cn

[H09] 带错误码的异常
来源：http://dmh.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uhb.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qjg.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yik.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://thu.ydjk.org.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://upo.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tpk.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://law.fengsongda.top

C#:   // 自定义异常类中加 Code 属性
来源：http://eyk.vehdjk.com

[H10] 资源自动释放
来源：http://nee.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rlh.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://udg.shuidangran.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bic.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hvz.jqgfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wcx.jiagoushi.top

Go:   defer f.Close()
来源：http://xvu.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://urt.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pef.xuanzx.com

================================================================================
来源：http://chq.tianlin.xyz

I. 正则表达式
来源：http://zwx.xinyue.icu

================================================================================
来源：http://fqn.tarul.cn

[I01] 判断是否匹配
来源：http://xyv.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ump.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://xxa.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://mmm.jinqigufen.top

TS:   /\d+/.test(s)
来源：http://rco.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fqu.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jlo.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://cvj.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rvi.zhengqikj.top

[I02] 提取所有匹配
来源：http://maf.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://skb.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tns.wangshuangyany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uwo.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://fkb.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oww.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sfq.daria6918.cn

Ruby: s.scan(/\d+/)
来源：http://vuk.fanxiaobao.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://olb.hfpthk.cn

[I03] 提取捕获分组
来源：http://yya.jiagoushi.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wxv.316326.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://coa.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://elv.tanke756.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cpt.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xrb.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bna.cucudq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ipr.wangdashe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rxy.yfazqb.com

[I04] 正则替换
来源：http://cwy.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fwr.jinqigfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://edk.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tiz.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://mgc.xuetiantiany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uiw.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ami.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bcj.yonumen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sce.fehbvm.com

[I05] 按正则拆分
来源：http://gij.shanyushiyangtech.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uqf.redwolf501.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ekf.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://jss.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://fwn.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://qjr.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mpv.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vxg.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kfw.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://okb.hongshengwenyu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://skc.jiagoushi.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://asp.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xfc.yj202588.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wub.nanxinkj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jej.mhx1999.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hax.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zzp.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zha.cashguo.top

[I07] 忽略大小写与多行模式
来源：http://xbv.yj202588.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pay.zhiwuduotai.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tjz.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ncz.yanxiufei.cn

TS:   /error/gim
来源：http://cxn.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aso.shanyushiyangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bwy.fktsv.cn

Ruby: s.scan(/error/i)
来源：http://wfg.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bla.hfpthk.cn

[I08] 贪婪与非贪婪匹配
来源：http://spy.meibo888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ljo.52xcode.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nda.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xhn.daria6918.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wbm.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://hrk.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ikp.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oqn.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wid.tanke756.top

================================================================================
来源：http://aaz.havefunace.top

J. 日期与时间
来源：http://lfj.hnqzz.top

================================================================================
来源：http://dug.ppjwa.cn

[J01] 获取当前时间
来源：http://gay.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://zub.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://utn.zycfv.cn

JS:   new Date();  Date.now()
来源：http://xvj.aizwys.cn

TS:   new Date();  Date.now()
来源：http://zrm.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zlh.pycfn.com

Go:   time.Now()
来源：http://lfn.ctjpmb.com

Ruby: Time.now
来源：http://nkp.yanxiufei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aty.nwbrower.top

[J02] 格式化输出
来源：http://xmf.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bfh.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rtj.ehwqpu.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qya.yueranfly.top

TS:   d.toISOString()
来源：http://tcs.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dwa.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qke.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vcp.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uio.sysykeji.top

[J03] 字符串解析为日期
来源：http://lpa.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fcf.jyoumei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xxq.ivvv.top

JS:   new Date("2024-01-02")
来源：http://uvf.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://xdj.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://rqc.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fmy.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://tad.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bli.yuxming.cn

[J04] 时间戳与日期互转
来源：http://qpx.jqgfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qgg.fzhhl.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jdz.birdmap.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lzf.jqgufenzy.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ttt.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wex.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wov.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xvb.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qns.dianchejie.cn

[J05] 时间加减（加 7 天）
来源：http://ixw.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://kmg.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jzt.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ykj.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mxx.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://hxw.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jrw.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://bil.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://hkq.gzhubu.top

[J06] 计算两时间之差
来源：http://bfh.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://nbt.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://pxk.9152youxi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xrt.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ont.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://njx.gaohongyu789.top

Go:   end.Sub(start).Hours()
来源：http://dpd.ivvv.top

Ruby: end - start                 # 返回秒数
来源：http://iob.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://mfe.shzxlz.cn

[J07] 比较两个日期
来源：http://knl.0kj1m.cn

Py:   d1 < d2;  d1 == d2
来源：http://qqc.sjlbkw.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yap.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ypy.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://rcp.svipenyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qos.vehdjk.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jww.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://kmc.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://ped.yj20258888.top

[J08] 提取年月日与星期
来源：http://wzs.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lxs.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fom.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ylg.uphjek.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fcm.cdnleiting.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ovz.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://okg.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pkf.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://unb.redwolf501.top

[J09] 时区处理
来源：http://icp.tanke756.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dac.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dkw.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xvs.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://exv.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cju.hnxiangtu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vbi.shangyingyoupin.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wlk.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vxb.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://fye.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xgj.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://thy.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qyz.fktsv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bwa.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pka.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lzb.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nkh.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dqn.ppjwa.cn

================================================================================
来源：http://ikq.gogol.net.cn

K. JSON 与序列化
来源：http://ojw.jinyuanbaomall.cn

================================================================================
来源：http://dsq.jyoumei.cn

[K01] 对象转 JSON 字符串
来源：http://flq.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://njr.aibaodan.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cmy.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://myr.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://zpm.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jiu.fktsv.cn

Go:   json.Marshal(obj)
来源：http://jkv.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://rjc.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://myq.vehdjk.com

[K02] JSON 字符串转对象
来源：http://jxg.gaohongyu789.top

Py:   json.loads(s)
来源：http://ltm.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nkr.jqgfzy.top

JS:   JSON.parse(s)
来源：http://hue.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://sla.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pad.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://gxa.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://csh.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aya.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://eax.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uhs.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zed.fktsv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ecz.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ics.zhijiandao.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rsz.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bfk.tarul.cn

Ruby: JSON.pretty_generate(obj)
来源：http://azg.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://luv.iojbl.cn

[K04] 读取 JSON 文件
来源：http://paz.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ufi.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wof.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xkx.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xpu.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ote.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jus.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sfv.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nuf.andypj.xyz

[K05] 深拷贝对象
来源：http://vqi.sweek.top

Py:   copy.deepcopy(obj)
来源：http://nbk.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://trp.ybcxt.top

JS:   structuredClone(obj)
来源：http://xeh.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://cju.svipenyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qwv.ywan-chungtsiang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zpr.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hoe.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://kgv.guannengcc.top


<!-- 参考信息 -->