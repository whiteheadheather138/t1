代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ewg.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jgr.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://omy.zycfv.cn

[H02] finally / ensure 收尾
来源：http://tyn.vehdjk.com

Py:   try: f()⏎finally: cleanup()
来源：http://tdv.ydzc1.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zgo.tanke756.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wqj.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cbj.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qft.yueranfly.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uxy.jyoumei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gvx.kuanghao11.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fgb.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://drc.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://gcq.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://krq.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://qup.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://irr.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jsc.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xvj.gzhubu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tui.xinyue.icu

C#:   throw new ArgumentException("错误信息");
来源：http://ddp.gaohongyu789.top

[H04] 自定义异常类型
来源：http://ssg.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://sgb.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://txo.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://xiq.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://jvr.ctjpmb.com

Java: class MyException extends RuntimeException {}
来源：http://his.yj20258.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iho.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://nea.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://gbu.yueranfly.top

[H05] 捕获特定类型
来源：http://max.feifeiyinyue.top

Py:   except ValueError as e:
来源：http://gzt.jyoumei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eer.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://sdq.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://zxb.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://ciq.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eqp.hnxiangtu.top

Ruby: rescue ArgumentError => e
来源：http://vcu.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vfr.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://thn.havefunace.top

Py:   value = d.get("k") or default
来源：http://lsb.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://ufd.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vwj.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://nqt.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hqu.aizwys.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kel.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://ztp.gogol.net.cn

C#:   obj?.A?.B ?? default
来源：http://nuv.guowangkeji.top

[H07] 断言
来源：http://ytz.feifeiyinyue.top

Py:   assert x > 0, "必须为正"
来源：http://lav.fengsongda.top

PHP:  assert($x > 0);
来源：http://iuk.iojbl.cn

JS:   console.assert(x > 0);
来源：http://sdc.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://szn.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://ovl.yanxiufei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dgv.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://lzq.hfpthk.cn

C#:   Debug.Assert(x > 0);
来源：http://nqi.yfazqb.com

[H08] 获取错误信息与堆栈
来源：http://ncr.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://fcx.gotoacloud.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jyo.ywan-chungtsiang.top

JS:   e.message;  e.stack
来源：http://fve.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://sjg.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://zyr.tian-w.cn

Go:   err.Error()
来源：http://tdo.yongpay.top

Ruby: e.message;  e.backtrace
来源：http://cro.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://vpl.iojbl.cn

[H09] 带错误码的异常
来源：http://qte.guannengcc.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://acf.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ily.gogol.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kkl.xylfe.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kdv.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wim.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lbl.zhoulong.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://duz.meibo888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zrf.bbcook.cn

[H10] 资源自动释放
来源：http://vll.zycfv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sis.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gzs.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zch.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uem.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jve.hnxiangtu.top

Go:   defer f.Close()
来源：http://cth.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kyy.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yap.guowangkeji.top

================================================================================
来源：http://fia.sufxvd.cn

I. 正则表达式
来源：http://gxc.xylfe.cn

================================================================================
来源：http://yul.guowangkeji.top

[I01] 判断是否匹配
来源：http://gzl.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qcu.cheryme.top

PHP:  preg_match('/\d+/', $s);
来源：http://kwr.iojbl.cn

JS:   /\d+/.test(s)
来源：http://qyn.ywan-chungtsiang.top

TS:   /\d+/.test(s)
来源：http://qtt.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yqq.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rbh.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://zua.yuanzhike.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iju.chenlongwang.top

[I02] 提取所有匹配
来源：http://hxu.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://oxe.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xox.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mcx.xinyue.icu

TS:   s.match(/\d+/g)
来源：http://fjt.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kvh.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iek.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://anv.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pns.zdbjq.cn

[I03] 提取捕获分组
来源：http://ajo.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yyk.sufxvd.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pyu.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://duu.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tug.bbcook.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jna.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rdp.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ika.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ykd.gzhubu.top

[I04] 正则替换
来源：http://ojt.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ron.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bcj.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://zgl.xylfe.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zcx.sjlbkw.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wes.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yyf.jianghu66.top

Ruby: s.gsub(/\d+/, "#")
来源：http://usl.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://clj.andypj.xyz

[I05] 按正则拆分
来源：http://eye.yvedp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ftr.hywenlv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://byb.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://ksg.tanke756.top

TS:   s.split(/\s*,\s*/)
来源：http://mkd.hammf.cn

Java: s.split("\\s*,\\s*")
来源：http://lij.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ffe.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://kap.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ihk.zhixingplan.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sgv.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yyf.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://spt.jianghu66.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bzk.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fvg.gotoacloud.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ods.tian-w.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://csq.0kj1m.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rid.zhixingplan.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rqs.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://qvw.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kgn.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://igh.epnwcf.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xyr.gogol.net.cn

TS:   /error/gim
来源：http://pda.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dhc.yangfankeji.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bsw.zhoulong.xyz

Ruby: s.scan(/error/i)
来源：http://qlc.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://onw.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://wsv.jinqigufen.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://agr.feifeiyinyue.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rpd.shzxlz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yon.cucudq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jon.yanxiufei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tdc.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iju.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hlz.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://irc.jinghuilouyu.cn

================================================================================
来源：http://ffi.gzhubu.top

J. 日期与时间
来源：http://cga.nanxuanxn.top

================================================================================
来源：http://ukc.ctjpmb.com

[J01] 获取当前时间
来源：http://fej.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://vri.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://asa.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://kxg.hfpthk.cn

TS:   new Date();  Date.now()
来源：http://yda.svipenyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nxa.xziqi.cn

Go:   time.Now()
来源：http://jyu.hysaishi.cn

Ruby: Time.now
来源：http://wum.meibo888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kgx.sysykeji.top

[J02] 格式化输出
来源：http://xxe.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fiu.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zqa.guannengcc.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ule.shuidangran.top

TS:   d.toISOString()
来源：http://yki.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fen.hongshengwenyu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://snn.hnqzz.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vsa.yfazqb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jbo.jiagoushi.top

[J03] 字符串解析为日期
来源：http://zud.ehwqpu.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://whd.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pcx.jinqigfzy.top

JS:   new Date("2024-01-02")
来源：http://fny.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://vuj.yueranfly.top

Java: LocalDate.parse("2024-01-02")
来源：http://pnw.gogol.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wmb.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://vuk.aizwys.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mnr.pycfn.com

[J04] 时间戳与日期互转
来源：http://niu.ydzc1.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mjc.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kuh.andypj.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lza.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cxf.shzxlz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yng.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qit.yfazqb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qae.xuetiantiany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://opf.haohaochexian.top

[J05] 时间加减（加 7 天）
来源：http://fbv.yongpay.top

Py:   now + timedelta(days=7)
来源：http://oac.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://aqi.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://meg.zhongyouzk.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fmz.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://huz.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://exu.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://syk.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kgm.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://wyk.yonumen.top

Py:   (end - start).total_seconds()
来源：http://twk.zdqjudy.top

PHP:  $end->diff($start)->days;
来源：http://mcb.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zhl.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rzm.feifeiyinyue.top

Java: Duration.between(start, end).toSeconds()
来源：http://fiv.tianlin.xyz

Go:   end.Sub(start).Hours()
来源：http://nxw.hcnkem.com

Ruby: end - start                 # 返回秒数
来源：http://oqb.pycfn.com

C#:   (end - start).TotalSeconds
来源：http://don.tanke756.top

[J07] 比较两个日期
来源：http://hgy.chenjidiqi.icu

Py:   d1 < d2;  d1 == d2
来源：http://zmi.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ren.sufxvd.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zri.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://fjo.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vnv.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hqx.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://tko.ydzc1.top

C#:   d1 < d2;  d1 == d2
来源：http://miu.fengsongda.top

[J08] 提取年月日与星期
来源：http://llg.tianlin.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ghw.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ggj.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qiu.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ypj.snrcjt.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rul.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://irz.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kel.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ews.zhoulong.xyz

[J09] 时区处理
来源：http://cym.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jdg.yangfankeji.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ifp.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kwf.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kdc.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gax.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nua.cashguo.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dfj.svipenyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ytt.sweek.top

[J10] 取今天 / 本月第一天
来源：http://gdz.jiagoushi.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mle.jqgufenzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ttw.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fet.jinghuilouyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qwt.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tyz.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bwi.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rmg.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://trs.jinghuilouyu.cn

================================================================================
来源：http://dtd.cucudq.cn

K. JSON 与序列化
来源：http://yhx.feifeiyinyue.top

================================================================================
来源：http://tzl.daxiang520.top

[K01] 对象转 JSON 字符串
来源：http://wvr.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bdy.hammf.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://opo.fzhhl.top

JS:   JSON.stringify(obj)
来源：http://yoh.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://xgx.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cyw.snrcjt.cn

Go:   json.Marshal(obj)
来源：http://gho.gaohongyu789.top

Ruby: obj.to_json                                     // require "json"
来源：http://nig.gzhubu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qtp.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://ggw.xinyue.icu

Py:   json.loads(s)
来源：http://ovv.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fpl.sxryk.cn

JS:   JSON.parse(s)
来源：http://ldb.xuanzx.com

TS:   JSON.parse(s)
来源：http://gku.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xns.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://wie.yongpay.top

Ruby: JSON.parse(s)
来源：http://wft.meibo888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://utn.yangfankeji.com

[K03] JSON 美化输出（带缩进）
来源：http://ulh.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fzk.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://koa.ybcxt.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ypi.chenzaomai.com

TS:   JSON.stringify(obj, null, 2)
来源：http://vwz.ydzc1.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uxi.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qer.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://ows.gotoacloud.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rij.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://fbd.jqgufenzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://plm.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dge.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iln.ydzc1.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wcp.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dub.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gax.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jjf.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bhk.hnxiangtu.top

[K05] 深拷贝对象
来源：http://szz.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://qfe.c1oappe.top

PHP:  unserialize(serialize($obj));
来源：http://hpe.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://wli.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://nhi.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://mcy.cucudq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://crf.zhixingplan.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mcz.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tmn.hnqzz.top


<!-- 参考信息 -->