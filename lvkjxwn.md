代发 wailian999

Py:   class User: pass
来源：http://www.m.share.yfazqb.com/Article/details/gouybimyg.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/gidqkeqiz.sHtML

JS:   class User {}
来源：http://www.share.epnwcf.com/Article/details/gjjdrbfgv.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.sjlbkw.cn/Article/details/gjkbmwnjp.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/gxlealcop.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/gafobkyry.sHtML

Ruby: class User; end
来源：http://blog.fktsv.cn/Article/details/gridhnxtf.sHtML

C#:   class User {}
来源：http://baike.tarul.cn/Article/details/grqzmxmei.sHtML

[G02] 构造函数
来源：http://baike.epnwcf.com/Article/details/gvemobjum.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fktsv.cn/Article/details/gwuwarjuz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gybrmpfbf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gouzfdpqv.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.bbcook.cn/Article/details/gccozauwg.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/gersazetz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.vehdjk.com/Article/details/gnophwcrr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.bbcook.cn/Article/details/grsmdumgz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/ghbtdmkws.sHtML

[G03] 实例属性
来源：http://mobile.sjlbkw.cn/Article/details/gvweebmgs.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/grgtkefkn.sHtML

PHP:  public string $name = "x";
来源：http://mobile.vehdjk.com/Article/details/goryjvqzg.sHtML

JS:   this.name = "x";
来源：http://mobile.yfazqb.com/Article/details/gcwjllcqs.sHtML

TS:   name: string = "x";
来源：http://m.share.vehdjk.com/Article/details/gtlprblac.sHtML

Java: private String name;
来源：http://mobile.epnwcf.com/Article/details/gyvgqtqcg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gtevfsucg.sHtML

Ruby: @name = "x"
来源：http://m.share.bbcook.cn/Article/details/gnoxhafwh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/gxbwvhrqa.sHtML

[G04] 定义方法
来源：http://wap.sjlbkw.cn/Article/details/gnovfukju.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gygxosdfa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/geiwtifcy.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gqtuoewoc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gwwdaosfr.sHtML

Java: String greet() { return name; }
来源：http://wap.yfazqb.com/Article/details/gjgisjzvv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gztieylil.sHtML

Ruby: def greet; @name; end
来源：http://mobile.bbcook.cn/Article/details/ghnwlaity.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/giirywohu.sHtML

[G05] 继承
来源：http://www.blog.sjlbkw.cn/Article/details/gutjvnyfa.sHtML

Py:   class Admin(User): pass
来源：http://read.share.vehdjk.com/Article/details/gdzzjgcee.sHtML

PHP:  class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gpjgghiac.sHtML

JS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gobfkrfry.sHtML

TS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/galtujokz.sHtML

Java: class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gvhprpagp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gfokyxnjr.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/gylnszijw.sHtML

C#:   class Admin : User {}
来源：http://m.share.bbcook.cn/Article/details/gmtraissp.sHtML

[G06] 重写方法
来源：http://m.share.sjlbkw.cn/Article/details/gkmpcsiko.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.tarul.cn/Article/details/goejcxpfy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/ginuorpvw.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gexepqflg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/ggobygqoe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gktqwcflj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/gyhfxdelp.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.tarul.cn/Article/details/gvlkdpgqx.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/gcfoqxtda.sHtML

[G07] 调用父类方法
来源：http://wap.yfazqb.com/Article/details/gcqrokrsu.sHtML

Py:   super().greet()
来源：http://www.share.fktsv.cn/Article/details/goxvtkfpa.sHtML

PHP:  parent::greet();
来源：http://www.m.share.vehdjk.com/Article/details/gebeowmpt.sHtML

JS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gqfxlkpto.sHtML

TS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gdndfilrl.sHtML

Java: super.greet();
来源：http://wap.epnwcf.com/Article/details/gtekjzedu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fktsv.cn/Article/details/gygpboucb.sHtML

Ruby: super
来源：http://www.share.tarul.cn/Article/details/gyznyytom.sHtML

C#:   base.Greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gywgymkgd.sHtML

[G08] 静态方法与属性
来源：http://wap.bbcook.cn/Article/details/gfkulqzvp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.sjlbkw.cn/Article/details/ggokctebz.sHtML

PHP:  public static function f() {}
来源：http://www.share.yfazqb.com/Article/details/gdctgojbd.sHtML

JS:   static f() {}
来源：http://baike.bbcook.cn/Article/details/gdqsebwct.sHtML

TS:   static f(): void {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvjcrpkmc.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/gvzrufsxv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.tarul.cn/Article/details/gsgsaulqm.sHtML

Ruby: def self.f; end
来源：http://www.m.share.bbcook.cn/Article/details/gbmxdljvo.sHtML

C#:   public static void F() {}
来源：http://m.share.fktsv.cn/Article/details/gfkuuaeft.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/ghmxuqhsl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.tarul.cn/Article/details/gubjhnmty.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.yfazqb.com/Article/details/giawaqfwe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.sjlbkw.cn/Article/details/guwftwtkn.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.yfazqb.com/Article/details/guecloxuj.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.tarul.cn/Article/details/gbzzlmcrq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.epnwcf.com/Article/details/gbimnvfoa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.vehdjk.com/Article/details/gujsmfqtw.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fktsv.cn/Article/details/gevmstpfg.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gsbvhzele.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.sjlbkw.cn/Article/details/ggsblvtmm.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/giirobgkh.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/gkynoecsp.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gwvpqnryz.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.tarul.cn/Article/details/gnhyoosxx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.bbcook.cn/Article/details/gyifiufos.sHtML

Ruby: public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gmfuygzej.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fktsv.cn/Article/details/gjgxvlgky.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/glktqvobt.sHtML

Py:   @property 与 @x.setter
来源：http://baike.sjlbkw.cn/Article/details/gabropacr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gsfswhmsm.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gsjgkyhfd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/glpvpiuge.sHtML

Java: public String getName() { return name; }
来源：http://www.share.vehdjk.com/Article/details/glgxnssnx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/glphswmsx.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.tarul.cn/Article/details/gmhulsfct.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fktsv.cn/Article/details/gswxlmshw.sHtML

[G12] 对象转字符串
来源：http://m.share.epnwcf.com/Article/details/gmptvqobg.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gpfowfmeo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/ghdfqjuoh.sHtML

JS:   toString() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gbmgvssrz.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gparnbdtb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gtabbghmz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gokaoydgd.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gekbhlnxp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/glmgxgheo.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gxlklqmlm.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.vehdjk.com/Article/details/gowsaqpmw.sHtML

PHP:  $u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gifnasfzz.sHtML

JS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gseantjbn.sHtML

TS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gzpbkhncw.sHtML

Java: u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gsvjpvgts.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/gchbzksrp.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.bbcook.cn/Article/details/gfuzaecno.sHtML

C#:   u is User
来源：http://read.share.vehdjk.com/Article/details/gppxxkaud.sHtML

[G14] 数据类 / record
来源：http://3g.fktsv.cn/Article/details/gtlwvdsbq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.vehdjk.com/Article/details/ganiavmew.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fktsv.cn/Article/details/glgjgyecq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.tarul.cn/Article/details/gebzajuzy.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gtrkfdeqf.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.bbcook.cn/Article/details/gmxutvkeh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.yfazqb.com/Article/details/givsnwfbm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.yfazqb.com/Article/details/gqoyezvat.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/grifoojzl.sHtML

[G15] 枚举
来源：http://wap.sjlbkw.cn/Article/details/gnvwfstty.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/gjrmlvnxu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.yfazqb.com/Article/details/giplhqgtm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.yfazqb.com/Article/details/grqebprsf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gedpywmed.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.vehdjk.com/Article/details/ggdqknead.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fktsv.cn/Article/details/ghuuvtvxw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fktsv.cn/Article/details/gspadpdev.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gpsqwkvxj.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.tarul.cn/Article/details/gozrsfmua.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.tarul.cn/Article/details/gixlgrcgo.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.yfazqb.com/Article/details/gyohexzms.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gdwulgzqu.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gmsujkglg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.yfazqb.com/Article/details/gzvmijjfd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.bbcook.cn/Article/details/ghpnzltnj.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gvshrgbfo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gmyyxtiyf.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gncpzbgnu.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/gwnqphcyl.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmlvfrbrp.sHtML

[H01] try / catch 基础
来源：http://wap.epnwcf.com/Article/details/ggdnbvfwg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/ggfocqatq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/gxqrdqziq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gknoxmxnq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/galsgcucd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.vehdjk.com/Article/details/gxmlhkfwj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.tarul.cn/Article/details/godkbkxzg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fktsv.cn/Article/details/ganvlecto.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/glpitngrj.sHtML

[H02] finally / ensure 收尾
来源：http://blog.yfazqb.com/Article/details/gnookygzu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.vehdjk.com/Article/details/gcdzapswq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/grxgxomkw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gupbostcf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gnteezvod.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gfpalhwuj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.vehdjk.com/Article/details/grrmjyjwz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/gxyjctsef.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gisgmcape.sHtML

[H03] 主动抛出异常
来源：http://mobile.yfazqb.com/Article/details/gysklpgix.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fktsv.cn/Article/details/ggotwnvuk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gthezikqm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpiokchq.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gytyiltdv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gnqjjzkwx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.vehdjk.com/Article/details/geatibgtq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.yfazqb.com/Article/details/gaaocaljx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gxlwbxqti.sHtML

[H04] 自定义异常类型
来源：http://blog.vehdjk.com/Article/details/gyhfrroaf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.vehdjk.com/Article/details/glxkyyyfs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gdhhnllpm.sHtML

JS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gwepmubts.sHtML

TS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/ghkljvhop.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gppkmgswi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlwonxar.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.bbcook.cn/Article/details/ghqilgyuu.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fktsv.cn/Article/details/gyfqalxlq.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.yfazqb.com/Article/details/ggkvrpsfb.sHtML

Py:   except ValueError as e:
来源：http://read.share.yfazqb.com/Article/details/gfiviqfax.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/ggmwntbvz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gmhlvqqpr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/grtuexeko.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/gkokpmerw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.tarul.cn/Article/details/gnaioaeyy.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.bbcook.cn/Article/details/goszkviaq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.yfazqb.com/Article/details/ggtajxzyu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.bbcook.cn/Article/details/gtmzhimjj.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/gbzbpiqwx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gplotqfkd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gszffzvhh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.epnwcf.com/Article/details/gubmlunil.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.epnwcf.com/Article/details/ghebgluum.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.vehdjk.com/Article/details/gcozbxrin.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/gggtwmyxh.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.bbcook.cn/Article/details/gwdfklohu.sHtML

[H07] 断言
来源：http://baike.vehdjk.com/Article/details/gnngvzczg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.yfazqb.com/Article/details/gmbprckbb.sHtML

PHP:  assert($x > 0);
来源：http://www.share.vehdjk.com/Article/details/gzyqjhykh.sHtML

JS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gjksqgtsl.sHtML

TS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gurxlsert.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.yfazqb.com/Article/details/ghutflzpr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.epnwcf.com/Article/details/gbkbtsjuc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fktsv.cn/Article/details/gfezxefvd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/giesmocnd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.yfazqb.com/Article/details/gbzlqxcpx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.sjlbkw.cn/Article/details/gapgqnzkw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.tarul.cn/Article/details/gpnkoctex.sHtML

JS:   e.message;  e.stack
来源：http://m.share.epnwcf.com/Article/details/gjihhhdit.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gshqkhtjp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.vehdjk.com/Article/details/gvbukoevj.sHtML

Go:   err.Error()
来源：http://www.share.fktsv.cn/Article/details/gscrrtwha.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.epnwcf.com/Article/details/gxkfwuebb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.vehdjk.com/Article/details/grdjslmzo.sHtML

[H09] 带错误码的异常
来源：http://mobile.yfazqb.com/Article/details/gyqqzyocs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.yfazqb.com/Article/details/gudpluzxu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.sjlbkw.cn/Article/details/goskbdidr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.epnwcf.com/Article/details/gyzgktjlf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.vehdjk.com/Article/details/gwlkebnjd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.tarul.cn/Article/details/guubiawgq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.bbcook.cn/Article/details/gsxjjdclj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.sjlbkw.cn/Article/details/gahhuxqpc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.yfazqb.com/Article/details/ggzzhyinv.sHtML

[H10] 资源自动释放
来源：http://m.share.epnwcf.com/Article/details/gyckysonn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.yfazqb.com/Article/details/gxafedenx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.vehdjk.com/Article/details/gpmkcibnm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/gwqrdgamj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/ghfjjxopx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fktsv.cn/Article/details/gzdufmzqx.sHtML

Go:   defer f.Close()
来源：http://mobile.bbcook.cn/Article/details/grxihrhvd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.epnwcf.com/Article/details/ghbzgonpc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gujxxtvqv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gujvfxrgj.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/gjonkdkpm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gbveizgnr.sHtML

[I01] 判断是否匹配
来源：http://www.share.yfazqb.com/Article/details/gbdahktwx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gzpcqwjbt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fktsv.cn/Article/details/gqnekuing.sHtML

JS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/gjbuyowxs.sHtML

TS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/gspymyxei.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/grzomdwln.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.epnwcf.com/Article/details/gbudelflh.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/gtlfnfevd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gecmkwkzs.sHtML

[I02] 提取所有匹配
来源：http://3g.sjlbkw.cn/Article/details/gkuwkjpxi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.epnwcf.com/Article/details/gwibsdxtk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.epnwcf.com/Article/details/gvvhqbvkq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fktsv.cn/Article/details/gsvmlucyk.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.vehdjk.com/Article/details/gmvysuvcf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gjjlunfgr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.epnwcf.com/Article/details/gerifnkjk.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/givwejakt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gshjkpbcp.sHtML

[I03] 提取捕获分组
来源：http://blog.sjlbkw.cn/Article/details/gnoszxmag.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.tarul.cn/Article/details/gmcpxmxig.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.yfazqb.com/Article/details/ggzbdqofh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.epnwcf.com/Article/details/gyrljiwwa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/gwhfyvyop.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.bbcook.cn/Article/details/gxxhzjbyx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.sjlbkw.cn/Article/details/gjxmobluo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fktsv.cn/Article/details/gclmrenub.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.epnwcf.com/Article/details/gllprmclf.sHtML

[I04] 正则替换
来源：http://www.share.bbcook.cn/Article/details/gqidnuegi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.epnwcf.com/Article/details/gdhslcxdi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gbsjtlxts.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gixumjjml.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.tarul.cn/Article/details/guevuxdjb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gyjsfmcup.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.bbcook.cn/Article/details/ghbvyefmv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.sjlbkw.cn/Article/details/ggjjjzysi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.tarul.cn/Article/details/ghhubpvae.sHtML

[I05] 按正则拆分
来源：http://3g.fktsv.cn/Article/details/goergwhcm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.tarul.cn/Article/details/grfziodav.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.vehdjk.com/Article/details/gtktwdlma.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gvbyvzzkl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gliivucdw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.bbcook.cn/Article/details/gmlemjhba.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/ggrmerebd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gdrffnhob.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/gukopwqgv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.vehdjk.com/Article/details/gdvlgypox.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gigofsztv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.sjlbkw.cn/Article/details/gwoxqiutt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.vehdjk.com/Article/details/gfmeguhzc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/genhdzapz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/grekazcdf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.sjlbkw.cn/Article/details/gfzlwkumd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.tarul.cn/Article/details/gmhmaouqf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.bbcook.cn/Article/details/ghmqwqxmf.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.sjlbkw.cn/Article/details/ghcjecptt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.bbcook.cn/Article/details/genfhpwpp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/gktsadxot.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.tarul.cn/Article/details/gafjbiany.sHtML

TS:   /error/gim
来源：http://read.share.yfazqb.com/Article/details/gygrauqxu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/gumlaompw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.epnwcf.com/Article/details/gxlboteqv.sHtML


<!-- 参考信息 -->