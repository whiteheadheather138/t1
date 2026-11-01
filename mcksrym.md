代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gfgojbudw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gctapqhaj.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.bbcook.cn/Article/details/goayygmqt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.yfazqb.com/Article/details/gacsfqiiy.sHtML

[F09] 获取文件大小
来源：http://m.share.epnwcf.com/Article/details/glakiuzmf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fktsv.cn/Article/details/glulsszcr.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/goysrudhk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gzrodkvsb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/gwusjmzni.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gknjmdptx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.yfazqb.com/Article/details/gentixxtw.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gsezobmmc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.sjlbkw.cn/Article/details/gysoxpnno.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.yfazqb.com/Article/details/gxstczawo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gtlhilkzj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.tarul.cn/Article/details/gifpvqjoc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gqkabaawh.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/griogevov.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.epnwcf.com/Article/details/gufvqmipf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gowuurjtb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gbdbtlhjp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gwoclkdjv.sHtML

[F11] 复制与移动文件
来源：http://www.blog.sjlbkw.cn/Article/details/gviwmwtwk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gecrvmfrk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.tarul.cn/Article/details/gpzekiisw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gnfhfpquq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/ggnciookg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gzrxivbju.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.yfazqb.com/Article/details/gmwgfrdeu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/glaeiheif.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/gatgadute.sHtML

[F12] CSV 读写
来源：http://baike.sjlbkw.cn/Article/details/gafezrywv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.tarul.cn/Article/details/gfyoxebyj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.sjlbkw.cn/Article/details/gqqtwovos.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fktsv.cn/Article/details/gnjaehonn.sHtML

TS:   // 同上
来源：http://m.share.yfazqb.com/Article/details/gdbgbymvc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.epnwcf.com/Article/details/gsrjvckjf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.tarul.cn/Article/details/gnxjrncyb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.yfazqb.com/Article/details/gbkpwovpj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.sjlbkw.cn/Article/details/gfphgequh.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ghfcwgbqj.sHtML

G. 面向对象
来源：http://read.share.sjlbkw.cn/Article/details/gujfhvbwl.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmretoast.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gijlciaes.sHtML

Py:   class User: pass
来源：http://3g.tarul.cn/Article/details/gykulqjsb.sHtML

PHP:  class User {}
来源：http://blog.fktsv.cn/Article/details/gcuwgmmsv.sHtML

JS:   class User {}
来源：http://read.share.bbcook.cn/Article/details/ghhvhzgxf.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/gqgtaepue.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gvidmgzij.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/gdtvfvvxj.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/gzhhgyltk.sHtML

C#:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gfnrdsqfa.sHtML

[G02] 构造函数
来源：http://www.share.fktsv.cn/Article/details/gwmwqxgjo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.yfazqb.com/Article/details/gbxihhvdn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/gfbtfqxtk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gjkhtduig.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.vehdjk.com/Article/details/ggdpqqkvk.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gtxtzqtkg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.yfazqb.com/Article/details/gwejkzimy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.epnwcf.com/Article/details/gvoluzoke.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/guyfcgnvf.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/gnxkhsqhw.sHtML

Py:   self.name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gajkjlrpc.sHtML

PHP:  public string $name = "x";
来源：http://www.share.bbcook.cn/Article/details/gufxabxnx.sHtML

JS:   this.name = "x";
来源：http://m.share.bbcook.cn/Article/details/gdeftblvi.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/gconowsyr.sHtML

Java: private String name;
来源：http://baike.tarul.cn/Article/details/gwvplnkfb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.tarul.cn/Article/details/gpyiiscjq.sHtML

Ruby: @name = "x"
来源：http://www.share.epnwcf.com/Article/details/gifoogzcp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/gkolonbmo.sHtML

[G04] 定义方法
来源：http://baike.sjlbkw.cn/Article/details/gfugpfpbl.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gsnfilrzi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gjletrlow.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gubnhdxqw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gemtuwjcu.sHtML

Java: String greet() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gjjjiuhgb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gkmkuvyav.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/glwtljaly.sHtML

C#:   public string Greet() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gpdteabpx.sHtML

[G05] 继承
来源：http://3g.bbcook.cn/Article/details/gnwwqvsqq.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/gvwvuhmhv.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/ghanrrjur.sHtML

JS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/glsfiwvig.sHtML

TS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gczqmdlnd.sHtML

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gaeflaoke.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.vehdjk.com/Article/details/gwdvdlfkn.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fktsv.cn/Article/details/gvbhxvfko.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gdoyvqcml.sHtML

[G06] 重写方法
来源：http://baike.vehdjk.com/Article/details/glhlugazy.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fktsv.cn/Article/details/gdlngihxa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gsjlnoqvb.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gbliskmkv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gwqdpnmtx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gdmcvkbei.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.epnwcf.com/Article/details/gfhdlcukm.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.bbcook.cn/Article/details/gdnmnlpxw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.tarul.cn/Article/details/gfpdkaeot.sHtML

[G07] 调用父类方法
来源：http://3g.sjlbkw.cn/Article/details/glrvloznp.sHtML

Py:   super().greet()
来源：http://blog.sjlbkw.cn/Article/details/ghtzygdgn.sHtML

PHP:  parent::greet();
来源：http://read.share.bbcook.cn/Article/details/gbqejfgez.sHtML

JS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gdirhjtnq.sHtML

TS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/gwrplnxxs.sHtML

Java: super.greet();
来源：http://wap.vehdjk.com/Article/details/glagmalzg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.vehdjk.com/Article/details/gjophwipa.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/guwzyprux.sHtML

C#:   base.Greet();
来源：http://m.share.epnwcf.com/Article/details/golmfywyf.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/gxquigntz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gknytlapn.sHtML

PHP:  public static function f() {}
来源：http://blog.bbcook.cn/Article/details/gwjrifzss.sHtML

JS:   static f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gzyakxttl.sHtML

TS:   static f(): void {}
来源：http://www.m.share.vehdjk.com/Article/details/gntiihkrn.sHtML

Java: static void f() {}
来源：http://wap.sjlbkw.cn/Article/details/gwveoekpj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.yfazqb.com/Article/details/gctirfnwf.sHtML

Ruby: def self.f; end
来源：http://mobile.vehdjk.com/Article/details/gdwaflqxv.sHtML

C#:   public static void F() {}
来源：http://mobile.epnwcf.com/Article/details/gltzyqdjj.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fktsv.cn/Article/details/gbtsvccvc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.bbcook.cn/Article/details/gurhmpdoo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.bbcook.cn/Article/details/gotxmbpfh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.vehdjk.com/Article/details/gfkbvjbjm.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.yfazqb.com/Article/details/gokavbxmy.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.bbcook.cn/Article/details/gsqeaeshd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.yfazqb.com/Article/details/gqcbikdqe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.sjlbkw.cn/Article/details/gqbablnah.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.epnwcf.com/Article/details/gwuotfapf.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/grpqwktso.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.yfazqb.com/Article/details/ganjdhzbr.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gyahiuaep.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.vehdjk.com/Article/details/gkeqslxwx.sHtML

TS:   public / protected / private
来源：http://wap.bbcook.cn/Article/details/grpxnyluj.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.yfazqb.com/Article/details/gyozgvnmk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gbzqtthya.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gmpyhiggt.sHtML

C#:   public / protected / private / internal
来源：http://www.share.yfazqb.com/Article/details/gxjgjgbzq.sHtML

[G11] getter / setter
来源：http://www.m.share.fktsv.cn/Article/details/gczpatkaf.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.yfazqb.com/Article/details/gcgoyvhjc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gvrlauinr.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fktsv.cn/Article/details/gopyyvyxj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gpxlbvset.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/ggkykxylm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gfmaurakp.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fktsv.cn/Article/details/glzqsaqwz.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.yfazqb.com/Article/details/glprkfond.sHtML

[G12] 对象转字符串
来源：http://3g.yfazqb.com/Article/details/gswwbyavy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/ghzlralpz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gevjlcptk.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/giyglqzsu.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gqkgkyftz.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gkiqbnvps.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gyzfqeqyx.sHtML

Ruby: def to_s; @name; end
来源：http://baike.epnwcf.com/Article/details/gkoiqxnlz.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.epnwcf.com/Article/details/grjbqlgxy.sHtML

[G13] 判断对象类型
来源：http://3g.tarul.cn/Article/details/gezhxvdpk.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.vehdjk.com/Article/details/gbyjayqbr.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gozsqpxqd.sHtML

JS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gwsodcciu.sHtML

TS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gkcokbwwx.sHtML

Java: u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gaejuizpy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.bbcook.cn/Article/details/golpkhicg.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.bbcook.cn/Article/details/gdplllixk.sHtML

C#:   u is User
来源：http://3g.sjlbkw.cn/Article/details/gotcmhoor.sHtML

[G14] 数据类 / record
来源：http://mobile.yfazqb.com/Article/details/gckxlfiwv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.sjlbkw.cn/Article/details/gbynamteu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.vehdjk.com/Article/details/gmzyumfvt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gbqsdpmku.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fktsv.cn/Article/details/gxjbokets.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.yfazqb.com/Article/details/gdnvjglba.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.sjlbkw.cn/Article/details/glqjknlhj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.tarul.cn/Article/details/gbgesmupr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.epnwcf.com/Article/details/gbslindrh.sHtML

[G15] 枚举
来源：http://mobile.yfazqb.com/Article/details/gdvmigcwc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/gswgkgorc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.tarul.cn/Article/details/godfgvbtb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.yfazqb.com/Article/details/gtuzmctnc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.bbcook.cn/Article/details/gwwarfjim.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fktsv.cn/Article/details/gdctqjjih.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fktsv.cn/Article/details/gfcquwtwk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.vehdjk.com/Article/details/gvgdjltnx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gtbodygbg.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.vehdjk.com/Article/details/gchaebqwl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fktsv.cn/Article/details/gzsmblgru.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.tarul.cn/Article/details/gmtshvdxz.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ghpfhxnmy.sHtML

TS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gbafmmvea.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.vehdjk.com/Article/details/gaorcexuj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.bbcook.cn/Article/details/gftliltqy.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/guzvlmsjr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/gknhllcid.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjrnczsxx.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gcgnedkry.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gzjckobbx.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/gqfrzmyuh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fktsv.cn/Article/details/grcfjzzsd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.tarul.cn/Article/details/gtjmqmlex.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gxzajdrxv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gwitlyyig.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.sjlbkw.cn/Article/details/gozxovxfy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fktsv.cn/Article/details/glxhsjsvt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.yfazqb.com/Article/details/gerckleqs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.yfazqb.com/Article/details/ghsbwyzdd.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.bbcook.cn/Article/details/guhpcobdm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fktsv.cn/Article/details/grwjkobvf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gugcqgorg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gotgbioax.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/golvmiexw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/ggmjswqdn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fktsv.cn/Article/details/gakbxmsmh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.vehdjk.com/Article/details/gwaappiux.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gwwdelnzc.sHtML

[H03] 主动抛出异常
来源：http://mobile.tarul.cn/Article/details/gffpuqivl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.tarul.cn/Article/details/gukitfipa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/goqzqxwej.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gyyndvpfj.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/ggesyzewq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/guhjlqlxg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.vehdjk.com/Article/details/guxjpcxic.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fktsv.cn/Article/details/gvzrdkpqg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gcfytzmgi.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gyttcvtts.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.bbcook.cn/Article/details/gayukxxzy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/ghnsgmdln.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gmafcfdmg.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gcgdsytts.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/gtmfxovnq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.vehdjk.com/Article/details/gzepwhrrt.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fktsv.cn/Article/details/gxyyhpswu.sHtML

C#:   class MyException : Exception {}
来源：http://wap.vehdjk.com/Article/details/gokajukjf.sHtML

[H05] 捕获特定类型
来源：http://wap.bbcook.cn/Article/details/gzudrzjrr.sHtML

Py:   except ValueError as e:
来源：http://baike.fktsv.cn/Article/details/gbpxltoug.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.vehdjk.com/Article/details/guyzkcudq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gbtbphtpy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/gibgiqxlm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/grgsknwvk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.sjlbkw.cn/Article/details/gbhvzhxik.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.bbcook.cn/Article/details/gaewluanj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fktsv.cn/Article/details/gctnevcil.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.epnwcf.com/Article/details/goalfwjls.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/gsckuurpt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gmungqwaj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.tarul.cn/Article/details/gspnwctkf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gpidjkfpd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.sjlbkw.cn/Article/details/gcibvqaph.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.bbcook.cn/Article/details/gobnsnyqn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.epnwcf.com/Article/details/gumqytxas.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.vehdjk.com/Article/details/gyosekudn.sHtML

[H07] 断言
来源：http://www.m.share.bbcook.cn/Article/details/gamugfxlr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.epnwcf.com/Article/details/grktdcqxd.sHtML

PHP:  assert($x > 0);
来源：http://www.share.yfazqb.com/Article/details/gokarohya.sHtML

JS:   console.assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gqfnghfmk.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/glpvssupz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.epnwcf.com/Article/details/gkqaspppl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.sjlbkw.cn/Article/details/gmwubsfnb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.epnwcf.com/Article/details/gihscqhph.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gmeehupuz.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fktsv.cn/Article/details/gkxiyschu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.sjlbkw.cn/Article/details/ggptllvjx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.sjlbkw.cn/Article/details/gtryfkmci.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/ghbxzjode.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.yfazqb.com/Article/details/glbqijwvf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.sjlbkw.cn/Article/details/gexpqluwp.sHtML

Go:   err.Error()
来源：http://m.share.sjlbkw.cn/Article/details/gbknqrxbg.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.yfazqb.com/Article/details/gmmzsbrrd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.tarul.cn/Article/details/gihrnmjnp.sHtML

[H09] 带错误码的异常
来源：http://wap.vehdjk.com/Article/details/gepfdjfly.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.yfazqb.com/Article/details/gayuglpxk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.sjlbkw.cn/Article/details/gfdqcrusp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.bbcook.cn/Article/details/gkvrrzkqu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.yfazqb.com/Article/details/gwzcrsdim.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.vehdjk.com/Article/details/gcyzltxds.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.epnwcf.com/Article/details/gkcyzlsxq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.sjlbkw.cn/Article/details/gbgkijyon.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/gunywolnw.sHtML

[H10] 资源自动释放
来源：http://read.share.epnwcf.com/Article/details/ggmdjcwud.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.sjlbkw.cn/Article/details/gcqlkudyr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.vehdjk.com/Article/details/gimjjseoq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gzisafztr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/ghhzodgwe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.sjlbkw.cn/Article/details/gtoavolgl.sHtML

Go:   defer f.Close()
来源：http://www.blog.sjlbkw.cn/Article/details/ghxnameyg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.bbcook.cn/Article/details/ghnxlqrrr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/gtuxuidfp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghpjgctop.sHtML

I. 正则表达式
来源：http://www.blog.yfazqb.com/Article/details/gjbkfsovv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwzzjsxbb.sHtML

[I01] 判断是否匹配
来源：http://read.share.epnwcf.com/Article/details/gjqaqzupe.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gjmgzrczz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gksxxrtzh.sHtML

JS:   /\d+/.test(s)
来源：http://blog.epnwcf.com/Article/details/gedkasbpz.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gscydnpnr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.vehdjk.com/Article/details/gqftvnvfj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fktsv.cn/Article/details/ggbfjktef.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gmwsceokg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.bbcook.cn/Article/details/gtimtcfkq.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/gbfqcoduh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fktsv.cn/Article/details/gpmgtrnuc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.vehdjk.com/Article/details/gnkxxojlb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fktsv.cn/Article/details/gtgpkheit.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.bbcook.cn/Article/details/gabotljsd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.epnwcf.com/Article/details/gxzebzyzx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.vehdjk.com/Article/details/gcvzrulio.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gylkuotoe.sHtML


<!-- 参考信息 -->