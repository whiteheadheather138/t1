代发 wailian999

C#:   record User(string Name, int Age);
来源：http://vob.cdnleiting.top

[G15] 枚举
来源：http://eah.tanke756.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mwn.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zdp.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yti.iojbl.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mjg.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://dbe.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yje.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://ijw.birdmap.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ubm.yueranfly.top

[G16] 对象转数组 / 字典
来源：http://wha.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zsa.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://hmf.havefunace.top

JS:   Object.entries(obj)
来源：http://mkg.yvedp.cn

TS:   Object.entries(obj)
来源：http://ebs.ydzc1.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://awu.jianghu66.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cay.xziqi.cn

Ruby: obj.instance_variables
来源：http://zbz.iojbl.cn

C#:   // 用反射或 System.Text.Json
来源：http://fxy.jinyuanbaomall.cn

================================================================================
来源：http://yjt.aizwys.cn

H. 异常与错误处理
来源：http://rej.snrcjt.cn

================================================================================
来源：http://qom.yfazqb.com

[H01] try / catch 基础
来源：http://mee.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://otw.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gjb.yonumen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vdi.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vbs.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kue.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://shz.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://suc.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://boo.jyoumei.cn

[H02] finally / ensure 收尾
来源：http://xqq.jiagoushi.top

Py:   try: f()⏎finally: cleanup()
来源：http://cdw.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ung.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hsc.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://diy.redwolf501.top

Java: try { f(); } finally { cleanup(); }
来源：http://poy.fehbvm.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://eah.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kwt.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lna.yuanzhike.top

[H03] 主动抛出异常
来源：http://lbu.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://kkb.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uda.sysykeji.top

JS:   throw new Error("错误信息");
来源：http://zvq.xinyue.icu

TS:   throw new Error("错误信息");
来源：http://zqt.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://brw.sweek.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bpd.gzhubu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ppj.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://grg.birdmap.top

[H04] 自定义异常类型
来源：http://yay.iojbl.cn

Py:   class MyError(Exception): pass
来源：http://wid.yueranfly.top

PHP:  class MyError extends RuntimeException {}
来源：http://fje.c1oappe.top

JS:   class MyError extends Error {}
来源：http://qpb.hysaishi.cn

TS:   class MyError extends Error {}
来源：http://rth.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://fci.havefunace.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://llh.gaohongyu789.top

Ruby: class MyError < StandardError; end
来源：http://vtc.xylfe.cn

C#:   class MyException : Exception {}
来源：http://llg.jqgfzy.top

[H05] 捕获特定类型
来源：http://pni.kuanghao11.cn

Py:   except ValueError as e:
来源：http://tmz.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qfz.wangdashe.top

JS:   if (e instanceof TypeError) {}
来源：http://zjw.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://gxq.ehwqpu.com

Java: catch (IOException | SQLException e) {}
来源：http://gbz.sufxvd.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xmv.ppjwa.cn

Ruby: rescue ArgumentError => e
来源：http://ckw.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dnw.nwbrower.top

[H06] 可选值 / 空值安全访问
来源：http://gsr.nanxinkj.top

Py:   value = d.get("k") or default
来源：http://wya.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lma.hnqzz.top

JS:   obj?.a?.b;  d ?? default
来源：http://rno.jinghuilouyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ydd.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ytd.daxiang520.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bxa.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://fhr.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://awx.jlsjyb.cn

[H07] 断言
来源：http://iul.gogol.net.cn

Py:   assert x > 0, "必须为正"
来源：http://hog.bbcook.cn

PHP:  assert($x > 0);
来源：http://oki.xylfe.cn

JS:   console.assert(x > 0);
来源：http://siy.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://abs.0kj1m.cn

Java: assert x > 0 : "必须为正";
来源：http://bxy.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gfn.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qno.jinqigfzy.top

C#:   Debug.Assert(x > 0);
来源：http://uej.hysaishi.cn

[H08] 获取错误信息与堆栈
来源：http://yqx.ydzc1.top

Py:   str(e);  traceback.format_exc()
来源：http://rfj.kuanghao11.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fhh.fzhhl.top

JS:   e.message;  e.stack
来源：http://ukf.havefunace.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tgm.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ybb.tanke756.top

Go:   err.Error()
来源：http://uit.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://jtm.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://eaq.nwbrower.top

[H09] 带错误码的异常
来源：http://jgf.jqgufenzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://enl.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xim.chenzaomai.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://szz.aizwys.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vbj.jianghu66.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gdl.ivvv.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fpr.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://dsi.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://gdk.sjlbkw.cn

[H10] 资源自动释放
来源：http://gjq.yongpay.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://chx.ehwqpu.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zfj.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://llh.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qsv.jyoumei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://asu.birdmap.top

Go:   defer f.Close()
来源：http://mam.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ylv.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dwq.feifeiyinyue.top

================================================================================
来源：http://tdb.birdmap.top

I. 正则表达式
来源：http://wyg.yj20258888.top

================================================================================
来源：http://jgv.havefunace.top

[I01] 判断是否匹配
来源：http://kqp.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wje.ivvv.top

PHP:  preg_match('/\d+/', $s);
来源：http://srx.zhaomingkeji.xyz

JS:   /\d+/.test(s)
来源：http://twn.epnwcf.com

TS:   /\d+/.test(s)
来源：http://wnm.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jma.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uxk.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://lzp.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tmx.nanxinkj.top

[I02] 提取所有匹配
来源：http://xlw.sweek.top

Py:   re.findall(r"\d+", s)
来源：http://fkh.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jst.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lzr.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://jpv.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://slp.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ohc.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://buf.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nqa.guowangkeji.top

[I03] 提取捕获分组
来源：http://lui.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rft.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ooo.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tfr.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rxf.bbcook.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wdx.havefunace.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dwo.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mbl.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vgm.jianghu66.top

[I04] 正则替换
来源：http://pfg.chenlongwang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qnz.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qqy.svipenyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zow.havefunace.top

TS:   s.replace(/\d+/g, "#")
来源：http://jrr.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rhr.yuanzhike.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lkd.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ixo.gzhubu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hib.gzhubu.top

[I05] 按正则拆分
来源：http://ehm.ivvv.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nrx.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mfx.yanxiufei.cn

JS:   s.split(/\s*,\s*/)
来源：http://cqc.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://vhs.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://mtf.yj20258888.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ebq.hfpthk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ylm.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xtj.svipenyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vhx.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rcl.daxiang520.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hby.uphjek.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lea.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kek.sysykeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ory.cqqwz.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ncj.shuidangran.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pqh.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://udy.yj20258.top

[I07] 忽略大小写与多行模式
来源：http://tel.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jdu.dianchejie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wuo.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zed.fzhhl.top

TS:   /error/gim
来源：http://oru.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zhm.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wwu.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://qqu.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uyg.shanyushiyangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://lek.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kpc.hnxiangtu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://awm.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lds.chenjidiqi.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oez.chenlongwang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zpl.yuxming.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pmq.yuanzhike.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bnd.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ueh.aibaodan.cn

================================================================================
来源：http://ymd.sjlbkw.cn

J. 日期与时间
来源：http://eyl.tian-w.cn

================================================================================
来源：http://gzg.andypj.xyz

[J01] 获取当前时间
来源：http://lfh.jinghuilouyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pgt.zhiwuduotai.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xad.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://xxa.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://eoy.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mjh.dianchejie.cn

Go:   time.Now()
来源：http://rer.sysykeji.top

Ruby: Time.now
来源：http://uac.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fxl.xinyue.icu

[J02] 格式化输出
来源：http://oqu.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://azt.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://idj.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iba.svipenyu.cn

TS:   d.toISOString()
来源：http://jaq.zycfv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://amm.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ytt.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aqw.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qzi.sysykeji.top

[J03] 字符串解析为日期
来源：http://ari.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mqa.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sjs.cashguo.top

JS:   new Date("2024-01-02")
来源：http://azk.jlsjyb.cn

TS:   new Date("2024-01-02")
来源：http://aok.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://mfl.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dul.ybcxt.top

Ruby: Date.parse("2024-01-02")
来源：http://isr.zhiwuduotai.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sgp.cucudq.cn

[J04] 时间戳与日期互转
来源：http://bcz.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yks.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mzl.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tph.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sah.xziqi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ulr.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yky.zhongyouzk.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://opq.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ogf.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://rpv.nanxuanxn.top

Py:   now + timedelta(days=7)
来源：http://new.fzhhl.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kfj.tianlin.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://shj.hammf.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lhp.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://epk.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hsm.pengpengdd.cyou

Ruby: Time.now + 7 * 86400
来源：http://owi.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://vjl.chenzaomai.com

[J06] 计算两时间之差
来源：http://xdv.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://ryt.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://rgl.yj20258888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wmd.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gip.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://srz.wangdashe.top

Go:   end.Sub(start).Hours()
来源：http://ytr.vqdsnc.cn

Ruby: end - start                 # 返回秒数
来源：http://yms.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://bhy.chenjidiqi.icu

[J07] 比较两个日期
来源：http://jfm.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://rxe.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fck.fktsv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kdu.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://xfs.fengsongda.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fke.vqdsnc.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kvn.zycfv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ahy.ybcxt.top

C#:   d1 < d2;  d1 == d2
来源：http://fwf.yongpay.top

[J08] 提取年月日与星期
来源：http://qad.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pof.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xih.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mfl.tian-w.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mem.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hjn.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://axc.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ncw.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xrq.shuidangran.top

[J09] 时区处理
来源：http://hkl.guannengcc.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uam.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://drq.vehdjk.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tjx.xingfuxueyuan.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zvs.guannengcc.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vkw.hcnkem.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://myx.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fev.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jdl.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://fdf.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rts.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gdv.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mrz.nanxuanxn.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oes.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wsn.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zqo.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vwz.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wmy.xuetiantiany.cn

================================================================================
来源：http://gmp.ydzc1.top

K. JSON 与序列化
来源：http://pmz.fehbvm.com

================================================================================
来源：http://qfn.gzhubu.top

[K01] 对象转 JSON 字符串
来源：http://urq.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pyy.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hxu.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://ohi.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://tmq.daxiang520.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ocb.xinyue.icu

Go:   json.Marshal(obj)
来源：http://vdu.yuxming.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mqp.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sjm.havefunace.top

[K02] JSON 字符串转对象
来源：http://sci.hywenlv.cn

Py:   json.loads(s)
来源：http://ree.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lua.ybcxt.top

JS:   JSON.parse(s)
来源：http://nti.hnqzz.top

TS:   JSON.parse(s)
来源：http://gqr.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fzu.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://fvq.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://kvb.sxryk.cn


<!-- 参考信息 -->