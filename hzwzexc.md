代发 wailian999

Py:   class User: pass
来源：http://www.m.share.yfazqb.com/Article/details/gjkzqlira.sHtML

PHP:  class User {}
来源：http://wap.fktsv.cn/Article/details/gxycwonmh.sHtML

JS:   class User {}
来源：http://blog.bbcook.cn/Article/details/gfiayxguu.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/gkczpzmsh.sHtML

Java: class User {}
来源：http://read.share.bbcook.cn/Article/details/ggeskwvpf.sHtML

Go:   type User struct { Name string }
来源：http://www.share.bbcook.cn/Article/details/gpqwuauqv.sHtML

Ruby: class User; end
来源：http://3g.yfazqb.com/Article/details/glnecjwpu.sHtML

C#:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gxpyrldbu.sHtML

[G02] 构造函数
来源：http://www.blog.tarul.cn/Article/details/gbkfaujar.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.tarul.cn/Article/details/gxqrifkfo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.bbcook.cn/Article/details/gifuxcnux.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gaavclsbq.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fktsv.cn/Article/details/gfjgwqppx.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gumnjefdw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.epnwcf.com/Article/details/ghjimznpm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/gomablxyh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/guvklyokt.sHtML

[G03] 实例属性
来源：http://www.blog.fktsv.cn/Article/details/gpowmqbev.sHtML

Py:   self.name = "x"
来源：http://3g.fktsv.cn/Article/details/gkkszhwcf.sHtML

PHP:  public string $name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gujptamut.sHtML

JS:   this.name = "x";
来源：http://read.share.epnwcf.com/Article/details/gnxtjamef.sHtML

TS:   name: string = "x";
来源：http://blog.tarul.cn/Article/details/gfdghdzzu.sHtML

Java: private String name;
来源：http://wap.bbcook.cn/Article/details/gsutwdpif.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.sjlbkw.cn/Article/details/gpqytzlxu.sHtML

Ruby: @name = "x"
来源：http://mobile.vehdjk.com/Article/details/gzrutgizc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.vehdjk.com/Article/details/gbvmqpbaz.sHtML

[G04] 定义方法
来源：http://wap.bbcook.cn/Article/details/garzokquv.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gjqlgrhit.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gpikdadwg.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gfqgykpyj.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gmtrsxpoz.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gkxagfczl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/grgufrviz.sHtML

Ruby: def greet; @name; end
来源：http://blog.sjlbkw.cn/Article/details/gbywwpskf.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/gewjgijzs.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/gbyppfvwi.sHtML

Py:   class Admin(User): pass
来源：http://blog.vehdjk.com/Article/details/gszmgfifw.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/grlmtyffc.sHtML

JS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gcrxiuypn.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gkqiovfyc.sHtML

Java: class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gvueaesrz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.vehdjk.com/Article/details/gteusqunq.sHtML

Ruby: class Admin < User; end
来源：http://read.share.yfazqb.com/Article/details/grvhwbzkz.sHtML

C#:   class Admin : User {}
来源：http://m.share.vehdjk.com/Article/details/gxojmsklf.sHtML

[G06] 重写方法
来源：http://www.share.tarul.cn/Article/details/gkjtyfmlq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gqdgcxhth.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/guuntjcwk.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gxzefqzcu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gwrgycgjd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gqwgdeekt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwtpefta.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.sjlbkw.cn/Article/details/gplwnkrxo.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.epnwcf.com/Article/details/gopeiittb.sHtML

[G07] 调用父类方法
来源：http://wap.vehdjk.com/Article/details/ginrrvkfy.sHtML

Py:   super().greet()
来源：http://mobile.yfazqb.com/Article/details/gxfalypxj.sHtML

PHP:  parent::greet();
来源：http://mobile.epnwcf.com/Article/details/gmasmhcda.sHtML

JS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gfvjeblej.sHtML

TS:   super.greet();
来源：http://baike.tarul.cn/Article/details/glllqbwwj.sHtML

Java: super.greet();
来源：http://wap.bbcook.cn/Article/details/gpsaiabyo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.yfazqb.com/Article/details/gieokaott.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/geevlejbe.sHtML

C#:   base.Greet();
来源：http://blog.sjlbkw.cn/Article/details/gtfijvcrz.sHtML

[G08] 静态方法与属性
来源：http://mobile.tarul.cn/Article/details/gsayozdtk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fktsv.cn/Article/details/gaqpdoiud.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/gwrfolppt.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gmgzgjsxc.sHtML

TS:   static f(): void {}
来源：http://blog.bbcook.cn/Article/details/grpomcknt.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gguikgvon.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.tarul.cn/Article/details/gtglqhlsd.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/gwdungvcb.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/gpnxpatqn.sHtML

[G09] 接口 / 抽象类
来源：http://wap.yfazqb.com/Article/details/gdbsnudev.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fktsv.cn/Article/details/gqqtbjrhq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/gddrnkdfh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.tarul.cn/Article/details/gfnaihros.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.epnwcf.com/Article/details/gsplmojij.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fktsv.cn/Article/details/gqykhsvpd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.epnwcf.com/Article/details/gknofcwis.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.sjlbkw.cn/Article/details/gwxqddrik.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/gmnzqgdeq.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gginljxqx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.vehdjk.com/Article/details/gvllszawf.sHtML

PHP:  public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gojzrynoo.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fktsv.cn/Article/details/gczusdint.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gqdeszwxj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/glpyouoof.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/gmpmrccde.sHtML

Ruby: public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/grbqbkwrt.sHtML

C#:   public / protected / private / internal
来源：http://baike.vehdjk.com/Article/details/gtyfghduw.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gnrglctsd.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/godwglydi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gsvmbohxp.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gezgrfoeq.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gsytrjcnp.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/giqkyoapt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gylcxqdmv.sHtML

Ruby: attr_accessor :name
来源：http://wap.fktsv.cn/Article/details/gbyxiyxwz.sHtML

C#:   public string Name { get; set; }
来源：http://blog.bbcook.cn/Article/details/gbqulxtcy.sHtML

[G12] 对象转字符串
来源：http://mobile.vehdjk.com/Article/details/geluofdgc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/grfmdtdwo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gkkimpdnl.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gasbncnvr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gevqimshl.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fktsv.cn/Article/details/gebrxqykt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzpulfrf.sHtML

Ruby: def to_s; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gwmnhxerp.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.bbcook.cn/Article/details/gfveksdea.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/gdiqhtgpx.sHtML

Py:   isinstance(u, User)
来源：http://wap.vehdjk.com/Article/details/gzluwuhqh.sHtML

PHP:  $u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gqnoufuxx.sHtML

JS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gyokzafut.sHtML

TS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gplqbbxge.sHtML

Java: u instanceof User
来源：http://wap.fktsv.cn/Article/details/guxxkptov.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.epnwcf.com/Article/details/gvhfcjixp.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/gexsjrkyr.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/gqxhhpuua.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/gfzpgnfox.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.epnwcf.com/Article/details/gahkfoodl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.bbcook.cn/Article/details/glcydrixr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.sjlbkw.cn/Article/details/gehjlqrli.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.bbcook.cn/Article/details/gbisoivrl.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fktsv.cn/Article/details/giorncnnq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.vehdjk.com/Article/details/gmcwdcwcz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.tarul.cn/Article/details/gtersdlqe.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.sjlbkw.cn/Article/details/gosvbzftm.sHtML

[G15] 枚举
来源：http://3g.yfazqb.com/Article/details/gxkznudeb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/gjprqihba.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.sjlbkw.cn/Article/details/gletswanz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.yfazqb.com/Article/details/gjdmfxesq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gravgqebf.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/gxbmfausn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.epnwcf.com/Article/details/gxkbceciz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.tarul.cn/Article/details/gtngmllsb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gvankrefn.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/gofkwsgcl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.vehdjk.com/Article/details/gzgxoukwy.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/gcjgduujr.sHtML

JS:   Object.entries(obj)
来源：http://baike.yfazqb.com/Article/details/ggffglwvw.sHtML

TS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gqlqbtnve.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.yfazqb.com/Article/details/gumosvtda.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.yfazqb.com/Article/details/gmweyyndc.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.sjlbkw.cn/Article/details/gmofbliis.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gxwatzlzq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtomtvrvi.sHtML

H. 异常与错误处理
来源：http://3g.fktsv.cn/Article/details/gosrjyflo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjmdpkkxs.sHtML

[H01] try / catch 基础
来源：http://www.share.bbcook.cn/Article/details/gzzgveehy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gacqfmwdb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.yfazqb.com/Article/details/gjhimzssp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/ggnfxlmpq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gsvpeqqzz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fktsv.cn/Article/details/gcyvpktys.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.yfazqb.com/Article/details/gzyntlgqn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.vehdjk.com/Article/details/gyprpukmd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/ghyxnlkka.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.yfazqb.com/Article/details/gmqepfnem.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.epnwcf.com/Article/details/gfrwthlfz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/ggzhauoxj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gadubnzgv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gmotgmnmj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gatytazrg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.bbcook.cn/Article/details/gfvtttscu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.epnwcf.com/Article/details/ghqoqaggs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gllamghlj.sHtML

[H03] 主动抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gvpjpppbv.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.yfazqb.com/Article/details/grtpxllfk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gowdtejyd.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gdxqbbruz.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gctbyhaqt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gadjssrvv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.tarul.cn/Article/details/goanxmtkz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.bbcook.cn/Article/details/gaeogtoye.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gfyittgkh.sHtML

[H04] 自定义异常类型
来源：http://www.blog.bbcook.cn/Article/details/gycsjdevq.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.epnwcf.com/Article/details/gsmtenfjh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/gqrfihtgh.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/gxldpymya.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/glmsjbqlo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gubhhwlzo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.tarul.cn/Article/details/gihvsdrhc.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gnsrgnoyp.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.yfazqb.com/Article/details/gagmkvqsf.sHtML

[H05] 捕获特定类型
来源：http://mobile.fktsv.cn/Article/details/gluiwgncp.sHtML

Py:   except ValueError as e:
来源：http://blog.vehdjk.com/Article/details/gmxinfdmk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.vehdjk.com/Article/details/gebaqayfk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gnjhcqybw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.sjlbkw.cn/Article/details/gkczalvjv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.sjlbkw.cn/Article/details/gatrttsjw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.yfazqb.com/Article/details/gkxmrxeum.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fktsv.cn/Article/details/gykbhpvmp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.epnwcf.com/Article/details/gqhfnekux.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.bbcook.cn/Article/details/ggjdbujsw.sHtML

Py:   value = d.get("k") or default
来源：http://baike.yfazqb.com/Article/details/gkazlhbte.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/gomjrvwiu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/grtcfgjgt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gxtdrlwna.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gwdlrmigv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.tarul.cn/Article/details/gprackbei.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.yfazqb.com/Article/details/gztgjpldu.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.tarul.cn/Article/details/gqprcqhlu.sHtML

[H07] 断言
来源：http://blog.yfazqb.com/Article/details/glqkdjxhh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.vehdjk.com/Article/details/gnywcvucr.sHtML

PHP:  assert($x > 0);
来源：http://wap.tarul.cn/Article/details/gtpbegppf.sHtML

JS:   console.assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/gdchqknrt.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gxxkvytog.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.vehdjk.com/Article/details/gwyhiwkau.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.yfazqb.com/Article/details/gdcdctzyt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.tarul.cn/Article/details/galapxtkf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gpfjzcilc.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.bbcook.cn/Article/details/gvghnjyek.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.yfazqb.com/Article/details/gfxgevuvq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fktsv.cn/Article/details/gsgaznbpq.sHtML

JS:   e.message;  e.stack
来源：http://baike.bbcook.cn/Article/details/gzlzdwovh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.epnwcf.com/Article/details/gbyimdrbz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.epnwcf.com/Article/details/gzpptuwvu.sHtML

Go:   err.Error()
来源：http://blog.fktsv.cn/Article/details/gbkmrsmoc.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.yfazqb.com/Article/details/gdjdnnuta.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.epnwcf.com/Article/details/gknasujvy.sHtML

[H09] 带错误码的异常
来源：http://www.share.bbcook.cn/Article/details/gzgitnmoz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gbpuvoefi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.tarul.cn/Article/details/gdjsgdtsp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.sjlbkw.cn/Article/details/gfpcwgsvj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.yfazqb.com/Article/details/ghfyadxlh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.sjlbkw.cn/Article/details/ghcqkeulq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fktsv.cn/Article/details/gamxogjro.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.sjlbkw.cn/Article/details/gblukccks.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.tarul.cn/Article/details/gqahotnri.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/grecsktit.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fktsv.cn/Article/details/gzqxkcvgw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.vehdjk.com/Article/details/gahwqwymh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/ggipeordp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/gfdzxfmio.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.vehdjk.com/Article/details/grlrivabg.sHtML

Go:   defer f.Close()
来源：http://www.blog.epnwcf.com/Article/details/glhviiocu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.tarul.cn/Article/details/gtkogesib.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gztgbwjld.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gugtqmudk.sHtML

I. 正则表达式
来源：http://wap.epnwcf.com/Article/details/gdqzpnmlm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gydfbqmwd.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.epnwcf.com/Article/details/gayyocuxf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/grurrefnu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/gokxqaizp.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gqhyqziog.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fktsv.cn/Article/details/gtbrbnrti.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.vehdjk.com/Article/details/grggyvmcm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/gzvpmulwh.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gbqymnxzo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.tarul.cn/Article/details/gwjpnjrtr.sHtML

[I02] 提取所有匹配
来源：http://read.share.epnwcf.com/Article/details/gvfjlsvoh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gqlfxsnkm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.yfazqb.com/Article/details/gtssleduw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.bbcook.cn/Article/details/gvngrtgpu.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.tarul.cn/Article/details/gmtnhyemq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.tarul.cn/Article/details/gwxqhfbal.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.vehdjk.com/Article/details/gbfsejveg.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.vehdjk.com/Article/details/gnvrursdj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.vehdjk.com/Article/details/glwpwhrxc.sHtML

[I03] 提取捕获分组
来源：http://mobile.tarul.cn/Article/details/gxfaifbpl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.bbcook.cn/Article/details/gcfjlqgbr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.epnwcf.com/Article/details/gncqozect.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gpntrgcok.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.tarul.cn/Article/details/grgbxpuzv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.bbcook.cn/Article/details/gitpqobes.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.vehdjk.com/Article/details/ggefkuuyw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.bbcook.cn/Article/details/gyfsnnphv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.epnwcf.com/Article/details/ghlkkkbrd.sHtML

[I04] 正则替换
来源：http://read.share.fktsv.cn/Article/details/gymbstfrm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fktsv.cn/Article/details/gtjscfsio.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gfzcegvjs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/gvunuhkco.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/gilxfykzx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gqwrbdwkg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.vehdjk.com/Article/details/gpobqxqac.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.tarul.cn/Article/details/gaqwdfcrs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/gqpkcucva.sHtML

[I05] 按正则拆分
来源：http://www.m.share.vehdjk.com/Article/details/gfdmbkwbk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.tarul.cn/Article/details/gitnxudra.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fktsv.cn/Article/details/ghvqurbhh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gtfmlumpg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gvqntogey.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.bbcook.cn/Article/details/gafzsajtg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fktsv.cn/Article/details/ggvpxlycl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gmqlbebuh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxgxritt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.bbcook.cn/Article/details/gmauhxwbo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gnlhtmmgh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.yfazqb.com/Article/details/givyumaop.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/ghsymgkdf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.yfazqb.com/Article/details/gmgushnwk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/girpsingw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fktsv.cn/Article/details/gqdhgxvqx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.bbcook.cn/Article/details/gsjfsjyhr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gvkjgpvbr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.vehdjk.com/Article/details/gruhxarfa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.sjlbkw.cn/Article/details/geciukucf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gniwxojun.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.bbcook.cn/Article/details/gsmftpsrn.sHtML

TS:   /error/gim
来源：http://blog.epnwcf.com/Article/details/gfhgssrnl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.sjlbkw.cn/Article/details/gzwfhwklq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/ghbiopemh.sHtML


<!-- 参考信息 -->