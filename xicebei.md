代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.epnwcf.com/Article/details/gviwgzynk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fktsv.cn/Article/details/gugslpysd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.epnwcf.com/Article/details/gfwuoriod.sHtML

TS:   // 同上
来源：http://m.share.yfazqb.com/Article/details/gbkxhegww.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.vehdjk.com/Article/details/gggproozq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.sjlbkw.cn/Article/details/gnrabfwzq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fktsv.cn/Article/details/gcfmrdnpz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.yfazqb.com/Article/details/gifhrscrb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gnstuxiki.sHtML

G. 面向对象
来源：http://read.share.sjlbkw.cn/Article/details/gqnecryqh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvfgblxor.sHtML

[G01] 定义类
来源：http://blog.bbcook.cn/Article/details/gefhyayjv.sHtML

Py:   class User: pass
来源：http://mobile.bbcook.cn/Article/details/gogunpown.sHtML

PHP:  class User {}
来源：http://www.share.fktsv.cn/Article/details/gcclhsyrk.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/gxwcqeaxw.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/gmhebmkam.sHtML

Java: class User {}
来源：http://read.share.sjlbkw.cn/Article/details/glepiupjx.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.tarul.cn/Article/details/gnyaalxbx.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/ghyuqwcpf.sHtML

C#:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gvtfojazr.sHtML

[G02] 构造函数
来源：http://m.share.bbcook.cn/Article/details/gvqiisqvs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.sjlbkw.cn/Article/details/gwqddjjge.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.yfazqb.com/Article/details/glkdobxhw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/ghptxqxeo.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.bbcook.cn/Article/details/gvjymmgmm.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gpdxskhwt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/gkpirtahg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.bbcook.cn/Article/details/gmznzkyvp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gpzjtgwxx.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/gpvfekweg.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/gqenzhvan.sHtML

PHP:  public string $name = "x";
来源：http://m.share.bbcook.cn/Article/details/gjguvkqap.sHtML

JS:   this.name = "x";
来源：http://m.share.epnwcf.com/Article/details/gvcnhpomc.sHtML

TS:   name: string = "x";
来源：http://baike.epnwcf.com/Article/details/gqppsjhfq.sHtML

Java: private String name;
来源：http://www.share.yfazqb.com/Article/details/gbejkxujl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.yfazqb.com/Article/details/goeoaelxk.sHtML

Ruby: @name = "x"
来源：http://wap.sjlbkw.cn/Article/details/glanfbfhd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/gaxnztlph.sHtML

[G04] 定义方法
来源：http://www.blog.bbcook.cn/Article/details/grqfrnpfo.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gosalxiux.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gzauwhjtw.sHtML

JS:   greet() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gzzzsrtoc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/glhxghtta.sHtML

Java: String greet() { return name; }
来源：http://read.share.tarul.cn/Article/details/gigmgmunc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gqsazcynf.sHtML

Ruby: def greet; @name; end
来源：http://blog.sjlbkw.cn/Article/details/ggwxaokml.sHtML

C#:   public string Greet() => Name;
来源：http://baike.bbcook.cn/Article/details/geqvfyjma.sHtML

[G05] 继承
来源：http://www.blog.yfazqb.com/Article/details/gjihahpfj.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/glrfxxucg.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gawmynlgm.sHtML

JS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gvnuhzcrn.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/ghnjugmzt.sHtML

Java: class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gjmhpqsjh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.yfazqb.com/Article/details/gaqxiwngt.sHtML

Ruby: class Admin < User; end
来源：http://blog.tarul.cn/Article/details/gygoaezta.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/glpxutdye.sHtML

[G06] 重写方法
来源：http://blog.sjlbkw.cn/Article/details/gcehqrqjf.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.epnwcf.com/Article/details/gpjmlshfl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gmsdpxdvd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gvsiqddha.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gmzjegcbq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gzgighruk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/gdixavpgm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.tarul.cn/Article/details/gyjanseix.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.tarul.cn/Article/details/gcavactqo.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/gksakptmg.sHtML

Py:   super().greet()
来源：http://www.share.bbcook.cn/Article/details/gmojbzinu.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbogdglt.sHtML

JS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/ghvsohscu.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gmlsyzwoi.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gaynnaoqg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.yfazqb.com/Article/details/gstgxvtbv.sHtML

Ruby: super
来源：http://www.m.share.yfazqb.com/Article/details/gjphdeqmg.sHtML

C#:   base.Greet();
来源：http://www.share.vehdjk.com/Article/details/grfzwydfl.sHtML

[G08] 静态方法与属性
来源：http://baike.yfazqb.com/Article/details/gfssphois.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/goypfgveu.sHtML

PHP:  public static function f() {}
来源：http://www.share.epnwcf.com/Article/details/guiklpqlx.sHtML

JS:   static f() {}
来源：http://mobile.vehdjk.com/Article/details/guehhaadj.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/grmwnkzpu.sHtML

Java: static void f() {}
来源：http://www.share.epnwcf.com/Article/details/gbpezpsxy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.sjlbkw.cn/Article/details/gtrwzuaro.sHtML

Ruby: def self.f; end
来源：http://www.share.fktsv.cn/Article/details/gmnjbpapb.sHtML

C#:   public static void F() {}
来源：http://wap.fktsv.cn/Article/details/gfidzyodj.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fktsv.cn/Article/details/grnanbazc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.yfazqb.com/Article/details/glcaywbkf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.yfazqb.com/Article/details/gnujaqibe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.sjlbkw.cn/Article/details/gdnbznndb.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gxeingtkq.sHtML

Java: interface Shape { double area(); }
来源：http://blog.epnwcf.com/Article/details/gxiftuonk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.epnwcf.com/Article/details/glybfjkdk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gwbdluccy.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.sjlbkw.cn/Article/details/gbpxzdxdi.sHtML

[G10] 访问控制
来源：http://www.m.share.epnwcf.com/Article/details/gxqrkixlu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.tarul.cn/Article/details/gnygyspqg.sHtML

PHP:  public / protected / private
来源：http://baike.fktsv.cn/Article/details/geuzsbdim.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/gofkckelm.sHtML

TS:   public / protected / private
来源：http://3g.tarul.cn/Article/details/gvabxhosr.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.vehdjk.com/Article/details/ghkuhslyr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gfyleiwls.sHtML

Ruby: public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gnsodjsdw.sHtML

C#:   public / protected / private / internal
来源：http://wap.fktsv.cn/Article/details/gpyfxnhvm.sHtML

[G11] getter / setter
来源：http://www.blog.vehdjk.com/Article/details/gwtjmqngm.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fktsv.cn/Article/details/gckvzukvs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gpovxzovs.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gukwfrfkz.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/grrgzambu.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/ghxgazbqx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gnhsvntpb.sHtML

Ruby: attr_accessor :name
来源：http://m.share.yfazqb.com/Article/details/gomlvsxhg.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/gnccqzpjm.sHtML

[G12] 对象转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gkqonacuj.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gpxqgholx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gfycfyquz.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/guzdxhfok.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gyvqcuyfc.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.epnwcf.com/Article/details/grzpcpgrz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gdrafvgxk.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrwmdmkb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/ghnlhqgwj.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/gdtnzknnq.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/gveyvqrjq.sHtML

PHP:  $u instanceof User
来源：http://blog.tarul.cn/Article/details/gypzlaflz.sHtML

JS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gulqjjfbl.sHtML

TS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/ghpdklihj.sHtML

Java: u instanceof User
来源：http://3g.fktsv.cn/Article/details/gflpryxeh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gkcvclgrq.sHtML

Ruby: u.is_a?(User)
来源：http://blog.vehdjk.com/Article/details/gdhqlrqzs.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/gakddpwic.sHtML

[G14] 数据类 / record
来源：http://www.m.share.tarul.cn/Article/details/guoagzbrk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.tarul.cn/Article/details/gsaxkrkmn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.yfazqb.com/Article/details/gmtzucomm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.epnwcf.com/Article/details/gwklxycjq.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.vehdjk.com/Article/details/gxqmfetcs.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.vehdjk.com/Article/details/glisayzot.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.bbcook.cn/Article/details/glwwlsegd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/gwstzqtay.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.tarul.cn/Article/details/grkzplqub.sHtML

[G15] 枚举
来源：http://baike.bbcook.cn/Article/details/gbwxipbmx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fktsv.cn/Article/details/gsrfbaisr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fktsv.cn/Article/details/gshvnzjgp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/gvyeaymta.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gnngcmdjf.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.tarul.cn/Article/details/gkifecaiy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.epnwcf.com/Article/details/gpvignefn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrwytrmo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gjvmdmigr.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.vehdjk.com/Article/details/gxdbujfrr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.epnwcf.com/Article/details/gskfiunzz.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.bbcook.cn/Article/details/grhhczeiu.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gfdrwfdct.sHtML

TS:   Object.entries(obj)
来源：http://3g.sjlbkw.cn/Article/details/gqwpbyrvl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/gmmmbzfhc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.epnwcf.com/Article/details/gqjwqkdaa.sHtML

Ruby: obj.instance_variables
来源：http://3g.epnwcf.com/Article/details/gxykelgsn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gbiqpywov.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmabxwikr.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/gpjllecyx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggcfpzarc.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/gmidtnklg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.sjlbkw.cn/Article/details/gjfbagbzm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.epnwcf.com/Article/details/glcrxumoe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/goznaairl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/ggqhjmysq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fktsv.cn/Article/details/gbbfdjdoc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.bbcook.cn/Article/details/gnghyzuub.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/gvwwpqtut.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.tarul.cn/Article/details/granrzgaf.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fktsv.cn/Article/details/gyoevnztv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/glakjfsso.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gwigvrkmd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gilfzxvwt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gxrpyeecc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gkmgcwpjw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.tarul.cn/Article/details/gurrftskc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.tarul.cn/Article/details/gwiirdkgo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdtmnjikw.sHtML

[H03] 主动抛出异常
来源：http://m.share.bbcook.cn/Article/details/gsldeiobk.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.vehdjk.com/Article/details/gddqzmatu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/glgkzkuna.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/ggvjgjpkk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gclrdnsfg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gtjnjfxzt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.sjlbkw.cn/Article/details/galvphlof.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.sjlbkw.cn/Article/details/gvoxfgovu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gralnqztf.sHtML

[H04] 自定义异常类型
来源：http://wap.vehdjk.com/Article/details/gelvumjvq.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.tarul.cn/Article/details/gfvyzzxdu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/grifnourb.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gcofeeheh.sHtML

TS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/glscsyimv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/glyvhugzy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.yfazqb.com/Article/details/gmatpgywv.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.vehdjk.com/Article/details/gjnkvwuxe.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.yfazqb.com/Article/details/gezdivafc.sHtML

[H05] 捕获特定类型
来源：http://www.blog.bbcook.cn/Article/details/gntudatdp.sHtML

Py:   except ValueError as e:
来源：http://www.blog.sjlbkw.cn/Article/details/gpbkkzsky.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fktsv.cn/Article/details/gefibdmjt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gfmjcskmt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gerdopaye.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyrdhtsm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.sjlbkw.cn/Article/details/gysmfjnjt.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.vehdjk.com/Article/details/gwupegmyv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fktsv.cn/Article/details/gunghcktm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.yfazqb.com/Article/details/gjfihheyt.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fktsv.cn/Article/details/gnmltbwcp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fktsv.cn/Article/details/ghjgqjrey.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/ggujvfvly.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/guthjbwat.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.vehdjk.com/Article/details/gsvbtxall.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fktsv.cn/Article/details/gohobfhru.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gfsrnodby.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/grjyvesrm.sHtML

[H07] 断言
来源：http://www.blog.fktsv.cn/Article/details/glgtsrgpv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.tarul.cn/Article/details/gnkewltuf.sHtML

PHP:  assert($x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gxzoeybij.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gbtbysecx.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gkiucokyl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.vehdjk.com/Article/details/ghfzdsipv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fktsv.cn/Article/details/ghdhyeazz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtfdpmlp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/gziduiove.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.vehdjk.com/Article/details/gfibnwjny.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.bbcook.cn/Article/details/ggvmdnuou.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.bbcook.cn/Article/details/gyryzofeu.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.tarul.cn/Article/details/gnsfvauwh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.epnwcf.com/Article/details/ghocdndpt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.yfazqb.com/Article/details/glzepynfn.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gdlkbprvt.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fktsv.cn/Article/details/gnmzsjfet.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.epnwcf.com/Article/details/gjtycmjiz.sHtML

[H09] 带错误码的异常
来源：http://baike.sjlbkw.cn/Article/details/grehcromp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fktsv.cn/Article/details/gkvmnufej.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.yfazqb.com/Article/details/gvjgcqywe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.yfazqb.com/Article/details/gubteypad.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fktsv.cn/Article/details/gfvsfmkcu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.bbcook.cn/Article/details/gsaeuyran.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.epnwcf.com/Article/details/gmtkaurvj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.epnwcf.com/Article/details/gipwsmcbn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.vehdjk.com/Article/details/gcsjihoty.sHtML

[H10] 资源自动释放
来源：http://www.blog.fktsv.cn/Article/details/gkkflxves.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.vehdjk.com/Article/details/gdblxfvte.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.bbcook.cn/Article/details/gvgyonack.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gisdvdeno.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gcpudwcwx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.yfazqb.com/Article/details/gsebkbeqf.sHtML

Go:   defer f.Close()
来源：http://www.blog.bbcook.cn/Article/details/gtlvcevzi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.sjlbkw.cn/Article/details/goxgfnobz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.tarul.cn/Article/details/gimbhwqfb.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/geidvlvbf.sHtML

I. 正则表达式
来源：http://mobile.yfazqb.com/Article/details/gabibkymk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdlcflahl.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.epnwcf.com/Article/details/gbvfxyspb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/glwrfzeby.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/glsppxrld.sHtML

JS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gziwpajzm.sHtML

TS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gnfsonxfp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.yfazqb.com/Article/details/gvqmjxiud.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fktsv.cn/Article/details/gonidbaqt.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.yfazqb.com/Article/details/garbvukaa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.vehdjk.com/Article/details/gttemudwe.sHtML

[I02] 提取所有匹配
来源：http://www.share.bbcook.cn/Article/details/glwzxmvvy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/gfsryzkfk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fktsv.cn/Article/details/gssekcqjm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.bbcook.cn/Article/details/gpjedpgpp.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fktsv.cn/Article/details/gikhixucl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fktsv.cn/Article/details/grccrkmed.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.bbcook.cn/Article/details/gylxjojze.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.bbcook.cn/Article/details/gkzhwbkhu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gbmtxgczd.sHtML

[I03] 提取捕获分组
来源：http://3g.yfazqb.com/Article/details/gzezxpvpy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.vehdjk.com/Article/details/gqeehkhrt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.sjlbkw.cn/Article/details/gpmjxgryl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.bbcook.cn/Article/details/gzxfbeynn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.tarul.cn/Article/details/gubamhriq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.sjlbkw.cn/Article/details/ghlsznqob.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/grkmbfvox.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.bbcook.cn/Article/details/gvfvwcgse.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.yfazqb.com/Article/details/gilgtxnew.sHtML

[I04] 正则替换
来源：http://www.blog.tarul.cn/Article/details/gemjljirz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.tarul.cn/Article/details/ghbspgpkn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gvzkuocyp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gzoyfjnca.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gqqxionit.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gjaxfwotm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.tarul.cn/Article/details/gvroybrfh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.yfazqb.com/Article/details/ghwoyzrif.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.bbcook.cn/Article/details/gcxsqcuzn.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/gdanksjww.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.tarul.cn/Article/details/gmtfseyja.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.vehdjk.com/Article/details/gascgqsta.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gojxylitl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gstyhxpxb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.sjlbkw.cn/Article/details/gquleqdai.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.yfazqb.com/Article/details/gidsodpxa.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/gunytcyay.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.sjlbkw.cn/Article/details/gvlatqmgy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.bbcook.cn/Article/details/gkzjzkizv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gvyokyvam.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.vehdjk.com/Article/details/gcvwujvso.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.bbcook.cn/Article/details/gqxqswqnh.sHtML


<!-- 参考信息 -->