代发 wailian999

[F09] 获取文件大小
来源：http://www.blog.sjlbkw.cn/Article/details/gssfmhahd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.tarul.cn/Article/details/ghfhztjsy.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fktsv.cn/Article/details/gvvnruvmv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gntyvhplf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gviphotdz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gftqorqls.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.sjlbkw.cn/Article/details/gdhixlzpm.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gxpqfnixk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.sjlbkw.cn/Article/details/goqtwjefi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.tarul.cn/Article/details/ghifmqwqu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/godbhhuip.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/gikjteejk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gxzmzwdrf.sHtML

TS:   path.extname("a.txt")
来源：http://baike.epnwcf.com/Article/details/glngpdmbw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fktsv.cn/Article/details/grtssqxmj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gbmxdkoak.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/grpttyosy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gmtyivdcg.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/gmijilugw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gywapymbx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/grrcaraay.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/ghozavdsc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/goshddydl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gtkfhdpnb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.vehdjk.com/Article/details/gvhowxhdt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gpggxzasp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fktsv.cn/Article/details/gjnqmxsmv.sHtML

[F12] CSV 读写
来源：http://blog.bbcook.cn/Article/details/gsczpkavd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.yfazqb.com/Article/details/gsztntbuw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/gycvsxarh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.vehdjk.com/Article/details/ghyfjlqay.sHtML

TS:   // 同上
来源：http://wap.bbcook.cn/Article/details/gxdnarvlk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gjxfjxuyx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fktsv.cn/Article/details/gstsxozbu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.tarul.cn/Article/details/gbzdercih.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.bbcook.cn/Article/details/gmxitcshl.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzpbwvteq.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/gkfrcczop.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzovixjul.sHtML

[G01] 定义类
来源：http://baike.epnwcf.com/Article/details/gyvbsvkkg.sHtML

Py:   class User: pass
来源：http://read.share.sjlbkw.cn/Article/details/grpfxhxqk.sHtML

PHP:  class User {}
来源：http://3g.tarul.cn/Article/details/gfoyoewuc.sHtML

JS:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gpimtjday.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.yfazqb.com/Article/details/gsodenruc.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gxosixiun.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/grtfslpmc.sHtML

Ruby: class User; end
来源：http://wap.sjlbkw.cn/Article/details/gprqdjuzw.sHtML

C#:   class User {}
来源：http://blog.yfazqb.com/Article/details/gtdkwgdfv.sHtML

[G02] 构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gbtjdiaqy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.tarul.cn/Article/details/ggmzausnr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.bbcook.cn/Article/details/gcbtfpsyi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/ggzqzrhre.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.bbcook.cn/Article/details/gvinhklgb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gjwgjgkvv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.sjlbkw.cn/Article/details/gcikutchp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.sjlbkw.cn/Article/details/gaiijzcmi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.bbcook.cn/Article/details/gwtdetcoj.sHtML

[G03] 实例属性
来源：http://3g.yfazqb.com/Article/details/gdeywypxf.sHtML

Py:   self.name = "x"
来源：http://m.share.tarul.cn/Article/details/gzgiebryo.sHtML

PHP:  public string $name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gquwxwclk.sHtML

JS:   this.name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gbfmemdgp.sHtML

TS:   name: string = "x";
来源：http://m.share.yfazqb.com/Article/details/gzbrxhzzp.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/gltmcvoyw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fktsv.cn/Article/details/gijjtpbrl.sHtML

Ruby: @name = "x"
来源：http://m.share.yfazqb.com/Article/details/gdwktrvbc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.yfazqb.com/Article/details/gxrgzajxl.sHtML

[G04] 定义方法
来源：http://3g.epnwcf.com/Article/details/gsnyatupm.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gxhablkvl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/ggweolnmy.sHtML

JS:   greet() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gsazdxuov.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/ggbbjbpai.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gekohpizk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gooctenxs.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/gqhxixvkx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.bbcook.cn/Article/details/gsphxepdk.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/ghcdjfjcr.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/gsjrueqlo.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gfpnbgpur.sHtML

JS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gcyrruswx.sHtML

TS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gfqzmeuac.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gcyphwpmo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fktsv.cn/Article/details/ghbpabckb.sHtML

Ruby: class Admin < User; end
来源：http://mobile.tarul.cn/Article/details/gjlksbrbe.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/goeizbxjs.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/gpkkxgprf.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.bbcook.cn/Article/details/gpxqgwvev.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gxbgudfvu.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gvterhxbi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gcnerfrxa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gikkhoele.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.tarul.cn/Article/details/gkreobkkl.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.epnwcf.com/Article/details/gfojihqst.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/gkfefjpwb.sHtML

[G07] 调用父类方法
来源：http://blog.bbcook.cn/Article/details/gdjignzfh.sHtML

Py:   super().greet()
来源：http://mobile.sjlbkw.cn/Article/details/gqcltrcck.sHtML

PHP:  parent::greet();
来源：http://m.share.vehdjk.com/Article/details/gxozfobcr.sHtML

JS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gfrlrhvww.sHtML

TS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/ghuvvvjgr.sHtML

Java: super.greet();
来源：http://m.share.bbcook.cn/Article/details/gtfwhqvmy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.bbcook.cn/Article/details/gfvmqfsnu.sHtML

Ruby: super
来源：http://www.share.sjlbkw.cn/Article/details/gafbtpbts.sHtML

C#:   base.Greet();
来源：http://www.blog.epnwcf.com/Article/details/ghuglcasp.sHtML

[G08] 静态方法与属性
来源：http://www.blog.vehdjk.com/Article/details/ghcfkrkcb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.tarul.cn/Article/details/gmainteyi.sHtML

PHP:  public static function f() {}
来源：http://m.share.tarul.cn/Article/details/gmlgflcos.sHtML

JS:   static f() {}
来源：http://3g.tarul.cn/Article/details/gsfwnriwb.sHtML

TS:   static f(): void {}
来源：http://m.share.yfazqb.com/Article/details/gitqdphrn.sHtML

Java: static void f() {}
来源：http://baike.bbcook.cn/Article/details/gcxlxeydb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/gmaddzfde.sHtML

Ruby: def self.f; end
来源：http://m.share.vehdjk.com/Article/details/gyveweqca.sHtML

C#:   public static void F() {}
来源：http://read.share.vehdjk.com/Article/details/gkkdzttgs.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.yfazqb.com/Article/details/gaaxtvdfl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.epnwcf.com/Article/details/glyrrybzu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.bbcook.cn/Article/details/gerncxtng.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.sjlbkw.cn/Article/details/guszidzat.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.bbcook.cn/Article/details/ghihowgtt.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.vehdjk.com/Article/details/gesnvnulp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fktsv.cn/Article/details/gyupxeyhw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.bbcook.cn/Article/details/gzqvbofgc.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gwnposwly.sHtML

[G10] 访问控制
来源：http://m.share.bbcook.cn/Article/details/gllrhxryj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.epnwcf.com/Article/details/gajqgurbp.sHtML

PHP:  public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gjryyuhec.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fktsv.cn/Article/details/gfujdbzxp.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gtdqzefmj.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fktsv.cn/Article/details/guhpudhzi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.sjlbkw.cn/Article/details/gtjqnhbat.sHtML

Ruby: public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gsgaywgoy.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/gqpitrgop.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/gsotbsdho.sHtML

Py:   @property 与 @x.setter
来源：http://3g.bbcook.cn/Article/details/galrmpotg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gekgmitos.sHtML

JS:   get name() { return this._name; }
来源：http://baike.tarul.cn/Article/details/gpfytueit.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.tarul.cn/Article/details/gtvaclwej.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/guvjdahzz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gfumyzbmj.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.vehdjk.com/Article/details/gnnjudyon.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.bbcook.cn/Article/details/gowavrjus.sHtML

[G12] 对象转字符串
来源：http://wap.sjlbkw.cn/Article/details/gxekwtkqe.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/gfljdllpt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gbioovmgg.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gywfcuosi.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/ggszbdabx.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fktsv.cn/Article/details/gqtbbcajl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gjmmsyawb.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.tarul.cn/Article/details/guevezsaq.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.epnwcf.com/Article/details/gtrsuudrx.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gmwavvnyb.sHtML

Py:   isinstance(u, User)
来源：http://baike.sjlbkw.cn/Article/details/gunvrpnyq.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gsqlymyci.sHtML

JS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/glrovackr.sHtML

TS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gjexujunx.sHtML

Java: u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gzypzcnhr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.bbcook.cn/Article/details/gkysvkolm.sHtML

Ruby: u.is_a?(User)
来源：http://wap.yfazqb.com/Article/details/gwbrizuzv.sHtML

C#:   u is User
来源：http://m.share.yfazqb.com/Article/details/gbrnidclf.sHtML

[G14] 数据类 / record
来源：http://www.share.bbcook.cn/Article/details/gnbiwrirt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.vehdjk.com/Article/details/gleyzeqdn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gexpyigwk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.vehdjk.com/Article/details/gfxypragk.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.yfazqb.com/Article/details/gsopnhvxi.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.tarul.cn/Article/details/gjjwshich.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.sjlbkw.cn/Article/details/gvyunuukg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gorparvdc.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.sjlbkw.cn/Article/details/gplcqgytr.sHtML

[G15] 枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrbvpcwn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.bbcook.cn/Article/details/gufsmtqqm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.sjlbkw.cn/Article/details/ggpslaexu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.sjlbkw.cn/Article/details/gtoxmksgv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gceeetlvb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.yfazqb.com/Article/details/gcycjkhpo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/ggbsormxt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/gfwrnunyh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gwgbjpilb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.tarul.cn/Article/details/gezheoduj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fktsv.cn/Article/details/gklrqfgnm.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.bbcook.cn/Article/details/gtizylvwl.sHtML

JS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gapmubzdd.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gketepozc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fktsv.cn/Article/details/gfiwfgkap.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.vehdjk.com/Article/details/gwwmmyxpf.sHtML

Ruby: obj.instance_variables
来源：http://wap.bbcook.cn/Article/details/gmswzkvmb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gxlvsziyd.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/glnaypuip.sHtML

H. 异常与错误处理
来源：http://m.share.epnwcf.com/Article/details/givuwjmqr.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghqkbybiz.sHtML

[H01] try / catch 基础
来源：http://3g.sjlbkw.cn/Article/details/gltvsqihm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/gzhurjzwz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.vehdjk.com/Article/details/gdtkganje.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/geyqjudgw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gdxyfklhi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gdvvsjvtc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.bbcook.cn/Article/details/glljgshzt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.yfazqb.com/Article/details/gbpjtgmtw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.vehdjk.com/Article/details/gaicpbyje.sHtML

[H02] finally / ensure 收尾
来源：http://3g.vehdjk.com/Article/details/gdiqmovcz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.vehdjk.com/Article/details/gidhcidzk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gvamcxtiv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gyxamcfyf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gljckcfmx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gabedejow.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fktsv.cn/Article/details/gxjtdovxh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.tarul.cn/Article/details/gezprjolf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gfblpkuwi.sHtML

[H03] 主动抛出异常
来源：http://www.share.tarul.cn/Article/details/gmdjdevvi.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.yfazqb.com/Article/details/gcxnpajlz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/grnjfxssk.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gzdnhanhi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gfpaubslu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/goqquzuuo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fktsv.cn/Article/details/gvakvfnrj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.yfazqb.com/Article/details/gviayfbhn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gnxyicdrt.sHtML

[H04] 自定义异常类型
来源：http://read.share.fktsv.cn/Article/details/gywbeyjjl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.epnwcf.com/Article/details/gqpexifex.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gslgdqyfd.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gljhyiojd.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gcykvwdce.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gtbqdozcd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.bbcook.cn/Article/details/gwzgojloo.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gimnryngn.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fktsv.cn/Article/details/gjdymtjgv.sHtML

[H05] 捕获特定类型
来源：http://m.share.vehdjk.com/Article/details/gwhyclvou.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.tarul.cn/Article/details/gwrwsqavq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.vehdjk.com/Article/details/gtganivjr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gxfcqtipz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gmapjwgft.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.tarul.cn/Article/details/gtfnrhjwd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.epnwcf.com/Article/details/gjckdovej.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.yfazqb.com/Article/details/grvfzjdre.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.bbcook.cn/Article/details/gchdqsefg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fktsv.cn/Article/details/gvvipofog.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/gwymophpj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/gztqvxyxl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gytovzurl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gzpqyhels.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fktsv.cn/Article/details/guwojtoxn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.yfazqb.com/Article/details/gylkaugut.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.tarul.cn/Article/details/gvyhcmagz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.tarul.cn/Article/details/gdmokvkpv.sHtML

[H07] 断言
来源：http://read.share.epnwcf.com/Article/details/gfyzacgsq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.yfazqb.com/Article/details/gzdyndomk.sHtML

PHP:  assert($x > 0);
来源：http://www.share.yfazqb.com/Article/details/gefprdpfm.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gymurcrcv.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gwkfynozm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.yfazqb.com/Article/details/gfvalkruz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.yfazqb.com/Article/details/ghdypnbfj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.epnwcf.com/Article/details/gnliimyjm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.vehdjk.com/Article/details/gdiwpwvjf.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.tarul.cn/Article/details/gtugcdhvn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gxrewidmi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.epnwcf.com/Article/details/grxmqdulc.sHtML

JS:   e.message;  e.stack
来源：http://3g.fktsv.cn/Article/details/gccibggby.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fktsv.cn/Article/details/gpibzyjlz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.tarul.cn/Article/details/gcydnklbc.sHtML

Go:   err.Error()
来源：http://m.share.vehdjk.com/Article/details/gpfilwekf.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.sjlbkw.cn/Article/details/glprbwtrs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.bbcook.cn/Article/details/gcedvpxob.sHtML

[H09] 带错误码的异常
来源：http://m.share.tarul.cn/Article/details/gbhtjkbwy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.tarul.cn/Article/details/goztrqrub.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.bbcook.cn/Article/details/gsyyuojng.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.bbcook.cn/Article/details/gmktyxlgc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.yfazqb.com/Article/details/gfosbbrqb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.vehdjk.com/Article/details/gxmadzlbv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.bbcook.cn/Article/details/gqcszljqc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtetytszc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.vehdjk.com/Article/details/gqrvqzfnl.sHtML

[H10] 资源自动释放
来源：http://www.m.share.epnwcf.com/Article/details/gijhpsvas.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fktsv.cn/Article/details/glxqofout.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.yfazqb.com/Article/details/grdulnpun.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/ghlwqccgp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.sjlbkw.cn/Article/details/gmrjqawfi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.sjlbkw.cn/Article/details/ghwojbjtc.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gnmqueouq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.epnwcf.com/Article/details/gsqpvchgv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gpysmtvbn.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/geexvdrwf.sHtML

I. 正则表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gduadyanp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gvehmmsrr.sHtML

[I01] 判断是否匹配
来源：http://www.share.fktsv.cn/Article/details/girensiqw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/govnyomrg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.tarul.cn/Article/details/gitzmakrp.sHtML

JS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/grhsmycoh.sHtML

TS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/gofrnjpaf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.yfazqb.com/Article/details/gqpyqdygn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.tarul.cn/Article/details/ggpjjbays.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/grxjtihwv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.bbcook.cn/Article/details/gwxxczqlr.sHtML

[I02] 提取所有匹配
来源：http://read.share.epnwcf.com/Article/details/gckyqgdhh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.yfazqb.com/Article/details/gtkcjpglv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gpnslxmxq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fktsv.cn/Article/details/gwdqvjlcd.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.vehdjk.com/Article/details/gnbokkdgg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fktsv.cn/Article/details/gorwfzurn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.tarul.cn/Article/details/gmdaxdpgw.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gcyipxymf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gurzgntku.sHtML

[I03] 提取捕获分组
来源：http://wap.vehdjk.com/Article/details/gdldvvfrm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fktsv.cn/Article/details/gnnejnory.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fktsv.cn/Article/details/gedsdfbal.sHtML


<!-- 参考信息 -->