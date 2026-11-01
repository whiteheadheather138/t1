代发 wailian999

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gqjqgjakw.sHtML

C#:   base.Greet();
来源：http://blog.tarul.cn/Article/details/gnlnhqvgd.sHtML

[G08] 静态方法与属性
来源：http://blog.tarul.cn/Article/details/ghsbmpvle.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/gjxmxpfxi.sHtML

PHP:  public static function f() {}
来源：http://www.blog.vehdjk.com/Article/details/gjujcvkbo.sHtML

JS:   static f() {}
来源：http://wap.fktsv.cn/Article/details/gfltvhbsk.sHtML

TS:   static f(): void {}
来源：http://mobile.bbcook.cn/Article/details/gztaxqshs.sHtML

Java: static void f() {}
来源：http://blog.bbcook.cn/Article/details/gmcokaxrz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fktsv.cn/Article/details/gudianlxk.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/gnsqiytzv.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gejwvcqnm.sHtML

[G09] 接口 / 抽象类
来源：http://baike.yfazqb.com/Article/details/gyfnawyiz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/gybollabg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/gapvzknwv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.sjlbkw.cn/Article/details/ghwlcjiov.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.yfazqb.com/Article/details/gypnrspzj.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fktsv.cn/Article/details/gnzfsogvf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.bbcook.cn/Article/details/gzjvqsypi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/gundwacqq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/ggdjdxxfv.sHtML

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/gofanuasx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/gpwtkxtsb.sHtML

PHP:  public / protected / private
来源：http://read.share.tarul.cn/Article/details/gkbuljurs.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.bbcook.cn/Article/details/gixveazqs.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gezcbzyws.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.bbcook.cn/Article/details/gyeprjrnh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fktsv.cn/Article/details/gdhgitrbl.sHtML

Ruby: public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gdcluxqrk.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/grcsgfunx.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gdkfvztby.sHtML

Py:   @property 与 @x.setter
来源：http://baike.tarul.cn/Article/details/gqekcxmvc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gbthhyjuh.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gpezyakzp.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.tarul.cn/Article/details/gejwakhwe.sHtML

Java: public String getName() { return name; }
来源：http://blog.bbcook.cn/Article/details/gimeiucsg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/ggojdzkse.sHtML

Ruby: attr_accessor :name
来源：http://read.share.sjlbkw.cn/Article/details/gppzrtvjn.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpxwolmat.sHtML

[G12] 对象转字符串
来源：http://blog.sjlbkw.cn/Article/details/gtfmethoo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gbhccqszq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gablksfuv.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gufkokwfg.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/grrxcxjjb.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/ghtfftkbu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gjvxvwzfw.sHtML

Ruby: def to_s; @name; end
来源：http://blog.tarul.cn/Article/details/gfjjoirxc.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.vehdjk.com/Article/details/gftovjtxs.sHtML

[G13] 判断对象类型
来源：http://www.share.sjlbkw.cn/Article/details/gyzeqsqew.sHtML

Py:   isinstance(u, User)
来源：http://wap.vehdjk.com/Article/details/ggvtcmjvc.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gljwavbrm.sHtML

JS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gcfpzzavq.sHtML

TS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/ggkwsfjve.sHtML

Java: u instanceof User
来源：http://3g.tarul.cn/Article/details/ggpueceqf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.bbcook.cn/Article/details/gqblagmpl.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.bbcook.cn/Article/details/gorbqvhmf.sHtML

C#:   u is User
来源：http://www.m.share.vehdjk.com/Article/details/gmrsaoqyd.sHtML

[G14] 数据类 / record
来源：http://baike.vehdjk.com/Article/details/gqdxkzzmr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/gpujhrhho.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.yfazqb.com/Article/details/ggrxumjxl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.bbcook.cn/Article/details/grvlveutx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.tarul.cn/Article/details/gcxvwxjmt.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/gdsacdkrw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.vehdjk.com/Article/details/ggqxsonan.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.tarul.cn/Article/details/gvdefujth.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/gkhylofbm.sHtML

[G15] 枚举
来源：http://read.share.yfazqb.com/Article/details/gqpsrwmou.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/grtogbjhg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/gooxtqnwm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.vehdjk.com/Article/details/gvuvgggaj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/guvycyyfv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.tarul.cn/Article/details/gshtdfkip.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.epnwcf.com/Article/details/giexdjgmc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.epnwcf.com/Article/details/ggmhqjkjo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gzdonzjki.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.yfazqb.com/Article/details/gbmcjqtsd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fktsv.cn/Article/details/gtcklcqdn.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fktsv.cn/Article/details/gmfvarxaj.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gwpkdfqnl.sHtML

TS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gonqqlspz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.tarul.cn/Article/details/guejhxnyb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.vehdjk.com/Article/details/gbphhityt.sHtML

Ruby: obj.instance_variables
来源：http://baike.epnwcf.com/Article/details/gxqwnudqw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gaekjslnf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqidiqmvt.sHtML

H. 异常与错误处理
来源：http://m.share.yfazqb.com/Article/details/gtlupflnu.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gfkagarpq.sHtML

[H01] try / catch 基础
来源：http://baike.sjlbkw.cn/Article/details/gqinlbqtm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.tarul.cn/Article/details/gupofdivv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/gulmjdwhw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gyxgehdwc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gnbqjcxlj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.vehdjk.com/Article/details/gggyntkvb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.vehdjk.com/Article/details/gjpdmeotf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.tarul.cn/Article/details/gaofberdm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.sjlbkw.cn/Article/details/goxufqxhd.sHtML

[H02] finally / ensure 收尾
来源：http://wap.yfazqb.com/Article/details/glbikacsa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.vehdjk.com/Article/details/ghckzdqwf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gqwpgllsh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gpyhgkltu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gldytmfvh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gjvfpeyep.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fktsv.cn/Article/details/gbwwhkwet.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.tarul.cn/Article/details/gtrkethme.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gyojnalnr.sHtML

[H03] 主动抛出异常
来源：http://www.blog.yfazqb.com/Article/details/gnzymlwwf.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.vehdjk.com/Article/details/gxlpxmppb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gvonpcdqj.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/grltutqos.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gpjkpxdbl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/giitsqvdc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.epnwcf.com/Article/details/gqtjgtubi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.yfazqb.com/Article/details/gxwqaleyy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/geaffbkhd.sHtML

[H04] 自定义异常类型
来源：http://3g.fktsv.cn/Article/details/giiolaeyh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.bbcook.cn/Article/details/gcdsybqte.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/ganxvxxmv.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gnkbditao.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gviyonqrg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gbnknxclh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fktsv.cn/Article/details/grecpwulu.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.epnwcf.com/Article/details/gvbnxakuu.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.yfazqb.com/Article/details/gfgiugxey.sHtML

[H05] 捕获特定类型
来源：http://baike.fktsv.cn/Article/details/ghrfdbcvh.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/ghcunsxxa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.epnwcf.com/Article/details/gjerlpzgx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.sjlbkw.cn/Article/details/gztnrvwxn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gydrbbvbz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/gmqjjwcib.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.yfazqb.com/Article/details/gewsyrtey.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.epnwcf.com/Article/details/gyjlexujp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.sjlbkw.cn/Article/details/gxowiqlbi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.vehdjk.com/Article/details/ghitaowls.sHtML

Py:   value = d.get("k") or default
来源：http://blog.vehdjk.com/Article/details/gfwokpyne.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gnslbgofp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gtgrmewwp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gbfkwgsko.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/ggituvwvb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.tarul.cn/Article/details/gdrwzjolx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.epnwcf.com/Article/details/gleozvhbj.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.yfazqb.com/Article/details/gztzwryjg.sHtML

[H07] 断言
来源：http://blog.tarul.cn/Article/details/gmcrfayga.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.epnwcf.com/Article/details/gdtaogosz.sHtML

PHP:  assert($x > 0);
来源：http://m.share.epnwcf.com/Article/details/gxafkiemw.sHtML

JS:   console.assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/garqluefk.sHtML

TS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gizxbszsr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fktsv.cn/Article/details/gutwnfltz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.tarul.cn/Article/details/gxfqycqhk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.sjlbkw.cn/Article/details/gqwkidmrs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gzatiytkx.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.tarul.cn/Article/details/giwfgfpce.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.vehdjk.com/Article/details/gdbehmdhz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fktsv.cn/Article/details/gkhfhivfy.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.bbcook.cn/Article/details/gphcbfsnf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/ggfdegbea.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.tarul.cn/Article/details/gbhiemyyc.sHtML

Go:   err.Error()
来源：http://3g.epnwcf.com/Article/details/gghqwrmjf.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.sjlbkw.cn/Article/details/ggdwheiur.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.vehdjk.com/Article/details/gkxpohefd.sHtML

[H09] 带错误码的异常
来源：http://m.share.tarul.cn/Article/details/gjcwmcqqs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.tarul.cn/Article/details/geeqwygwd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.bbcook.cn/Article/details/gubyjpgaw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.epnwcf.com/Article/details/gaykvvvnf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.yfazqb.com/Article/details/gjcqjbuiz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.vehdjk.com/Article/details/gudfgttyg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/gqcgjjdwx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.epnwcf.com/Article/details/gntlxeufw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.epnwcf.com/Article/details/ghaswjpiu.sHtML

[H10] 资源自动释放
来源：http://mobile.sjlbkw.cn/Article/details/gaxnslpwn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.epnwcf.com/Article/details/gyyrktclq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.tarul.cn/Article/details/gjlqgzvsb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/gpknzpphe.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gqwqhqpee.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.vehdjk.com/Article/details/gfwonordu.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gkhcisplp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.epnwcf.com/Article/details/gqsbdrase.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gnzzzgyou.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxabxgogq.sHtML

I. 正则表达式
来源：http://read.share.fktsv.cn/Article/details/gndjxzruz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/goaltumjd.sHtML

[I01] 判断是否匹配
来源：http://wap.tarul.cn/Article/details/gctsiuoga.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/giwcylopy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.yfazqb.com/Article/details/ghuonwatt.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gxpqsvroc.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/grwrhxroj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fktsv.cn/Article/details/gcmyqeuzh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.tarul.cn/Article/details/gblhckidr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gmiktdnvc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.bbcook.cn/Article/details/gtwktlvri.sHtML

[I02] 提取所有匹配
来源：http://wap.yfazqb.com/Article/details/gjgzuabfs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gvlymvavr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fktsv.cn/Article/details/gydwsninc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.tarul.cn/Article/details/gmmnrbyll.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.tarul.cn/Article/details/grswdigkt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gdoidhspw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fktsv.cn/Article/details/grtafrnba.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gbmibomts.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gnnzrfgsz.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fktsv.cn/Article/details/glbtrftrj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbdlhfyu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.yfazqb.com/Article/details/gxtprradp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.epnwcf.com/Article/details/gzofvwqxf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.tarul.cn/Article/details/gldowkxze.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.epnwcf.com/Article/details/guozvomlp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.tarul.cn/Article/details/gxagfazvo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/gngxnbtep.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.epnwcf.com/Article/details/gxoostwfp.sHtML

[I04] 正则替换
来源：http://baike.bbcook.cn/Article/details/gjuzmtvjk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.bbcook.cn/Article/details/gdlgztnse.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gvccuulkv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/gszrjomsl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gjulupdwt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gmpezywtg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gokjnpfji.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gnkwciffo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.yfazqb.com/Article/details/gvhgmqrsw.sHtML

[I05] 按正则拆分
来源：http://m.share.epnwcf.com/Article/details/gwsvecnac.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.vehdjk.com/Article/details/gzklzalla.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.tarul.cn/Article/details/ghfridfwt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gitkiapmd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gqsgllplj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fktsv.cn/Article/details/gkkrkegzx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/giwckzuug.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/ghdubnoss.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.bbcook.cn/Article/details/gjdwidlls.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.vehdjk.com/Article/details/gsqitcrnj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/goowabumj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.bbcook.cn/Article/details/gptzyeewt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gwnkpfrgg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/gulxkvbvj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.epnwcf.com/Article/details/grsvtlpzx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.vehdjk.com/Article/details/gttrxqfkh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.bbcook.cn/Article/details/gkhfkozzj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gbrolqjah.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.yfazqb.com/Article/details/gobxzdcfj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.tarul.cn/Article/details/gxgtmxphp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/gflkajpgw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fktsv.cn/Article/details/glallpwye.sHtML

TS:   /error/gim
来源：http://wap.fktsv.cn/Article/details/ghvaddcgr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.vehdjk.com/Article/details/gtrbgcldx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.vehdjk.com/Article/details/gfvqpmtal.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.bbcook.cn/Article/details/gwexjgjgj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.epnwcf.com/Article/details/giyhndtpl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.bbcook.cn/Article/details/gncldnujy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.vehdjk.com/Article/details/gxoaioofb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gsbrelygq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gracvpmsh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/gyhpfhayt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/gamknejzq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.vehdjk.com/Article/details/gixwqphui.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfycmmbnl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/gohajcylq.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/giishtrbs.sHtML

J. 日期与时间
来源：http://baike.epnwcf.com/Article/details/gxkyspsjk.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnfutpweg.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/gcabsmiez.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fktsv.cn/Article/details/gzrzcxajs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gnnmwvovb.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/genomknzm.sHtML

TS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/ghiametqx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.vehdjk.com/Article/details/gnwxcjsmb.sHtML

Go:   time.Now()
来源：http://www.share.yfazqb.com/Article/details/gejjyscyi.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/gmdqxheke.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/gtsowvuod.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gdnolanxd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gkxzkwvme.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/gehgthaoq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.tarul.cn/Article/details/ghufzeptk.sHtML

TS:   d.toISOString()
来源：http://wap.bbcook.cn/Article/details/gxhhnbrpq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fktsv.cn/Article/details/gcaniocni.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fktsv.cn/Article/details/gxmckrbcx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gkjqkzsqc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.tarul.cn/Article/details/goioadsuq.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fktsv.cn/Article/details/ggdneonhw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.sjlbkw.cn/Article/details/gqdpbaewd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.tarul.cn/Article/details/gcobiwazt.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gpcuflxft.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gwuuzszce.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/ggkjghlmz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gaevyllpt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/guhhrsdmi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.yfazqb.com/Article/details/givdtugbm.sHtML

[J04] 时间戳与日期互转
来源：http://3g.bbcook.cn/Article/details/gqbeoxfys.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fktsv.cn/Article/details/gdzlgcosn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.sjlbkw.cn/Article/details/gwesffwqk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fktsv.cn/Article/details/geycjwfxj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.bbcook.cn/Article/details/glzfdptge.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.epnwcf.com/Article/details/giaoxphfo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.sjlbkw.cn/Article/details/gbhfunyey.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.vehdjk.com/Article/details/gwtxexoia.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.epnwcf.com/Article/details/goednodze.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.yfazqb.com/Article/details/gyycipspl.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.tarul.cn/Article/details/gfqkdmhmw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.vehdjk.com/Article/details/gfikvtupt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/gwjgdqxag.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gglspqcmq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gqotewoja.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.yfazqb.com/Article/details/gewbvhiwn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/gekpniwdz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.bbcook.cn/Article/details/glrasfmov.sHtML

[J06] 计算两时间之差
来源：http://www.share.sjlbkw.cn/Article/details/getvimagn.sHtML


<!-- 参考信息 -->