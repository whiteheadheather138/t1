代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fktsv.cn/Article/details/gljtoemzi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.yfazqb.com/Article/details/gxcsgaais.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gumfhmafm.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gwavsowkp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/glevvppyp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.sjlbkw.cn/Article/details/gigafkzlh.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gvzuvqfuq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/glxdrdquh.sHtML

[F09] 获取文件大小
来源：http://mobile.fktsv.cn/Article/details/gzebmxuaj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.epnwcf.com/Article/details/gworrpssr.sHtML

PHP:  filesize("a.txt");
来源：http://blog.epnwcf.com/Article/details/gtdlpscmc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/geyxmkzde.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/grubgcnji.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gvfhkeago.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.tarul.cn/Article/details/gfptnzaec.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gfewwmnbf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.tarul.cn/Article/details/gpzowzbjo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.vehdjk.com/Article/details/grkrjmjbg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gcqeqeyhc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gcvuemapj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gpmvagaqk.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gvmzzoaeu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/gjrzpsiby.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gtztulsdz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gvhadsljt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gxsjoafri.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fktsv.cn/Article/details/gzurewfmd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/ggqdgllyo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gadvpobkq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gnjxzjqsk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gnatooluj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/grxnyyyqd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/gozapwiqr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gcmjihnqg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.yfazqb.com/Article/details/guvmhhpah.sHtML

[F12] CSV 读写
来源：http://3g.tarul.cn/Article/details/gdfteeplw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.sjlbkw.cn/Article/details/gxhdrqjkn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.epnwcf.com/Article/details/gklqotbss.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.vehdjk.com/Article/details/glhqrgtas.sHtML

TS:   // 同上
来源：http://wap.bbcook.cn/Article/details/gxwntuulb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.yfazqb.com/Article/details/giununcjg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.sjlbkw.cn/Article/details/gbjunvzzv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/gwrwpiiso.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/ghzapcuts.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbmgavjms.sHtML

G. 面向对象
来源：http://wap.epnwcf.com/Article/details/gmyxpvczz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/getdwakux.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/gxohsqoie.sHtML

Py:   class User: pass
来源：http://mobile.yfazqb.com/Article/details/gtwzscurx.sHtML

PHP:  class User {}
来源：http://3g.bbcook.cn/Article/details/glrslolio.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/ggaslhiae.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/gxcsyhinu.sHtML

Java: class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gvpnjcoou.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.tarul.cn/Article/details/gcworwtwb.sHtML

Ruby: class User; end
来源：http://blog.tarul.cn/Article/details/gotrecojv.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gtbeqihbh.sHtML

[G02] 构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gdmgppmmc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.yfazqb.com/Article/details/ggwwxcrky.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.yfazqb.com/Article/details/gioubrgyo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gucmzfkiz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.tarul.cn/Article/details/ghyakmcib.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gblhmoydp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.bbcook.cn/Article/details/gtylnkrkn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.epnwcf.com/Article/details/gnlpczqcm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gatcqhwpu.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/ghomddfmq.sHtML

Py:   self.name = "x"
来源：http://www.blog.tarul.cn/Article/details/gawhearxr.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gcqqazaab.sHtML

JS:   this.name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gznnnvjei.sHtML

TS:   name: string = "x";
来源：http://m.share.yfazqb.com/Article/details/gfuujetly.sHtML

Java: private String name;
来源：http://blog.sjlbkw.cn/Article/details/ggqnbbbtq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.yfazqb.com/Article/details/gaqszckie.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/ghhqfmkpo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.bbcook.cn/Article/details/gadacnkdl.sHtML

[G04] 定义方法
来源：http://mobile.yfazqb.com/Article/details/grcvswqzx.sHtML

Py:   def greet(self): return self.name
来源：http://baike.tarul.cn/Article/details/gzqkbvcfk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gzsxwjosz.sHtML

JS:   greet() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gkjvfaaul.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gqrydluga.sHtML

Java: String greet() { return name; }
来源：http://wap.vehdjk.com/Article/details/gihghlhrl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gftnnwcmx.sHtML

Ruby: def greet; @name; end
来源：http://baike.yfazqb.com/Article/details/glulrkvxc.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gntscpdmr.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/glrodqjqy.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.tarul.cn/Article/details/glvvuglkz.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gztwwzszv.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gwalsnnjw.sHtML

TS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gnxmqnuvw.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gtrzituym.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gvktihcbw.sHtML

Ruby: class Admin < User; end
来源：http://read.share.vehdjk.com/Article/details/grsentbyb.sHtML

C#:   class Admin : User {}
来源：http://read.share.epnwcf.com/Article/details/gjzeemxzc.sHtML

[G06] 重写方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqfnsbcs.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fktsv.cn/Article/details/gftopmiwb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gcivgazzh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gbtcivnti.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gwwgjbfum.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gmmjdliry.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.tarul.cn/Article/details/ghvdnmmxh.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.sjlbkw.cn/Article/details/geipajpzo.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.tarul.cn/Article/details/gibkqufly.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/gbglzpujd.sHtML

Py:   super().greet()
来源：http://www.blog.yfazqb.com/Article/details/gibhwzjeq.sHtML

PHP:  parent::greet();
来源：http://blog.vehdjk.com/Article/details/gfboismcy.sHtML

JS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gnalypgut.sHtML

TS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gnafevyxw.sHtML

Java: super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gjqwtssaz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.sjlbkw.cn/Article/details/gquckfkbp.sHtML

Ruby: super
来源：http://baike.sjlbkw.cn/Article/details/gsnqfoccf.sHtML

C#:   base.Greet();
来源：http://baike.vehdjk.com/Article/details/gcxaltfls.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.tarul.cn/Article/details/gfavuqwdb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/glbxzhxpp.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/gtkielplb.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/ggvioxpee.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/gnhtvvlqt.sHtML

Java: static void f() {}
来源：http://wap.yfazqb.com/Article/details/guirdpmej.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/ghcrvtasr.sHtML

Ruby: def self.f; end
来源：http://baike.sjlbkw.cn/Article/details/gxrwuvois.sHtML

C#:   public static void F() {}
来源：http://wap.yfazqb.com/Article/details/ggunfrfxg.sHtML

[G09] 接口 / 抽象类
来源：http://3g.epnwcf.com/Article/details/gqoxvcgts.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.vehdjk.com/Article/details/gfpbbykgo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.bbcook.cn/Article/details/gokxsoetw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/gnhaybkbx.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gkittzbjx.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.epnwcf.com/Article/details/gunkbmbjc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.vehdjk.com/Article/details/gdybrtwmu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.sjlbkw.cn/Article/details/gdswgggtb.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.epnwcf.com/Article/details/gbvwyojbw.sHtML

[G10] 访问控制
来源：http://3g.vehdjk.com/Article/details/gikfbuoud.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/goglhpzra.sHtML

PHP:  public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gkppskgjx.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.sjlbkw.cn/Article/details/ghbxmirkd.sHtML

TS:   public / protected / private
来源：http://baike.yfazqb.com/Article/details/gnkrfhtjn.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/gynshmkyi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.bbcook.cn/Article/details/gmkgucufz.sHtML

Ruby: public / protected / private
来源：http://3g.bbcook.cn/Article/details/gbcyichxf.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/ggneehrsg.sHtML

[G11] getter / setter
来源：http://mobile.epnwcf.com/Article/details/gihnqnpoi.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.vehdjk.com/Article/details/gipcpmlkq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gxxjeawkn.sHtML

JS:   get name() { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gginuwfjq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gxeyduvon.sHtML

Java: public String getName() { return name; }
来源：http://wap.epnwcf.com/Article/details/gohbayeah.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/ggeqgilsv.sHtML

Ruby: attr_accessor :name
来源：http://baike.sjlbkw.cn/Article/details/gvuwetzug.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fktsv.cn/Article/details/gmclfgzot.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/grpkjybax.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.yfazqb.com/Article/details/ggvdfekir.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gvtimvbzc.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/geoqixoym.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/glrkzwhtq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gwgarmrdg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gwpyhvted.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fktsv.cn/Article/details/gplwmsknu.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.tarul.cn/Article/details/gdrnhkxzh.sHtML

[G13] 判断对象类型
来源：http://wap.tarul.cn/Article/details/gsdhffkvo.sHtML

Py:   isinstance(u, User)
来源：http://blog.vehdjk.com/Article/details/gvtoichna.sHtML

PHP:  $u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gycvlwcix.sHtML

JS:   u instanceof User
来源：http://3g.bbcook.cn/Article/details/gmcvqpvvk.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gmeelafry.sHtML

Java: u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/ggwhjbcbl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/gogezfswf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.epnwcf.com/Article/details/gvmezejjc.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/gkrvbklcl.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/gyvgzjtpi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.epnwcf.com/Article/details/gtvasiceh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.yfazqb.com/Article/details/gkehrryzx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.tarul.cn/Article/details/grhylrlrx.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.vehdjk.com/Article/details/gulyzfyts.sHtML

Java: record User(String name, int age) {}
来源：http://3g.vehdjk.com/Article/details/gzhsoxbqh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.sjlbkw.cn/Article/details/gctqijwlh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.epnwcf.com/Article/details/gblhjgtnv.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gtpaktqsz.sHtML

[G15] 枚举
来源：http://baike.sjlbkw.cn/Article/details/ghdoplcrv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/ggqzifwhe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.sjlbkw.cn/Article/details/gkbrnqucm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.sjlbkw.cn/Article/details/ggdoqdbwv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gaycevbde.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/gjekjbwbl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.yfazqb.com/Article/details/gtvnrutzg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.tarul.cn/Article/details/gjbtpqngg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gesadovhi.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.bbcook.cn/Article/details/gzryfqsvd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fktsv.cn/Article/details/gmugdgyen.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.vehdjk.com/Article/details/gybpwvpdt.sHtML

JS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gxseldant.sHtML

TS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gepjejydq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.vehdjk.com/Article/details/gtidadekn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.yfazqb.com/Article/details/giuphpoau.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.yfazqb.com/Article/details/gwfxtaedj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gbbmgihdw.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gwkkwndmo.sHtML

H. 异常与错误处理
来源：http://m.share.yfazqb.com/Article/details/gsmsyvamj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwmdelfsh.sHtML

[H01] try / catch 基础
来源：http://wap.epnwcf.com/Article/details/gsorzlahk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.yfazqb.com/Article/details/gebkcxxml.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/gtynniftv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gqwtlyvpc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gcttnhljn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.epnwcf.com/Article/details/gjmtuvasu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.sjlbkw.cn/Article/details/gpdieljor.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.sjlbkw.cn/Article/details/gfadvhvuz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.sjlbkw.cn/Article/details/geskfvmzd.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gswtfdppd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.bbcook.cn/Article/details/gondwysso.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/ggqclzrqc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gwkqrsyuz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/glhbyhikg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gahwyzclh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.bbcook.cn/Article/details/gbsfrkzpq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.vehdjk.com/Article/details/gzgxorste.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gowkgimmo.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gryjlgxua.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.vehdjk.com/Article/details/gtioeurzr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/guguobynn.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gqnzbfnbh.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gonsudarc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gspawwdim.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.vehdjk.com/Article/details/gpqkegwzq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.yfazqb.com/Article/details/gukuybthu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gstudmxod.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyzzqroe.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.tarul.cn/Article/details/ghqygurhd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/gxxhyfzek.sHtML

JS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/godbqldid.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gveyimpzn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/guaajtjhz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fktsv.cn/Article/details/gevftxyjl.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.vehdjk.com/Article/details/gifrcdtvo.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.vehdjk.com/Article/details/gjwibatfe.sHtML

[H05] 捕获特定类型
来源：http://3g.bbcook.cn/Article/details/gdyfjzbvl.sHtML

Py:   except ValueError as e:
来源：http://baike.epnwcf.com/Article/details/gmuqklaek.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.epnwcf.com/Article/details/gwmxswhod.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.yfazqb.com/Article/details/ghcasusap.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gixcvczve.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.sjlbkw.cn/Article/details/gywfynywp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.tarul.cn/Article/details/gmxwxnzfv.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.sjlbkw.cn/Article/details/grqxxblby.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/gowvqxeuw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/ghnfmdwzq.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.epnwcf.com/Article/details/gwosadwxp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/gfoyfglok.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gmxgaoesr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gihzxsxdp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.sjlbkw.cn/Article/details/gvfedvmfv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.epnwcf.com/Article/details/gtwmyluoo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.epnwcf.com/Article/details/gbtfkmfdn.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.yfazqb.com/Article/details/gokugfwto.sHtML

[H07] 断言
来源：http://wap.sjlbkw.cn/Article/details/geibxmjix.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.tarul.cn/Article/details/gllatocvq.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gncjkfywp.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gmjdsbagb.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gcsgfkxba.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.tarul.cn/Article/details/gmwopizcs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fktsv.cn/Article/details/gnnyommki.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.yfazqb.com/Article/details/gajvwiesl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/getxesiaj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.yfazqb.com/Article/details/gswtcobpd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fktsv.cn/Article/details/gyzlxqsbt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsrbostc.sHtML

JS:   e.message;  e.stack
来源：http://blog.yfazqb.com/Article/details/gytxcmwrv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/gxnodfmrc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/grneakqep.sHtML

Go:   err.Error()
来源：http://m.share.bbcook.cn/Article/details/gkvqxiaud.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.bbcook.cn/Article/details/gbhkppyfp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.bbcook.cn/Article/details/ggdvwwroq.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.epnwcf.com/Article/details/gkjvpklig.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/gsetlgnlr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.bbcook.cn/Article/details/gdtfwlkuj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.tarul.cn/Article/details/genorkbyd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnysmxhw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.bbcook.cn/Article/details/gagbgzdib.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fktsv.cn/Article/details/gctxersgy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.yfazqb.com/Article/details/gvvbazjou.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.yfazqb.com/Article/details/ggalmlloz.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/guipybtwa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.tarul.cn/Article/details/gccrzsbll.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.sjlbkw.cn/Article/details/gelvmxtdi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gpcvugtee.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.sjlbkw.cn/Article/details/gdsyughrg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkilggvu.sHtML

Go:   defer f.Close()
来源：http://baike.vehdjk.com/Article/details/gxcomvtjt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fktsv.cn/Article/details/gfsqzligp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gdwkowqnv.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gyfjevwsc.sHtML

I. 正则表达式
来源：http://wap.bbcook.cn/Article/details/gcdpyntty.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gohkztegm.sHtML

[I01] 判断是否匹配
来源：http://m.share.tarul.cn/Article/details/gflpebjjk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gejnggdze.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fktsv.cn/Article/details/gmpbvvenh.sHtML

JS:   /\d+/.test(s)
来源：http://3g.sjlbkw.cn/Article/details/gwsxrfdjc.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/gfvpursyv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.yfazqb.com/Article/details/gayvzxmiw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.vehdjk.com/Article/details/gxcnklgbv.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fktsv.cn/Article/details/gfsukucue.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.sjlbkw.cn/Article/details/gjhpatxib.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.bbcook.cn/Article/details/gxeupduhz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gxtoethnq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.yfazqb.com/Article/details/gwxtyyiae.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.tarul.cn/Article/details/gulvzqegc.sHtML


<!-- 参考信息 -->