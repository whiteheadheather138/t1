代发 wailian999

PHP:  public static function f() {}
来源：http://read.share.tarul.cn/Article/details/gakwtbasr.sHtML

JS:   static f() {}
来源：http://www.m.share.bbcook.cn/Article/details/ghklrshcj.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/gjcojoctf.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gxdhfmikk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.tarul.cn/Article/details/gijraipww.sHtML

Ruby: def self.f; end
来源：http://mobile.yfazqb.com/Article/details/gymikhnvd.sHtML

C#:   public static void F() {}
来源：http://www.blog.bbcook.cn/Article/details/gmymfvuhn.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/gndmmhyem.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/guadpdxhg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.sjlbkw.cn/Article/details/glwchoguw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/gihyjxyww.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.sjlbkw.cn/Article/details/ghwzvdbwb.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/gomrhrfdt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.epnwcf.com/Article/details/gxcbcztlp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.vehdjk.com/Article/details/gxhauxqiv.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.yfazqb.com/Article/details/gufxpkdpq.sHtML

[G10] 访问控制
来源：http://www.m.share.bbcook.cn/Article/details/gzexrslgu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fktsv.cn/Article/details/glwikrvqv.sHtML

PHP:  public / protected / private
来源：http://blog.bbcook.cn/Article/details/gpioxzdee.sHtML

JS:   #private 字段；其余公开
来源：http://wap.epnwcf.com/Article/details/gmjlxfljr.sHtML

TS:   public / protected / private
来源：http://wap.epnwcf.com/Article/details/gkvackwuj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/gzfjsiull.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.tarul.cn/Article/details/gpuxesdjf.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gtmhtvncr.sHtML

C#:   public / protected / private / internal
来源：http://www.share.yfazqb.com/Article/details/gkmztgquz.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gdpejcpiv.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.vehdjk.com/Article/details/gtpvnmjev.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/govaulqfn.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gqwjekblz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/gcsdgvwee.sHtML

Java: public String getName() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gggqcsbug.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gjrubrwfh.sHtML

Ruby: attr_accessor :name
来源：http://blog.epnwcf.com/Article/details/gferqflda.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.yfazqb.com/Article/details/gqakmjeee.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/gyhdvxuus.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gsuqawdru.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gyczfuoza.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/ghutzphuo.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gwkfruwri.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.tarul.cn/Article/details/gdnqasfjg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gzampeymh.sHtML

Ruby: def to_s; @name; end
来源：http://blog.epnwcf.com/Article/details/grugjycyv.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/giwgvbxut.sHtML

[G13] 判断对象类型
来源：http://wap.sjlbkw.cn/Article/details/gfumzozan.sHtML

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/gckpvrgbv.sHtML

PHP:  $u instanceof User
来源：http://blog.bbcook.cn/Article/details/gdlvvwrim.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gsdmspzzh.sHtML

TS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gwwldirgh.sHtML

Java: u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/ghjnvigub.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.vehdjk.com/Article/details/gglvdljkw.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/gsayjygcu.sHtML

C#:   u is User
来源：http://www.share.sjlbkw.cn/Article/details/gwwipavaf.sHtML

[G14] 数据类 / record
来源：http://baike.epnwcf.com/Article/details/gwjlcnzzl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/ghfrhcswm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.sjlbkw.cn/Article/details/gobwozpkd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.sjlbkw.cn/Article/details/gdxjvmqtb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.vehdjk.com/Article/details/ggvfgijcv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.epnwcf.com/Article/details/gcbavwigm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.sjlbkw.cn/Article/details/gbjjnazkq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.tarul.cn/Article/details/gtftaawdp.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.yfazqb.com/Article/details/gzntgycpe.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/gyykgajyq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.sjlbkw.cn/Article/details/gphwjjgcy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.tarul.cn/Article/details/gbxfkpgjk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/gsprpjhuh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gizgyrylb.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.epnwcf.com/Article/details/gptpmugpq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.tarul.cn/Article/details/gnyvmxdnz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.tarul.cn/Article/details/gjlxqvdyk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gxhvkytsf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.vehdjk.com/Article/details/grlzkxtrd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.bbcook.cn/Article/details/ggxoimfrs.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.epnwcf.com/Article/details/gerdurcwm.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gsikumdwx.sHtML

TS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/gsjogqxkq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gfpqninmf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.vehdjk.com/Article/details/gubsfsrda.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fktsv.cn/Article/details/gklrupkqg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gadyvpwgs.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gfwzztosr.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/gldxpdrfg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gayfdgysz.sHtML

[H01] try / catch 基础
来源：http://www.blog.epnwcf.com/Article/details/grkszzgrt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.epnwcf.com/Article/details/gdhezospx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fktsv.cn/Article/details/gjcpcmybj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gmmcwdojj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/grmrnnvtu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.tarul.cn/Article/details/ghmelyuow.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.epnwcf.com/Article/details/gtvokqevq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.epnwcf.com/Article/details/gvcboccuv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.epnwcf.com/Article/details/gttnophir.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.vehdjk.com/Article/details/gdagjelvo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.sjlbkw.cn/Article/details/gwvhkmnak.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gxchvpdka.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gvscevvyp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gzommtjtl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gisvdmmga.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.vehdjk.com/Article/details/gjwroxgdk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/guiipdphy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gnhuczplq.sHtML

[H03] 主动抛出异常
来源：http://3g.yfazqb.com/Article/details/gjdxgnklw.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.sjlbkw.cn/Article/details/getvegpxx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrirqoky.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gzdnndvey.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gnbduzkrc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gxtawttcp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.yfazqb.com/Article/details/gkzktnkfd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.vehdjk.com/Article/details/ghsaqrsbb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gwzpdcxgo.sHtML

[H04] 自定义异常类型
来源：http://www.share.fktsv.cn/Article/details/glibdrvve.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fktsv.cn/Article/details/gbpllokfo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/guivdjdxa.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gqnppzeon.sHtML

TS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/grjsqtkbl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/gmbpwkgoz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.vehdjk.com/Article/details/gqtpdvypq.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gbokpryql.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.epnwcf.com/Article/details/gmlaspdkj.sHtML

[H05] 捕获特定类型
来源：http://3g.yfazqb.com/Article/details/guuakayic.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.bbcook.cn/Article/details/gswmxhcqy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/gmulwjxxm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/gjfoqfhya.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/ggiutimkt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.tarul.cn/Article/details/gquqqmhtf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fktsv.cn/Article/details/ghstoyiag.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.yfazqb.com/Article/details/gwzvbssbx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.yfazqb.com/Article/details/gclcfbykv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.epnwcf.com/Article/details/ggqebqobr.sHtML

Py:   value = d.get("k") or default
来源：http://wap.vehdjk.com/Article/details/gdqzallnd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gqqgnzsnx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/gxjswxgwm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gtrcnatvl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.yfazqb.com/Article/details/gavmbivmn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgnajggj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.epnwcf.com/Article/details/goprcsebt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.bbcook.cn/Article/details/gksoiearq.sHtML

[H07] 断言
来源：http://mobile.yfazqb.com/Article/details/gtjuqwpao.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/gibthnutd.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gegkwzrnd.sHtML

JS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gbeqtgbft.sHtML

TS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/grnvhmlqu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.sjlbkw.cn/Article/details/ggwbfkmci.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.tarul.cn/Article/details/gcvaauwqy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.vehdjk.com/Article/details/gqbzahzwt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gyeyqtgqy.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.tarul.cn/Article/details/gubpsmdyl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fktsv.cn/Article/details/gubhtmtaq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gabxphusr.sHtML

JS:   e.message;  e.stack
来源：http://read.share.sjlbkw.cn/Article/details/gmrajywcv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.vehdjk.com/Article/details/grplreuxx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.yfazqb.com/Article/details/ghglpbnbm.sHtML

Go:   err.Error()
来源：http://baike.bbcook.cn/Article/details/gaseourbn.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsghzgqr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.epnwcf.com/Article/details/gmbqlzjcx.sHtML

[H09] 带错误码的异常
来源：http://www.blog.epnwcf.com/Article/details/gjcdrpghk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fktsv.cn/Article/details/gzhxhftgd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.bbcook.cn/Article/details/goyuhswfl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.tarul.cn/Article/details/gfvakoqst.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.epnwcf.com/Article/details/gmijefopy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.tarul.cn/Article/details/gwgaoxsta.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.vehdjk.com/Article/details/gzmtjumre.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.vehdjk.com/Article/details/gtfroacxv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.bbcook.cn/Article/details/gjevaupmd.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gohzhcuxe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.bbcook.cn/Article/details/gdksewspr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.tarul.cn/Article/details/gefkhfwxh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.sjlbkw.cn/Article/details/gnlpvbaqm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gkgsrpbty.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.sjlbkw.cn/Article/details/gabrvyvdr.sHtML

Go:   defer f.Close()
来源：http://www.share.fktsv.cn/Article/details/ghusgztej.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.bbcook.cn/Article/details/gmqcbfrwz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gboroubgp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gqlwrewuq.sHtML

I. 正则表达式
来源：http://3g.fktsv.cn/Article/details/ghkxauybk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwspcjubu.sHtML

[I01] 判断是否匹配
来源：http://wap.fktsv.cn/Article/details/gnmfsuxoe.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gtlfaxezm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fktsv.cn/Article/details/gszimixvo.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/grfpwoxpa.sHtML

TS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gujlmgami.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fktsv.cn/Article/details/gokpxwkys.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.bbcook.cn/Article/details/geamzflve.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gyyhcyilq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fktsv.cn/Article/details/gqzveslon.sHtML

[I02] 提取所有匹配
来源：http://baike.yfazqb.com/Article/details/gunisbnhx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gizsjsbgo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/gdwiyochi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.vehdjk.com/Article/details/gtoubqmdw.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.tarul.cn/Article/details/gpaixwjmx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.tarul.cn/Article/details/ggapsemyi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.yfazqb.com/Article/details/gokigcwvn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gdzgfvivh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fktsv.cn/Article/details/gjhljowev.sHtML

[I03] 提取捕获分组
来源：http://blog.fktsv.cn/Article/details/gfjinebie.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.yfazqb.com/Article/details/gkkvhybbu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.bbcook.cn/Article/details/gqwctqpti.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.tarul.cn/Article/details/gybfooxap.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.yfazqb.com/Article/details/gfqyzldcb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.yfazqb.com/Article/details/gcjxnayax.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.epnwcf.com/Article/details/ggbdchxus.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/gjklucdca.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.tarul.cn/Article/details/gflysqoec.sHtML

[I04] 正则替换
来源：http://blog.bbcook.cn/Article/details/gnphzttnd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.bbcook.cn/Article/details/gjdywjvst.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/gjgxbswmq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gexpalfyn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gdddowhec.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gwgdlsniy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gqfmosfyu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.vehdjk.com/Article/details/gzpugfvrm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gtyzjlbmi.sHtML

[I05] 按正则拆分
来源：http://3g.tarul.cn/Article/details/gvmxzznge.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.vehdjk.com/Article/details/gewppequp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/gbpnkapvq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gmyjtogdn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.bbcook.cn/Article/details/gbvihkbxj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gdudzjgro.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.epnwcf.com/Article/details/gkfznjzgz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gpfzlvxte.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fktsv.cn/Article/details/gbnklhezn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.vehdjk.com/Article/details/gzilybvio.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gfgnjxtoy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.tarul.cn/Article/details/gwrlsdysb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gcqggxeth.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.tarul.cn/Article/details/gyibukorm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.tarul.cn/Article/details/gwmwzutit.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.vehdjk.com/Article/details/gmnoteupy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.epnwcf.com/Article/details/gnyweujbp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gpzzwlhuh.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.epnwcf.com/Article/details/geomrruab.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fktsv.cn/Article/details/gguetrpyo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gsoceplzr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.bbcook.cn/Article/details/gxektfgop.sHtML

TS:   /error/gim
来源：http://mobile.vehdjk.com/Article/details/gtaiuqtlp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.sjlbkw.cn/Article/details/gcdrpsfyi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/grsubcxye.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.epnwcf.com/Article/details/gbonnwalo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fktsv.cn/Article/details/glfqztrdt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/gjtokuhnz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.sjlbkw.cn/Article/details/gbojmeahx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.sjlbkw.cn/Article/details/gdlhyvuxe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gzevstbfj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fktsv.cn/Article/details/gyvufleyy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/ghzfbjwbt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/gorflhnns.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/gwwexxwip.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/gqrtwjlic.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gehnxwjux.sHtML

J. 日期与时间
来源：http://wap.vehdjk.com/Article/details/gthabhaed.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gnnoidgan.sHtML

[J01] 获取当前时间
来源：http://www.share.yfazqb.com/Article/details/gqjonlxmk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.bbcook.cn/Article/details/gfbmpexrt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/glcgedqpt.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/gnechejfz.sHtML

TS:   new Date();  Date.now()
来源：http://wap.epnwcf.com/Article/details/gzyeksxjq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fktsv.cn/Article/details/gyndgzikk.sHtML

Go:   time.Now()
来源：http://mobile.fktsv.cn/Article/details/gqjgmnape.sHtML

Ruby: Time.now
来源：http://www.blog.fktsv.cn/Article/details/ggpcsolmt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fktsv.cn/Article/details/gwodoafus.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gxgpytmdj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/gtzqfcjss.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/gesjnuogr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.epnwcf.com/Article/details/gubjlsmwn.sHtML

TS:   d.toISOString()
来源：http://read.share.bbcook.cn/Article/details/gbckjddpb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/gckpawbqt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.tarul.cn/Article/details/geidxiavl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.yfazqb.com/Article/details/gjkzcpivs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.sjlbkw.cn/Article/details/gggrlwfal.sHtML

[J03] 字符串解析为日期
来源：http://read.share.epnwcf.com/Article/details/gipcktowu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.epnwcf.com/Article/details/gptooyfxw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fktsv.cn/Article/details/geculloak.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gyqzetwid.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gnlgdukpx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gifxxafjr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gwnonwlny.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gjcwxpqrp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.bbcook.cn/Article/details/gipuzgcgj.sHtML

[J04] 时间戳与日期互转
来源：http://baike.sjlbkw.cn/Article/details/gfqqrumzt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.tarul.cn/Article/details/glxrkbuoa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/gzykriezw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/gqcyouelx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.bbcook.cn/Article/details/gslnucjlx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.yfazqb.com/Article/details/ggergbgfm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/gnqtitawq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.vehdjk.com/Article/details/gipmtqahj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.epnwcf.com/Article/details/guqvfjxuo.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.vehdjk.com/Article/details/gdoghabas.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.bbcook.cn/Article/details/gvtfsmfjy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.epnwcf.com/Article/details/gpjctshzm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/gbsdjslbr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gcracvgah.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.yfazqb.com/Article/details/gvrqoowtm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.tarul.cn/Article/details/gylccraaa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.yfazqb.com/Article/details/gmuzgzkfg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.tarul.cn/Article/details/gbrmnzety.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gmalucmji.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.bbcook.cn/Article/details/grtduoqjd.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.yfazqb.com/Article/details/gzipocish.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.yfazqb.com/Article/details/gmiautrup.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.epnwcf.com/Article/details/grnvdxvee.sHtML


<!-- 参考信息 -->