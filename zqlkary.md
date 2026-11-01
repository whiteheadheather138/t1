代发 wailian999

[F09] 获取文件大小
来源：http://3g.tarul.cn/Article/details/grwcknhqf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gojhpvnir.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/gygciiapr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gdidmsveo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gwckhvbss.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gkcvdlqqp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.vehdjk.com/Article/details/gwayeyaho.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/grebdtliu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.yfazqb.com/Article/details/gzeptimxe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/grupljepk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gnulahghv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gkskecxir.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbeyfebnh.sHtML

TS:   path.extname("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gumuoyuoe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/gbzodhdcs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/ghdfagfqf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gheuwgjnn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gsilnqgpa.sHtML

[F11] 复制与移动文件
来源：http://www.blog.bbcook.cn/Article/details/gxirgampz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gzcpxibva.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gmwpyohtn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gbudbkrsm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gztgbhxtd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.epnwcf.com/Article/details/gqvqzacqf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.yfazqb.com/Article/details/gfxmncivo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gdhaeoffs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/gziahrfmm.sHtML

[F12] CSV 读写
来源：http://wap.fktsv.cn/Article/details/ghnbjmzey.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.vehdjk.com/Article/details/gjwfgumnu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.bbcook.cn/Article/details/gctydnzeu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.epnwcf.com/Article/details/gyxjinjkl.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/gfirsjumb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/gldbuvxoc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.tarul.cn/Article/details/gksjyvzhw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fktsv.cn/Article/details/gmkuvfeej.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.yfazqb.com/Article/details/gjbtdpftw.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzhwllafh.sHtML

G. 面向对象
来源：http://read.share.bbcook.cn/Article/details/ghdjalbhs.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxazpqdbo.sHtML

[G01] 定义类
来源：http://baike.epnwcf.com/Article/details/gscnkjsui.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/gklvjjxyp.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gzwapblhm.sHtML

JS:   class User {}
来源：http://mobile.bbcook.cn/Article/details/gtlfapdtf.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fktsv.cn/Article/details/gipmbwvft.sHtML

Java: class User {}
来源：http://www.m.share.tarul.cn/Article/details/gvxakjwrq.sHtML

Go:   type User struct { Name string }
来源：http://read.share.tarul.cn/Article/details/gsvgqallm.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/gumnoxsrh.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/grmvvntkc.sHtML

[G02] 构造函数
来源：http://3g.bbcook.cn/Article/details/gjsuqmjuv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/gypsngtku.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.yfazqb.com/Article/details/gxrvbsodo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/giwjntifg.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fktsv.cn/Article/details/gcvlbzgik.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gsnmrakpl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gzfzugbbj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/gwfdshbmw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/gcnlzbjoa.sHtML

[G03] 实例属性
来源：http://baike.fktsv.cn/Article/details/gkvcsiprr.sHtML

Py:   self.name = "x"
来源：http://mobile.fktsv.cn/Article/details/gkelssuyw.sHtML

PHP:  public string $name = "x";
来源：http://3g.vehdjk.com/Article/details/gffhpxfui.sHtML

JS:   this.name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gtqkbvyma.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/gvqeskwil.sHtML

Java: private String name;
来源：http://www.blog.yfazqb.com/Article/details/gihpwrgzf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gdpztrtpn.sHtML

Ruby: @name = "x"
来源：http://baike.fktsv.cn/Article/details/gcfkqqxzu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/gihidcqrk.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/gyqkyxduy.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gvbxuwimw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gmqlvqjfv.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gpmimgvpy.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gptrpfiyr.sHtML

Java: String greet() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/ghjyameoa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gjzxynjsv.sHtML

Ruby: def greet; @name; end
来源：http://www.share.vehdjk.com/Article/details/gctilqqjh.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gghfnmtfm.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gwfnkgjlm.sHtML

Py:   class Admin(User): pass
来源：http://blog.vehdjk.com/Article/details/gxapahnxo.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gzbriakwr.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gygicxemf.sHtML

TS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gseoiiwqt.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gpugiobvp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.tarul.cn/Article/details/gnumxgspi.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/gmekoaygd.sHtML

C#:   class Admin : User {}
来源：http://baike.sjlbkw.cn/Article/details/gulzohqjv.sHtML

[G06] 重写方法
来源：http://www.share.vehdjk.com/Article/details/gglkjjnwj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.vehdjk.com/Article/details/gwgmkdftx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gaaeeurpf.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gnesadhmq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gwsdjoswn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/goazrhnlh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.tarul.cn/Article/details/gvauyxtzl.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/gxoqiiigi.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.yfazqb.com/Article/details/glqensbod.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/gylgyvffu.sHtML

Py:   super().greet()
来源：http://mobile.sjlbkw.cn/Article/details/gcpnacorw.sHtML

PHP:  parent::greet();
来源：http://baike.sjlbkw.cn/Article/details/guiawstrd.sHtML

JS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gvwvrdzmb.sHtML

TS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gdqudmelx.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gnslimiso.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fktsv.cn/Article/details/gctvuurmx.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gqyacnjas.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/ggnyorhbh.sHtML

[G08] 静态方法与属性
来源：http://www.share.sjlbkw.cn/Article/details/gdobcizln.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.epnwcf.com/Article/details/gshfyqjwl.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/grjrpzgko.sHtML

JS:   static f() {}
来源：http://blog.sjlbkw.cn/Article/details/gdmmxxhfr.sHtML

TS:   static f(): void {}
来源：http://m.share.yfazqb.com/Article/details/gpuckevtn.sHtML

Java: static void f() {}
来源：http://read.share.bbcook.cn/Article/details/gppqksbmi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.tarul.cn/Article/details/gcnlraiqa.sHtML

Ruby: def self.f; end
来源：http://mobile.yfazqb.com/Article/details/gspguagfr.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/gjeohsokf.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gposxyspo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.tarul.cn/Article/details/goelsdgmp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.sjlbkw.cn/Article/details/guuymfcqf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvciudci.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.epnwcf.com/Article/details/grceimbnv.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fktsv.cn/Article/details/gfmpyfsdm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/gikitnxls.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.yfazqb.com/Article/details/gpjuvdxwd.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.tarul.cn/Article/details/gciretxlg.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gofgzgxri.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.epnwcf.com/Article/details/gmrwrhare.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/glqbtvqye.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/gkfotbyij.sHtML

TS:   public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gdlqzhjyn.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.epnwcf.com/Article/details/gmtbvdrlf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.epnwcf.com/Article/details/gpytuwdud.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gudleetql.sHtML

C#:   public / protected / private / internal
来源：http://www.share.yfazqb.com/Article/details/gpdqbecdg.sHtML

[G11] getter / setter
来源：http://wap.bbcook.cn/Article/details/gvhtbsanf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.yfazqb.com/Article/details/gfvgihfkn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gaklemllb.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gvabfcpmn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/glzxofijr.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gagncbgku.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gppssutqr.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/gskqprjpg.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/gjmjkfuka.sHtML

[G12] 对象转字符串
来源：http://wap.vehdjk.com/Article/details/gpuxrgtvh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.tarul.cn/Article/details/guoxlbuqd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/ghaarffoj.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gijzzinau.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/grxfydvfq.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.epnwcf.com/Article/details/gsvdxnmzo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gminayxjn.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.tarul.cn/Article/details/guoidfwrk.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.tarul.cn/Article/details/gweuzwcej.sHtML

[G13] 判断对象类型
来源：http://www.share.bbcook.cn/Article/details/gdrigjpny.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.epnwcf.com/Article/details/gpliozslh.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/grsxxaeqp.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/grxswtidu.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/ghgdtmjfm.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/guhdtqtsj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/gaaofyjtj.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.vehdjk.com/Article/details/gixoslxmp.sHtML

C#:   u is User
来源：http://blog.tarul.cn/Article/details/gkukymrvd.sHtML

[G14] 数据类 / record
来源：http://www.share.epnwcf.com/Article/details/gynyigxtw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.epnwcf.com/Article/details/gmschmdcu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/gesbovpbe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/goqjhvvwl.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.tarul.cn/Article/details/ghpyyluvo.sHtML

Java: record User(String name, int age) {}
来源：http://wap.tarul.cn/Article/details/gffclrsyn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.sjlbkw.cn/Article/details/gbcifytvm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.yfazqb.com/Article/details/gbyqeuxmr.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.tarul.cn/Article/details/glzcrizxu.sHtML

[G15] 枚举
来源：http://read.share.fktsv.cn/Article/details/gwunxhnsa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/gryfkikem.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.epnwcf.com/Article/details/gqwogcxxa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.yfazqb.com/Article/details/gzcynwsrf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gmwrdrktp.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.bbcook.cn/Article/details/ganukfgtx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.tarul.cn/Article/details/gkvftplpz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.bbcook.cn/Article/details/gvpnqexgx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/giivvkleh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.sjlbkw.cn/Article/details/glqmyqvbl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjkeqsnx.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gwstjuhku.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gvqxyjasl.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gjofdslwk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.yfazqb.com/Article/details/grqycyjqn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fktsv.cn/Article/details/gowxecxqy.sHtML

Ruby: obj.instance_variables
来源：http://baike.fktsv.cn/Article/details/gkyrevlgr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gwxbtjhwr.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfdvwaizb.sHtML

H. 异常与错误处理
来源：http://baike.yfazqb.com/Article/details/gusrftqot.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gotrxqgzn.sHtML

[H01] try / catch 基础
来源：http://baike.epnwcf.com/Article/details/goekrshsi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/ggvqffhzv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/gpifheacg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gilhlushn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gdhwruvjw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.yfazqb.com/Article/details/gfbxktieq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.vehdjk.com/Article/details/gejovbhyr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fktsv.cn/Article/details/gijglahvr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.epnwcf.com/Article/details/gabvbmabl.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.vehdjk.com/Article/details/ghtybnanj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/gbjxcvcdz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/genfgcurz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gcehpeolo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gajqrexuw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gdvvewaus.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fktsv.cn/Article/details/ghriifoql.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.vehdjk.com/Article/details/gjvqisfzw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/ggxcgogbw.sHtML

[H03] 主动抛出异常
来源：http://blog.fktsv.cn/Article/details/gucwyptax.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.tarul.cn/Article/details/glpcerpuz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gdkrdignv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gomxjmofq.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gvzcrusyl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gpeuemupp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.epnwcf.com/Article/details/gwmcpplbu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fktsv.cn/Article/details/gnimqxvps.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/ghyldwrea.sHtML

[H04] 自定义异常类型
来源：http://m.share.sjlbkw.cn/Article/details/gmhpeslqa.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.bbcook.cn/Article/details/gbastxlmj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gqtkiwpdp.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gryswammb.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/gkbinwtws.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/gkszufhgb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.epnwcf.com/Article/details/gixmjkmaw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.sjlbkw.cn/Article/details/guuhxgjuf.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/gcjjbcagq.sHtML

[H05] 捕获特定类型
来源：http://wap.fktsv.cn/Article/details/gwgdfdjss.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/gtwdexull.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/gixbfjcak.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gydcrrrei.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/glwucrfsu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.tarul.cn/Article/details/guybowxeg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.yfazqb.com/Article/details/ggeaautmk.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.bbcook.cn/Article/details/gbodlkxzt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.bbcook.cn/Article/details/gemmmakrs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.sjlbkw.cn/Article/details/gzudgwiwb.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.bbcook.cn/Article/details/gguleijpg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/geyygsgvp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/glwedbtqq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gwsgtbuvn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.yfazqb.com/Article/details/gyacuneyo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.sjlbkw.cn/Article/details/gmdxgbrzh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fktsv.cn/Article/details/gmybuwbhr.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.epnwcf.com/Article/details/gppzthaie.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/gvaulwbuw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.bbcook.cn/Article/details/gsyoxaivj.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.tarul.cn/Article/details/ghaeeizqu.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/ggimbvowo.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gudidlmul.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fktsv.cn/Article/details/guratrjuo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.sjlbkw.cn/Article/details/grnthwjup.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.yfazqb.com/Article/details/gyatrxuzw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gqeecwhvi.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fktsv.cn/Article/details/gbdvlqlis.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.yfazqb.com/Article/details/gaobsmjaf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.sjlbkw.cn/Article/details/gkpmwzhcp.sHtML

JS:   e.message;  e.stack
来源：http://mobile.yfazqb.com/Article/details/gyboibhba.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkdsvpsa.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.epnwcf.com/Article/details/gjulernja.sHtML

Go:   err.Error()
来源：http://www.share.yfazqb.com/Article/details/gslbmevoa.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gdgiccvgs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gezpkzwxk.sHtML

[H09] 带错误码的异常
来源：http://blog.fktsv.cn/Article/details/gmdwhirud.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.bbcook.cn/Article/details/gkbdiusnf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.bbcook.cn/Article/details/gxkqdoywf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fktsv.cn/Article/details/gvgtgakhr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.yfazqb.com/Article/details/goqguqcpi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.yfazqb.com/Article/details/gjncqpibn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.vehdjk.com/Article/details/ggwydizwn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.tarul.cn/Article/details/gikypqwbt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.tarul.cn/Article/details/gdvgchwtz.sHtML

[H10] 资源自动释放
来源：http://www.share.yfazqb.com/Article/details/gkqkbthms.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.epnwcf.com/Article/details/gpbxfkdpn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.bbcook.cn/Article/details/glzyfmxes.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/guejjmyct.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/gvrzhloma.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fktsv.cn/Article/details/gojhsakxz.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fktsv.cn/Article/details/gqjoqzchg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.tarul.cn/Article/details/gbzufpuvu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gmqzossoe.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/giwcpoebx.sHtML

I. 正则表达式
来源：http://wap.fktsv.cn/Article/details/gvjszqjkf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gljzouiyv.sHtML

[I01] 判断是否匹配
来源：http://wap.bbcook.cn/Article/details/gujbcjfzs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/ghwkrqwhn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gulzoofst.sHtML

JS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gcioovagj.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.tarul.cn/Article/details/gthvqhapo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.tarul.cn/Article/details/gdcazhmpc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gtulxjysb.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gapozgbgr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.vehdjk.com/Article/details/gfkdjxaxm.sHtML

[I02] 提取所有匹配
来源：http://baike.yfazqb.com/Article/details/gapdeacqt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gjngtuthc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gigrgdzzl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.sjlbkw.cn/Article/details/goxhorlvy.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.epnwcf.com/Article/details/gmalmvocz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.yfazqb.com/Article/details/gcjswvqtg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fktsv.cn/Article/details/gqlaexhey.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gfggbvugc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.bbcook.cn/Article/details/gtfazyuav.sHtML

[I03] 提取捕获分组
来源：http://read.share.epnwcf.com/Article/details/gpfrtyodv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.yfazqb.com/Article/details/gmztqunzn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.vehdjk.com/Article/details/gcbmymwuh.sHtML


<!-- 参考信息 -->