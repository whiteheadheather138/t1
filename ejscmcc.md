代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gyezbztrc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gaesuslef.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gzwitvkqz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.epnwcf.com/Article/details/gsokhgjpu.sHtML

[F09] 获取文件大小
来源：http://read.share.tarul.cn/Article/details/gjcpwwsrz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fktsv.cn/Article/details/gwtjakfro.sHtML

PHP:  filesize("a.txt");
来源：http://blog.epnwcf.com/Article/details/giqgrkykw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/gtjtbgenv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gfzhhtjkt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gpxihmnpe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.bbcook.cn/Article/details/gwxbzmqiu.sHtML

Ruby: File.size("a.txt")
来源：http://3g.epnwcf.com/Article/details/gswgtjifz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fktsv.cn/Article/details/gfnxwuvdz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fktsv.cn/Article/details/gxynkzdeh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gljshtloa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.vehdjk.com/Article/details/gtbqqkbza.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gmrjpwggp.sHtML

TS:   path.extname("a.txt")
来源：http://blog.epnwcf.com/Article/details/gbmyesuwv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.epnwcf.com/Article/details/gtjqipyur.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gnjpgesvu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/guhmxcnkj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gfbzrcann.sHtML

[F11] 复制与移动文件
来源：http://read.share.yfazqb.com/Article/details/gtvsrdgyg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gakzvfmor.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.yfazqb.com/Article/details/gxujitrtx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gkxnatouu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gkqikwydt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.vehdjk.com/Article/details/gpjlvbswj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.yfazqb.com/Article/details/gbsdoujjb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gfjqwehom.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gdztordxw.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gnadwfodi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/gdmaykhbo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.epnwcf.com/Article/details/gxwudvwmj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.sjlbkw.cn/Article/details/gerkzrnrn.sHtML

TS:   // 同上
来源：http://read.share.sjlbkw.cn/Article/details/ggsfzkjbc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.tarul.cn/Article/details/gmkyefbty.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.yfazqb.com/Article/details/gzpnrhsoq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.tarul.cn/Article/details/grbsfirqw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.vehdjk.com/Article/details/gzjxyouik.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtjhlirey.sHtML

G. 面向对象
来源：http://read.share.tarul.cn/Article/details/geciepmll.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gigzqficn.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/gyxrviiwj.sHtML

Py:   class User: pass
来源：http://read.share.vehdjk.com/Article/details/gtnmixvrk.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/gkeujydkh.sHtML

JS:   class User {}
来源：http://mobile.tarul.cn/Article/details/gvetqkcju.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/gkkwunpoj.sHtML

Java: class User {}
来源：http://3g.fktsv.cn/Article/details/gcdubdryz.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.bbcook.cn/Article/details/gqxqnvouh.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gebjfwqhq.sHtML

C#:   class User {}
来源：http://www.share.tarul.cn/Article/details/gcrpqxcvd.sHtML

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/goufajrcr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fktsv.cn/Article/details/gczfndlxg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fktsv.cn/Article/details/guirqwcuj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gdkkbqnym.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.yfazqb.com/Article/details/gtrfcfkoh.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gouljxtuv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.tarul.cn/Article/details/gvqgnlfki.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gsdrbcuhs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.tarul.cn/Article/details/giqeazsym.sHtML

[G03] 实例属性
来源：http://m.share.sjlbkw.cn/Article/details/guppousql.sHtML

Py:   self.name = "x"
来源：http://m.share.tarul.cn/Article/details/gstorwtxc.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/gjoafiwhs.sHtML

JS:   this.name = "x";
来源：http://m.share.fktsv.cn/Article/details/gnqalmzuf.sHtML

TS:   name: string = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gauphkinl.sHtML

Java: private String name;
来源：http://www.m.share.tarul.cn/Article/details/ghwfgfwph.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.sjlbkw.cn/Article/details/gixtvpdrs.sHtML

Ruby: @name = "x"
来源：http://m.share.epnwcf.com/Article/details/grhmdotre.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.vehdjk.com/Article/details/gohspkjxl.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/gqhixlpsn.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gncqvktwy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gkwsfizjm.sHtML

JS:   greet() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gvygykver.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gncbhrzco.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/ghvejobav.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/grhfuyewd.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/gfffzhatr.sHtML

C#:   public string Greet() => Name;
来源：http://baike.tarul.cn/Article/details/gvghadnwk.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gazpkrqza.sHtML

Py:   class Admin(User): pass
来源：http://m.share.sjlbkw.cn/Article/details/gasuebuso.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gafzubxum.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gxavulhvy.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gqarcihrq.sHtML

Java: class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gpftbsher.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.epnwcf.com/Article/details/gbtwfpkzi.sHtML

Ruby: class Admin < User; end
来源：http://read.share.bbcook.cn/Article/details/gutjmrrfv.sHtML

C#:   class Admin : User {}
来源：http://mobile.bbcook.cn/Article/details/gjxeuhmdq.sHtML

[G06] 重写方法
来源：http://www.blog.bbcook.cn/Article/details/gvzonkurr.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.epnwcf.com/Article/details/gmvhooymd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/guoickcty.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gjpundzmc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gyiqtltyk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/geqzavycl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.sjlbkw.cn/Article/details/gdixyhjdz.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.yfazqb.com/Article/details/giwcgqpfa.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gkymeqkzx.sHtML

[G07] 调用父类方法
来源：http://3g.vehdjk.com/Article/details/ggufnfynv.sHtML

Py:   super().greet()
来源：http://baike.fktsv.cn/Article/details/gkyvdsekf.sHtML

PHP:  parent::greet();
来源：http://www.m.share.yfazqb.com/Article/details/ghnpzskcg.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gvgtdehtt.sHtML

TS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/glknjthqe.sHtML

Java: super.greet();
来源：http://wap.sjlbkw.cn/Article/details/ghhnbtsve.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/geumutnpe.sHtML

Ruby: super
来源：http://read.share.bbcook.cn/Article/details/grxkoeqkl.sHtML

C#:   base.Greet();
来源：http://baike.sjlbkw.cn/Article/details/gknpvfqju.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fktsv.cn/Article/details/gfrqzzdcc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.bbcook.cn/Article/details/gvyabdxoh.sHtML

PHP:  public static function f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gtvpylnzp.sHtML

JS:   static f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gcvhqrwzn.sHtML

TS:   static f(): void {}
来源：http://3g.fktsv.cn/Article/details/guezhdkbj.sHtML

Java: static void f() {}
来源：http://www.share.tarul.cn/Article/details/grtmcvdmg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.epnwcf.com/Article/details/gvjjedxob.sHtML

Ruby: def self.f; end
来源：http://www.share.fktsv.cn/Article/details/ghcvdlobh.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/gskppvwjg.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.bbcook.cn/Article/details/gaprrcfdx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fktsv.cn/Article/details/gvoluxjfe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.tarul.cn/Article/details/gtfcmqkus.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fktsv.cn/Article/details/grrgahdki.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fktsv.cn/Article/details/gatpcccee.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gjzoircnc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/gdnqscvgc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.bbcook.cn/Article/details/gjrcpuhqp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.vehdjk.com/Article/details/gizathnjz.sHtML

[G10] 访问控制
来源：http://mobile.epnwcf.com/Article/details/gtdgcwtxv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.epnwcf.com/Article/details/ghhupqnat.sHtML

PHP:  public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gredkiadl.sHtML

JS:   #private 字段；其余公开
来源：http://blog.vehdjk.com/Article/details/gsyuwzmgw.sHtML

TS:   public / protected / private
来源：http://3g.vehdjk.com/Article/details/gteadptyq.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.vehdjk.com/Article/details/giovmydgv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fktsv.cn/Article/details/gmtromzil.sHtML

Ruby: public / protected / private
来源：http://baike.bbcook.cn/Article/details/gkfurncuq.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fktsv.cn/Article/details/gnuevqhhf.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/gdjcscpxh.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.tarul.cn/Article/details/ggwlaztrp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/ghgisjwvc.sHtML

JS:   get name() { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gskubxzym.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gyheexxyb.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gdrcyiqfg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gkwhqssun.sHtML

Ruby: attr_accessor :name
来源：http://www.share.sjlbkw.cn/Article/details/getdeflpd.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.epnwcf.com/Article/details/gpazqsdaf.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/gdmihyymf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gnxvfaqag.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gxqjcczig.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gjyzzpnuu.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gysqkujmf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gomdpxaco.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gurmaaeax.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.tarul.cn/Article/details/gkkaryiok.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.tarul.cn/Article/details/gxzjokqtc.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/ghfeyykzh.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/giibfrkxc.sHtML

PHP:  $u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gcyxizcpp.sHtML

JS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gnzmlnzfr.sHtML

TS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gdvuldhja.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gpcutqxqg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.sjlbkw.cn/Article/details/geflkodpz.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/gnqxfghjd.sHtML

C#:   u is User
来源：http://www.share.vehdjk.com/Article/details/giottruql.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/ghgpfygxz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.tarul.cn/Article/details/gbqoujyql.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gtdlsjvgz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.bbcook.cn/Article/details/gmlgudvhq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gwjwbqiyh.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.bbcook.cn/Article/details/gwmflqicp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.vehdjk.com/Article/details/gwlizuobr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.yfazqb.com/Article/details/gvlhoxezi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fktsv.cn/Article/details/gsyhbibhk.sHtML

[G15] 枚举
来源：http://www.share.yfazqb.com/Article/details/gvboyljvp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/glbrqidle.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gjucffjfg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.sjlbkw.cn/Article/details/gganknwqm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gxvjejopx.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.yfazqb.com/Article/details/gylumjjsp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.tarul.cn/Article/details/gpbupensr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gfvsprulp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gpfodqubz.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/gvcyxbqba.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.bbcook.cn/Article/details/gvihpwfbe.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.vehdjk.com/Article/details/gqiwwjjkp.sHtML

JS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gogpwxuew.sHtML

TS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gqjlqlzop.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gvyccjzdr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.sjlbkw.cn/Article/details/ghibomlfg.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.yfazqb.com/Article/details/gemdksckx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gcfbzoebx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbhatmawk.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/gnnyqaqcj.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzdqharnz.sHtML

[H01] try / catch 基础
来源：http://3g.sjlbkw.cn/Article/details/grudfamsb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/gdjbcotrg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/guilbywqk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/gfpiulqeu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gbglmkpsn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.vehdjk.com/Article/details/gkewbmmkk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.epnwcf.com/Article/details/grtskqqzb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/gkciticrt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.bbcook.cn/Article/details/gprvjpjso.sHtML

[H02] finally / ensure 收尾
来源：http://3g.sjlbkw.cn/Article/details/gbakeuepj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.bbcook.cn/Article/details/gzbrshwwr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gzwjjacaa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gnbfkbgmn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/giqvyuahc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/guwpvptxd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.vehdjk.com/Article/details/gtxybtdnl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.sjlbkw.cn/Article/details/gfeavjfor.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gpcqtqwhz.sHtML

[H03] 主动抛出异常
来源：http://m.share.tarul.cn/Article/details/gidrpwwtm.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.bbcook.cn/Article/details/goxtnlecj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gtbkqesti.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gznvstvzi.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gvhvletuj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gvpevunmg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.vehdjk.com/Article/details/gvbhyzfwq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgfvrzmi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gkdpvynuu.sHtML

[H04] 自定义异常类型
来源：http://www.share.fktsv.cn/Article/details/gohjzdxuj.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.tarul.cn/Article/details/gfjewqkrd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/ggcmfctxr.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gsdjpmvyz.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/ggocrodbn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gdwyxqekq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.vehdjk.com/Article/details/gspipbonn.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.vehdjk.com/Article/details/glvipazcj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.vehdjk.com/Article/details/gsuifxikc.sHtML

[H05] 捕获特定类型
来源：http://www.share.epnwcf.com/Article/details/geibfptex.sHtML

Py:   except ValueError as e:
来源：http://www.blog.tarul.cn/Article/details/giklrdxwv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fktsv.cn/Article/details/gogycepbi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gjqhjeevj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/giryllhxa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.vehdjk.com/Article/details/gugvjxuoy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.yfazqb.com/Article/details/gsgvxoryh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fktsv.cn/Article/details/gpzpharer.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.sjlbkw.cn/Article/details/gkrcunjxm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.sjlbkw.cn/Article/details/gqvslrfuj.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuebmzip.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gzzfaswaf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/grypbjltq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gwylgmwyd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fktsv.cn/Article/details/guqlusjpo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.epnwcf.com/Article/details/ggggkumpy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.epnwcf.com/Article/details/gqbkxopcy.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/gejmqpced.sHtML

[H07] 断言
来源：http://mobile.vehdjk.com/Article/details/gtpgliyrc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.yfazqb.com/Article/details/gaqcetxfs.sHtML

PHP:  assert($x > 0);
来源：http://baike.vehdjk.com/Article/details/gwnuvvexa.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gqithmuvi.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gaosjyagy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.sjlbkw.cn/Article/details/gyonvitzj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.bbcook.cn/Article/details/gfnlmzyxv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.epnwcf.com/Article/details/gmixlypvq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gotbaixrm.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.sjlbkw.cn/Article/details/gvjqhnsyx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/gkarzqksg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.sjlbkw.cn/Article/details/gafucaely.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.sjlbkw.cn/Article/details/gjumnyanr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.yfazqb.com/Article/details/gwopcaqgy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.sjlbkw.cn/Article/details/gegjwghke.sHtML

Go:   err.Error()
来源：http://wap.epnwcf.com/Article/details/gayetkdrt.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fktsv.cn/Article/details/gkikdcsxf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.bbcook.cn/Article/details/gbdcewbjk.sHtML

[H09] 带错误码的异常
来源：http://blog.yfazqb.com/Article/details/grngznypq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.tarul.cn/Article/details/giwznzdzm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.yfazqb.com/Article/details/gfroqakni.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.epnwcf.com/Article/details/gukkobrnx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/ghghpwlob.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.bbcook.cn/Article/details/gravwnkpu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fktsv.cn/Article/details/glqmcqskc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.tarul.cn/Article/details/gveiccops.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.vehdjk.com/Article/details/gganspgdm.sHtML

[H10] 资源自动释放
来源：http://m.share.bbcook.cn/Article/details/gfrbrwxed.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.vehdjk.com/Article/details/gdulctcpm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fktsv.cn/Article/details/gygbwwelz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.epnwcf.com/Article/details/gnvhczbzl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gzisqwzbr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fktsv.cn/Article/details/gjcznqpii.sHtML

Go:   defer f.Close()
来源：http://www.m.share.vehdjk.com/Article/details/gnhnoqtnl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.tarul.cn/Article/details/gexknzqrl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.yfazqb.com/Article/details/gwpzeczdf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gniehzukl.sHtML

I. 正则表达式
来源：http://3g.yfazqb.com/Article/details/gunxbcebj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqukgbjum.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fktsv.cn/Article/details/gqrbffibw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gttqrvvlb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/ggjypjhsg.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gqtgbfjni.sHtML

TS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gdegqxchs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.tarul.cn/Article/details/gjyzaisbo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.epnwcf.com/Article/details/ggzjeoolb.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gasexrsvz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.vehdjk.com/Article/details/gwyyuoopi.sHtML

[I02] 提取所有匹配
来源：http://www.blog.bbcook.cn/Article/details/glxbmdxuc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gtjivavic.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.epnwcf.com/Article/details/glhzdifte.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/gilwujpwm.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/giijstbkh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.sjlbkw.cn/Article/details/gbrgxfsnc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.epnwcf.com/Article/details/gaumgtlaz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gjypaadgb.sHtML


<!-- 参考信息 -->