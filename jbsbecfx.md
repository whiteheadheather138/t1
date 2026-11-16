代发 wailian999

C#:   record User(string Name, int Age);
来源：http://run.yfazqb.com

[G15] 枚举
来源：http://mrt.shanyushiyangtech.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rsi.yj20258888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fbg.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://itz.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pqj.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://tdz.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gdl.uphjek.com

Ruby: Color = %i[red green].freeze
来源：http://qsn.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wui.yj202588.top

[G16] 对象转数组 / 字典
来源：http://uzp.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qtb.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://zve.yuanzhike.top

JS:   Object.entries(obj)
来源：http://aro.yj20258888.top

TS:   Object.entries(obj)
来源：http://ktt.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dtt.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cga.chenjidiqi.icu

Ruby: obj.instance_variables
来源：http://mzg.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://mgc.shanyushiyangtech.top

================================================================================
来源：http://pzv.xinyue.icu

H. 异常与错误处理
来源：http://kng.aibaodan.cn

================================================================================
来源：http://yeq.jqgufenzy.top

[H01] try / catch 基础
来源：http://dbj.zhengqikj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lyx.hesvh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kob.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://klq.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dda.shangyingyoupin.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zlq.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aky.xuetiantiany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mhc.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kmk.hfpthk.cn

[H02] finally / ensure 收尾
来源：http://iws.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://unb.birdmap.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pzi.hysaishi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nqr.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qay.sjlbkw.cn

Java: try { f(); } finally { cleanup(); }
来源：http://efp.0kj1m.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mln.shuidangran.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bba.yonumen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yyp.snrcjt.cn

[H03] 主动抛出异常
来源：http://yjs.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://jcw.hfpthk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xeh.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://kwi.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://vnp.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://use.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://psn.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://yox.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://klh.hysaishi.cn

[H04] 自定义异常类型
来源：http://vlq.zdbjq.cn

Py:   class MyError(Exception): pass
来源：http://mtz.zycfv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pfy.gotoacloud.top

JS:   class MyError extends Error {}
来源：http://fkb.hesvh.cn

TS:   class MyError extends Error {}
来源：http://iiq.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://gru.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bpx.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://hgk.yueranfly.top

C#:   class MyException : Exception {}
来源：http://tzi.yj202588.top

[H05] 捕获特定类型
来源：http://mwe.hywenlv.cn

Py:   except ValueError as e:
来源：http://sdm.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zzk.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://jls.gaohongyu789.top

TS:   if (e instanceof TypeError) {}
来源：http://ano.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://cie.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dqy.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://nha.yfazqb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wvy.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://uik.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://edp.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mfi.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://shd.zhijiandao.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vxl.sxryk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://exs.hnqzz.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ena.nanxuanxn.top

Ruby: d&.dig(:a, :b)
来源：http://qfr.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://clt.guannengcc.top

[H07] 断言
来源：http://dea.jinqigfzy.top

Py:   assert x > 0, "必须为正"
来源：http://fnt.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://flj.gzhubu.top

JS:   console.assert(x > 0);
来源：http://xns.xingfuxueyuan.xyz

TS:   console.assert(x > 0);
来源：http://aiw.ywan-chungtsiang.top

Java: assert x > 0 : "必须为正";
来源：http://rxl.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cpo.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://jzw.fengsongda.top

C#:   Debug.Assert(x > 0);
来源：http://ouc.gotoacloud.top

[H08] 获取错误信息与堆栈
来源：http://fzu.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://ins.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bsq.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://pok.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jtk.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://eyp.jlsjyb.cn

Go:   err.Error()
来源：http://uww.jqgfzy.top

Ruby: e.message;  e.backtrace
来源：http://dcd.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://fhp.jqgfzy.top

[H09] 带错误码的异常
来源：http://ijd.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fnu.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://xce.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hsj.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rru.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vac.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mrx.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://cdm.uphjek.com

C#:   // 自定义异常类中加 Code 属性
来源：http://jxw.epnwcf.com

[H10] 资源自动释放
来源：http://sgl.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tta.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hww.gogol.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mab.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jre.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vlh.fehbvm.com

Go:   defer f.Close()
来源：http://xep.yongpay.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nlh.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://idj.hcnkem.com

================================================================================
来源：http://zyt.chenjidiqi.icu

I. 正则表达式
来源：http://qwt.gotoacloud.top

================================================================================
来源：http://kbi.fehbvm.com

[I01] 判断是否匹配
来源：http://dpm.epnwcf.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hbd.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wow.mhx1999.top

JS:   /\d+/.test(s)
来源：http://gcm.yj202588.top

TS:   /\d+/.test(s)
来源：http://rum.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vsl.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vvz.yj20258888.top

Ruby: s.match?(/\d+/)
来源：http://ypd.dianchejie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cns.shzxlz.cn

[I02] 提取所有匹配
来源：http://bcn.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://rwf.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hqu.jiagoushi.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cfz.tanke756.top

TS:   s.match(/\d+/g)
来源：http://mdn.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jsl.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tqg.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://vaq.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://csu.yuanzhike.top

[I03] 提取捕获分组
来源：http://wbv.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zil.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://svr.pengpengdd.cyou

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://apo.zhoulong.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yfh.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pnw.fzhhl.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nhv.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qtp.yueranfly.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cbl.epnwcf.com

[I04] 正则替换
来源：http://awt.zhengqikj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mll.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jtf.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://htd.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://svh.hongshengwenyu.top

Java: s.replaceAll("\\d+", "#")
来源：http://ren.guowangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qaz.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fdt.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pcx.sysykeji.top

[I05] 按正则拆分
来源：http://ueg.zycfv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://btw.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kos.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://lre.smart0.xyz

TS:   s.split(/\s*,\s*/)
来源：http://bqq.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://yyk.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dwm.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://ttm.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://brh.dianchejie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lgq.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tjw.dashuyun.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gud.yj202588.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kqu.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sdv.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bwa.52xcode.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jiz.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xwn.shzxlz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wut.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://skk.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://waw.pengpengdd.cyou

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lki.meibo888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kku.redwolf501.top

TS:   /error/gim
来源：http://nil.yvedp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://frx.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://emi.ivvv.top

Ruby: s.scan(/error/i)
来源：http://pui.shangyingyoupin.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fco.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://bel.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dts.aizwys.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tmz.yangfankeji.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qch.bbcook.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rqb.sufxvd.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zrz.zhijiandao.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hwp.yfazqb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://krw.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yrn.gaohongyu789.top

================================================================================
来源：http://mak.iojbl.cn

J. 日期与时间
来源：http://gie.tianlin.xyz

================================================================================
来源：http://ewg.zdbjq.cn

[J01] 获取当前时间
来源：http://fru.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://upv.sxryk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qzb.hcnkem.com

JS:   new Date();  Date.now()
来源：http://cps.yvedp.cn

TS:   new Date();  Date.now()
来源：http://mts.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://wgp.hnqzz.top

Go:   time.Now()
来源：http://hmx.ydzc1.top

Ruby: Time.now
来源：http://ccp.cqqwz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hsx.nanxuanxn.top

[J02] 格式化输出
来源：http://qmz.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cse.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xwr.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ffu.jqgufenzy.top

TS:   d.toISOString()
来源：http://imx.nanxinkj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jbu.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lcg.fengsongda.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nit.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dmm.jqgufenzy.top

[J03] 字符串解析为日期
来源：http://fnj.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hpa.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dhh.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://aex.ivvv.top

TS:   new Date("2024-01-02")
来源：http://nxt.jinyuanbaomall.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tlc.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pgh.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://qwc.yonumen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uwk.smart0.xyz

[J04] 时间戳与日期互转
来源：http://pcg.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lzz.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gll.hysaishi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jra.hnxiangtu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://rzx.tian-w.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dfu.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qvn.bbcook.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://guh.vqdsnc.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rpm.jinqigufen.top

[J05] 时间加减（加 7 天）
来源：http://wbg.tanke756.top

Py:   now + timedelta(days=7)
来源：http://wpc.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aue.yj20258888.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zrh.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gcg.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://hwd.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://czb.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://fbj.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://utk.jinghuilouyu.cn

[J06] 计算两时间之差
来源：http://xtc.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://qxy.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://slg.yonumen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xex.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qbe.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://spk.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://nea.jinqigfzy.top

Ruby: end - start                 # 返回秒数
来源：http://jsv.wangshuangyany.cn

C#:   (end - start).TotalSeconds
来源：http://rai.andypj.xyz

[J07] 比较两个日期
来源：http://lyv.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://jgg.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://por.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://euh.gogol.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ktn.hysaishi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mnw.jianghu66.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nap.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://eyj.vqdsnc.cn

C#:   d1 < d2;  d1 == d2
来源：http://lmn.tarul.cn

[J08] 提取年月日与星期
来源：http://mys.ywan-chungtsiang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://myg.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jim.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qmz.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uvg.tian-w.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mce.xingfuxueyuan.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aka.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kst.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vtc.cashguo.top

[J09] 时区处理
来源：http://exo.wangshuangyany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fke.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vzl.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://reo.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zbo.pengpengdd.cyou

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yjq.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://myr.ehwqpu.com

Ruby: Time.now.getlocal("+08:00")
来源：http://nlx.snrcjt.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jrv.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://xfz.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://sfp.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gjg.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vfv.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kef.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mzk.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mfv.zhijiandao.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ftw.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uwj.jinqigufen.top

================================================================================
来源：http://xxh.dashuyun.cn

K. JSON 与序列化
来源：http://ilt.xuetiantiany.cn

================================================================================
来源：http://sov.pengpengdd.cyou

[K01] 对象转 JSON 字符串
来源：http://njp.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zoe.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qqs.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://ulh.snrcjt.cn

TS:   JSON.stringify(obj)
来源：http://upw.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cak.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://mlg.316326.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://pme.shuidangran.top

C#:   JsonSerializer.Serialize(obj)
来源：http://akf.sysykeji.top

[K02] JSON 字符串转对象
来源：http://ntz.epnwcf.com

Py:   json.loads(s)
来源：http://eev.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pjo.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://gsj.hcnkem.com

TS:   JSON.parse(s)
来源：http://wdh.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oaz.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://pmu.yongpay.top

Ruby: JSON.parse(s)
来源：http://abn.nanxuanxn.top


<!-- 参考信息 -->