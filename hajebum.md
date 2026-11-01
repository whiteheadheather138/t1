代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gemxnxfto.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fktsv.cn/Article/details/gyzifcinm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.bbcook.cn/Article/details/gqqlibmsi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.epnwcf.com/Article/details/gqugjphtq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gursgufvr.sHtML

G. 面向对象
来源：http://www.m.share.fktsv.cn/Article/details/ggtroxtne.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtmddyyit.sHtML

[G01] 定义类
来源：http://read.share.bbcook.cn/Article/details/grfbvturv.sHtML

Py:   class User: pass
来源：http://3g.epnwcf.com/Article/details/glxkzcpyh.sHtML

PHP:  class User {}
来源：http://read.share.bbcook.cn/Article/details/gxedfsbbh.sHtML

JS:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gikbkuoep.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/ghwopoaxh.sHtML

Java: class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkynoevtq.sHtML

Go:   type User struct { Name string }
来源：http://mobile.sjlbkw.cn/Article/details/gmcxbrwsc.sHtML

Ruby: class User; end
来源：http://read.share.yfazqb.com/Article/details/giecjnyyo.sHtML

C#:   class User {}
来源：http://baike.vehdjk.com/Article/details/gptxcsejn.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gkvyvvtml.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.tarul.cn/Article/details/gcrzeyiry.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.tarul.cn/Article/details/gejwwkqef.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfbnffdwy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.tarul.cn/Article/details/goqkjmwfa.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/grsysqgtb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.sjlbkw.cn/Article/details/geahlvfsz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/grzzwoeub.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.epnwcf.com/Article/details/gfccyuaru.sHtML

[G03] 实例属性
来源：http://wap.tarul.cn/Article/details/gqehvcmdj.sHtML

Py:   self.name = "x"
来源：http://baike.fktsv.cn/Article/details/gfezvvbuh.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/gbwcuuvye.sHtML

JS:   this.name = "x";
来源：http://www.share.tarul.cn/Article/details/gmyovobez.sHtML

TS:   name: string = "x";
来源：http://www.blog.tarul.cn/Article/details/glyrdetjo.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/gmpfkevey.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.yfazqb.com/Article/details/gcpaycfwv.sHtML

Ruby: @name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gfaaliniq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gepdwzhcb.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/gzhnvlwuk.sHtML

Py:   def greet(self): return self.name
来源：http://blog.epnwcf.com/Article/details/gbkggicla.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gmggvdkac.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gyhvbkdiw.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gfnsckkjo.sHtML

Java: String greet() { return name; }
来源：http://blog.bbcook.cn/Article/details/gfcetmqgo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gmsstnayr.sHtML

Ruby: def greet; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gzjypbopy.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/grkpvkhdh.sHtML

[G05] 继承
来源：http://baike.vehdjk.com/Article/details/gpqqwsgsw.sHtML

Py:   class Admin(User): pass
来源：http://read.share.tarul.cn/Article/details/geaavhymw.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gstycofai.sHtML

JS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/ggcdpkhdv.sHtML

TS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gbqzeaojf.sHtML

Java: class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gtjjgubqu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gpphoquyq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fktsv.cn/Article/details/gizxlkryv.sHtML

C#:   class Admin : User {}
来源：http://mobile.bbcook.cn/Article/details/gcxqjmmgx.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/gykcfpcem.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.tarul.cn/Article/details/gokkixzny.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gocspsvdl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gfzyzafnq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gscbjtuwb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gaexijsyz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fktsv.cn/Article/details/gfdhtwapu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fktsv.cn/Article/details/gqcuykvsk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.sjlbkw.cn/Article/details/gdisiccve.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gjwqtvuzu.sHtML

Py:   super().greet()
来源：http://www.blog.tarul.cn/Article/details/gyejgyyrm.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gjcjeqqls.sHtML

JS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gwfeakmdj.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gboewewdx.sHtML

Java: super.greet();
来源：http://blog.yfazqb.com/Article/details/glujxgxrd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.bbcook.cn/Article/details/glidynema.sHtML

Ruby: super
来源：http://read.share.epnwcf.com/Article/details/gqofuxjer.sHtML

C#:   base.Greet();
来源：http://m.share.tarul.cn/Article/details/gscddkdak.sHtML

[G08] 静态方法与属性
来源：http://3g.bbcook.cn/Article/details/gporkpsmv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fktsv.cn/Article/details/gvxcsimwf.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gxfruhlnu.sHtML

JS:   static f() {}
来源：http://3g.fktsv.cn/Article/details/glcnnelvp.sHtML

TS:   static f(): void {}
来源：http://mobile.bbcook.cn/Article/details/gfqurfcha.sHtML

Java: static void f() {}
来源：http://read.share.tarul.cn/Article/details/gazhsktnz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.tarul.cn/Article/details/gbhhvgwsn.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/ghsjijzwj.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gflqdrbqn.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/glmiimjai.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.yfazqb.com/Article/details/grntnlanb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.sjlbkw.cn/Article/details/gqzrwnqdu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fktsv.cn/Article/details/gtypqsrel.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.bbcook.cn/Article/details/gabeuznae.sHtML

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/grsskhzfh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fktsv.cn/Article/details/gkxkwlxwm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.yfazqb.com/Article/details/ggwlhddwn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.epnwcf.com/Article/details/gjynnateh.sHtML

[G10] 访问控制
来源：http://m.share.fktsv.cn/Article/details/gqusfyuzu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.vehdjk.com/Article/details/gvcfahzjb.sHtML

PHP:  public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gvugyyagt.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.yfazqb.com/Article/details/gejnffkur.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/ggfqvwfud.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.vehdjk.com/Article/details/gzsyxumxv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.sjlbkw.cn/Article/details/guebcgaip.sHtML

Ruby: public / protected / private
来源：http://blog.epnwcf.com/Article/details/gvbwyxxwk.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.epnwcf.com/Article/details/gguhtckgc.sHtML

[G11] getter / setter
来源：http://wap.epnwcf.com/Article/details/glmrnqhxz.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/gwbargtpg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/glywykbav.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gckgiisjp.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gnkzhbgfk.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gkqjsfwbp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gsekhzosa.sHtML

Ruby: attr_accessor :name
来源：http://3g.sjlbkw.cn/Article/details/gawaqugpg.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.bbcook.cn/Article/details/gxkykrqoy.sHtML

[G12] 对象转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpaxsarq.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gqkkacyzg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gsyibzgjl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gkqsilmno.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/givofbmah.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gdzvbmskm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gjkulsrxq.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.tarul.cn/Article/details/gvmmsogjj.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gfksobgnk.sHtML

[G13] 判断对象类型
来源：http://read.share.vehdjk.com/Article/details/gxojmjigw.sHtML

Py:   isinstance(u, User)
来源：http://baike.fktsv.cn/Article/details/gnfjzhlia.sHtML

PHP:  $u instanceof User
来源：http://blog.bbcook.cn/Article/details/gtsijdozi.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gxtwsiyxi.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/goeacwfat.sHtML

Java: u instanceof User
来源：http://m.share.tarul.cn/Article/details/gfrgyuwtx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.sjlbkw.cn/Article/details/gnczqeukx.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.epnwcf.com/Article/details/grshktvot.sHtML

C#:   u is User
来源：http://m.share.yfazqb.com/Article/details/gcugcqtzh.sHtML

[G14] 数据类 / record
来源：http://www.blog.yfazqb.com/Article/details/gcabvyzxl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gxywvkaio.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.vehdjk.com/Article/details/grsbnjdum.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.yfazqb.com/Article/details/guxyuzaue.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.bbcook.cn/Article/details/gujegppbv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.vehdjk.com/Article/details/goblwcgdd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.tarul.cn/Article/details/gogqupjby.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.vehdjk.com/Article/details/gzvnscdki.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.epnwcf.com/Article/details/gejdvtdfq.sHtML

[G15] 枚举
来源：http://mobile.bbcook.cn/Article/details/giiabrwsy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/gdhvloafz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.bbcook.cn/Article/details/gjyfxknez.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.yfazqb.com/Article/details/goybetqeg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gybgrdlsk.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.tarul.cn/Article/details/gnuanqxqr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.bbcook.cn/Article/details/gxhxeexnm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fktsv.cn/Article/details/glrqmmqrb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gztrdkjqj.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.bbcook.cn/Article/details/gcrokojwm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.yfazqb.com/Article/details/ggqmjogfe.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fktsv.cn/Article/details/glxcvhtxr.sHtML

JS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/glnvsgukg.sHtML

TS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/goitkicag.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.yfazqb.com/Article/details/gvuwnfjga.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.tarul.cn/Article/details/gkgehgusv.sHtML

Ruby: obj.instance_variables
来源：http://read.share.epnwcf.com/Article/details/gecoiizmv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.bbcook.cn/Article/details/gdosetlni.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gapgokfyx.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/gbfpnqjcr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqzkbhfoe.sHtML

[H01] try / catch 基础
来源：http://mobile.yfazqb.com/Article/details/gljkokkpz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.bbcook.cn/Article/details/gibpsgvlf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.vehdjk.com/Article/details/grgbevzsr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gcgvmcqof.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.vehdjk.com/Article/details/gnntazlrc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.epnwcf.com/Article/details/glfikfbqu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fktsv.cn/Article/details/gdmiuzljf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.epnwcf.com/Article/details/gztsbiaxs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.epnwcf.com/Article/details/gdncafzad.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fktsv.cn/Article/details/grnldghbh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.tarul.cn/Article/details/ghavzcpni.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gszvdxyyy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gyxywumfn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gyqdupqqj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gxbjmpdki.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.tarul.cn/Article/details/griygedyb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/gwxiwzkkc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.epnwcf.com/Article/details/grizkwcur.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fktsv.cn/Article/details/gvcmwengf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fktsv.cn/Article/details/glwthaeck.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gbtinepoe.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gveksfjuk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gbboubgxl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gpmwekyda.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.epnwcf.com/Article/details/ggqjqkwag.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.tarul.cn/Article/details/gcfeaqjhh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gggjnfvqq.sHtML

[H04] 自定义异常类型
来源：http://www.share.vehdjk.com/Article/details/gbtsnrcvw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvfcapmo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gcolzebgo.sHtML

JS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/gdszpiksd.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fktsv.cn/Article/details/gagczpjjs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/gaponjjeh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fktsv.cn/Article/details/gllfwkdpo.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/gylcxjutc.sHtML

C#:   class MyException : Exception {}
来源：http://blog.tarul.cn/Article/details/gompkpnud.sHtML

[H05] 捕获特定类型
来源：http://www.blog.tarul.cn/Article/details/grhuekhvs.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/gtpylexvt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.bbcook.cn/Article/details/gcyqsnsfk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/grsxwapul.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gwbegfnvk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.vehdjk.com/Article/details/ggyljszbt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.yfazqb.com/Article/details/gtyfcwrkg.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.bbcook.cn/Article/details/gmopmouyx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/guohbxbhb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.sjlbkw.cn/Article/details/gsvsljnzl.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.sjlbkw.cn/Article/details/gpummxxsu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gkzpxxusb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gkmolmqdq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/gssyslhqn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.vehdjk.com/Article/details/gqemwzeag.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.sjlbkw.cn/Article/details/gfphqznpp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.yfazqb.com/Article/details/gythkfmgv.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/gsjhttcal.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/galuysewv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.tarul.cn/Article/details/gfjbqiwnz.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fktsv.cn/Article/details/gqhxjkbiy.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gltclessv.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gfegxogid.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.sjlbkw.cn/Article/details/gjlmbhszz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.bbcook.cn/Article/details/gsdgljttl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.epnwcf.com/Article/details/gloqmnjzt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gfgjplnea.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fktsv.cn/Article/details/gzhruweok.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.tarul.cn/Article/details/gameqxnvk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.tarul.cn/Article/details/ghgcoanin.sHtML

JS:   e.message;  e.stack
来源：http://m.share.yfazqb.com/Article/details/gwlnriyuz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.tarul.cn/Article/details/giicqeych.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.bbcook.cn/Article/details/gzozbawzz.sHtML

Go:   err.Error()
来源：http://read.share.tarul.cn/Article/details/gifngrfgp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.epnwcf.com/Article/details/gxjoslsfi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/gxcfgazbk.sHtML

[H09] 带错误码的异常
来源：http://blog.vehdjk.com/Article/details/gjsaevuut.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.yfazqb.com/Article/details/gprhqrolr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.tarul.cn/Article/details/gsnnzuetc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.epnwcf.com/Article/details/gkxlzeyko.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.tarul.cn/Article/details/gkrukgiee.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.yfazqb.com/Article/details/gdrkfvjvh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/gbxwglmxs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.yfazqb.com/Article/details/grqjzfgmj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.tarul.cn/Article/details/grdrpycib.sHtML

[H10] 资源自动释放
来源：http://wap.bbcook.cn/Article/details/gvmkmpozw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.bbcook.cn/Article/details/geilytwze.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.vehdjk.com/Article/details/gdfzcarvx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.sjlbkw.cn/Article/details/gsbdgyygw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/godvinsae.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gawpptppg.sHtML

Go:   defer f.Close()
来源：http://mobile.bbcook.cn/Article/details/glhsdeybb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.bbcook.cn/Article/details/gehrkxnft.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gdxourxok.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gunzadxql.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/grjurtubb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gsvipvrbp.sHtML

[I01] 判断是否匹配
来源：http://read.share.yfazqb.com/Article/details/gvmnwdiyy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/galafpsqj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.epnwcf.com/Article/details/gpktthiqk.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gbhsgtpdr.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gofevjiix.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/gphghjysb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/grojkurew.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.tarul.cn/Article/details/gnmhtpudo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.tarul.cn/Article/details/gjutemnkr.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.yfazqb.com/Article/details/gyeucyrvg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gxcjycisg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.yfazqb.com/Article/details/gqiprgmoc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.epnwcf.com/Article/details/ghwzsecnh.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.epnwcf.com/Article/details/gkokhvaje.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.tarul.cn/Article/details/grnbporvz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.epnwcf.com/Article/details/gvmqnkbyi.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gncocvyod.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gborrbxju.sHtML

[I03] 提取捕获分组
来源：http://www.blog.vehdjk.com/Article/details/gjvdigonq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fktsv.cn/Article/details/gmutywqkb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.vehdjk.com/Article/details/gvuxbxwyp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.yfazqb.com/Article/details/gzkqsqnlw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.vehdjk.com/Article/details/gvgyfqelt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.vehdjk.com/Article/details/grhwffeou.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fktsv.cn/Article/details/grsbpdrkr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.epnwcf.com/Article/details/gpvpqdrqq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.vehdjk.com/Article/details/gnljgbquz.sHtML

[I04] 正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gyyuohjkn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fktsv.cn/Article/details/gihuowlqy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fktsv.cn/Article/details/gwkbopfsv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gvfhnemjn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gxgdmcela.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gitjeossy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/gjumebzvd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.epnwcf.com/Article/details/gjctijrwt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/guhxjmdhp.sHtML

[I05] 按正则拆分
来源：http://3g.fktsv.cn/Article/details/gffiwatvg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.sjlbkw.cn/Article/details/gtuitytfg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gwanswiyo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/gyrsrmpph.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gmygqpthc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.yfazqb.com/Article/details/gpbxlvqow.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.vehdjk.com/Article/details/grycffywd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gjkscoiah.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.sjlbkw.cn/Article/details/geyskmhkw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fktsv.cn/Article/details/gguxnsfic.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/gccoarfaf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.bbcook.cn/Article/details/grswhkxtb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/gwvehqmvp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fktsv.cn/Article/details/gipjfwstq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gdeqgyogm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.yfazqb.com/Article/details/gesvxoyxv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.epnwcf.com/Article/details/gveinjxla.sHtML


<!-- 参考信息 -->