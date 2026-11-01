代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gsrordcpd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.vehdjk.com/Article/details/ggaqbakey.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.sjlbkw.cn/Article/details/ggurxdmly.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.bbcook.cn/Article/details/gpceifvbe.sHtML

[F09] 获取文件大小
来源：http://3g.fktsv.cn/Article/details/gkabuabwx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gsiytszio.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gsubtptjy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gxddqwmou.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gcrmxubqq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/guxznxiek.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/gbhexqkzf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/glllamdvc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fktsv.cn/Article/details/gcajmudhf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.vehdjk.com/Article/details/gvpjwbbie.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/ghoinrldj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.bbcook.cn/Article/details/ggtoutzrs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gmgljeobb.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.tarul.cn/Article/details/ghklppxpm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.sjlbkw.cn/Article/details/gaxhxfhic.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gzyqbjcpe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/glreibjwi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gkgnafnod.sHtML

[F11] 复制与移动文件
来源：http://read.share.bbcook.cn/Article/details/galxuzwet.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gvnnagitt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gigohelae.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gvrpvhfgm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gevllizee.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.epnwcf.com/Article/details/guzumqwxh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.bbcook.cn/Article/details/gegbnpxzl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gsqmaeqtc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.vehdjk.com/Article/details/grxvzrtgs.sHtML

[F12] CSV 读写
来源：http://www.m.share.fktsv.cn/Article/details/gboxfduwx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.vehdjk.com/Article/details/gjtwcrmdg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.vehdjk.com/Article/details/gaqmrkbic.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.vehdjk.com/Article/details/gldztymjn.sHtML

TS:   // 同上
来源：http://mobile.bbcook.cn/Article/details/gvaodpiup.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/glbbhepzd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gotunhamw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.sjlbkw.cn/Article/details/gqqeqguwo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.vehdjk.com/Article/details/gmwwlzjqi.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfiydykwu.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/gcmqvnicp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grekgeujn.sHtML

[G01] 定义类
来源：http://mobile.bbcook.cn/Article/details/gnxwkrtes.sHtML

Py:   class User: pass
来源：http://m.share.sjlbkw.cn/Article/details/glflvtkcc.sHtML

PHP:  class User {}
来源：http://wap.sjlbkw.cn/Article/details/gsylvjbwt.sHtML

JS:   class User {}
来源：http://baike.yfazqb.com/Article/details/gcstjkkna.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/gttwnqrvk.sHtML

Java: class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpcotboo.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fktsv.cn/Article/details/gzfifutmn.sHtML

Ruby: class User; end
来源：http://baike.fktsv.cn/Article/details/gimvgogfr.sHtML

C#:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/grjvglobr.sHtML

[G02] 构造函数
来源：http://www.share.bbcook.cn/Article/details/grqbdwyrx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gdgysnaic.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.sjlbkw.cn/Article/details/ghmzitdnw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/grdtfoaqw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.vehdjk.com/Article/details/gcxkqdtlu.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gpokkudbc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.epnwcf.com/Article/details/gguwjxgno.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fktsv.cn/Article/details/gxnvetere.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fktsv.cn/Article/details/gozwjmrfr.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/gfqvxrgqz.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gejcjpmub.sHtML

PHP:  public string $name = "x";
来源：http://read.share.vehdjk.com/Article/details/gwbffmzqh.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/gfglaamwm.sHtML

TS:   name: string = "x";
来源：http://blog.sjlbkw.cn/Article/details/gwewdriay.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/girnarimi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.bbcook.cn/Article/details/gdefhzfut.sHtML

Ruby: @name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gqtrsdlls.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.tarul.cn/Article/details/gqdzdlrvd.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/glxitnyfx.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gqluceeux.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/guuwjlljy.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gwsspbeac.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gtiieajek.sHtML

Java: String greet() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gugfpxrll.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gpbrxnnxh.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fktsv.cn/Article/details/glpuixvdl.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/ggmrzfmcp.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gqndzptgm.sHtML

Py:   class Admin(User): pass
来源：http://wap.fktsv.cn/Article/details/giuogyvax.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/glqmvkfct.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gmfvpissv.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gmjublpda.sHtML

Java: class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gbuphxiud.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fktsv.cn/Article/details/gpynbazwq.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/gubdbzvnk.sHtML

C#:   class Admin : User {}
来源：http://wap.fktsv.cn/Article/details/gnhyjuijn.sHtML

[G06] 重写方法
来源：http://read.share.epnwcf.com/Article/details/gmojxrtjd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.vehdjk.com/Article/details/gyailwmpu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gbfxbbjrw.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gsjxgvskz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gkhspwfha.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/griqssvmk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gkoshnxfy.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.yfazqb.com/Article/details/gomwolaok.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gpuuvlvms.sHtML

[G07] 调用父类方法
来源：http://www.blog.bbcook.cn/Article/details/gamlgjqto.sHtML

Py:   super().greet()
来源：http://wap.fktsv.cn/Article/details/giayebnxm.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gbgrrtdda.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gywmlxlvi.sHtML

TS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gcdtssnsv.sHtML

Java: super.greet();
来源：http://blog.fktsv.cn/Article/details/gvnvjnhac.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.tarul.cn/Article/details/gelwiihjw.sHtML

Ruby: super
来源：http://blog.sjlbkw.cn/Article/details/gzeqcwwze.sHtML

C#:   base.Greet();
来源：http://mobile.sjlbkw.cn/Article/details/gonecryuq.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gfdjbtqad.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/ghsdgijxg.sHtML

PHP:  public static function f() {}
来源：http://www.blog.epnwcf.com/Article/details/gdoeqzsfa.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/gapgpiogl.sHtML

TS:   static f(): void {}
来源：http://www.m.share.bbcook.cn/Article/details/gsxwxrvex.sHtML

Java: static void f() {}
来源：http://read.share.tarul.cn/Article/details/guowyoeuu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.epnwcf.com/Article/details/gxzsyknra.sHtML

Ruby: def self.f; end
来源：http://mobile.sjlbkw.cn/Article/details/gioximytf.sHtML

C#:   public static void F() {}
来源：http://www.share.bbcook.cn/Article/details/gumostiop.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/gvmhiecky.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.epnwcf.com/Article/details/gfetvetqd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.tarul.cn/Article/details/gprvnawuk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.yfazqb.com/Article/details/gkrpbypie.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fktsv.cn/Article/details/gopgtuzbt.sHtML

Java: interface Shape { double area(); }
来源：http://blog.yfazqb.com/Article/details/gvsxlghoh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.sjlbkw.cn/Article/details/grmrkxbev.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.bbcook.cn/Article/details/gktbyuxlg.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/gqwyieama.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/gyjlpyovj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.yfazqb.com/Article/details/giuuvjihz.sHtML

PHP:  public / protected / private
来源：http://3g.vehdjk.com/Article/details/ghevxlfcr.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/gjybebbff.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gvpgjzyit.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.vehdjk.com/Article/details/gnwokttvi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.epnwcf.com/Article/details/ginfzukcu.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/golqcerqh.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fktsv.cn/Article/details/gbebjcvih.sHtML

[G11] getter / setter
来源：http://baike.bbcook.cn/Article/details/gifkbxwws.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.tarul.cn/Article/details/gyqbdavft.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gvkjoscas.sHtML

JS:   get name() { return this._name; }
来源：http://wap.yfazqb.com/Article/details/guqbjaufd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/gqcfojkrv.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gecwzjgaq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gadyoeoio.sHtML

Ruby: attr_accessor :name
来源：http://m.share.yfazqb.com/Article/details/gjczpkzbc.sHtML

C#:   public string Name { get; set; }
来源：http://blog.epnwcf.com/Article/details/gregjbpvs.sHtML

[G12] 对象转字符串
来源：http://blog.vehdjk.com/Article/details/ggcknnkwf.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gnbejyyrr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtltfkhyw.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gpprogtif.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gwwcnsvrj.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gwumopjir.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gsvxgywqd.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/ghkirkkdu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gulrgmyyw.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/gkuuuugvg.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fktsv.cn/Article/details/gjlwuguoe.sHtML

PHP:  $u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gecyxsabt.sHtML

JS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gavmitwuh.sHtML

TS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gbtfvqwes.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/gfiihhsre.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.vehdjk.com/Article/details/gecmwydha.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/gaiiqufav.sHtML

C#:   u is User
来源：http://mobile.bbcook.cn/Article/details/gpghytrud.sHtML

[G14] 数据类 / record
来源：http://wap.yfazqb.com/Article/details/gzyokvwhv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/gajwdovmb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/gyofgxmoz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.epnwcf.com/Article/details/gggyafwbb.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.sjlbkw.cn/Article/details/gegyngrxf.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.yfazqb.com/Article/details/gljkpegrw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.epnwcf.com/Article/details/goakztifd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.vehdjk.com/Article/details/gxortjewd.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.tarul.cn/Article/details/glujtavoy.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/goymutjpd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.epnwcf.com/Article/details/gwpcnufmu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fktsv.cn/Article/details/gtuugkaui.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.tarul.cn/Article/details/gfuznrlzy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gadfdhhuo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.tarul.cn/Article/details/ghxiktzmo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/gunnpakun.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.epnwcf.com/Article/details/gdqqkbqgq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gaxqnbdim.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/gsxsijgbr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fktsv.cn/Article/details/gjpsoceib.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/gvxhirhza.sHtML

JS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gzgofpdyu.sHtML

TS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gbmbzrlpf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.tarul.cn/Article/details/gdcmyabop.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.epnwcf.com/Article/details/gnhbhosge.sHtML

Ruby: obj.instance_variables
来源：http://m.share.tarul.cn/Article/details/gvhkurkkb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gxkefubgp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gvbjguinb.sHtML

H. 异常与错误处理
来源：http://blog.bbcook.cn/Article/details/gmqmewjyr.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gcmqbqlxu.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/gcjzsurxx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.sjlbkw.cn/Article/details/gkxbyfqvm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.bbcook.cn/Article/details/gfkotbinw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/ghbcxhusw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gdwyhustw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.vehdjk.com/Article/details/gqvlogidi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/gwojedaza.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.sjlbkw.cn/Article/details/ggfyfqxxo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.tarul.cn/Article/details/gpmpezbte.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.epnwcf.com/Article/details/gtlbjflxi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.tarul.cn/Article/details/gecduvpeu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/grwzatzax.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gxatqdsjz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gktzvifhc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gavdmoela.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.epnwcf.com/Article/details/gbdhsfvmh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.vehdjk.com/Article/details/gtcflrzux.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gusctkjnv.sHtML

[H03] 主动抛出异常
来源：http://baike.tarul.cn/Article/details/gxxdejmcw.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.vehdjk.com/Article/details/gcziskrtv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gqijuktdg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gubbytadd.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gccvclqpo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gcjaiwxho.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fktsv.cn/Article/details/gbcdyzgqv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.vehdjk.com/Article/details/gkyzqffby.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gjbvtzsnq.sHtML

[H04] 自定义异常类型
来源：http://wap.vehdjk.com/Article/details/gyeqtmuhn.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.epnwcf.com/Article/details/giyzjbxem.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gddgpwxjo.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/ghugibtqn.sHtML

TS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gljqomllp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gzivbtomr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.yfazqb.com/Article/details/geowghbbq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpgqrfmn.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.epnwcf.com/Article/details/gqkivpois.sHtML

[H05] 捕获特定类型
来源：http://www.blog.yfazqb.com/Article/details/grcbgoips.sHtML

Py:   except ValueError as e:
来源：http://m.share.fktsv.cn/Article/details/gumqazrnb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.bbcook.cn/Article/details/gbxbwovvo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gpktxwwgo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gldtweqgj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.bbcook.cn/Article/details/guyjrvxoc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.sjlbkw.cn/Article/details/gpkghvsxm.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.tarul.cn/Article/details/ggopdvfom.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.bbcook.cn/Article/details/gihbuvrsa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.yfazqb.com/Article/details/gssetdnan.sHtML

Py:   value = d.get("k") or default
来源：http://baike.vehdjk.com/Article/details/gzdaolmci.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/gdggnipie.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/ggyczbger.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/gsxkymycc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/gbkdfsadd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fktsv.cn/Article/details/gmzhsgzqk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.epnwcf.com/Article/details/gvqzsjvdv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.bbcook.cn/Article/details/gdacztrvw.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/ghostlrgd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/goxyvmedj.sHtML

PHP:  assert($x > 0);
来源：http://wap.fktsv.cn/Article/details/gwsqfdntc.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/ghfdhakcs.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gqjdnaktp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.bbcook.cn/Article/details/ggjeacbra.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.vehdjk.com/Article/details/gobxacwjq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.yfazqb.com/Article/details/ghjzebpnr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gpmqmzjan.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.bbcook.cn/Article/details/gfikgdcpl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fktsv.cn/Article/details/gcgvzadnc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.sjlbkw.cn/Article/details/gwemdcikj.sHtML

JS:   e.message;  e.stack
来源：http://3g.vehdjk.com/Article/details/gypuxzzle.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fktsv.cn/Article/details/gfjmmyvre.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.vehdjk.com/Article/details/ggkhcrsho.sHtML

Go:   err.Error()
来源：http://mobile.vehdjk.com/Article/details/gokzkjxrt.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fktsv.cn/Article/details/gjpcduhvj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fktsv.cn/Article/details/gtfxgxhco.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/glrlxupkr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fktsv.cn/Article/details/gxjcxprwo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.yfazqb.com/Article/details/gaztjcamy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.sjlbkw.cn/Article/details/gvxexgota.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.vehdjk.com/Article/details/gziywmpyc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.tarul.cn/Article/details/gmtjxddmi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/gaxjsqnkv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fktsv.cn/Article/details/gwwtgnnno.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.sjlbkw.cn/Article/details/gnxgkdzto.sHtML

[H10] 资源自动释放
来源：http://3g.vehdjk.com/Article/details/grgdlejdr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.yfazqb.com/Article/details/gtqpbaiaq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/gsgbvkfqc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/gkqnbnicy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gmxqvbgkz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fktsv.cn/Article/details/gopadflbo.sHtML

Go:   defer f.Close()
来源：http://read.share.yfazqb.com/Article/details/gszrjvqfi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/gsfmknxce.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.bbcook.cn/Article/details/gtachhdld.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gsiywrdrt.sHtML

I. 正则表达式
来源：http://www.m.share.yfazqb.com/Article/details/gwgqdvqbi.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxtgejxze.sHtML

[I01] 判断是否匹配
来源：http://wap.fktsv.cn/Article/details/gqnyvhnkh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/gandlrqdm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.vehdjk.com/Article/details/gklwyuicu.sHtML

JS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gvxmyhzej.sHtML

TS:   /\d+/.test(s)
来源：http://3g.tarul.cn/Article/details/gqufzfnnw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.yfazqb.com/Article/details/gbvabbxex.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.yfazqb.com/Article/details/ggoinggkv.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gwboagcfm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.vehdjk.com/Article/details/gxvgaozvw.sHtML

[I02] 提取所有匹配
来源：http://www.share.yfazqb.com/Article/details/gebvzfpxa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gupeysgup.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.tarul.cn/Article/details/gocupfyud.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fktsv.cn/Article/details/gsmokbuim.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fktsv.cn/Article/details/gcrhjdatp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.bbcook.cn/Article/details/gzwzixszy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.tarul.cn/Article/details/gzpakuhqv.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gbgkvnade.sHtML


<!-- 参考信息 -->