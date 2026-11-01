代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fktsv.cn/Article/details/gecxomcak.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gjpipbhmu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.epnwcf.com/Article/details/gdogdpocw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/gkfatlefr.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gdyzmnmxx.sHtML

G. 面向对象
来源：http://www.m.share.yfazqb.com/Article/details/gkupvbefz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfkjxtaxq.sHtML

[G01] 定义类
来源：http://www.m.share.bbcook.cn/Article/details/gvevlivrw.sHtML

Py:   class User: pass
来源：http://mobile.fktsv.cn/Article/details/gvijmbwcf.sHtML

PHP:  class User {}
来源：http://baike.sjlbkw.cn/Article/details/gzaiiovjs.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/gyvxwrnwx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/gnsdikell.sHtML

Java: class User {}
来源：http://m.share.tarul.cn/Article/details/gjnfwzffv.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/gasatwgce.sHtML

Ruby: class User; end
来源：http://blog.sjlbkw.cn/Article/details/gaarkqahc.sHtML

C#:   class User {}
来源：http://baike.vehdjk.com/Article/details/ghzqyqpep.sHtML

[G02] 构造函数
来源：http://blog.bbcook.cn/Article/details/gdelqjnmc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.bbcook.cn/Article/details/gaeavppfc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gdlrwibra.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/ghndkmfvw.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.epnwcf.com/Article/details/gowiatbxy.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gyntsutsw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.vehdjk.com/Article/details/gbueroure.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.epnwcf.com/Article/details/gpaxvlpdh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.epnwcf.com/Article/details/gsrhllvmh.sHtML

[G03] 实例属性
来源：http://wap.yfazqb.com/Article/details/gwfaxtqyt.sHtML

Py:   self.name = "x"
来源：http://baike.tarul.cn/Article/details/gpxuqkbmn.sHtML

PHP:  public string $name = "x";
来源：http://baike.fktsv.cn/Article/details/gxkupmvdt.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/goxtigres.sHtML

TS:   name: string = "x";
来源：http://blog.tarul.cn/Article/details/glsavfhfv.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/gqyxgrawu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.epnwcf.com/Article/details/gdcxjstid.sHtML

Ruby: @name = "x"
来源：http://mobile.epnwcf.com/Article/details/gpuawkuws.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.tarul.cn/Article/details/gtphsfzcv.sHtML

[G04] 定义方法
来源：http://read.share.vehdjk.com/Article/details/gggxngacs.sHtML

Py:   def greet(self): return self.name
来源：http://3g.tarul.cn/Article/details/golyryuxr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gjyowbtle.sHtML

JS:   greet() { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gwdabzufa.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gzdwjxbxt.sHtML

Java: String greet() { return name; }
来源：http://m.share.tarul.cn/Article/details/guqedkico.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gadcphlsd.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/gdtoxjgwk.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.yfazqb.com/Article/details/gkryyecai.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/gvvnxdgei.sHtML

Py:   class Admin(User): pass
来源：http://www.share.bbcook.cn/Article/details/gkjgpgwsp.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gjnvotjue.sHtML

JS:   class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gdidmvlxi.sHtML

TS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gdjzweebx.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gjjpburcd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.epnwcf.com/Article/details/ghlrhaixb.sHtML

Ruby: class Admin < User; end
来源：http://m.share.yfazqb.com/Article/details/gfonhyycn.sHtML

C#:   class Admin : User {}
来源：http://3g.tarul.cn/Article/details/geqxkvzov.sHtML

[G06] 重写方法
来源：http://mobile.sjlbkw.cn/Article/details/gwjqpclnm.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/guwlpjhcw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gxtglnmce.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gatfiekup.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gdqbrlgwe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gteseawtj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/gswypxcya.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/gdbmyacve.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/grarhkwmy.sHtML

[G07] 调用父类方法
来源：http://wap.yfazqb.com/Article/details/ggozjwlfh.sHtML

Py:   super().greet()
来源：http://wap.fktsv.cn/Article/details/gncaoofki.sHtML

PHP:  parent::greet();
来源：http://www.share.epnwcf.com/Article/details/goztayknl.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gonxiqxjk.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gijjwlcbh.sHtML

Java: super.greet();
来源：http://www.share.tarul.cn/Article/details/gnmvatrep.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fktsv.cn/Article/details/gpsuiwulu.sHtML

Ruby: super
来源：http://read.share.tarul.cn/Article/details/geqsjnfjy.sHtML

C#:   base.Greet();
来源：http://read.share.vehdjk.com/Article/details/guxrspibu.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/gjotwfqkk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmvxtclc.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/geagqwihp.sHtML

JS:   static f() {}
来源：http://mobile.yfazqb.com/Article/details/gakciiruq.sHtML

TS:   static f(): void {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gedcemwgq.sHtML

Java: static void f() {}
来源：http://blog.tarul.cn/Article/details/gzfsporvs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/gmriuybpi.sHtML

Ruby: def self.f; end
来源：http://read.share.fktsv.cn/Article/details/gvebqbsjp.sHtML

C#:   public static void F() {}
来源：http://www.blog.sjlbkw.cn/Article/details/glwkaasdi.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.vehdjk.com/Article/details/gprcyuyfg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.bbcook.cn/Article/details/gtlvchtjn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.bbcook.cn/Article/details/gsdindowf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.tarul.cn/Article/details/guybrrqzo.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.sjlbkw.cn/Article/details/gouifjxdr.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.bbcook.cn/Article/details/gceqedpxu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.sjlbkw.cn/Article/details/gevsilxkd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/geswifewz.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/gfpcjlyvr.sHtML

[G10] 访问控制
来源：http://mobile.yfazqb.com/Article/details/giztchtkx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.yfazqb.com/Article/details/gtnximwrq.sHtML

PHP:  public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gewntxnjn.sHtML

JS:   #private 字段；其余公开
来源：http://3g.vehdjk.com/Article/details/gdwhjoyfg.sHtML

TS:   public / protected / private
来源：http://baike.yfazqb.com/Article/details/gofyredks.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/gehgzcffu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.bbcook.cn/Article/details/gropgggld.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gzfrgkhzq.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.bbcook.cn/Article/details/gvpbdlkqf.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/gulyquwtj.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fktsv.cn/Article/details/genquajuj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gznvswubz.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/ghrpuqveq.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.epnwcf.com/Article/details/gpsppmczu.sHtML

Java: public String getName() { return name; }
来源：http://mobile.bbcook.cn/Article/details/ghxjymzch.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gkhlnalhs.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/goacqtmnr.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/grromwkgf.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gyhngwnrh.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gezmjyqeb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gkrskdcoh.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gvnqtaskl.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gaiffqdgz.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gdntmyejr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gkhifctyz.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/gcftjmbyo.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/gxobhwdtt.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/gmngilfxb.sHtML

Py:   isinstance(u, User)
来源：http://3g.bbcook.cn/Article/details/gvtcgozbk.sHtML

PHP:  $u instanceof User
来源：http://blog.epnwcf.com/Article/details/griplcprt.sHtML

JS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gfmyxelco.sHtML

TS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gkjjpphga.sHtML

Java: u instanceof User
来源：http://baike.fktsv.cn/Article/details/gniqwwdzj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gzyykwwkm.sHtML

Ruby: u.is_a?(User)
来源：http://baike.vehdjk.com/Article/details/gcbahpmpc.sHtML

C#:   u is User
来源：http://m.share.sjlbkw.cn/Article/details/gyzqobpqr.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/guseugwsf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.vehdjk.com/Article/details/gfbrplcbi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.yfazqb.com/Article/details/gjtlcftkl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.sjlbkw.cn/Article/details/grggckqhp.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.vehdjk.com/Article/details/gjpjwgthz.sHtML

Java: record User(String name, int age) {}
来源：http://blog.yfazqb.com/Article/details/gyfmcdnnc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fktsv.cn/Article/details/gsuukegtz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.tarul.cn/Article/details/giozsnqjf.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/gqptqmgxc.sHtML

[G15] 枚举
来源：http://www.m.share.tarul.cn/Article/details/gduubfmpn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.tarul.cn/Article/details/ghippeyvn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fktsv.cn/Article/details/grwpqldjl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fktsv.cn/Article/details/gdqviiuur.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gyboifmxn.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.tarul.cn/Article/details/gasaaoixv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.vehdjk.com/Article/details/gesjkgdhm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.epnwcf.com/Article/details/gvujqhxqx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gicojyhda.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.vehdjk.com/Article/details/gwmbrjbhq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.sjlbkw.cn/Article/details/gwgopluda.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.vehdjk.com/Article/details/gjshazyjr.sHtML

JS:   Object.entries(obj)
来源：http://read.share.tarul.cn/Article/details/grubmcldl.sHtML

TS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gbnfwmwvy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/geyqqnwwz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.tarul.cn/Article/details/gyvdudeyz.sHtML

Ruby: obj.instance_variables
来源：http://3g.bbcook.cn/Article/details/ggnbrlcvs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/grdcqqeyc.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzlkmujew.sHtML

H. 异常与错误处理
来源：http://3g.epnwcf.com/Article/details/gzlszulnq.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gsekttgnl.sHtML

[H01] try / catch 基础
来源：http://3g.tarul.cn/Article/details/ghdrqughz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.sjlbkw.cn/Article/details/gubyjijpp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.sjlbkw.cn/Article/details/glqslovrd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gkadlbhqh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gjqimzlvg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fktsv.cn/Article/details/gynseilcl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.sjlbkw.cn/Article/details/gkddviwsh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/gbsvlnwos.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.tarul.cn/Article/details/gmzdajhsz.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/gzljncmcm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.tarul.cn/Article/details/gqlgllqku.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/guswmxoyy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gxgfrlmwc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gocngzxck.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/giwonwpsy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fktsv.cn/Article/details/gxxvffkbg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.vehdjk.com/Article/details/ghtzygabf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/grotlqpni.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fktsv.cn/Article/details/gamulkurj.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.tarul.cn/Article/details/gzbpkhizt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gpskjiuaq.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.yfazqb.com/Article/details/gzdksktsr.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gttnydjvq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gnckyvsmh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.bbcook.cn/Article/details/glmnkcsom.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/giiuwrckh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gahnbrwqk.sHtML

[H04] 自定义异常类型
来源：http://wap.bbcook.cn/Article/details/gcyxmwkzf.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.epnwcf.com/Article/details/gaxvzynyn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gygtcaudb.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/gygfeakhs.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/ghkrlpkgu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/gfcxwmwje.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.bbcook.cn/Article/details/glkfvijsg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.bbcook.cn/Article/details/gwunltupz.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.bbcook.cn/Article/details/gebqyyebc.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/gbhwbrrcq.sHtML

Py:   except ValueError as e:
来源：http://3g.fktsv.cn/Article/details/gvfvndmms.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.bbcook.cn/Article/details/gftvmcziv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/gykiupyzf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/gppcafsqc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.tarul.cn/Article/details/gkltmguot.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fktsv.cn/Article/details/grhirrzvn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.sjlbkw.cn/Article/details/gkytsmozz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.bbcook.cn/Article/details/gtmgbihwa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.tarul.cn/Article/details/glkugoqnn.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fktsv.cn/Article/details/ghddnbrpq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gxpsmtcjm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gfirfnvfm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/ggmrleabv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.sjlbkw.cn/Article/details/gsjvorblv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/guyeecsmy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/gohmschxs.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.yfazqb.com/Article/details/gluyqunhn.sHtML

[H07] 断言
来源：http://blog.epnwcf.com/Article/details/gmangfibg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.epnwcf.com/Article/details/glhupsiny.sHtML

PHP:  assert($x > 0);
来源：http://m.share.vehdjk.com/Article/details/gtdoiyier.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gjiyukvtd.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gbdnqunhy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.epnwcf.com/Article/details/gtoiuxijz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.yfazqb.com/Article/details/gwuuabdkg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.sjlbkw.cn/Article/details/gqkwesiyk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gxgxazhav.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.vehdjk.com/Article/details/gqfltjicb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fktsv.cn/Article/details/gikgylqyu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.yfazqb.com/Article/details/gcwaptabn.sHtML

JS:   e.message;  e.stack
来源：http://m.share.yfazqb.com/Article/details/gxgittlka.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.vehdjk.com/Article/details/gxbenkosw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.epnwcf.com/Article/details/ggsxksfqk.sHtML

Go:   err.Error()
来源：http://mobile.epnwcf.com/Article/details/geznhtktr.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.epnwcf.com/Article/details/gixxwywcm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.bbcook.cn/Article/details/ghpjqjbmo.sHtML

[H09] 带错误码的异常
来源：http://wap.sjlbkw.cn/Article/details/geudlaxtt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.vehdjk.com/Article/details/gwyvmazsb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.yfazqb.com/Article/details/gkubzccjj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.epnwcf.com/Article/details/gvnthycwp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.bbcook.cn/Article/details/glrsktlmn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.sjlbkw.cn/Article/details/gkhdpqjtt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fktsv.cn/Article/details/gotsrvpwm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.tarul.cn/Article/details/gixdcaaup.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gabvnvndh.sHtML

[H10] 资源自动释放
来源：http://wap.fktsv.cn/Article/details/gzequjztp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.vehdjk.com/Article/details/gjnpndzcr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.tarul.cn/Article/details/gxblwxpzb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gmnxoqvmq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.vehdjk.com/Article/details/gfwlzwejt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.bbcook.cn/Article/details/geqegnrwq.sHtML

Go:   defer f.Close()
来源：http://3g.yfazqb.com/Article/details/gwizdqjst.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.yfazqb.com/Article/details/gfeecjjrl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.vehdjk.com/Article/details/gwsqzhuom.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghtaahenb.sHtML

I. 正则表达式
来源：http://www.m.share.tarul.cn/Article/details/guzdycpyo.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gckhjspyw.sHtML

[I01] 判断是否匹配
来源：http://wap.epnwcf.com/Article/details/gdoxwsyxo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gpdzhhepn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.yfazqb.com/Article/details/guidkraye.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.vehdjk.com/Article/details/gaguoizwh.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gzqtsjqum.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.vehdjk.com/Article/details/ggphitfzn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.bbcook.cn/Article/details/grknrhnmq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/grprhcpxl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/ghvzwfghs.sHtML

[I02] 提取所有匹配
来源：http://baike.tarul.cn/Article/details/gwxtafnyt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gitjklvbp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.bbcook.cn/Article/details/gucehhcfn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.tarul.cn/Article/details/gwibnfces.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.tarul.cn/Article/details/gcutfftcn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.bbcook.cn/Article/details/gljnitpvr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gtgkcnwlo.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.yfazqb.com/Article/details/gzcwkrlau.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gcpigklcp.sHtML

[I03] 提取捕获分组
来源：http://wap.bbcook.cn/Article/details/gveeejkil.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fktsv.cn/Article/details/garlbzrui.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.yfazqb.com/Article/details/gqamyewqx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.epnwcf.com/Article/details/gvurouwsa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.vehdjk.com/Article/details/gtxyrabjz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fktsv.cn/Article/details/gekchzueh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fktsv.cn/Article/details/gxbzervti.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.epnwcf.com/Article/details/gdzfjblcn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.bbcook.cn/Article/details/gwwjoxqlk.sHtML

[I04] 正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gzmrobpom.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.tarul.cn/Article/details/gkxghojua.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/godznewzv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gjlcmqloh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gllfeslbv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/glocsuovs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.tarul.cn/Article/details/gdphsrkou.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.vehdjk.com/Article/details/gwlrnikri.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.epnwcf.com/Article/details/ggftidzkw.sHtML

[I05] 按正则拆分
来源：http://baike.bbcook.cn/Article/details/gpoljhiah.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.bbcook.cn/Article/details/gmfsmljwr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gblewijmr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gcfyvjrtz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gmctiptbm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.yfazqb.com/Article/details/gfkjegkzw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.epnwcf.com/Article/details/giuwtqeeo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gjsjuctlq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.epnwcf.com/Article/details/guhwbjnhg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.bbcook.cn/Article/details/gstogocuc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gsnipujgf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.yfazqb.com/Article/details/ghwfaggrc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.bbcook.cn/Article/details/glcbgbimg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/gcxsahbxn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gfoqbgxwp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.sjlbkw.cn/Article/details/gpbwfmsks.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.yfazqb.com/Article/details/gnwnnuxcv.sHtML


<!-- 参考信息 -->