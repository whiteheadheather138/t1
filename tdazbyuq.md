代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kky.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://afn.zdqjudy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://klr.zhaomingkeji.xyz

[H02] finally / ensure 收尾
来源：http://pbd.redwolf501.top

Py:   try: f()⏎finally: cleanup()
来源：http://qhm.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://bqd.hcnkem.com

JS:   try { f(); } finally { cleanup(); }
来源：http://buy.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bae.hongshengwenyu.top

Java: try { f(); } finally { cleanup(); }
来源：http://cnh.ydzc1.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rgq.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://arr.jinqigfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qnw.yuxming.cn

[H03] 主动抛出异常
来源：http://bfn.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://xhd.yj20258.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zze.zhijiandao.cn

JS:   throw new Error("错误信息");
来源：http://nid.jyoumei.cn

TS:   throw new Error("错误信息");
来源：http://kpw.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tnq.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lfy.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dqh.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fhc.svipenyu.cn

[H04] 自定义异常类型
来源：http://zpq.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://mlz.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://iqv.ydjk.org.cn

JS:   class MyError extends Error {}
来源：http://abj.yuxming.cn

TS:   class MyError extends Error {}
来源：http://gud.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://pff.cashguo.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wax.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://has.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://ryd.guowangkeji.top

[H05] 捕获特定类型
来源：http://jva.52xcode.cn

Py:   except ValueError as e:
来源：http://hxi.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mby.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://jzo.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://zus.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://klv.pengpengdd.cyou

Go:   errors.Is(err, os.ErrNotExist)
来源：http://soy.jinghuilouyu.cn

Ruby: rescue ArgumentError => e
来源：http://zzo.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://som.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://rmi.cqqwz.cn

Py:   value = d.get("k") or default
来源：http://pym.wangdashe.top

PHP:  $v = $d["k"] ?? null;
来源：http://iej.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rbp.birdmap.top

TS:   obj?.a?.b;  d ?? default
来源：http://emt.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lvy.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://shz.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://fov.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://hmg.zhixingplan.top

[H07] 断言
来源：http://qoq.meibo888.top

Py:   assert x > 0, "必须为正"
来源：http://cfu.uphjek.com

PHP:  assert($x > 0);
来源：http://zza.hcnkem.com

JS:   console.assert(x > 0);
来源：http://ohu.zycfv.cn

TS:   console.assert(x > 0);
来源：http://ikl.chenzaomai.com

Java: assert x > 0 : "必须为正";
来源：http://pyl.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tuv.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wcq.yueranfly.top

C#:   Debug.Assert(x > 0);
来源：http://uga.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://zpy.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://wcb.zhiwuduotai.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wij.xuanzx.com

JS:   e.message;  e.stack
来源：http://fwf.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://drv.fengsongda.top

Java: e.getMessage();  e.printStackTrace()
来源：http://oat.aizwys.cn

Go:   err.Error()
来源：http://lrw.chenzaomai.com

Ruby: e.message;  e.backtrace
来源：http://ahv.vqdsnc.cn

C#:   e.Message;  e.StackTrace
来源：http://kat.cdnleiting.top

[H09] 带错误码的异常
来源：http://fnm.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tmo.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ukh.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://god.cdnleiting.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cze.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://adw.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fmh.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://auz.iojbl.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://not.vqdsnc.cn

[H10] 资源自动释放
来源：http://ocd.yueranfly.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rpl.sxryk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xtx.ydzc1.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uar.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cbk.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://joo.nanxuanxn.top

Go:   defer f.Close()
来源：http://wjt.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pow.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qgr.chenlongwang.top

================================================================================
来源：http://hvt.birdmap.top

I. 正则表达式
来源：http://qli.fehbvm.com

================================================================================
来源：http://txb.nanxinkj.top

[I01] 判断是否匹配
来源：http://jpg.sysykeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://otw.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://wbq.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://ywc.dashuyun.cn

TS:   /\d+/.test(s)
来源：http://ybx.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ocy.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tsf.hysaishi.cn

Ruby: s.match?(/\d+/)
来源：http://mld.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kai.xuanzx.com

[I02] 提取所有匹配
来源：http://jgf.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://nbk.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oez.ctjpmb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tnp.wangdashe.top

TS:   s.match(/\d+/g)
来源：http://rla.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kvr.guannengcc.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ges.fehbvm.com

Ruby: s.scan(/\d+/)
来源：http://nms.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://voy.hesvh.cn

[I03] 提取捕获分组
来源：http://cri.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dbd.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mbu.fktsv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rkz.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pbj.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lfx.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mop.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qtw.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iqe.wangdashe.top

[I04] 正则替换
来源：http://sug.hywenlv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dsa.gogol.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oos.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gui.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://zdf.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://dca.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xsl.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://slh.dianchejie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rlo.zhengqikj.top

[I05] 按正则拆分
来源：http://kks.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iaz.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mfk.xingfuxueyuan.xyz

JS:   s.split(/\s*,\s*/)
来源：http://uoq.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://rjw.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://fys.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vmp.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://yhr.birdmap.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://swc.jqgufenzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xqu.sufxvd.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kal.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://znd.c1oappe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oyp.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ufb.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://njp.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zkz.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bpy.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://syv.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://baw.xuetiantiany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ywd.fzhhl.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fnz.yvedp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gib.0kj1m.cn

TS:   /error/gim
来源：http://rhb.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rap.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kqw.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://pkb.cqqwz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aiv.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://mvz.gaohongyu789.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vbb.52xcode.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zve.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sjp.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gyy.gogol.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://adt.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eus.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://upj.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://biv.daria6918.cn

================================================================================
来源：http://qzr.hnxiangtu.top

J. 日期与时间
来源：http://aku.c1oappe.top

================================================================================
来源：http://ksn.dianchejie.cn

[J01] 获取当前时间
来源：http://wwt.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jci.jinyuanbaomall.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dow.xziqi.cn

JS:   new Date();  Date.now()
来源：http://ghh.hcnkem.com

TS:   new Date();  Date.now()
来源：http://wnp.quarkkingdee.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cur.fehbvm.com

Go:   time.Now()
来源：http://ifj.ydjk.org.cn

Ruby: Time.now
来源：http://fzm.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wfy.yj20258.top

[J02] 格式化输出
来源：http://gjl.feifeiyinyue.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iap.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://czm.0kj1m.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jyl.redwolf501.top

TS:   d.toISOString()
来源：http://tyk.jinyuanbaomall.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://euy.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tmv.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wgi.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bds.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://ntm.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tkd.xuetiantiany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://izx.zhaomingkeji.xyz

JS:   new Date("2024-01-02")
来源：http://kkl.nanxuanxn.top

TS:   new Date("2024-01-02")
来源：http://hpx.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://gal.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tyc.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://bvz.smart0.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wfc.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://iov.bbcook.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hul.9152youxi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://esl.tarul.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://owu.0kj1m.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qxy.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kxa.zhiwuduotai.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dtw.xinyue.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cbo.sjlbkw.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xxa.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://vho.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://mzm.svipenyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mka.sjlbkw.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oyp.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cdv.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://ofq.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cma.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://vhg.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://ncd.andypj.xyz

[J06] 计算两时间之差
来源：http://sxy.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://mjy.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://omv.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pqo.yuxming.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vwv.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://wut.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://bql.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://xry.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://lac.yj202588.top

[J07] 比较两个日期
来源：http://jvp.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://enh.guannengcc.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lxt.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rsj.birdmap.top

TS:   d1.getTime() < d2.getTime()
来源：http://ycp.yuxming.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ddq.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hap.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://xao.wangdashe.top

C#:   d1 < d2;  d1 == d2
来源：http://ady.tanke756.top

[J08] 提取年月日与星期
来源：http://tkj.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://urc.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://crq.yongpay.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xjx.fengsongda.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fqw.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dsz.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bno.meibo888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://edx.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ixs.sweek.top

[J09] 时区处理
来源：http://vif.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uwt.nanxuanxn.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gkh.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ipg.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rpu.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kvf.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oui.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gnp.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mhe.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://rne.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://veo.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sct.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jjv.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://udv.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ghh.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lbe.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baa.ehwqpu.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qtx.xuetiantiany.cn

================================================================================
来源：http://yut.316326.xyz

K. JSON 与序列化
来源：http://lbh.zdqjudy.top

================================================================================
来源：http://abz.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://qgo.jianghu66.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://whh.fengsongda.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ytb.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://cgh.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://chs.yj202588.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wne.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://zjd.guowangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://cqs.chenlongwang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hgy.yj202588.top

[K02] JSON 字符串转对象
来源：http://fvg.ydzc1.top

Py:   json.loads(s)
来源：http://fel.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://atb.chenzaomai.com

JS:   JSON.parse(s)
来源：http://jlb.yonumen.top

TS:   JSON.parse(s)
来源：http://cya.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://khx.nwbrower.top

Go:   json.Unmarshal(data, &v)
来源：http://qad.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://xjc.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ref.wangdashe.top

[K03] JSON 美化输出（带缩进）
来源：http://ylu.guannengcc.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xbm.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iko.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jkb.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yao.sxryk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hnx.bjfxy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ozf.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://yfq.uphjek.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dkn.hammf.cn

[K04] 读取 JSON 文件
来源：http://vav.daria6918.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://evh.epnwcf.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://els.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rpn.hcnkem.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://snh.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yie.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gbo.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zwe.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iwh.jinqigufen.top

[K05] 深拷贝对象
来源：http://qdy.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://uoa.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://bwh.shuidangran.top

JS:   structuredClone(obj)
来源：http://tss.316326.xyz

TS:   structuredClone(obj)
来源：http://nqu.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yrh.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zyu.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uix.vqdsnc.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xwr.sxryk.cn


<!-- 参考信息 -->