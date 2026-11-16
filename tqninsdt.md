代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qnf.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bmr.zhengqikj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mcd.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nnx.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vdo.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fri.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cxj.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://eao.pycfn.com

Py:   try: f()⏎finally: cleanup()
来源：http://unn.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://zrd.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ixz.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yks.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ztf.yfazqb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://upf.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://upw.zdbjq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ybl.yongpay.top

[H03] 主动抛出异常
来源：http://xyk.vqdsnc.cn

Py:   raise ValueError("错误信息")
来源：http://msc.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://psi.fengsongda.top

JS:   throw new Error("错误信息");
来源：http://unl.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://wfr.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://obm.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ihd.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nrk.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wih.xinyue.icu

[H04] 自定义异常类型
来源：http://chk.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://nnn.nanxuanxn.top

PHP:  class MyError extends RuntimeException {}
来源：http://kql.sysykeji.top

JS:   class MyError extends Error {}
来源：http://rgz.chenzaomai.com

TS:   class MyError extends Error {}
来源：http://ehm.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://utj.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://apb.havefunace.top

Ruby: class MyError < StandardError; end
来源：http://xkm.pengpengdd.cyou

C#:   class MyException : Exception {}
来源：http://osy.tarul.cn

[H05] 捕获特定类型
来源：http://tpa.yongpay.top

Py:   except ValueError as e:
来源：http://gpx.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lls.ybcxt.top

JS:   if (e instanceof TypeError) {}
来源：http://qeu.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://kid.shanyushiyangtech.top

Java: catch (IOException | SQLException e) {}
来源：http://nxo.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://por.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://lpy.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iir.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://psg.fehbvm.com

Py:   value = d.get("k") or default
来源：http://mot.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://cqn.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://djy.jqgufenzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://olk.jinyuanbaomall.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ghy.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gdp.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://qno.hfpthk.cn

C#:   obj?.A?.B ?? default
来源：http://szx.tianlin.xyz

[H07] 断言
来源：http://cmr.dianchejie.cn

Py:   assert x > 0, "必须为正"
来源：http://fcr.yanxiufei.cn

PHP:  assert($x > 0);
来源：http://evj.0kj1m.cn

JS:   console.assert(x > 0);
来源：http://ukx.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://unu.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://gdp.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://upy.mhx1999.top

Ruby: raise "必须为正" unless x > 0
来源：http://ssk.yj20258.top

C#:   Debug.Assert(x > 0);
来源：http://cvo.cqqwz.cn

[H08] 获取错误信息与堆栈
来源：http://qli.smart0.xyz

Py:   str(e);  traceback.format_exc()
来源：http://hjh.ivvv.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kgb.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://ojt.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dkj.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cxg.yuxming.cn

Go:   err.Error()
来源：http://qnw.pycfn.com

Ruby: e.message;  e.backtrace
来源：http://nmg.jyoumei.cn

C#:   e.Message;  e.StackTrace
来源：http://ave.jyoumei.cn

[H09] 带错误码的异常
来源：http://wtb.yangfankeji.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mpu.fanxiaobao.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://blh.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oqg.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kxv.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pjs.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://big.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kdc.daxiang520.top

C#:   // 自定义异常类中加 Code 属性
来源：http://sim.c1oappe.top

[H10] 资源自动释放
来源：http://bul.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://irk.pengpengdd.cyou

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nhl.jinyuanbaomall.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cvw.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://puc.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bfz.sweek.top

Go:   defer f.Close()
来源：http://jzs.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oan.hongshengwenyu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://suh.gotoacloud.top

================================================================================
来源：http://adt.xuetiantiany.cn

I. 正则表达式
来源：http://mgy.cdnleiting.top

================================================================================
来源：http://ynp.hysaishi.cn

[I01] 判断是否匹配
来源：http://avp.sysykeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jqf.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://uai.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://inx.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://acv.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://drh.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ono.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://yeh.smart0.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nkf.cqqwz.cn

[I02] 提取所有匹配
来源：http://nmp.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://hhm.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iic.9152youxi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hhq.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://ogp.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zio.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ljy.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://siv.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lmr.kuanghao11.cn

[I03] 提取捕获分组
来源：http://cuv.iojbl.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://icm.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://soi.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ztl.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qec.c1oappe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ziw.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dpj.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gxx.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kuk.shuidangran.top

[I04] 正则替换
来源：http://fxw.aizwys.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cbj.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://roy.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://tvw.hysaishi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dwo.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://uqr.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://igf.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://idd.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nuq.shzxlz.cn

[I05] 按正则拆分
来源：http://wvx.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kma.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lny.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://squ.hcnkem.com

TS:   s.split(/\s*,\s*/)
来源：http://jam.jqgfzy.top

Java: s.split("\\s*,\\s*")
来源：http://ylw.redwolf501.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xss.uphjek.com

Ruby: s.split(/\s*,\s*/)
来源：http://cur.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://drc.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oxk.yj20258.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://duu.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eym.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://twj.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://seu.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pue.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vsl.uphjek.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yky.gaohongyu789.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nqw.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://wsv.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jsp.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qjh.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fcb.andypj.xyz

TS:   /error/gim
来源：http://sff.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dkw.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nqd.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://pbo.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xyb.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://szv.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ers.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mfq.0kj1m.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ovc.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kuy.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://xxw.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nqs.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iui.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://czq.shanyushiyangkeji.top

================================================================================
来源：http://ute.guowangkeji.top

J. 日期与时间
来源：http://mcv.yuxming.cn

================================================================================
来源：http://sbk.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://jvh.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hly.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ize.c1oappe.top

JS:   new Date();  Date.now()
来源：http://qra.dashuyun.cn

TS:   new Date();  Date.now()
来源：http://vom.shanyushiyangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zuz.nanxuanxn.top

Go:   time.Now()
来源：http://tuu.hcnkem.com

Ruby: Time.now
来源：http://npv.chenlongwang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lrn.xylfe.cn

[J02] 格式化输出
来源：http://gae.jiagoushi.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nky.tanke756.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://itf.9152youxi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://brp.hfpthk.cn

TS:   d.toISOString()
来源：http://wbo.zdqjudy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wzd.yueranfly.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pol.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pdg.nwbrower.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://shk.tianlin.xyz

[J03] 字符串解析为日期
来源：http://bih.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xss.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xdd.epnwcf.com

JS:   new Date("2024-01-02")
来源：http://flf.pycfn.com

TS:   new Date("2024-01-02")
来源：http://hom.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sip.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qip.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://lge.xinyue.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://awb.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://cdg.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uer.shuidangran.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://awi.birdmap.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xvw.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qyq.cdnleiting.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://siu.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zue.cashguo.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mhg.nwbrower.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gbw.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://bsa.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://uxg.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://flp.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yac.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tmj.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://ktn.dianchejie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qsu.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://oni.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://glw.gaohongyu789.top

[J06] 计算两时间之差
来源：http://pbw.9152youxi.cn

Py:   (end - start).total_seconds()
来源：http://zms.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://lxa.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ygb.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tdv.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://mgt.pengpengdd.cyou

Go:   end.Sub(start).Hours()
来源：http://zob.xziqi.cn

Ruby: end - start                 # 返回秒数
来源：http://gfx.yuxming.cn

C#:   (end - start).TotalSeconds
来源：http://xvy.quarkkingdee.top

[J07] 比较两个日期
来源：http://gwn.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://ckk.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sgg.zhaomingkeji.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://fcy.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://jps.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lgx.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cbb.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zaz.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://csz.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://buq.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tuv.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ztd.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dhk.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xhs.cheryme.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ajl.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fzw.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pkp.c1oappe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://daw.yonumen.top

[J09] 时区处理
来源：http://hqq.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wii.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zio.daria6918.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sbr.pycfn.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fix.daria6918.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zdf.chenzaomai.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uzm.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lml.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hqv.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://qwr.hcnkem.com

Py:   date.today();  date.today().replace(day=1)
来源：http://uzw.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kvl.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zgo.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://csg.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://csv.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mjf.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://znr.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qpc.jlsjyb.cn

================================================================================
来源：http://vzv.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://jtr.yueranfly.top

================================================================================
来源：http://kyw.sweek.top

[K01] 对象转 JSON 字符串
来源：http://spe.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jsf.fengsongda.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kzw.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://miv.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://fpn.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hqc.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://ehu.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://sle.smart0.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://ltk.nanxuanxn.top

[K02] JSON 字符串转对象
来源：http://tqm.zdqjudy.top

Py:   json.loads(s)
来源：http://kcu.jinqigufen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xkr.jinyuanbaomall.cn

JS:   JSON.parse(s)
来源：http://lki.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://ahx.pengpengdd.cyou

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yjc.fzhhl.top

Go:   json.Unmarshal(data, &v)
来源：http://vhz.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://hvz.tarul.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gpt.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://bxz.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pwa.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lwg.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://col.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://kba.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vkx.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dyp.ybcxt.top

Ruby: JSON.pretty_generate(obj)
来源：http://jyf.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oyz.vqdsnc.cn

[K04] 读取 JSON 文件
来源：http://uxs.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ydx.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uqz.shangyingyoupin.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://exs.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bmp.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yci.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wop.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://wjj.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qfs.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://ycp.pengpengdd.cyou

Py:   copy.deepcopy(obj)
来源：http://yov.hywenlv.cn

PHP:  unserialize(serialize($obj));
来源：http://qxt.jiagoushi.top

JS:   structuredClone(obj)
来源：http://ggc.xinyue.icu

TS:   structuredClone(obj)
来源：http://ijj.chenjidiqi.icu


<!-- 参考信息 -->