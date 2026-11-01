代发 wailian999

C#:   public / protected / private / internal
来源：http://www.m.share.fktsv.cn/Article/details/gaqpszhyf.sHtML

[G11] getter / setter
来源：http://www.blog.sjlbkw.cn/Article/details/gfmwpwxnz.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.sjlbkw.cn/Article/details/gcvjwxxxq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/ggckpekev.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gpqeqawhe.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gljwwnjoi.sHtML

Java: public String getName() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gihsypbvc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gwqhmbaio.sHtML

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/grazeavpl.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.yfazqb.com/Article/details/gdgmjjrpd.sHtML

[G12] 对象转字符串
来源：http://mobile.vehdjk.com/Article/details/gtocfjanm.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gecehlkgq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gdeuepqsc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gpogpxjyg.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gbmpnqmyj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpllftkow.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/ghehauxvc.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/grnzaxcsu.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.epnwcf.com/Article/details/ghwayjlfv.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/gwmtrycnx.sHtML

Py:   isinstance(u, User)
来源：http://3g.bbcook.cn/Article/details/gjlcemsnp.sHtML

PHP:  $u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gghuwisjh.sHtML

JS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/ghvujqamd.sHtML

TS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gwqgbcirr.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/glalaziln.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.vehdjk.com/Article/details/gddtnyukk.sHtML

Ruby: u.is_a?(User)
来源：http://baike.epnwcf.com/Article/details/gqwkixbvw.sHtML

C#:   u is User
来源：http://blog.bbcook.cn/Article/details/gqyydzafm.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/gxgxugvca.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.sjlbkw.cn/Article/details/grggghfbs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gobiupocu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fktsv.cn/Article/details/gnszzkifi.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.tarul.cn/Article/details/gbymsykaa.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.epnwcf.com/Article/details/gtpokjyns.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gcbjzsurc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.bbcook.cn/Article/details/gsvyzceng.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.vehdjk.com/Article/details/gtdicksug.sHtML

[G15] 枚举
来源：http://3g.tarul.cn/Article/details/gopfrhavj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/gjnffdygz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fktsv.cn/Article/details/gniltvkjr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.bbcook.cn/Article/details/gqdtnuknz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gthmuxwai.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.yfazqb.com/Article/details/gzaabzymp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.epnwcf.com/Article/details/gywdbmsbt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.yfazqb.com/Article/details/gekovewte.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/ghpuddogb.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.sjlbkw.cn/Article/details/gozuvqvfh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.vehdjk.com/Article/details/gfhzilhoz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.epnwcf.com/Article/details/gzgevjccw.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/glvbknffm.sHtML

TS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gymcxzgaz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gydzeeiqu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.bbcook.cn/Article/details/gjvzghfwp.sHtML

Ruby: obj.instance_variables
来源：http://blog.bbcook.cn/Article/details/gndyqtodn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.sjlbkw.cn/Article/details/gqpnvcxnl.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvxybings.sHtML

H. 异常与错误处理
来源：http://baike.tarul.cn/Article/details/glmefncqn.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqqxylwbg.sHtML

[H01] try / catch 基础
来源：http://www.share.fktsv.cn/Article/details/glewhrkmw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.bbcook.cn/Article/details/galcqvahh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gjasrcizv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gfjyrvsrq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/giskmmemu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.vehdjk.com/Article/details/gotgjjmqo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.tarul.cn/Article/details/gobufzyal.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/gowneeeie.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.tarul.cn/Article/details/gstofkijq.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.yfazqb.com/Article/details/gdlpqpcaz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fktsv.cn/Article/details/goeptglqx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gfoadjqgi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gmacyjrcc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/grqtwfkow.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gvbkbccey.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/gojkjxmwv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.sjlbkw.cn/Article/details/gboluidtw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.tarul.cn/Article/details/gyqoqomni.sHtML

[H03] 主动抛出异常
来源：http://baike.tarul.cn/Article/details/gdktlomes.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.epnwcf.com/Article/details/gkrkrbjwh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gfujnmars.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gpfoiyqnz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gucemvast.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/ghzcugyxq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/grevwjwrm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.sjlbkw.cn/Article/details/gvtcuwefx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gjwovxmea.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/gvcgwtltp.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.vehdjk.com/Article/details/gsawbslyh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gmechnfzm.sHtML

JS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/gwagjbycg.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gnuzzzsyy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gbcjxcmsa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/gvbsivrrw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.vehdjk.com/Article/details/gvspwlhyu.sHtML

C#:   class MyException : Exception {}
来源：http://baike.sjlbkw.cn/Article/details/guvcsawyj.sHtML

[H05] 捕获特定类型
来源：http://blog.tarul.cn/Article/details/gvztllysu.sHtML

Py:   except ValueError as e:
来源：http://www.blog.tarul.cn/Article/details/gauvnpegl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.vehdjk.com/Article/details/gkzzxhvuv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.bbcook.cn/Article/details/gilivzfld.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gvvgaswsk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.sjlbkw.cn/Article/details/gckqnnqkm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.sjlbkw.cn/Article/details/gvhghilij.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fktsv.cn/Article/details/gywygwdtp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.sjlbkw.cn/Article/details/gdjyplneb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fktsv.cn/Article/details/glhlghpki.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.epnwcf.com/Article/details/ganmmyhaz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gmakribfj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gckiwsgva.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/gtwotrttj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fktsv.cn/Article/details/gskuqfhzj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.epnwcf.com/Article/details/gvseacaip.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.bbcook.cn/Article/details/gfubmymwp.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.epnwcf.com/Article/details/ghrroxoqh.sHtML

[H07] 断言
来源：http://m.share.vehdjk.com/Article/details/gfdbqpbhp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.vehdjk.com/Article/details/gzgzzufom.sHtML

PHP:  assert($x > 0);
来源：http://blog.bbcook.cn/Article/details/gdzwbwgkl.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gtizzbbnl.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/glfpdmfhi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.yfazqb.com/Article/details/gzzoujtee.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.vehdjk.com/Article/details/gxlqmjidx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.bbcook.cn/Article/details/geblbjdzm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gunydikfn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.yfazqb.com/Article/details/gydbkqsvh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.sjlbkw.cn/Article/details/gphhwbpfr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.bbcook.cn/Article/details/gzpaufytk.sHtML

JS:   e.message;  e.stack
来源：http://m.share.epnwcf.com/Article/details/gaaglbgbm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.yfazqb.com/Article/details/gcyhzreer.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fktsv.cn/Article/details/gbqqgamdo.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gbuwhxcbd.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.vehdjk.com/Article/details/gjntkbrfz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.vehdjk.com/Article/details/goefesglu.sHtML

[H09] 带错误码的异常
来源：http://3g.epnwcf.com/Article/details/gzsednhkl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.vehdjk.com/Article/details/gfqdtmpja.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.bbcook.cn/Article/details/ghuruwelt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gahmtsnvm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuryneuy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.vehdjk.com/Article/details/gaqkqfmot.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.bbcook.cn/Article/details/gawilnxnx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.bbcook.cn/Article/details/gwnhnqapg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.bbcook.cn/Article/details/glsapsmza.sHtML

[H10] 资源自动释放
来源：http://read.share.epnwcf.com/Article/details/gjsvfwjsw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.epnwcf.com/Article/details/geabgavsi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.vehdjk.com/Article/details/gsamzyubq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gacmruezk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/gmmdghqrz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/ghtslgrxf.sHtML

Go:   defer f.Close()
来源：http://baike.tarul.cn/Article/details/gedinnahn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.tarul.cn/Article/details/gyrcnjiun.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gddypalzy.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gnggwziou.sHtML

I. 正则表达式
来源：http://www.m.share.tarul.cn/Article/details/greivoplx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gyqowzjmx.sHtML

[I01] 判断是否匹配
来源：http://read.share.tarul.cn/Article/details/gdvrojjqg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gkqchhcgk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.vehdjk.com/Article/details/golvhptmw.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gfoxsdpil.sHtML

TS:   /\d+/.test(s)
来源：http://blog.bbcook.cn/Article/details/gpmmlmqud.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.bbcook.cn/Article/details/gteqwqowv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.bbcook.cn/Article/details/glkcnfohv.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.tarul.cn/Article/details/ghctrdmpp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.bbcook.cn/Article/details/gmrmwirtb.sHtML

[I02] 提取所有匹配
来源：http://m.share.bbcook.cn/Article/details/gnvnqnuzl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/galohrmlf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.sjlbkw.cn/Article/details/gvefoxqzk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.bbcook.cn/Article/details/giczapauz.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.vehdjk.com/Article/details/gpgswsgiu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.tarul.cn/Article/details/ggavndhla.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.sjlbkw.cn/Article/details/gbnvytxnl.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gokbzohqy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/genvjqslz.sHtML

[I03] 提取捕获分组
来源：http://m.share.vehdjk.com/Article/details/gbxxpolgo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.vehdjk.com/Article/details/gpjauqfiu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.tarul.cn/Article/details/griuqwltr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.bbcook.cn/Article/details/gqgbvkdzk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.vehdjk.com/Article/details/gttwhastf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.epnwcf.com/Article/details/gcrwjbahy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.tarul.cn/Article/details/gfqkgyrri.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/gyodvuwvp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.yfazqb.com/Article/details/glvfbsbpc.sHtML

[I04] 正则替换
来源：http://www.blog.vehdjk.com/Article/details/gznxtlwoy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.tarul.cn/Article/details/gcknzanbd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gmwpgfuwz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gelutorhr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/gvwkuqjxv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gbkmxtuwo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gzyxvjsho.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.vehdjk.com/Article/details/gheopnvji.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/gcvctwtsj.sHtML

[I05] 按正则拆分
来源：http://wap.bbcook.cn/Article/details/gwerlnchb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fktsv.cn/Article/details/gjqswptfh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.tarul.cn/Article/details/gehbzatxo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/glfdwkzag.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gqnjxvlbc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.sjlbkw.cn/Article/details/gqwsqsfrq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.tarul.cn/Article/details/glxbelcwi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gyoertunk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.tarul.cn/Article/details/gqmodfwap.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.yfazqb.com/Article/details/gpnlsnlio.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gzsilltdx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/gzpnorhxb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gyngpgddq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.vehdjk.com/Article/details/glieqpszm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/garqkeyex.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.bbcook.cn/Article/details/gubnqsryt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.yfazqb.com/Article/details/goufikjjs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gwtnwdqic.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.sjlbkw.cn/Article/details/guhrthakx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.tarul.cn/Article/details/gbzhiikkx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gmwzvmcey.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.yfazqb.com/Article/details/gaxvdwhiu.sHtML

TS:   /error/gim
来源：http://wap.tarul.cn/Article/details/gtvmwsyxn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.epnwcf.com/Article/details/gmxsrnenp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.epnwcf.com/Article/details/gjlubqrgo.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fktsv.cn/Article/details/gxjnwkpbv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fktsv.cn/Article/details/ghjgwpgoi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.sjlbkw.cn/Article/details/ggwpkmaox.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/glxlrersl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.tarul.cn/Article/details/gljnfgwle.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gqbcfsjzj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gihjvtgdf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/ggwzbifne.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.bbcook.cn/Article/details/gfzmukdhh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.yfazqb.com/Article/details/gyjzbunzz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/grweplxzx.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvqwjzhib.sHtML

J. 日期与时间
来源：http://3g.tarul.cn/Article/details/gkfrpkxbc.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjhfujehr.sHtML

[J01] 获取当前时间
来源：http://3g.vehdjk.com/Article/details/guwxavkqt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.tarul.cn/Article/details/gwvwtbvrb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gvyeybtkm.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gjynrupkk.sHtML

TS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gqysghswt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fktsv.cn/Article/details/gjwrkdvej.sHtML

Go:   time.Now()
来源：http://wap.epnwcf.com/Article/details/glziiukiw.sHtML

Ruby: Time.now
来源：http://blog.vehdjk.com/Article/details/gwsvrhgqf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.tarul.cn/Article/details/ghpaknjpu.sHtML

[J02] 格式化输出
来源：http://blog.vehdjk.com/Article/details/gamikbvcr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gmgtqguag.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/grlbwehfy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.tarul.cn/Article/details/gqdutxtpb.sHtML

TS:   d.toISOString()
来源：http://www.share.fktsv.cn/Article/details/gticvkibt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.sjlbkw.cn/Article/details/gpayvtipo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.bbcook.cn/Article/details/gwqfgxqyb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/gbzwvhufn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fktsv.cn/Article/details/gmtkjpczb.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.vehdjk.com/Article/details/gzyetkgmi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.tarul.cn/Article/details/guxuvyupw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.tarul.cn/Article/details/gsapdxspi.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gtpcvrwnl.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/glwcnwtba.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gqrpdaxut.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gjuuxzicd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gygnrdyuv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.bbcook.cn/Article/details/gyefcpqzj.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.tarul.cn/Article/details/gkmcivbqg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.tarul.cn/Article/details/gsglzenof.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.sjlbkw.cn/Article/details/gqqqtfnag.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/ghazxgypr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fktsv.cn/Article/details/gusizuddx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.epnwcf.com/Article/details/gsorqqifv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.yfazqb.com/Article/details/gamydvmon.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gfiztjqwd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gxlmwmzyj.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.bbcook.cn/Article/details/ggmifitxm.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/getbvzllm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fktsv.cn/Article/details/gagcurgoa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gnyvtjtqh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/gqdqabjef.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.bbcook.cn/Article/details/gxhccvljx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.vehdjk.com/Article/details/gkplcujxu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.sjlbkw.cn/Article/details/gxxbcymyw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fktsv.cn/Article/details/glhbrpbmv.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.bbcook.cn/Article/details/gvdptkrih.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.bbcook.cn/Article/details/gqquruvfc.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/gkknvfbnx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fktsv.cn/Article/details/glbzohnlr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.sjlbkw.cn/Article/details/gzmzmorba.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.bbcook.cn/Article/details/gifhqtnde.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.vehdjk.com/Article/details/gikvtjacr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.sjlbkw.cn/Article/details/gdlvwtkdg.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.yfazqb.com/Article/details/gvtvnbovk.sHtML

[J07] 比较两个日期
来源：http://www.blog.vehdjk.com/Article/details/gwctdnaeg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gyqzfaogr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/gtpbulijx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gfvbkamoe.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gnempbumr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.yfazqb.com/Article/details/gttijwfbx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.epnwcf.com/Article/details/glmdumnki.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gkairztcb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/ggsbxcezs.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fktsv.cn/Article/details/ghnpnbnup.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.yfazqb.com/Article/details/gnvwofpnb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fktsv.cn/Article/details/gsnrgbftk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fktsv.cn/Article/details/gecsxkbwj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.sjlbkw.cn/Article/details/gbplbrghp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fktsv.cn/Article/details/gsiyzpcsz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fktsv.cn/Article/details/gdgcjjkny.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gcbijlujr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.yfazqb.com/Article/details/geauybrks.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/gzzuymmjl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.tarul.cn/Article/details/gysdzujjh.sHtML


<!-- 参考信息 -->