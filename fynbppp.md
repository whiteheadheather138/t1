代发 wailian999

Java: class User {}
来源：http://blog.bbcook.cn/Article/details/gbbezccgt.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/gqumhjrhq.sHtML

Ruby: class User; end
来源：http://wap.sjlbkw.cn/Article/details/ginaypbqp.sHtML

C#:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gwnbtayii.sHtML

[G02] 构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvymfqcsv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.sjlbkw.cn/Article/details/glgrvjmxe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.yfazqb.com/Article/details/gdcpzdjhe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/gtpvxqqjv.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.tarul.cn/Article/details/gqjlmswbj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gnfxayyov.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fktsv.cn/Article/details/gibymwdbi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.tarul.cn/Article/details/gmgcrvnxp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.tarul.cn/Article/details/georrmlqb.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/guuoanxsh.sHtML

Py:   self.name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/gmmcfkese.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/ggcgjndox.sHtML

JS:   this.name = "x";
来源：http://baike.fktsv.cn/Article/details/gyauhqbfl.sHtML

TS:   name: string = "x";
来源：http://read.share.tarul.cn/Article/details/gqqmrsarf.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/gqvdtvylk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.vehdjk.com/Article/details/gleofsuvk.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/grkbiozuu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.yfazqb.com/Article/details/gncwgbldn.sHtML

[G04] 定义方法
来源：http://read.share.vehdjk.com/Article/details/gjdftlqor.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/graxonica.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gjuvtuiih.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gfciotwst.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gxbopoxxl.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gtguteupm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gwcuptdyp.sHtML

Ruby: def greet; @name; end
来源：http://3g.bbcook.cn/Article/details/gskvgfoom.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.yfazqb.com/Article/details/gesjjdnxv.sHtML

[G05] 继承
来源：http://m.share.bbcook.cn/Article/details/gimgesuyi.sHtML

Py:   class Admin(User): pass
来源：http://blog.vehdjk.com/Article/details/gqtwwygwd.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gckqvgxoc.sHtML

JS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gwrhtkbkg.sHtML

TS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gqakzrimw.sHtML

Java: class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gzsulhfcr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.yfazqb.com/Article/details/gslkygqjq.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gqkxihppj.sHtML

C#:   class Admin : User {}
来源：http://read.share.tarul.cn/Article/details/gvaeavhth.sHtML

[G06] 重写方法
来源：http://www.blog.epnwcf.com/Article/details/gqdmbssix.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.epnwcf.com/Article/details/gojucpubd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gusqpbngt.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/goxcubnbh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzyzjxrja.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gwymkkgox.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fktsv.cn/Article/details/gbbqjiqan.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/gaqpkzjkr.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/giziyqljw.sHtML

[G07] 调用父类方法
来源：http://3g.fktsv.cn/Article/details/gzsexoori.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/gwfurolns.sHtML

PHP:  parent::greet();
来源：http://m.share.tarul.cn/Article/details/gpxqsywnw.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gmxlawlte.sHtML

TS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gdltjjpyf.sHtML

Java: super.greet();
来源：http://3g.yfazqb.com/Article/details/gveophxcl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.yfazqb.com/Article/details/gdhmzlbms.sHtML

Ruby: super
来源：http://baike.fktsv.cn/Article/details/gvlufnzyw.sHtML

C#:   base.Greet();
来源：http://baike.fktsv.cn/Article/details/gkrtsxchi.sHtML

[G08] 静态方法与属性
来源：http://mobile.sjlbkw.cn/Article/details/ghlkzqptx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.tarul.cn/Article/details/grxzsbvdp.sHtML

PHP:  public static function f() {}
来源：http://blog.vehdjk.com/Article/details/gmqrnvyju.sHtML

JS:   static f() {}
来源：http://3g.vehdjk.com/Article/details/ginjstotl.sHtML

TS:   static f(): void {}
来源：http://www.blog.epnwcf.com/Article/details/gwpimyxur.sHtML

Java: static void f() {}
来源：http://baike.fktsv.cn/Article/details/gjpabqgge.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.epnwcf.com/Article/details/gheptvlej.sHtML

Ruby: def self.f; end
来源：http://wap.epnwcf.com/Article/details/giszmauhj.sHtML

C#:   public static void F() {}
来源：http://wap.fktsv.cn/Article/details/gurobsulz.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.vehdjk.com/Article/details/gdsgfpftn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/grxyfqmba.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.tarul.cn/Article/details/gwhrrvyep.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.tarul.cn/Article/details/ggdhwrxth.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.vehdjk.com/Article/details/gnnjwgobh.sHtML

Java: interface Shape { double area(); }
来源：http://3g.vehdjk.com/Article/details/gmdhvbofp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gvlmpgsff.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.tarul.cn/Article/details/gqshxdkwx.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/gvxnxcqxq.sHtML

[G10] 访问控制
来源：http://3g.vehdjk.com/Article/details/gfapqctqi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.sjlbkw.cn/Article/details/gaxsxklqm.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gmevdinig.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gpznwcvdd.sHtML

TS:   public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gpvkkavez.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fktsv.cn/Article/details/gfxmvnlcc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fktsv.cn/Article/details/ghgamefuc.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gwweyvact.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/gthlfwakc.sHtML

[G11] getter / setter
来源：http://www.m.share.yfazqb.com/Article/details/gcrtjtthn.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fktsv.cn/Article/details/gvuzdepxx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gxgbntytc.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gitjnotfs.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gvhujhaps.sHtML

Java: public String getName() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gwjlhwryi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gnvkvhfgy.sHtML

Ruby: attr_accessor :name
来源：http://baike.bbcook.cn/Article/details/guxqfcunw.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.yfazqb.com/Article/details/goxpzmsqf.sHtML

[G12] 对象转字符串
来源：http://read.share.fktsv.cn/Article/details/ghfzvento.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/ghmjlgsfk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gjomxydrc.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gsaicurvn.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gmhepuxal.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.bbcook.cn/Article/details/ggmoefnea.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/ggzxfduco.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/gsfyudgyy.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.yfazqb.com/Article/details/gvylbufcs.sHtML

[G13] 判断对象类型
来源：http://www.blog.tarul.cn/Article/details/gzaqxvtdi.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.tarul.cn/Article/details/gkjxuxpkn.sHtML

PHP:  $u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gkrmqpfyz.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gbqnhtlym.sHtML

TS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gjkravfbo.sHtML

Java: u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gajglzshl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/grpwcokev.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gquhsvapo.sHtML

C#:   u is User
来源：http://baike.tarul.cn/Article/details/galbaqrgr.sHtML

[G14] 数据类 / record
来源：http://m.share.vehdjk.com/Article/details/gkbvftksz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fktsv.cn/Article/details/gerizrhgk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/gmuldkzmg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.tarul.cn/Article/details/glkjshbrn.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.epnwcf.com/Article/details/gluuntpov.sHtML

Java: record User(String name, int age) {}
来源：http://blog.bbcook.cn/Article/details/gkkkhazbm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.yfazqb.com/Article/details/gpozyxjjk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gcmvrrbxl.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fktsv.cn/Article/details/gyombpuou.sHtML

[G15] 枚举
来源：http://www.m.share.vehdjk.com/Article/details/grkvwcrks.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.yfazqb.com/Article/details/ghtrojodw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.sjlbkw.cn/Article/details/gkfkbdmmy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.tarul.cn/Article/details/gngdatmhf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gtvtuzwrz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.bbcook.cn/Article/details/gluntuhul.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.vehdjk.com/Article/details/gjzqxhhxc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.epnwcf.com/Article/details/gwofytrfz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gcbynqebg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.sjlbkw.cn/Article/details/gpwvlihvj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.sjlbkw.cn/Article/details/gfceshsuz.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gdysjvbom.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gbwxpnnas.sHtML

TS:   Object.entries(obj)
来源：http://mobile.epnwcf.com/Article/details/gkwobovoa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.tarul.cn/Article/details/gznyhunzv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fktsv.cn/Article/details/gttzzwqep.sHtML

Ruby: obj.instance_variables
来源：http://mobile.epnwcf.com/Article/details/gzgemtrmf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gsglhcynx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghffegrec.sHtML

H. 异常与错误处理
来源：http://www.share.epnwcf.com/Article/details/gmvabnahu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glsguzuiz.sHtML

[H01] try / catch 基础
来源：http://blog.yfazqb.com/Article/details/gwviafrfl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/gzufbskgu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.yfazqb.com/Article/details/grjnrrpqb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.vehdjk.com/Article/details/gftlpemrp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gjopgjhhk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.sjlbkw.cn/Article/details/gwuwdxsxa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fktsv.cn/Article/details/gtuuubprz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fktsv.cn/Article/details/gewehknin.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fktsv.cn/Article/details/gfpvteszc.sHtML

[H02] finally / ensure 收尾
来源：http://wap.yfazqb.com/Article/details/gnanlgayc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.sjlbkw.cn/Article/details/ggwsiekbm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gmaivsxij.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gfqqrridm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/ggmcteshh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gpuyjplfa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.vehdjk.com/Article/details/gdxflkdkm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrcqykqu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gtqwhgcfj.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.yfazqb.com/Article/details/ggvwcxxst.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyfrrpxh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gvsiflgms.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gkwpsjnkt.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gtrjejwkl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gaxangaja.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/gttqtixif.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.bbcook.cn/Article/details/goywrkbpj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/glrfovnng.sHtML

[H04] 自定义异常类型
来源：http://m.share.sjlbkw.cn/Article/details/gtghfsqbh.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.vehdjk.com/Article/details/gmgahsjva.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gwxgsgltq.sHtML

JS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gxicukqfc.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gblmhyrcn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gbamxpgcl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.sjlbkw.cn/Article/details/gocedxnpp.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.epnwcf.com/Article/details/gehkuezhl.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.epnwcf.com/Article/details/gobolbogi.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fktsv.cn/Article/details/gzpyjheqs.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/ggoegsulw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.yfazqb.com/Article/details/gbmjuwziq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gtxzhjpai.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gmkyjmlcy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.sjlbkw.cn/Article/details/gkkwzozfd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/geootystp.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fktsv.cn/Article/details/girwbuqbm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.vehdjk.com/Article/details/glmenxfbz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.bbcook.cn/Article/details/ghydnqznp.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.bbcook.cn/Article/details/gweqtqtza.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gomvloucp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gkvkcfogn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/ghbmpojaf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.yfazqb.com/Article/details/ggfjdapdc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.tarul.cn/Article/details/gvodmoywg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fktsv.cn/Article/details/gicljbvyq.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/gpkoeakhc.sHtML

[H07] 断言
来源：http://www.share.tarul.cn/Article/details/gpzvxdrds.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.epnwcf.com/Article/details/gcmdiwdct.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/gqfigmsjy.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gscopjyzs.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gaoqekiuo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.bbcook.cn/Article/details/gipzxaolu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fktsv.cn/Article/details/gbynxqlft.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.epnwcf.com/Article/details/gxvdryvbi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gnraejojw.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.epnwcf.com/Article/details/gycsxozmf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.bbcook.cn/Article/details/gfvdttwha.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.tarul.cn/Article/details/gwcfyavap.sHtML

JS:   e.message;  e.stack
来源：http://wap.fktsv.cn/Article/details/gctwsieao.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.vehdjk.com/Article/details/gfqdyaoqu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.bbcook.cn/Article/details/gimirgkfl.sHtML

Go:   err.Error()
来源：http://baike.yfazqb.com/Article/details/gsbzkkblp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.tarul.cn/Article/details/ghwrgxktg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/ggqryakvv.sHtML

[H09] 带错误码的异常
来源：http://wap.tarul.cn/Article/details/ghkqrgvbd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.sjlbkw.cn/Article/details/giovzksjo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.tarul.cn/Article/details/gbtgfxlsh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.bbcook.cn/Article/details/gahitgrkw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.tarul.cn/Article/details/gjmfjkhfx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.tarul.cn/Article/details/gldvwoafn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.epnwcf.com/Article/details/gcupirqts.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fktsv.cn/Article/details/grpmqyssj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.tarul.cn/Article/details/gsriuqcbu.sHtML

[H10] 资源自动释放
来源：http://read.share.sjlbkw.cn/Article/details/gkomjcwux.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.epnwcf.com/Article/details/gbegxpauk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.epnwcf.com/Article/details/gopechdlz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gtrzxrewf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.sjlbkw.cn/Article/details/gflmpnowj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.epnwcf.com/Article/details/gcligjixz.sHtML

Go:   defer f.Close()
来源：http://3g.vehdjk.com/Article/details/gfdeknhrl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.yfazqb.com/Article/details/gzjmlakyy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.yfazqb.com/Article/details/ghrzvgptg.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnaxiylcv.sHtML

I. 正则表达式
来源：http://www.share.vehdjk.com/Article/details/glgppeklj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvvpcpzyq.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.yfazqb.com/Article/details/gobqcwhoq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/gqsqdfftw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gwrpfmiux.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/gfuefemso.sHtML

TS:   /\d+/.test(s)
来源：http://wap.bbcook.cn/Article/details/gdsauezmn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fktsv.cn/Article/details/gkyvkmryn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.epnwcf.com/Article/details/gmzspwhnv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/gmrplccjg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gjzcgvgyi.sHtML

[I02] 提取所有匹配
来源：http://mobile.fktsv.cn/Article/details/gghnnixhn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gryzfkkmf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.sjlbkw.cn/Article/details/gjrcspmqj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.tarul.cn/Article/details/gzdggfxqd.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.yfazqb.com/Article/details/gcesyvcvu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.epnwcf.com/Article/details/gdqcftmjt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/gcrcphuge.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gkyuwxpvu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.vehdjk.com/Article/details/gkzfolhxv.sHtML

[I03] 提取捕获分组
来源：http://mobile.bbcook.cn/Article/details/guoixetfl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.epnwcf.com/Article/details/gfzfepljl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.epnwcf.com/Article/details/gjzulwlvq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.vehdjk.com/Article/details/gxxextazy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fktsv.cn/Article/details/gexngtziq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gwvektrjg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.bbcook.cn/Article/details/gthvfhksq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gnbfshmke.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.sjlbkw.cn/Article/details/gwwxqjedd.sHtML

[I04] 正则替换
来源：http://baike.vehdjk.com/Article/details/gwrueolen.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fktsv.cn/Article/details/gmtwllfur.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gvnfvwyep.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.vehdjk.com/Article/details/godnqkuug.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gpefzjxat.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gsvnrcihd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.vehdjk.com/Article/details/gfpkwaqay.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.tarul.cn/Article/details/gadqtdyop.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/geyobmgwj.sHtML

[I05] 按正则拆分
来源：http://www.m.share.yfazqb.com/Article/details/gvinyjppa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.vehdjk.com/Article/details/gcxgulnik.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.yfazqb.com/Article/details/gfsoprhjj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gmiasfijb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gzukvfnrr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fktsv.cn/Article/details/gwgdlohjt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.vehdjk.com/Article/details/gvclvcids.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gdccwklza.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gouzlbijb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/gbskwhvax.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/ggtqalqfq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.bbcook.cn/Article/details/gzleaktam.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gxdbaomln.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/gnczgnxhi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gwxfzndya.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.yfazqb.com/Article/details/gaanxonbf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/ghxnfpccx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gdnguorbr.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/gzrblzocc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.yfazqb.com/Article/details/gujpculvx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gjqrggorc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.bbcook.cn/Article/details/gswkajhra.sHtML

TS:   /error/gim
来源：http://mobile.sjlbkw.cn/Article/details/gvlativuo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.vehdjk.com/Article/details/glaktfiqp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.vehdjk.com/Article/details/gqvdipoeu.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fktsv.cn/Article/details/gjnltaytp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.sjlbkw.cn/Article/details/gtyepgddr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.sjlbkw.cn/Article/details/gnealwoil.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.bbcook.cn/Article/details/gggmkveev.sHtML


<!-- 参考信息 -->