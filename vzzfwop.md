代发 wailian999

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/grjdgymzz.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/geeaafzpu.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/gommkpwpk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fktsv.cn/Article/details/gwvhbxhos.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/gdzqkmxqc.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gohnrafzy.sHtML

[G08] 静态方法与属性
来源：http://wap.tarul.cn/Article/details/gmugwlfly.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/gegzvkpyb.sHtML

PHP:  public static function f() {}
来源：http://m.share.epnwcf.com/Article/details/gobbrxjnm.sHtML

JS:   static f() {}
来源：http://www.share.epnwcf.com/Article/details/gxwioqffl.sHtML

TS:   static f(): void {}
来源：http://m.share.sjlbkw.cn/Article/details/gefaofbiv.sHtML

Java: static void f() {}
来源：http://wap.bbcook.cn/Article/details/gvmyjjdkk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.tarul.cn/Article/details/gxdkryrwx.sHtML

Ruby: def self.f; end
来源：http://baike.tarul.cn/Article/details/gsurmrkgf.sHtML

C#:   public static void F() {}
来源：http://www.share.yfazqb.com/Article/details/gypkswdep.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.vehdjk.com/Article/details/gkuqfeokz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.epnwcf.com/Article/details/gbyuissln.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.tarul.cn/Article/details/gwfvfwkxk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.yfazqb.com/Article/details/glrjwtlva.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fktsv.cn/Article/details/gkteduhpa.sHtML

Java: interface Shape { double area(); }
来源：http://blog.vehdjk.com/Article/details/gakrikedb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/grytrwekr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.yfazqb.com/Article/details/gplpiwvhq.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.sjlbkw.cn/Article/details/gsvvedevb.sHtML

[G10] 访问控制
来源：http://m.share.epnwcf.com/Article/details/grlourcje.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/gchoymckj.sHtML

PHP:  public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gguuzxyxx.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.bbcook.cn/Article/details/gsgcryhiu.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gbnqbqeiv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.sjlbkw.cn/Article/details/gfblxgtgk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.bbcook.cn/Article/details/gnkntquka.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gmdamjmvk.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/gndxclkik.sHtML

[G11] getter / setter
来源：http://wap.yfazqb.com/Article/details/garawmbyr.sHtML

Py:   @property 与 @x.setter
来源：http://blog.tarul.cn/Article/details/ganbcnwud.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gaudxtwhg.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gcwuhxlmu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/ggqvmoxdn.sHtML

Java: public String getName() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/glzhvykbo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gdlsinhnq.sHtML

Ruby: attr_accessor :name
来源：http://baike.fktsv.cn/Article/details/gddxnewsa.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/ghnukobze.sHtML

[G12] 对象转字符串
来源：http://baike.fktsv.cn/Article/details/gbkrxwmzs.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.yfazqb.com/Article/details/guuhtyfib.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gjfjfpopl.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gumondbct.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gsqqjaaoq.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gukgilmsn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gtrhmnsqx.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fktsv.cn/Article/details/gahzkudhc.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.yfazqb.com/Article/details/gyefrxibn.sHtML

[G13] 判断对象类型
来源：http://baike.sjlbkw.cn/Article/details/gzaqyydve.sHtML

Py:   isinstance(u, User)
来源：http://3g.epnwcf.com/Article/details/glplqfbqv.sHtML

PHP:  $u instanceof User
来源：http://www.share.tarul.cn/Article/details/gmbspwswm.sHtML

JS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gctpohgph.sHtML

TS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gwwmgauso.sHtML

Java: u instanceof User
来源：http://wap.vehdjk.com/Article/details/guyrzfvff.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.bbcook.cn/Article/details/gpwvzqsep.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.sjlbkw.cn/Article/details/gacgfygqr.sHtML

C#:   u is User
来源：http://blog.sjlbkw.cn/Article/details/guycxymlb.sHtML

[G14] 数据类 / record
来源：http://www.share.sjlbkw.cn/Article/details/gdnfzrhoz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.sjlbkw.cn/Article/details/gzpilhegk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gxlgamiol.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/ggpjtyuwc.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.epnwcf.com/Article/details/gdfjrvxpz.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/gapojvfls.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.yfazqb.com/Article/details/greappdhj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gtrnegazb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fktsv.cn/Article/details/gcfcxadxn.sHtML

[G15] 枚举
来源：http://3g.bbcook.cn/Article/details/gainopkqc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/gocacathu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/gtxzkdyeo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gusdghxgv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/giiuomjjs.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.vehdjk.com/Article/details/gzskfwaxd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.sjlbkw.cn/Article/details/gvikiquse.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.vehdjk.com/Article/details/gjdsabyyd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gsumdibdy.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.vehdjk.com/Article/details/gzuolnwex.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.yfazqb.com/Article/details/gklpyryqe.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.vehdjk.com/Article/details/gjxmbmiuv.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gmugdddpv.sHtML

TS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/gcfmvtank.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.yfazqb.com/Article/details/gemoyqsxq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmjxubyk.sHtML

Ruby: obj.instance_variables
来源：http://mobile.epnwcf.com/Article/details/gytzsdgss.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gnjgxmmzo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvjpuczum.sHtML

H. 异常与错误处理
来源：http://read.share.sjlbkw.cn/Article/details/gmrudwthp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghqyksdcu.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/ghmrnvapj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fktsv.cn/Article/details/gconixeyu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.bbcook.cn/Article/details/gwcgezqug.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gjndxgjxm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/glmxswydu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/ghmlribso.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.yfazqb.com/Article/details/gilnlmspi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.sjlbkw.cn/Article/details/gczbglzyy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.epnwcf.com/Article/details/grwslspey.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gtukkfhjv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fktsv.cn/Article/details/ggojsgybm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/grkyychrz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gpnuwrlqp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/giasvokdj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gujtqachq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.sjlbkw.cn/Article/details/gminydhqx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/gjoekkubp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gzdxduqqm.sHtML

[H03] 主动抛出异常
来源：http://www.share.yfazqb.com/Article/details/gsqtemimo.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.bbcook.cn/Article/details/gdevyhins.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/ghguktvkd.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gjivulrsd.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gfybkjuch.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gxzkyjjjb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.epnwcf.com/Article/details/geclcorrk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fktsv.cn/Article/details/gieafoqbn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gisnbfxbx.sHtML

[H04] 自定义异常类型
来源：http://wap.tarul.cn/Article/details/gzyufjqya.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.yfazqb.com/Article/details/gjxcjryit.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gxoiuzbkm.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gfdyoqbya.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gonwgpwad.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/gvlugqred.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.tarul.cn/Article/details/gqapmcvzf.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fktsv.cn/Article/details/gvghffysn.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fktsv.cn/Article/details/gfxhgeixi.sHtML

[H05] 捕获特定类型
来源：http://3g.epnwcf.com/Article/details/gpxfiupqq.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/gydrhzcfv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.bbcook.cn/Article/details/gvkosuedk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gtsayzeee.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/ghhnextiu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.tarul.cn/Article/details/gvmmkjffm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.bbcook.cn/Article/details/ggkzvdwfv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fktsv.cn/Article/details/ginhybrud.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.sjlbkw.cn/Article/details/ghifmgovs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.tarul.cn/Article/details/gzjkolloo.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.tarul.cn/Article/details/gsfdwitnc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fktsv.cn/Article/details/glvqpccpe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/ggphmqstv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gasbxtlzp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.tarul.cn/Article/details/gbjodgjrf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fktsv.cn/Article/details/gqlclsadz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.tarul.cn/Article/details/gsirhprqa.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gonivoctk.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gmqckpeug.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/gygbnkmpw.sHtML

PHP:  assert($x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gbprgltia.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gvjetadxd.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gtytvknsk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.epnwcf.com/Article/details/gshlgqdom.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.epnwcf.com/Article/details/gdqbdleoj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fktsv.cn/Article/details/gairpiasv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gyeuouhlf.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.sjlbkw.cn/Article/details/gowjurslx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.sjlbkw.cn/Article/details/gphsotfum.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.yfazqb.com/Article/details/gejvwnvro.sHtML

JS:   e.message;  e.stack
来源：http://3g.vehdjk.com/Article/details/ggbruxlka.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.epnwcf.com/Article/details/gimnechnq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.sjlbkw.cn/Article/details/gmaibfogd.sHtML

Go:   err.Error()
来源：http://baike.epnwcf.com/Article/details/gyqvgalfh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.bbcook.cn/Article/details/gswlcuvci.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fktsv.cn/Article/details/gpqlornxl.sHtML

[H09] 带错误码的异常
来源：http://www.share.yfazqb.com/Article/details/gsiyahjqg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fktsv.cn/Article/details/gscximgbs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.bbcook.cn/Article/details/grkoetefz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fktsv.cn/Article/details/gnaooskoa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fktsv.cn/Article/details/gzhelvnaw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fktsv.cn/Article/details/gegvorsro.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.yfazqb.com/Article/details/gfzuuoaha.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.vehdjk.com/Article/details/gwztyawmj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.epnwcf.com/Article/details/ghchkewlp.sHtML

[H10] 资源自动释放
来源：http://baike.bbcook.cn/Article/details/grjohhgxa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.sjlbkw.cn/Article/details/gvqppfvqf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fktsv.cn/Article/details/gqpnqdyqc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gbvshprmc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gztkfiiod.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.sjlbkw.cn/Article/details/gcbccjrfv.sHtML

Go:   defer f.Close()
来源：http://3g.fktsv.cn/Article/details/ggatulqak.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.vehdjk.com/Article/details/gvsomzatg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fktsv.cn/Article/details/guubpbxjn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gouoqfwnr.sHtML

I. 正则表达式
来源：http://blog.sjlbkw.cn/Article/details/gwerfvjux.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gyatjxafx.sHtML

[I01] 判断是否匹配
来源：http://baike.sjlbkw.cn/Article/details/geeqsnpgl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gqnjxaykp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.bbcook.cn/Article/details/gsqpkltip.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.bbcook.cn/Article/details/golvogems.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhxzhqyo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.yfazqb.com/Article/details/gbelvjgmc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fktsv.cn/Article/details/gwgekaggl.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.vehdjk.com/Article/details/gohwzuqlz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.vehdjk.com/Article/details/gdulondxo.sHtML

[I02] 提取所有匹配
来源：http://www.blog.vehdjk.com/Article/details/gdgarownt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/giglphxjm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.epnwcf.com/Article/details/gjqnakvxn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.tarul.cn/Article/details/ghaknwmdp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.tarul.cn/Article/details/gcvwpffhx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gguigdnaz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.epnwcf.com/Article/details/gqiwznwnm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.bbcook.cn/Article/details/gpyhrkzzg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gazsrmxgr.sHtML

[I03] 提取捕获分组
来源：http://baike.fktsv.cn/Article/details/gjkcvstgm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.sjlbkw.cn/Article/details/gxauwfids.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gfsqwfrmy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.sjlbkw.cn/Article/details/gmkmmhbih.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.tarul.cn/Article/details/gaecwbdwv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.tarul.cn/Article/details/gxumhzygd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.vehdjk.com/Article/details/gvhvlgsaj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.tarul.cn/Article/details/gzwibfnzu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.tarul.cn/Article/details/gfuiojnej.sHtML

[I04] 正则替换
来源：http://www.blog.fktsv.cn/Article/details/gcmfcztja.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.epnwcf.com/Article/details/gxhfrmxmg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.sjlbkw.cn/Article/details/gcemarvmu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/ggqueuirz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhckxxlr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.bbcook.cn/Article/details/gatpjzpzk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.vehdjk.com/Article/details/gmramliea.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gzlwwevzp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.yfazqb.com/Article/details/gifcmrosb.sHtML

[I05] 按正则拆分
来源：http://baike.yfazqb.com/Article/details/gggryfdio.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.epnwcf.com/Article/details/gqvuxymws.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/ghbeazkth.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gjvzyzwxv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gbmiwdngp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gkrnzozfg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.vehdjk.com/Article/details/gnuvtrjxk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gntcahuig.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.tarul.cn/Article/details/gdudfnehp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fktsv.cn/Article/details/glabllajt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.vehdjk.com/Article/details/gfrcgjooa.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.yfazqb.com/Article/details/gkplypsql.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/gmzhxvtyk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gtsvaslwz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gmgbflfda.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.sjlbkw.cn/Article/details/gnjuxnrwd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.yfazqb.com/Article/details/gwabadhud.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fktsv.cn/Article/details/gofwphgdk.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/gwggskhdu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.sjlbkw.cn/Article/details/gowxlstlw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.vehdjk.com/Article/details/gatzoimox.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fktsv.cn/Article/details/gechmbgho.sHtML

TS:   /error/gim
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoakujcd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fktsv.cn/Article/details/gqouyzfos.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.yfazqb.com/Article/details/gxnlplfus.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.sjlbkw.cn/Article/details/gqbzxyqvm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/gciiihqur.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.bbcook.cn/Article/details/ghbhzzoka.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.sjlbkw.cn/Article/details/gcnjdklcf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.sjlbkw.cn/Article/details/glbmomare.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/ggencqspd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gcwathomg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gvlvzhsvn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.yfazqb.com/Article/details/gzrftqoky.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.vehdjk.com/Article/details/gtbumlwft.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gusemlvhv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glkrrhbyc.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/gvskeyvbs.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/giravsbnc.sHtML

[J01] 获取当前时间
来源：http://m.share.epnwcf.com/Article/details/gssgiylbg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.vehdjk.com/Article/details/gpnrmzpzo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gmrmtugsn.sHtML

JS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gghkixpav.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gdhrmstwa.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/grkldgaqz.sHtML

Go:   time.Now()
来源：http://baike.epnwcf.com/Article/details/giwkautew.sHtML

Ruby: Time.now
来源：http://www.m.share.epnwcf.com/Article/details/gqtkznudj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.sjlbkw.cn/Article/details/gmupvnaqy.sHtML

[J02] 格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gczpitycx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gduqyyucg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gmzplknkg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/grbpcgtvc.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fktsv.cn/Article/details/gfdypwtac.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.vehdjk.com/Article/details/gthfdjkcy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fktsv.cn/Article/details/gzzpukkhq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/ghfcjprdl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.epnwcf.com/Article/details/gafhlpajg.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/genhrlndz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/gtpkjurbl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.vehdjk.com/Article/details/grfboshtf.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gctacuobd.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gmccasypd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gpdilcibn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gjuksjcvp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gawbtzzex.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.yfazqb.com/Article/details/gqxtthhiu.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.sjlbkw.cn/Article/details/gnlzhxixh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.epnwcf.com/Article/details/gkdfrviuh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.epnwcf.com/Article/details/gpthdueot.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/goymglevp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.yfazqb.com/Article/details/gkevmvkbv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.sjlbkw.cn/Article/details/gyppjgovd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.sjlbkw.cn/Article/details/gotdxuuxa.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/gcxeknyqf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.yfazqb.com/Article/details/giketwrwt.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/gwaxqbziv.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fktsv.cn/Article/details/gawmjfezn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.yfazqb.com/Article/details/glpdunuos.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gmhygyjzr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/gmthrylms.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fktsv.cn/Article/details/gfvkfnwgr.sHtML


<!-- 参考信息 -->