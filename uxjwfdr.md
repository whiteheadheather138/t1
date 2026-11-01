代发 wailian999

[F09] 获取文件大小
来源：http://wap.sjlbkw.cn/Article/details/gaepnjcfe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/gqkrseryz.sHtML

PHP:  filesize("a.txt");
来源：http://blog.epnwcf.com/Article/details/ghkdrsmyx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gpdateanc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gvuavttfv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gyrrhixwl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.yfazqb.com/Article/details/gfextdjgc.sHtML

Ruby: File.size("a.txt")
来源：http://blog.bbcook.cn/Article/details/gjjeufizp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.epnwcf.com/Article/details/ghkokwpyn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.epnwcf.com/Article/details/gnrlsaizq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gxjgqfonf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gothqxqys.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gsmkbqjsf.sHtML

TS:   path.extname("a.txt")
来源：http://baike.vehdjk.com/Article/details/gkcyggtfl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fktsv.cn/Article/details/gpsyswemi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/grzhsancw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gajxhenwq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gyvhhqivu.sHtML

[F11] 复制与移动文件
来源：http://blog.fktsv.cn/Article/details/gnlvayfgk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gxffdwyzc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.yfazqb.com/Article/details/gfdiyxton.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gbrjwtyxp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gxacocrer.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.vehdjk.com/Article/details/gcouakqah.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gnqnlmghm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gzbvajhyr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.yfazqb.com/Article/details/gcypqevcf.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/gotlkjwbo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/glvjnjcru.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/giggztigo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gwxdfmmwo.sHtML

TS:   // 同上
来源：http://wap.yfazqb.com/Article/details/ganrprkms.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.yfazqb.com/Article/details/gmhovceqi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.sjlbkw.cn/Article/details/gxjnunted.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.sjlbkw.cn/Article/details/gqlmvjqyo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fktsv.cn/Article/details/gozfneewd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/goiciigkp.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/gzcxvgjkx.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsdakktgn.sHtML

[G01] 定义类
来源：http://baike.tarul.cn/Article/details/gahigzxfs.sHtML

Py:   class User: pass
来源：http://mobile.sjlbkw.cn/Article/details/geuingxti.sHtML

PHP:  class User {}
来源：http://www.m.share.tarul.cn/Article/details/gtvjtiaww.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gjvkkjypz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/gysmcjwuc.sHtML

Java: class User {}
来源：http://blog.vehdjk.com/Article/details/gwouxftfd.sHtML

Go:   type User struct { Name string }
来源：http://m.share.sjlbkw.cn/Article/details/gibtdnmvx.sHtML

Ruby: class User; end
来源：http://3g.epnwcf.com/Article/details/ghrqyjaqp.sHtML

C#:   class User {}
来源：http://wap.epnwcf.com/Article/details/grmivkhos.sHtML

[G02] 构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gjsyibzkq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fktsv.cn/Article/details/gfqynbugh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.bbcook.cn/Article/details/gftyynbak.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gefobynji.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.tarul.cn/Article/details/gqfemuuei.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/ghgcvreun.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fktsv.cn/Article/details/gynpbyjyu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.vehdjk.com/Article/details/gmtbcvifc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gequcwkxs.sHtML

[G03] 实例属性
来源：http://baike.tarul.cn/Article/details/gcxjvmxqv.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/gvfbnlpbi.sHtML

PHP:  public string $name = "x";
来源：http://baike.yfazqb.com/Article/details/grqzykdke.sHtML

JS:   this.name = "x";
来源：http://3g.bbcook.cn/Article/details/gmdizgyrq.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/gghgtmzjx.sHtML

Java: private String name;
来源：http://www.share.bbcook.cn/Article/details/gccaibcsq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.epnwcf.com/Article/details/groeaegrd.sHtML

Ruby: @name = "x"
来源：http://www.blog.epnwcf.com/Article/details/gvdbtammk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.yfazqb.com/Article/details/gpcmeiwqo.sHtML

[G04] 定义方法
来源：http://www.m.share.bbcook.cn/Article/details/ggokmcaup.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.yfazqb.com/Article/details/gpoavvwxl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/grffxdyjw.sHtML

JS:   greet() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gzlhlcgsi.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gktvgyqyv.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/gssvviatw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gppuspahm.sHtML

Ruby: def greet; @name; end
来源：http://blog.epnwcf.com/Article/details/ghnnaggzw.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/gdsaksdwz.sHtML

[G05] 继承
来源：http://blog.sjlbkw.cn/Article/details/gbvmllwzz.sHtML

Py:   class Admin(User): pass
来源：http://read.share.vehdjk.com/Article/details/gteseiwwh.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/giziroilt.sHtML

JS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gucaavqiy.sHtML

TS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gaiyeejdx.sHtML

Java: class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/glpwmdqhm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.epnwcf.com/Article/details/gnmhkdnwt.sHtML

Ruby: class Admin < User; end
来源：http://baike.yfazqb.com/Article/details/gwtbavrqe.sHtML

C#:   class Admin : User {}
来源：http://www.share.yfazqb.com/Article/details/gminfnajg.sHtML

[G06] 重写方法
来源：http://m.share.epnwcf.com/Article/details/gwzgmgbii.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/gmebadoso.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gwsprlezn.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gxnkrsfze.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/grmzhrrwm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gpvmxuflz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.vehdjk.com/Article/details/gayqwjhpc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.bbcook.cn/Article/details/gtvuibafy.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.sjlbkw.cn/Article/details/gvkkocgkk.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/ggvbxrscs.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/gvsgpibqj.sHtML

PHP:  parent::greet();
来源：http://m.share.yfazqb.com/Article/details/gaxpjmhmb.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gcrxcflwp.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/glxfihyjz.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gnduikedm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.yfazqb.com/Article/details/gvexbnsou.sHtML

Ruby: super
来源：http://wap.bbcook.cn/Article/details/grjljpmjo.sHtML

C#:   base.Greet();
来源：http://baike.epnwcf.com/Article/details/gxcqttcal.sHtML

[G08] 静态方法与属性
来源：http://3g.sjlbkw.cn/Article/details/ghdxdbbgx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fktsv.cn/Article/details/guggfjvqe.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/gmrewpnxw.sHtML

JS:   static f() {}
来源：http://www.blog.yfazqb.com/Article/details/gmemxzmfc.sHtML

TS:   static f(): void {}
来源：http://blog.vehdjk.com/Article/details/gscccwrgw.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gnwwktndx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fktsv.cn/Article/details/gxqqsmtub.sHtML

Ruby: def self.f; end
来源：http://m.share.yfazqb.com/Article/details/gxkrnakxj.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gnmdafenn.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.sjlbkw.cn/Article/details/gviwnbuiv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.epnwcf.com/Article/details/gwjljurdo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.vehdjk.com/Article/details/gvnobosuc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.tarul.cn/Article/details/gorrkqesf.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.bbcook.cn/Article/details/gvfvozmyg.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.vehdjk.com/Article/details/ghxaxfqlj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.epnwcf.com/Article/details/gpzqagndm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.yfazqb.com/Article/details/gkomfqtxj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.yfazqb.com/Article/details/glnnowdme.sHtML

[G10] 访问控制
来源：http://www.m.share.tarul.cn/Article/details/gibqcdwcf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fktsv.cn/Article/details/gmvaahurh.sHtML

PHP:  public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gkeszzklx.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fktsv.cn/Article/details/giijlsetp.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gczhzuigr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.sjlbkw.cn/Article/details/gemvlwuaf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.tarul.cn/Article/details/gszlqnyyd.sHtML

Ruby: public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gxzonavft.sHtML

C#:   public / protected / private / internal
来源：http://3g.epnwcf.com/Article/details/gddfqzvnv.sHtML

[G11] getter / setter
来源：http://wap.epnwcf.com/Article/details/giixcgist.sHtML

Py:   @property 与 @x.setter
来源：http://3g.tarul.cn/Article/details/gmdknqzvi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gljjopdat.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gietbymml.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gdcgcomay.sHtML

Java: public String getName() { return name; }
来源：http://wap.bbcook.cn/Article/details/gyitrokwh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gunizrhrt.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/gpjzokjqz.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/gizayvfry.sHtML

[G12] 对象转字符串
来源：http://blog.bbcook.cn/Article/details/gkykoewvt.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gidwbtwqc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/ghgmyieht.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gmmuhoxfd.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gvooecwiu.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fktsv.cn/Article/details/gjfqpoouv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gspqfkzbq.sHtML

Ruby: def to_s; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gwxxqegwl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gkqxzbqbr.sHtML

[G13] 判断对象类型
来源：http://wap.yfazqb.com/Article/details/gblinbavk.sHtML

Py:   isinstance(u, User)
来源：http://3g.vehdjk.com/Article/details/gsxruqiok.sHtML

PHP:  $u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/ghoourmvv.sHtML

JS:   u instanceof User
来源：http://3g.bbcook.cn/Article/details/glmfcchtk.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gehjilpww.sHtML

Java: u instanceof User
来源：http://3g.fktsv.cn/Article/details/grqkmjlgg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.tarul.cn/Article/details/gkcvpczbd.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/gcctudtia.sHtML

C#:   u is User
来源：http://www.share.sjlbkw.cn/Article/details/gomkutctn.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/gzrpotsas.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fktsv.cn/Article/details/gpnvgamds.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/gwernkhhk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.tarul.cn/Article/details/gqwfmyrsa.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.vehdjk.com/Article/details/gyveqiuld.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gumchkvyz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gppzaelmg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.bbcook.cn/Article/details/gvnipcqsl.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.epnwcf.com/Article/details/gwgkofukg.sHtML

[G15] 枚举
来源：http://wap.tarul.cn/Article/details/gzftovtds.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.sjlbkw.cn/Article/details/ghbjvqwrn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/gbnrfrzyj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.epnwcf.com/Article/details/ggbcsncpj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.bbcook.cn/Article/details/glatluywe.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fktsv.cn/Article/details/gkufuqacl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fktsv.cn/Article/details/gzhpyojzu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fktsv.cn/Article/details/gxptlgstr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/gvigqaamz.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gnoenthaw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.bbcook.cn/Article/details/gsxkekvtv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.vehdjk.com/Article/details/glenusnnf.sHtML

JS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gcvekezfz.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gtwcblanu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.yfazqb.com/Article/details/gmqwtfymg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.sjlbkw.cn/Article/details/gfxfnycdh.sHtML

Ruby: obj.instance_variables
来源：http://3g.yfazqb.com/Article/details/gdpdogqey.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gqimstaac.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ghbfinmcx.sHtML

H. 异常与错误处理
来源：http://baike.fktsv.cn/Article/details/gntekwfie.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gbcoybzyi.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/gbyjfgnyi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.tarul.cn/Article/details/gdripnung.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.bbcook.cn/Article/details/gxfifmixa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gzoezmjel.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gwgledqln.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/gaxbvavwc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.yfazqb.com/Article/details/gvzihlnpt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.epnwcf.com/Article/details/gtyixsgwi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fktsv.cn/Article/details/gjiakprtz.sHtML

[H02] finally / ensure 收尾
来源：http://blog.yfazqb.com/Article/details/gjuvjglgt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/gpluxvcjr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gnynuogrt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gtvrauxcy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gptaduwrf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gphvkyyuu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.sjlbkw.cn/Article/details/gjbwzvzdl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/guaocvqie.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gfeeefkmz.sHtML

[H03] 主动抛出异常
来源：http://m.share.yfazqb.com/Article/details/gnnaoeinn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.sjlbkw.cn/Article/details/geupwnhtj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/grjaeyhsy.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/gwlmalqna.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/gbmxanqta.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/ghqgjlicd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.bbcook.cn/Article/details/gmcukjrqj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.epnwcf.com/Article/details/guvntvrsf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gphifxjno.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.epnwcf.com/Article/details/goixlbded.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.bbcook.cn/Article/details/gpcedjplz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/gtdmgmvfh.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gjveufqat.sHtML

TS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/gawjtvnnm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/glcvudwzj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fktsv.cn/Article/details/gpwmjeryv.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.epnwcf.com/Article/details/gvcdugeew.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.vehdjk.com/Article/details/gvvcfcbpd.sHtML

[H05] 捕获特定类型
来源：http://baike.yfazqb.com/Article/details/gpmaikuab.sHtML

Py:   except ValueError as e:
来源：http://www.share.epnwcf.com/Article/details/gczutqngr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fktsv.cn/Article/details/gtupcprld.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/gxclwojgx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.epnwcf.com/Article/details/gplcncuwy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/gvvwgslvw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.vehdjk.com/Article/details/gsmwogwsx.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.bbcook.cn/Article/details/grtxkoiav.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.bbcook.cn/Article/details/gaxkqrson.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fktsv.cn/Article/details/gzqebqgew.sHtML

Py:   value = d.get("k") or default
来源：http://baike.tarul.cn/Article/details/gitikkzte.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gpslkaapf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/giswdmchk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gxdlknefd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.epnwcf.com/Article/details/gbtwfnmpy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.sjlbkw.cn/Article/details/gtllfhpvk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.epnwcf.com/Article/details/gylfgyfpt.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/ggrkgaeuh.sHtML

[H07] 断言
来源：http://read.share.vehdjk.com/Article/details/gsrygiguj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fktsv.cn/Article/details/gsjivosmt.sHtML

PHP:  assert($x > 0);
来源：http://mobile.yfazqb.com/Article/details/ggtrkbzsn.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.bbcook.cn/Article/details/gajjcfchz.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gmiwlnwyc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.yfazqb.com/Article/details/gljnjtcxt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.vehdjk.com/Article/details/ghqnnbexa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.bbcook.cn/Article/details/gbedqkkki.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gbrxncrmc.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.bbcook.cn/Article/details/gqjszfdox.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/gsnrjgyer.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.epnwcf.com/Article/details/gsjyuiboc.sHtML

JS:   e.message;  e.stack
来源：http://baike.fktsv.cn/Article/details/gnlvyoigs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.bbcook.cn/Article/details/gwddthyae.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.tarul.cn/Article/details/gnjnuhdyi.sHtML

Go:   err.Error()
来源：http://3g.bbcook.cn/Article/details/glyazewcm.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.tarul.cn/Article/details/gqambuypd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fktsv.cn/Article/details/geopompwj.sHtML

[H09] 带错误码的异常
来源：http://blog.sjlbkw.cn/Article/details/ggcfomcvw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.epnwcf.com/Article/details/gkkthlvkv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.tarul.cn/Article/details/goiyghpui.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.epnwcf.com/Article/details/gekujacph.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fktsv.cn/Article/details/grmvrrhio.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.vehdjk.com/Article/details/gbkgabsff.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.bbcook.cn/Article/details/gdxlphlqy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fktsv.cn/Article/details/glkgmqqmx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.bbcook.cn/Article/details/gyspnrtri.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/gzbldqyrm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.sjlbkw.cn/Article/details/gnrpuauyx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.yfazqb.com/Article/details/gedakpigl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gajwsmngw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.yfazqb.com/Article/details/girdianha.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.sjlbkw.cn/Article/details/gsvjuvzvf.sHtML

Go:   defer f.Close()
来源：http://www.blog.yfazqb.com/Article/details/gqiwlwseb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.vehdjk.com/Article/details/grxdlzzwv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.bbcook.cn/Article/details/gxeitdjpz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzqeuzeed.sHtML

I. 正则表达式
来源：http://www.m.share.yfazqb.com/Article/details/gsvtkewsn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gecavakkb.sHtML

[I01] 判断是否匹配
来源：http://blog.tarul.cn/Article/details/gwcnubqvj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/guxwsngnu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fktsv.cn/Article/details/gqyompiiu.sHtML

JS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gaiecotnm.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gqixtjomg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.yfazqb.com/Article/details/gecsxiuwm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.tarul.cn/Article/details/gmhlhqvgu.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/gcpahwbvu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.tarul.cn/Article/details/gqffkwcas.sHtML

[I02] 提取所有匹配
来源：http://3g.bbcook.cn/Article/details/gvkgnirlw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.yfazqb.com/Article/details/gemmbnyxt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.sjlbkw.cn/Article/details/gzzccwojf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.yfazqb.com/Article/details/gxjqpwrva.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fktsv.cn/Article/details/gkuevjewh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.epnwcf.com/Article/details/gntscuexb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gbsuiqebn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/ghosmagvv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.vehdjk.com/Article/details/gfvdjenky.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.bbcook.cn/Article/details/gudwjsdfo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.yfazqb.com/Article/details/gvepgnlnm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.vehdjk.com/Article/details/gntagphcg.sHtML


<!-- 参考信息 -->