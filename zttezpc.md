代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.bbcook.cn/Article/details/geasqiwbl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/goasoxihb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fktsv.cn/Article/details/gzixxgtpt.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/gvzfyzrdm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.sjlbkw.cn/Article/details/gtbjpadnr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.bbcook.cn/Article/details/gfgwzmlbs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.vehdjk.com/Article/details/gsieomckh.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/gyriuyizc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.epnwcf.com/Article/details/gswrdprhn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.sjlbkw.cn/Article/details/gmbuxhzwj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.bbcook.cn/Article/details/gbuneqtke.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.bbcook.cn/Article/details/gjjvaijds.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gtmbjkpko.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/gnzjxagxv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gtbrfvacg.sHtML

[G01] 定义类
来源：http://www.m.share.vehdjk.com/Article/details/gtvxbiyln.sHtML

Py:   class User: pass
来源：http://m.share.epnwcf.com/Article/details/gcfyxzejq.sHtML

PHP:  class User {}
来源：http://blog.tarul.cn/Article/details/gxldazxqv.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gykptpwga.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/gvsqaplml.sHtML

Java: class User {}
来源：http://m.share.fktsv.cn/Article/details/gxyyunnvq.sHtML

Go:   type User struct { Name string }
来源：http://blog.epnwcf.com/Article/details/griyvcazh.sHtML

Ruby: class User; end
来源：http://www.share.sjlbkw.cn/Article/details/gvstnvxjd.sHtML

C#:   class User {}
来源：http://3g.fktsv.cn/Article/details/gdfbvdnib.sHtML

[G02] 构造函数
来源：http://wap.epnwcf.com/Article/details/gusxbdcyv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.epnwcf.com/Article/details/gkdvobxwo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/gsnfgqbxj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/gxztsbtfr.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.epnwcf.com/Article/details/gevhiigai.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gzfmtsjmb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.tarul.cn/Article/details/gbdasulnl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.vehdjk.com/Article/details/gshpfmksi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.tarul.cn/Article/details/goroprgie.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/gshzqbvvy.sHtML

Py:   self.name = "x"
来源：http://wap.bbcook.cn/Article/details/gzkipamkg.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gfhjrfmrp.sHtML

JS:   this.name = "x";
来源：http://www.blog.tarul.cn/Article/details/gcefrlavl.sHtML

TS:   name: string = "x";
来源：http://read.share.bbcook.cn/Article/details/gpacnwabh.sHtML

Java: private String name;
来源：http://3g.fktsv.cn/Article/details/gsltacafh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.yfazqb.com/Article/details/gdplmoulo.sHtML

Ruby: @name = "x"
来源：http://m.share.fktsv.cn/Article/details/gskcpwvwk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/gjfhswuci.sHtML

[G04] 定义方法
来源：http://mobile.bbcook.cn/Article/details/grchseyfm.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/glfgnkegf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gxpiklpma.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/glmihcwcb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/goxwvbkku.sHtML

Java: String greet() { return name; }
来源：http://3g.tarul.cn/Article/details/giiocaqmy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gytosgltc.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/gxrwyuemu.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/ghdqctwik.sHtML

[G05] 继承
来源：http://read.share.sjlbkw.cn/Article/details/gmaomrrgo.sHtML

Py:   class Admin(User): pass
来源：http://3g.sjlbkw.cn/Article/details/gujpvpupn.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gjmvtyfai.sHtML

JS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/goodyxbyg.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/glxlsmcpi.sHtML

Java: class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gcjgzqkog.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.epnwcf.com/Article/details/ggjaejjac.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/gnbjvkbav.sHtML

C#:   class Admin : User {}
来源：http://read.share.epnwcf.com/Article/details/gkzkhrlfu.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/gwuxdhlbw.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fktsv.cn/Article/details/gnlcvitzz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gqyzjzafk.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gwqqpyyil.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/goylqhwcn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gzyfrdjgg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/grtbrwdac.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlltvkhc.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gtoipxlux.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/gntcmxjfw.sHtML

Py:   super().greet()
来源：http://read.share.yfazqb.com/Article/details/gstvzjmvi.sHtML

PHP:  parent::greet();
来源：http://wap.bbcook.cn/Article/details/gzxqqfstp.sHtML

JS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gqyyiuhyl.sHtML

TS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/ghgxuptnn.sHtML

Java: super.greet();
来源：http://mobile.bbcook.cn/Article/details/gqlcduaac.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.bbcook.cn/Article/details/gjixanuyq.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/gcyxekxns.sHtML

C#:   base.Greet();
来源：http://wap.epnwcf.com/Article/details/gmavavtcu.sHtML

[G08] 静态方法与属性
来源：http://m.share.sjlbkw.cn/Article/details/gkgbrkvvi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.vehdjk.com/Article/details/gcpgfkkmk.sHtML

PHP:  public static function f() {}
来源：http://m.share.epnwcf.com/Article/details/gbzogioye.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gcfyflbld.sHtML

TS:   static f(): void {}
来源：http://www.blog.bbcook.cn/Article/details/gebwinubm.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/gjrlxbilf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fktsv.cn/Article/details/gjddqxxwi.sHtML

Ruby: def self.f; end
来源：http://read.share.epnwcf.com/Article/details/gzcimdeyk.sHtML

C#:   public static void F() {}
来源：http://www.m.share.bbcook.cn/Article/details/ggrdawlyv.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/gtnjcprwy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/ggwanianm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.yfazqb.com/Article/details/gzwrtwkdt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.bbcook.cn/Article/details/gxmntnwoi.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gcsmiytiz.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.tarul.cn/Article/details/gkxqpgmlh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.sjlbkw.cn/Article/details/gxzgtqkci.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.yfazqb.com/Article/details/gqyjbvwig.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gtpegbesb.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/ghdxrjhif.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/gmglqkmvx.sHtML

PHP:  public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gohitakju.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/geerjtoty.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gjjnxsptv.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.sjlbkw.cn/Article/details/gryyghywe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/gaozmcdqt.sHtML

Ruby: public / protected / private
来源：http://wap.bbcook.cn/Article/details/gorijsinx.sHtML

C#:   public / protected / private / internal
来源：http://blog.sjlbkw.cn/Article/details/gtstnvgve.sHtML

[G11] getter / setter
来源：http://blog.yfazqb.com/Article/details/gxmaivzri.sHtML

Py:   @property 与 @x.setter
来源：http://3g.epnwcf.com/Article/details/gazizapqs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gyiqsyfsy.sHtML

JS:   get name() { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gorsmlmxb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gfqnvjrue.sHtML

Java: public String getName() { return name; }
来源：http://read.share.tarul.cn/Article/details/gikvvgdrn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gnuzfupfb.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fktsv.cn/Article/details/gbhtckbix.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.sjlbkw.cn/Article/details/gujqgabje.sHtML

[G12] 对象转字符串
来源：http://baike.sjlbkw.cn/Article/details/grbstcfif.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gcgdeswop.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gguqbrocf.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gqqkwuhfe.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gfxpserol.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gbuyujiqj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gnerfthtx.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gendktbhl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gmdoyvjxx.sHtML

[G13] 判断对象类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gowtofrlw.sHtML

Py:   isinstance(u, User)
来源：http://wap.tarul.cn/Article/details/gqrcssotk.sHtML

PHP:  $u instanceof User
来源：http://mobile.yfazqb.com/Article/details/ggdnimsvp.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gpyexjewe.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gwuebgqkg.sHtML

Java: u instanceof User
来源：http://wap.fktsv.cn/Article/details/giqgejyyo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.sjlbkw.cn/Article/details/guddukysv.sHtML

Ruby: u.is_a?(User)
来源：http://3g.epnwcf.com/Article/details/goqzcoxgz.sHtML

C#:   u is User
来源：http://blog.yfazqb.com/Article/details/gfdmcwaic.sHtML

[G14] 数据类 / record
来源：http://read.share.sjlbkw.cn/Article/details/gwnrlmkko.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.bbcook.cn/Article/details/gcfqnjwuw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gynsryfza.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.yfazqb.com/Article/details/gheldixje.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.bbcook.cn/Article/details/gomyjxaix.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/grwzuwjpv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.bbcook.cn/Article/details/gdjlfcqba.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/gutwfuvra.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/gabafmqll.sHtML

[G15] 枚举
来源：http://wap.sjlbkw.cn/Article/details/gotmxpvtb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.vehdjk.com/Article/details/grfthjirs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.bbcook.cn/Article/details/ghdrkbgrc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.yfazqb.com/Article/details/gogcmvyvk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gehfauyrk.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.epnwcf.com/Article/details/gmjpewwst.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/gxjhybkno.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.yfazqb.com/Article/details/gglewgjme.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gaqqltsgb.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fktsv.cn/Article/details/gskmnqhih.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwnbqxjh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.tarul.cn/Article/details/gwdrrzeqg.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gyqxgnair.sHtML

TS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gtirvzeye.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.epnwcf.com/Article/details/gyknbhwwt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/gbpnynsre.sHtML

Ruby: obj.instance_variables
来源：http://www.share.vehdjk.com/Article/details/gyyejivsf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.yfazqb.com/Article/details/gxsvkrfll.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzuvxkohi.sHtML

H. 异常与错误处理
来源：http://mobile.epnwcf.com/Article/details/gyvugzvdh.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxcxtpbzd.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gopttuqjj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.tarul.cn/Article/details/gegckxblz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.tarul.cn/Article/details/gxdsmyjbt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/glbquphht.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gvbbujhrb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.vehdjk.com/Article/details/gkbszxkeb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/gzaqtxetd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.bbcook.cn/Article/details/gdzdviepv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fktsv.cn/Article/details/gbqxxhtef.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvdvlikq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.yfazqb.com/Article/details/gzvmnhygf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/guocwketz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/glftkxdbk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/grtvjbhuz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gnetofytv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.epnwcf.com/Article/details/gzqfqaaep.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.bbcook.cn/Article/details/gjyenmawm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fktsv.cn/Article/details/ggjqnxsdw.sHtML

[H03] 主动抛出异常
来源：http://mobile.vehdjk.com/Article/details/gjmwckfgs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fktsv.cn/Article/details/gvhjunmow.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gxiaezroh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gughmqcqm.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gehibsjjr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gwiqxymen.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.yfazqb.com/Article/details/gqtdhlphs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.bbcook.cn/Article/details/gfozwimxf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gqsoopcvm.sHtML

[H04] 自定义异常类型
来源：http://m.share.sjlbkw.cn/Article/details/gmbzqnatu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.bbcook.cn/Article/details/guoqajrri.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/gunxejsnn.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gorrxakmv.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gejsosdjr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/glozhkhmo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.vehdjk.com/Article/details/gwivehttb.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.bbcook.cn/Article/details/gzxefqxmc.sHtML

C#:   class MyException : Exception {}
来源：http://3g.bbcook.cn/Article/details/gugirhmea.sHtML

[H05] 捕获特定类型
来源：http://read.share.tarul.cn/Article/details/gbuawelrf.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fktsv.cn/Article/details/ghuwzceim.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.epnwcf.com/Article/details/gkzxqifvs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/geweqodsu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/givyczjkd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fktsv.cn/Article/details/greefohcg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.yfazqb.com/Article/details/gwiwpfvuj.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/gzsyvqdwi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fktsv.cn/Article/details/gjdfrkssq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.tarul.cn/Article/details/gaspeeiti.sHtML

Py:   value = d.get("k") or default
来源：http://3g.yfazqb.com/Article/details/gytewrzdz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gqvuunkof.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/gjuwfdkzd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gnclwcqhw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.sjlbkw.cn/Article/details/glldnkquc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.vehdjk.com/Article/details/gxrlpjlry.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.yfazqb.com/Article/details/gqzxfahhp.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.tarul.cn/Article/details/gkxfxxwok.sHtML

[H07] 断言
来源：http://blog.vehdjk.com/Article/details/gxjqnknsc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gegzvngeq.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gxbozmist.sHtML

JS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gjgnfmksu.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gxfmciljp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fktsv.cn/Article/details/gduatzoym.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.epnwcf.com/Article/details/glqvfblyf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.yfazqb.com/Article/details/glqythfug.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.tarul.cn/Article/details/gclffcmka.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.sjlbkw.cn/Article/details/gxlwrpdmu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.vehdjk.com/Article/details/gspqofrxm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.vehdjk.com/Article/details/gsccuoynq.sHtML

JS:   e.message;  e.stack
来源：http://blog.yfazqb.com/Article/details/gdbudnlrg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.sjlbkw.cn/Article/details/griebyamd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.yfazqb.com/Article/details/grubjccsp.sHtML

Go:   err.Error()
来源：http://www.share.epnwcf.com/Article/details/gpvqfrmod.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.yfazqb.com/Article/details/geuqsxsao.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/gnhscusey.sHtML

[H09] 带错误码的异常
来源：http://3g.fktsv.cn/Article/details/gtubuolhz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.epnwcf.com/Article/details/gbxkvlwui.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.vehdjk.com/Article/details/glkconxzs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.tarul.cn/Article/details/gxeoeuapq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.vehdjk.com/Article/details/ghvxltvdv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.sjlbkw.cn/Article/details/gmuwflulu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.epnwcf.com/Article/details/gnggukajl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fktsv.cn/Article/details/gtsimmitp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.tarul.cn/Article/details/gkgwpbmlu.sHtML

[H10] 资源自动释放
来源：http://www.m.share.sjlbkw.cn/Article/details/glwwmeycb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.bbcook.cn/Article/details/gzsudtymx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fktsv.cn/Article/details/gszeythnc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.sjlbkw.cn/Article/details/gklmdpomg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/glrtrlnax.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.tarul.cn/Article/details/gbhlxyvhv.sHtML

Go:   defer f.Close()
来源：http://3g.sjlbkw.cn/Article/details/gtmyzdwsn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.epnwcf.com/Article/details/gdurturpd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.vehdjk.com/Article/details/gpwfpifev.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gcmgoskni.sHtML

I. 正则表达式
来源：http://www.share.vehdjk.com/Article/details/gwogpagyy.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gzvydoris.sHtML

[I01] 判断是否匹配
来源：http://baike.tarul.cn/Article/details/gwccebfdv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/gqiwruogd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.tarul.cn/Article/details/guundqhor.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/goaaontes.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gcdoefmml.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.epnwcf.com/Article/details/glwdfmlei.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.vehdjk.com/Article/details/gugjbbsgb.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gmtcfrzxn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gikgtfxuz.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/gyupdmsku.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/grnghjgjm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.yfazqb.com/Article/details/glpavefmd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fktsv.cn/Article/details/gngdcdnhv.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fktsv.cn/Article/details/giuxbagkv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.tarul.cn/Article/details/gxtmifrnj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.tarul.cn/Article/details/gietepzai.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.yfazqb.com/Article/details/gxevbqszv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.yfazqb.com/Article/details/gadrihbun.sHtML

[I03] 提取捕获分组
来源：http://baike.sjlbkw.cn/Article/details/gdfzlqaud.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.tarul.cn/Article/details/gwwhsuzue.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.sjlbkw.cn/Article/details/glcspuzap.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fktsv.cn/Article/details/gvunjmkwa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fktsv.cn/Article/details/gjvyafodm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gocbhqlmp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.yfazqb.com/Article/details/gjfaezykm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.epnwcf.com/Article/details/gbziyauct.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.tarul.cn/Article/details/gkuftvssh.sHtML

[I04] 正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gwbvyzkcn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.vehdjk.com/Article/details/gnegtmjtv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.bbcook.cn/Article/details/golzhlhew.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fktsv.cn/Article/details/gkaiodfnl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.sjlbkw.cn/Article/details/gsbdkgibt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gnkmfqpzy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.yfazqb.com/Article/details/ghlqwbylr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.tarul.cn/Article/details/ghgmehdep.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gxevdifad.sHtML

[I05] 按正则拆分
来源：http://www.m.share.epnwcf.com/Article/details/gdugfkdos.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.epnwcf.com/Article/details/gtildpuct.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fktsv.cn/Article/details/gepgoqleq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gpbbswuso.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/geprpqdgw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gkherulvk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gewruxzfq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gvdjigyex.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.yfazqb.com/Article/details/gxespyrmq.sHtML


<!-- 参考信息 -->