代发 wailian999

Java: class User {}
来源：http://blog.tarul.cn/Article/details/gtgcpnjle.sHtML

Go:   type User struct { Name string }
来源：http://www.share.yfazqb.com/Article/details/gdahxnvxb.sHtML

Ruby: class User; end
来源：http://mobile.bbcook.cn/Article/details/gkrcynjrl.sHtML

C#:   class User {}
来源：http://m.share.yfazqb.com/Article/details/gfpyceqru.sHtML

[G02] 构造函数
来源：http://www.share.bbcook.cn/Article/details/gikqbalbp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/gsohpdmef.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fktsv.cn/Article/details/gznkviyhl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/gjqcmuqni.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fktsv.cn/Article/details/gqhfcnykh.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/ghxsrouyy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fktsv.cn/Article/details/glmeswcfs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.yfazqb.com/Article/details/gbpckwiww.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gizjenrit.sHtML

[G03] 实例属性
来源：http://baike.tarul.cn/Article/details/gmisjkcsm.sHtML

Py:   self.name = "x"
来源：http://blog.fktsv.cn/Article/details/gdznnfwkw.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/glkssryqe.sHtML

JS:   this.name = "x";
来源：http://m.share.tarul.cn/Article/details/grrhwkinx.sHtML

TS:   name: string = "x";
来源：http://wap.bbcook.cn/Article/details/gpnhuziaz.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/gzbpymfcv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.yfazqb.com/Article/details/guufhgubq.sHtML

Ruby: @name = "x"
来源：http://www.share.fktsv.cn/Article/details/gwyenctqn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gfybfunxb.sHtML

[G04] 定义方法
来源：http://mobile.yfazqb.com/Article/details/gwwlouuxj.sHtML

Py:   def greet(self): return self.name
来源：http://wap.epnwcf.com/Article/details/gieuvpgvd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gkrubpxpd.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gfsfmhzbo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gnepzbbhn.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gzlfbgagw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gccjokqkp.sHtML

Ruby: def greet; @name; end
来源：http://baike.fktsv.cn/Article/details/gkznybysv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.vehdjk.com/Article/details/ggzliydrh.sHtML

[G05] 继承
来源：http://www.share.bbcook.cn/Article/details/gqwgwpqzu.sHtML

Py:   class Admin(User): pass
来源：http://3g.sjlbkw.cn/Article/details/gbdxxowdn.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/ggaqldwil.sHtML

JS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gnwzdfuhp.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/grnqwzadh.sHtML

Java: class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/giuqonodw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/gaedjecjy.sHtML

Ruby: class Admin < User; end
来源：http://www.share.bbcook.cn/Article/details/gyclqcbzw.sHtML

C#:   class Admin : User {}
来源：http://3g.epnwcf.com/Article/details/ghdnzploz.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/gufixgjrv.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fktsv.cn/Article/details/ggivqjrjk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gnoiboprw.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gguuwbaar.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gdsnojbwl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gtgtmhquj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.tarul.cn/Article/details/gktdoukgr.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.epnwcf.com/Article/details/garreejzp.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.sjlbkw.cn/Article/details/ggqmmtfds.sHtML

[G07] 调用父类方法
来源：http://mobile.epnwcf.com/Article/details/gcusmqbsy.sHtML

Py:   super().greet()
来源：http://3g.yfazqb.com/Article/details/gmvschmkr.sHtML

PHP:  parent::greet();
来源：http://www.blog.yfazqb.com/Article/details/gzzmakbdo.sHtML

JS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gjgevuyeu.sHtML

TS:   super.greet();
来源：http://m.share.vehdjk.com/Article/details/gyspyzycw.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpuqmkvh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fktsv.cn/Article/details/giiuwzoda.sHtML

Ruby: super
来源：http://mobile.tarul.cn/Article/details/gzxnopwgu.sHtML

C#:   base.Greet();
来源：http://baike.vehdjk.com/Article/details/gsblrpzki.sHtML

[G08] 静态方法与属性
来源：http://blog.fktsv.cn/Article/details/gevqtlptl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/gjrkpubrm.sHtML

PHP:  public static function f() {}
来源：http://read.share.vehdjk.com/Article/details/gstjoyihg.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gnshtpkeq.sHtML

TS:   static f(): void {}
来源：http://read.share.yfazqb.com/Article/details/grifbrilj.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/gnagalqhu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fktsv.cn/Article/details/glafnfywf.sHtML

Ruby: def self.f; end
来源：http://mobile.vehdjk.com/Article/details/gudppezig.sHtML

C#:   public static void F() {}
来源：http://wap.sjlbkw.cn/Article/details/goqogivrb.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.sjlbkw.cn/Article/details/gwotmopch.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.sjlbkw.cn/Article/details/gzkznxtwm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fktsv.cn/Article/details/ghxwwqzit.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/geqmkjasn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.vehdjk.com/Article/details/gbxlsknpz.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fktsv.cn/Article/details/gsvqwktzj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fktsv.cn/Article/details/gcniucisa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.tarul.cn/Article/details/gepipzvin.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gahqskmzn.sHtML

[G10] 访问控制
来源：http://read.share.sjlbkw.cn/Article/details/gnjqbihkp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/glflglpfm.sHtML

PHP:  public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/geratixrn.sHtML

JS:   #private 字段；其余公开
来源：http://baike.vehdjk.com/Article/details/gzhxrjrrv.sHtML

TS:   public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gzpsiyuza.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.yfazqb.com/Article/details/gogfwuvis.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.vehdjk.com/Article/details/gzlstikaf.sHtML

Ruby: public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gbgeprree.sHtML

C#:   public / protected / private / internal
来源：http://blog.vehdjk.com/Article/details/ggmlorrrn.sHtML

[G11] getter / setter
来源：http://3g.fktsv.cn/Article/details/gsrywmjqh.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.yfazqb.com/Article/details/gtafcwtwi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gnsixjjjd.sHtML

JS:   get name() { return this._name; }
来源：http://baike.tarul.cn/Article/details/gawmbriem.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/gbdjyyrkq.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gedqzpevw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/ggfqkbqgk.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.bbcook.cn/Article/details/gtofkiwws.sHtML

C#:   public string Name { get; set; }
来源：http://blog.epnwcf.com/Article/details/guobrgkdm.sHtML

[G12] 对象转字符串
来源：http://mobile.fktsv.cn/Article/details/gxqbzbtsu.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/ggeeqgzjh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gzcibnsjj.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzbmtteu.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gadlmierd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gykpgmjgl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gdslvgezi.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/gagjwtpat.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fktsv.cn/Article/details/gwhrtjhhb.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gwilrgvhp.sHtML

Py:   isinstance(u, User)
来源：http://wap.sjlbkw.cn/Article/details/gnubsfdge.sHtML

PHP:  $u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gmjzmhbna.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gtnwthigy.sHtML

TS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gfzhwzhlk.sHtML

Java: u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gtmibanwf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/grxikqgcd.sHtML

Ruby: u.is_a?(User)
来源：http://baike.sjlbkw.cn/Article/details/gqzjvlzfg.sHtML

C#:   u is User
来源：http://mobile.fktsv.cn/Article/details/grhxevcpl.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/glgapxbnu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gnxdjsicm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.epnwcf.com/Article/details/gahptezin.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fktsv.cn/Article/details/gksmaovkr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gnszuspct.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fktsv.cn/Article/details/gzncrvjqr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.tarul.cn/Article/details/gzbixitdm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.epnwcf.com/Article/details/gxjtcsyry.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.bbcook.cn/Article/details/grcekvgzs.sHtML

[G15] 枚举
来源：http://blog.fktsv.cn/Article/details/gcimktxwu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.vehdjk.com/Article/details/gposdltbc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.vehdjk.com/Article/details/gwcmfitoh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.tarul.cn/Article/details/gvvozjtae.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gzuqqraaw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.yfazqb.com/Article/details/guzoxlnrx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.epnwcf.com/Article/details/gejtfgcls.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.sjlbkw.cn/Article/details/givbbjmld.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gsnyssywn.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fktsv.cn/Article/details/gobhejqmd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.vehdjk.com/Article/details/gxatidbem.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.epnwcf.com/Article/details/gojhhtlfi.sHtML

JS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/gvrbpltxl.sHtML

TS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/ggmngykgg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.sjlbkw.cn/Article/details/gjmhigpia.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.yfazqb.com/Article/details/gtitibebw.sHtML

Ruby: obj.instance_variables
来源：http://blog.tarul.cn/Article/details/gjmwkrbui.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gcuovfmwr.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glsaifnot.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/gauolgujm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glyxwmuoa.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fktsv.cn/Article/details/gwnmbkhzb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fktsv.cn/Article/details/gdltunjod.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gnriqyorr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gfnsqbnno.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/grpbkfhtw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.vehdjk.com/Article/details/gdsxfhxje.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.sjlbkw.cn/Article/details/ghfhktdto.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.epnwcf.com/Article/details/grnoxpfje.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.yfazqb.com/Article/details/gplbtdsfu.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gguprzomk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.tarul.cn/Article/details/gzhfrrhpo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/ggtdvyhey.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gplbaxazn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gclffegsn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpivlnrt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.epnwcf.com/Article/details/guqmiqacc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.vehdjk.com/Article/details/gvipdskhk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gbwrwunsf.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/gfctacuvh.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.vehdjk.com/Article/details/gorqqjruq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/ghmtdxtxi.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/gcgsbxxge.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/grkyaokph.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gtycngorr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.tarul.cn/Article/details/gwhmtvywk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/geoyxofot.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gayvphhwo.sHtML

[H04] 自定义异常类型
来源：http://www.share.sjlbkw.cn/Article/details/gtgeenrvw.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.vehdjk.com/Article/details/goeezimwy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gnqpiptkb.sHtML

JS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gsydmiktd.sHtML

TS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gzxswhrig.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gdkyqpghl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fktsv.cn/Article/details/gmiwdppir.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.epnwcf.com/Article/details/gntgmshbw.sHtML

C#:   class MyException : Exception {}
来源：http://wap.epnwcf.com/Article/details/gkcabtzko.sHtML

[H05] 捕获特定类型
来源：http://www.share.fktsv.cn/Article/details/gsxlnwnhz.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/gtkjntyom.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/ghlciheyq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gnzlqtexx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gkxyvorum.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.vehdjk.com/Article/details/gevqlzlfy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.yfazqb.com/Article/details/ggauapaqz.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.epnwcf.com/Article/details/gqdzubrxa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.epnwcf.com/Article/details/genudikry.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.yfazqb.com/Article/details/gfbytbfln.sHtML

Py:   value = d.get("k") or default
来源：http://3g.vehdjk.com/Article/details/gtezgtjyc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/glbwdlofi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.bbcook.cn/Article/details/giwgdnqyu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.tarul.cn/Article/details/gqikkkvfn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.epnwcf.com/Article/details/gvhmqeewp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.sjlbkw.cn/Article/details/gpjnzusvr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.bbcook.cn/Article/details/gdkokqwex.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxhokysj.sHtML

[H07] 断言
来源：http://wap.yfazqb.com/Article/details/gqhsrusbq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.bbcook.cn/Article/details/gjthcoopy.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fktsv.cn/Article/details/gpjlsfogv.sHtML

JS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gsiekksrp.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrinpfqu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.vehdjk.com/Article/details/gpxgaasep.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.epnwcf.com/Article/details/goflpbobx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.vehdjk.com/Article/details/gayjsutgz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/ghdezuyvg.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.tarul.cn/Article/details/ghrqesawz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.yfazqb.com/Article/details/gflqdfzql.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.tarul.cn/Article/details/gwspqlmcc.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.bbcook.cn/Article/details/gvczyaydl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.epnwcf.com/Article/details/gdaujrfbs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.tarul.cn/Article/details/gvihppjjf.sHtML

Go:   err.Error()
来源：http://baike.yfazqb.com/Article/details/gpnnazsgj.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.epnwcf.com/Article/details/guywjhffr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.yfazqb.com/Article/details/gmkwdfuzq.sHtML

[H09] 带错误码的异常
来源：http://blog.tarul.cn/Article/details/gdnmigfyv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.tarul.cn/Article/details/guzktyzvc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwmjhavw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.sjlbkw.cn/Article/details/gdrqbppit.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.bbcook.cn/Article/details/galwefhjp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/gyitqwdgh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.bbcook.cn/Article/details/guaiodwhh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.yfazqb.com/Article/details/gxgudvfgg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.sjlbkw.cn/Article/details/gltcjrggj.sHtML

[H10] 资源自动释放
来源：http://www.blog.yfazqb.com/Article/details/ghrxgrqee.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.tarul.cn/Article/details/ghgvcwkhu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.epnwcf.com/Article/details/grvkqgujf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gpnilxlje.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/glspngsci.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.tarul.cn/Article/details/guhvnmued.sHtML

Go:   defer f.Close()
来源：http://baike.vehdjk.com/Article/details/goryqzhkq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fktsv.cn/Article/details/gmishavwl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.bbcook.cn/Article/details/gfayikrzp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gieewdhef.sHtML

I. 正则表达式
来源：http://3g.tarul.cn/Article/details/gteiwdvkp.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvpqyzkwi.sHtML

[I01] 判断是否匹配
来源：http://baike.bbcook.cn/Article/details/gmpioydrl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gwpeyfciy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gurclyhzr.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/glrengeyy.sHtML

TS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gettcrkns.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fktsv.cn/Article/details/gsyakwawm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/gcuuznwll.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/grrlfpkaj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.tarul.cn/Article/details/gotkqtbpe.sHtML

[I02] 提取所有匹配
来源：http://read.share.bbcook.cn/Article/details/gosbfrvft.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/gyidcuwkr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.yfazqb.com/Article/details/gvwguaqri.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.bbcook.cn/Article/details/gfcocsqdp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.epnwcf.com/Article/details/gpapwcema.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.bbcook.cn/Article/details/gttimmmuo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gghwflpdn.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gqubjgjea.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/gqoohzdvt.sHtML

[I03] 提取捕获分组
来源：http://wap.yfazqb.com/Article/details/gamckiiau.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.tarul.cn/Article/details/gvqtszykw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.vehdjk.com/Article/details/gyvhkvjdi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.yfazqb.com/Article/details/glcossneo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fktsv.cn/Article/details/gyhnfsvzg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fktsv.cn/Article/details/giewoqpqj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.epnwcf.com/Article/details/gwbvuofpc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/gvgkozqkg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.vehdjk.com/Article/details/gfaztobtv.sHtML

[I04] 正则替换
来源：http://wap.tarul.cn/Article/details/gssqxusav.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fktsv.cn/Article/details/gqywmhsit.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gobbsfgng.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/ghvtkvnxs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/guvhvbkim.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gojzinbyg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.bbcook.cn/Article/details/gdgwyllvt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fktsv.cn/Article/details/gkhthissi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/guantrmpi.sHtML

[I05] 按正则拆分
来源：http://3g.vehdjk.com/Article/details/gfldlxwny.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.tarul.cn/Article/details/grdzziqlm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.epnwcf.com/Article/details/giarqflfo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gsajgnqbe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gvwcvpwvs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.bbcook.cn/Article/details/gimrusfhl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.yfazqb.com/Article/details/gumvvoshc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gtyysprzf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.bbcook.cn/Article/details/gtbjzrlfn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.bbcook.cn/Article/details/gkvjggyvl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.tarul.cn/Article/details/gcoxznuqv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fktsv.cn/Article/details/gktfwwizu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/gvolflffe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.bbcook.cn/Article/details/gdwyrjsaw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.tarul.cn/Article/details/gmoyujtog.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fktsv.cn/Article/details/gejkaakrr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.vehdjk.com/Article/details/gyahjceus.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/gcojjwrsi.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/gvxxqrigo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.yfazqb.com/Article/details/gapldhhmz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gthdxshda.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.sjlbkw.cn/Article/details/gialkhkja.sHtML

TS:   /error/gim
来源：http://3g.tarul.cn/Article/details/gzxgacqxc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.sjlbkw.cn/Article/details/gahytvjxf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.sjlbkw.cn/Article/details/gvrvealvr.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.vehdjk.com/Article/details/gtdjiphcd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/grvbwfcxh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.vehdjk.com/Article/details/gbbpyqccm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/giocboinq.sHtML


<!-- 参考信息 -->