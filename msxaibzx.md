代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://scg.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://utp.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vvh.chenjidiqi.icu

[H02] finally / ensure 收尾
来源：http://lbs.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yua.zycfv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lfe.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://foo.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fzi.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gtl.xylfe.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tdm.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wot.yuxming.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://aia.gaohongyu789.top

[H03] 主动抛出异常
来源：http://crx.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://obh.meibo888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ale.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://xzk.hywenlv.cn

TS:   throw new Error("错误信息");
来源：http://sxp.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lvq.bbcook.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://flp.wangdashe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kuc.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pmy.snrcjt.cn

[H04] 自定义异常类型
来源：http://gps.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://zfh.aibaodan.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mbg.shanyushiyangtech.top

JS:   class MyError extends Error {}
来源：http://qiq.fanxiaobao.xyz

TS:   class MyError extends Error {}
来源：http://gtj.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://yjg.shangyingyoupin.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wzp.jqgfzy.top

Ruby: class MyError < StandardError; end
来源：http://feh.nanxinkj.top

C#:   class MyException : Exception {}
来源：http://sxs.jianghu66.top

[H05] 捕获特定类型
来源：http://yqe.hfpthk.cn

Py:   except ValueError as e:
来源：http://qgc.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://elo.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://wxd.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://qcm.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://eqw.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://irb.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://qvq.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sed.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://eir.guowangkeji.top

Py:   value = d.get("k") or default
来源：http://ykk.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://ins.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://irm.uphjek.com

TS:   obj?.a?.b;  d ?? default
来源：http://bhk.tarul.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bgx.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://oyx.sxryk.cn

Ruby: d&.dig(:a, :b)
来源：http://ruq.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://ayn.yuxming.cn

[H07] 断言
来源：http://yfh.sweek.top

Py:   assert x > 0, "必须为正"
来源：http://smg.shanyushiyangtech.top

PHP:  assert($x > 0);
来源：http://wac.daxiang520.top

JS:   console.assert(x > 0);
来源：http://vti.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://kdy.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://cah.nanxinkj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ugk.hammf.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bbd.hesvh.cn

C#:   Debug.Assert(x > 0);
来源：http://zmb.kuanghao11.cn

[H08] 获取错误信息与堆栈
来源：http://pxj.quarkkingdee.top

Py:   str(e);  traceback.format_exc()
来源：http://ngs.xinyue.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://etq.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://zsx.jqgfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xcu.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fob.jinyuanbaomall.cn

Go:   err.Error()
来源：http://rgp.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://jmv.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://svn.nanxinkj.top

[H09] 带错误码的异常
来源：http://nxc.wangshuangyany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://joh.cucudq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ipi.havefunace.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lum.zdqjudy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dgv.vehdjk.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jgm.shanyushiyangkeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zwv.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://inh.jqgufenzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ibr.ydzc1.top

[H10] 资源自动释放
来源：http://qpf.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://ufk.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://drq.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://adt.tian-w.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wqq.aibaodan.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wyw.tanke756.top

Go:   defer f.Close()
来源：http://vpy.xuanzx.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aju.jinghuilouyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rox.gotoacloud.top

================================================================================
来源：http://hjo.havefunace.top

I. 正则表达式
来源：http://kzr.aizwys.cn

================================================================================
来源：http://zmo.aizwys.cn

[I01] 判断是否匹配
来源：http://yui.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qjz.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nfq.bbcook.cn

JS:   /\d+/.test(s)
来源：http://pbe.ivvv.top

TS:   /\d+/.test(s)
来源：http://ocv.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cjj.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qus.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://lpy.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://prw.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://jat.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://lum.tianlin.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kip.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ukz.hywenlv.cn

TS:   s.match(/\d+/g)
来源：http://jhe.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://owy.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xyd.redwolf501.top

Ruby: s.scan(/\d+/)
来源：http://zuc.gaohongyu789.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pdc.shanyushiyangtech.top

[I03] 提取捕获分组
来源：http://buf.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jvq.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ijm.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zcw.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ifh.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ogg.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wmq.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rdq.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fba.yfazqb.com

[I04] 正则替换
来源：http://gdk.snrcjt.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lpn.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ohf.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gjv.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://jnq.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ddp.tarul.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oho.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zrm.shangyingyoupin.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tfn.yj20258888.top

[I05] 按正则拆分
来源：http://tej.gotoacloud.top

Py:   re.split(r"\s*,\s*", s)
来源：http://viy.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cwy.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://ckc.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://fcl.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://daf.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zjq.vqdsnc.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hzr.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ouj.meibo888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xpm.shzxlz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zte.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qik.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fpg.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gqz.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uwp.zhijiandao.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://duc.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oph.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rcb.cashguo.top

[I07] 忽略大小写与多行模式
来源：http://vht.gzhubu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zvw.dashuyun.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hfj.zhiwuduotai.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rza.jinqigfzy.top

TS:   /error/gim
来源：http://qza.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cjd.yanxiufei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mij.svipenyu.cn

Ruby: s.scan(/error/i)
来源：http://rrm.hcnkem.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kok.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://esf.jiagoushi.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aak.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rox.zycfv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mml.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lao.hywenlv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ogt.yuxming.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bkd.hesvh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xgg.xylfe.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jra.tarul.cn

================================================================================
来源：http://vme.sysykeji.top

J. 日期与时间
来源：http://rxx.jinqigfzy.top

================================================================================
来源：http://iuc.dianchejie.cn

[J01] 获取当前时间
来源：http://oez.hcnkem.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://opy.xylfe.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gvp.aibaodan.cn

JS:   new Date();  Date.now()
来源：http://vgt.hesvh.cn

TS:   new Date();  Date.now()
来源：http://icl.pycfn.com

Java: LocalDateTime.now();  Instant.now()
来源：http://meq.ywan-chungtsiang.top

Go:   time.Now()
来源：http://yai.zhixingplan.top

Ruby: Time.now
来源：http://yey.haohaochexian.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wvs.aizwys.cn

[J02] 格式化输出
来源：http://qqj.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pgi.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ovr.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xgk.pengpengdd.cyou

TS:   d.toISOString()
来源：http://jbh.svipenyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xtt.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zgg.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eiz.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tnr.ydzc1.top

[J03] 字符串解析为日期
来源：http://ofo.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://epi.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fym.zhiwuduotai.top

JS:   new Date("2024-01-02")
来源：http://wgy.jlsjyb.cn

TS:   new Date("2024-01-02")
来源：http://qrd.xingfuxueyuan.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://eia.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lcy.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://uoj.shanyushiyangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wxu.bjfxy.top

[J04] 时间戳与日期互转
来源：http://hmj.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vkk.sufxvd.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xof.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tyc.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://clw.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://akn.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://csp.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aph.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vwt.yj20258.top

[J05] 时间加减（加 7 天）
来源：http://qis.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://zbn.yj20258888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wse.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rtm.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cwm.hongshengwenyu.top

Java: LocalDate.now().plusDays(7)
来源：http://xna.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rej.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://gdo.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jsl.snrcjt.cn

[J06] 计算两时间之差
来源：http://yda.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://uuu.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://auy.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jup.zdqjudy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xkw.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://vsg.bjfxy.top

Go:   end.Sub(start).Hours()
来源：http://hsd.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://asd.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://val.gaohongyu789.top

[J07] 比较两个日期
来源：http://ryi.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://asz.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qgc.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://fqv.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://sel.52xcode.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qks.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ihy.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://pyj.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://pgf.c1oappe.top

[J08] 提取年月日与星期
来源：http://goy.wangdashe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rkp.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vwk.jyoumei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ahi.hcnkem.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jog.pycfn.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dwd.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://obm.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cdf.zhoulong.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dzt.ppjwa.cn

[J09] 时区处理
来源：http://zly.shangyingyoupin.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ben.yueranfly.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yaf.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qoo.zhoulong.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://han.cashguo.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vpr.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zuv.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rui.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bie.sufxvd.cn

[J10] 取今天 / 本月第一天
来源：http://lmx.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://wsl.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mxf.ywan-chungtsiang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hif.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tsk.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gxi.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ypj.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://esl.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dxb.ybcxt.top

================================================================================
来源：http://sbo.yuxming.cn

K. JSON 与序列化
来源：http://xte.mhx1999.top

================================================================================
来源：http://vee.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://mhw.ctjpmb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gdr.fktsv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cwc.cashguo.top

JS:   JSON.stringify(obj)
来源：http://jlv.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://jfb.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fxs.cqqwz.cn

Go:   json.Marshal(obj)
来源：http://mbj.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://gzt.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hok.bjfxy.top

[K02] JSON 字符串转对象
来源：http://rsj.cashguo.top

Py:   json.loads(s)
来源：http://vbx.9152youxi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wvv.zdbjq.cn

JS:   JSON.parse(s)
来源：http://yhx.tian-w.cn

TS:   JSON.parse(s)
来源：http://hfs.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oxl.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://zxw.yanxiufei.cn

Ruby: JSON.parse(s)
来源：http://fik.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xzb.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://tmt.hnxiangtu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pei.sjlbkw.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kka.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ssh.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://igo.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qpp.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lhe.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://nmz.ybcxt.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hoo.jlsjyb.cn

[K04] 读取 JSON 文件
来源：http://xfs.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zgf.vqdsnc.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cav.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://inr.nanxuanxn.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://anw.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hql.zdqjudy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vpe.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gsl.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dbu.ydjk.org.cn

[K05] 深拷贝对象
来源：http://uvc.cucudq.cn

Py:   copy.deepcopy(obj)
来源：http://uwh.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://qhl.gogol.net.cn

JS:   structuredClone(obj)
来源：http://bqq.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://veo.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nsw.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dfk.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://axk.epnwcf.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ssf.ivvv.top


<!-- 参考信息 -->