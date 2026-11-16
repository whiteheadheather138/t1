代发 wailian999

Py:   isinstance(u, User)
来源：http://lvz.fzhhl.top

PHP:  $u instanceof User
来源：http://bkh.meibo888.top

JS:   u instanceof User
来源：http://yuz.gzhubu.top

TS:   u instanceof User
来源：http://ypx.fanxiaobao.xyz

Java: u instanceof User
来源：http://otf.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rox.fengsongda.top

Ruby: u.is_a?(User)
来源：http://vgo.guowangkeji.top

C#:   u is User
来源：http://dnz.tanke756.top

[G14] 数据类 / record
来源：http://jwx.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://waj.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://pny.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mai.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://wxi.havefunace.top

Java: record User(String name, int age) {}
来源：http://apf.zdqjudy.top

Go:   type User struct { Name string; Age int }
来源：http://nma.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ejk.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://ono.jqgfzy.top

[G15] 枚举
来源：http://hgt.snrcjt.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sjd.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lpg.feifeiyinyue.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gpm.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qag.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://los.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ujx.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://oxv.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wkq.jinqigfzy.top

[G16] 对象转数组 / 字典
来源：http://cfi.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://orj.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://cxq.yfazqb.com

JS:   Object.entries(obj)
来源：http://cnz.ehwqpu.com

TS:   Object.entries(obj)
来源：http://fmz.0kj1m.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lgf.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nfj.shuidangran.top

Ruby: obj.instance_variables
来源：http://kaa.hongshengwenyu.top

C#:   // 用反射或 System.Text.Json
来源：http://bhx.ybcxt.top

================================================================================
来源：http://lvq.ydjk.org.cn

H. 异常与错误处理
来源：http://ozo.nanxinkj.top

================================================================================
来源：http://riz.zdqjudy.top

[H01] try / catch 基础
来源：http://hgr.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://evl.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://msv.yuanzhike.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://waq.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nnd.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ksj.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dua.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ged.chenjidiqi.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tfk.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://svc.xziqi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ysq.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tbm.316326.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://dgv.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rpg.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://amv.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qhr.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://set.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qzl.jlsjyb.cn

[H03] 主动抛出异常
来源：http://jme.iojbl.cn

Py:   raise ValueError("错误信息")
来源：http://ice.shanyushiyangtech.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xer.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://lqb.chenlongwang.top

TS:   throw new Error("错误信息");
来源：http://onq.52xcode.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kxf.haohaochexian.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jtd.xuetiantiany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bxk.uphjek.com

C#:   throw new ArgumentException("错误信息");
来源：http://gih.fengsongda.top

[H04] 自定义异常类型
来源：http://pnt.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://okm.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://fco.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://fhj.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://kyw.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://hde.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ear.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://rnt.sweek.top

C#:   class MyException : Exception {}
来源：http://sil.sysykeji.top

[H05] 捕获特定类型
来源：http://wtu.iojbl.cn

Py:   except ValueError as e:
来源：http://pox.dashuyun.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dky.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://dsj.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://iew.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://svx.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iai.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://gpb.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mbb.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://hfh.zdqjudy.top

Py:   value = d.get("k") or default
来源：http://jud.yj202588.top

PHP:  $v = $d["k"] ?? null;
来源：http://pcx.xuetiantiany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://reu.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hkk.shzxlz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wwd.zycfv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lfz.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://pcy.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://fke.birdmap.top

[H07] 断言
来源：http://ecn.shuidangran.top

Py:   assert x > 0, "必须为正"
来源：http://pmc.meibo888.top

PHP:  assert($x > 0);
来源：http://prz.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://ufd.yfazqb.com

TS:   console.assert(x > 0);
来源：http://mxa.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://uzb.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ady.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lzk.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://znv.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://jte.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://yit.fzhhl.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://taa.smart0.xyz

JS:   e.message;  e.stack
来源：http://hox.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://abo.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yng.xylfe.cn

Go:   err.Error()
来源：http://jgd.andypj.xyz

Ruby: e.message;  e.backtrace
来源：http://ynt.sxryk.cn

C#:   e.Message;  e.StackTrace
来源：http://bns.xziqi.cn

[H09] 带错误码的异常
来源：http://tcs.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vdo.bbcook.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://blk.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ruv.ivvv.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lvp.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ett.daria6918.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uvm.yuanzhike.top

Ruby: raise MyError.new("fail", 500)
来源：http://nhx.ivvv.top

C#:   // 自定义异常类中加 Code 属性
来源：http://etu.dashuyun.cn

[H10] 资源自动释放
来源：http://kqk.shanyushiyangtech.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://egd.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jju.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tuy.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ott.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fhi.havefunace.top

Go:   defer f.Close()
来源：http://qgd.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ide.bbcook.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pbz.hywenlv.cn

================================================================================
来源：http://hor.chenlongwang.top

I. 正则表达式
来源：http://ayx.fktsv.cn

================================================================================
来源：http://dcd.hcnkem.com

[I01] 判断是否匹配
来源：http://uym.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rcx.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://uqo.xziqi.cn

JS:   /\d+/.test(s)
来源：http://yes.yonumen.top

TS:   /\d+/.test(s)
来源：http://sen.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fqr.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ldj.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://agl.zhaomingkeji.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fee.ybcxt.top

[I02] 提取所有匹配
来源：http://eos.jqgfzy.top

Py:   re.findall(r"\d+", s)
来源：http://mlg.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kmz.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://djx.nanxuanxn.top

TS:   s.match(/\d+/g)
来源：http://ybe.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ggo.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yqi.hongshengwenyu.top

Ruby: s.scan(/\d+/)
来源：http://qso.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kqx.nwbrower.top

[I03] 提取捕获分组
来源：http://pqx.ydzc1.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bfo.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ixf.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rbu.cheryme.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sjk.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vgg.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fnc.svipenyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://der.svipenyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oco.hcnkem.com

[I04] 正则替换
来源：http://jfz.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ckg.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cqz.c1oappe.top

JS:   s.replace(/\d+/g, "#")
来源：http://wjt.shzxlz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hqq.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://ses.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rpt.hnqzz.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qdn.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://njo.jiagoushi.top

[I05] 按正则拆分
来源：http://uiz.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zbp.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lst.gotoacloud.top

JS:   s.split(/\s*,\s*/)
来源：http://cem.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://nnb.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://kzd.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fkh.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://gwa.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bzj.tianlin.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vdl.fanxiaobao.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vfa.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vfb.zhixingplan.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aci.vehdjk.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dka.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ier.shanyushiyangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dqb.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bgq.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://por.c1oappe.top

[I07] 忽略大小写与多行模式
来源：http://vmw.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qve.jinqigfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sub.jlsjyb.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aog.jinghuilouyu.cn

TS:   /error/gim
来源：http://rxq.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ary.hcnkem.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://doh.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://veu.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://stu.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://tac.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://upb.epnwcf.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fsu.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vem.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://urt.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://iai.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ywp.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yto.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://krn.yj20258.top

================================================================================
来源：http://vpt.epnwcf.com

J. 日期与时间
来源：http://ogf.ybcxt.top

================================================================================
来源：http://jgt.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://xbo.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uoo.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lso.sysykeji.top

JS:   new Date();  Date.now()
来源：http://ozc.tarul.cn

TS:   new Date();  Date.now()
来源：http://qah.nanxinkj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gau.cdnleiting.top

Go:   time.Now()
来源：http://hcw.redwolf501.top

Ruby: Time.now
来源：http://gtt.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xft.jiagoushi.top

[J02] 格式化输出
来源：http://oko.hammf.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lav.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jmo.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rwf.ybcxt.top

TS:   d.toISOString()
来源：http://uzr.cqqwz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qxb.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rkk.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xyv.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tco.guannengcc.top

[J03] 字符串解析为日期
来源：http://fct.yfazqb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://reh.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wah.mhx1999.top

JS:   new Date("2024-01-02")
来源：http://xqn.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://avp.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://fpf.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dxe.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://cmi.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://etc.fzhhl.top

[J04] 时间戳与日期互转
来源：http://gmu.tian-w.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ruq.guannengcc.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bfk.gzhubu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://agv.guannengcc.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kfy.shanyushiyangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uhz.tian-w.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gzq.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bnp.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vlp.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://fts.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://ich.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://box.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zbh.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mzq.gzhubu.top

Java: LocalDate.now().plusDays(7)
来源：http://nku.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tzf.yuxming.cn

Ruby: Time.now + 7 * 86400
来源：http://ksj.zhiwuduotai.top

C#:   DateTime.Now.AddDays(7)
来源：http://jiu.sysykeji.top

[J06] 计算两时间之差
来源：http://hcd.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://tog.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://lak.shanyushiyangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://got.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://coi.zycfv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jyo.zdbjq.cn

Go:   end.Sub(start).Hours()
来源：http://jty.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://mii.daria6918.cn

C#:   (end - start).TotalSeconds
来源：http://cib.ehwqpu.com

[J07] 比较两个日期
来源：http://uej.xuetiantiany.cn

Py:   d1 < d2;  d1 == d2
来源：http://stw.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nvs.wangdashe.top

JS:   d1.getTime() < d2.getTime()
来源：http://cjt.zhongyouzk.top

TS:   d1.getTime() < d2.getTime()
来源：http://naa.yangfankeji.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://plb.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://abw.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://blb.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://sao.daxiang520.top

[J08] 提取年月日与星期
来源：http://epr.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jjw.yvedp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vqf.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lrf.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nhv.hongshengwenyu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mat.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ksz.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://imv.fehbvm.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://klj.aibaodan.cn

[J09] 时区处理
来源：http://moy.cucudq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nat.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://acv.jinghuilouyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mkq.xinyue.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yeo.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dbf.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ezd.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mwp.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nun.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://mue.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://odk.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://piw.chenlongwang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bcx.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mmk.jyoumei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sho.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://geg.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hhd.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jpy.vqdsnc.cn

================================================================================
来源：http://lrm.cdnleiting.top

K. JSON 与序列化
来源：http://szb.9152youxi.cn

================================================================================
来源：http://smg.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://raq.cqqwz.cn


<!-- 参考信息 -->