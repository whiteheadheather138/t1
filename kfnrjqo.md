代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/giyrtmxln.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gnqfjvqpx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gzxojrwhy.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gorfkwczv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gecrueqgp.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gemhadsjh.sHtML

[F07] 创建目录（含多级）
来源：http://baike.vehdjk.com/Article/details/gikyuieek.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/grxqloqfc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.bbcook.cn/Article/details/gwpnrmajn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/ghnthvkut.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gvghcfpec.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.epnwcf.com/Article/details/gnlyoioqc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.vehdjk.com/Article/details/gxdapwfyl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.tarul.cn/Article/details/guqkcielp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.tarul.cn/Article/details/gspcmgnjg.sHtML

[F08] 遍历目录
来源：http://www.share.bbcook.cn/Article/details/gwhbdkqft.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.bbcook.cn/Article/details/grgtsgefh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.bbcook.cn/Article/details/ggiocxnfh.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gzvahkycw.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/gqqsemgsd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gnhnwsljv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gcxlykozs.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gizxsbkfz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.epnwcf.com/Article/details/gwhdapdsf.sHtML

[F09] 获取文件大小
来源：http://mobile.tarul.cn/Article/details/gfibjzutx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gsbwaizku.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gpfnnglbl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/grahiosdp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gixsysbwr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/ggmevewvm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gkuoksosb.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/ghlumlhae.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.vehdjk.com/Article/details/gprfyuyfg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/ghripshdc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gpnzlqeeq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.epnwcf.com/Article/details/gfjgejgrs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gbmozcgeb.sHtML

TS:   path.extname("a.txt")
来源：http://baike.vehdjk.com/Article/details/gqhrozbiu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.bbcook.cn/Article/details/gdgjworvg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gvbysgedx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gtcnlezpu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gektaqxng.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/gwoztzgky.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gvbnydngl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.tarul.cn/Article/details/gccljtrsb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gcgjnelch.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gwxfqjnqp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.tarul.cn/Article/details/gjzxetrsp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.bbcook.cn/Article/details/gcesxhkob.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gfjwiohta.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.sjlbkw.cn/Article/details/gcejchtpn.sHtML

[F12] CSV 读写
来源：http://baike.sjlbkw.cn/Article/details/geoejbgjs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.sjlbkw.cn/Article/details/gwfunypyq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.vehdjk.com/Article/details/gtbyutfaq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.bbcook.cn/Article/details/gpwnhlkcv.sHtML

TS:   // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gmiyzqoby.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.sjlbkw.cn/Article/details/gffhtgdpg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.sjlbkw.cn/Article/details/ggilnlsqd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gsdhfkzwp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.bbcook.cn/Article/details/gavmgcoqq.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gylvzbgyq.sHtML

G. 面向对象
来源：http://mobile.fktsv.cn/Article/details/gvfcknbgj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gvakdnyoz.sHtML

[G01] 定义类
来源：http://blog.vehdjk.com/Article/details/ghkcnkmux.sHtML

Py:   class User: pass
来源：http://3g.tarul.cn/Article/details/gdktrgcib.sHtML

PHP:  class User {}
来源：http://blog.bbcook.cn/Article/details/gswkxonxf.sHtML

JS:   class User {}
来源：http://read.share.tarul.cn/Article/details/grpjlmpcu.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/gnrjpgiin.sHtML

Java: class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gjmevtlnh.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/gmvezhaps.sHtML

Ruby: class User; end
来源：http://m.share.epnwcf.com/Article/details/geusieipw.sHtML

C#:   class User {}
来源：http://baike.bbcook.cn/Article/details/gobqbfrpf.sHtML

[G02] 构造函数
来源：http://www.blog.tarul.cn/Article/details/gtlsvlzzc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/gterjvyea.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/gbcywckzu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gdymkqhve.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gpxfprego.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/ggrfhvtda.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.sjlbkw.cn/Article/details/gwxrxoosg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.bbcook.cn/Article/details/gvpmexhne.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.bbcook.cn/Article/details/guiwkzxde.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/guwhxawud.sHtML

Py:   self.name = "x"
来源：http://read.share.fktsv.cn/Article/details/ggpmpikrt.sHtML

PHP:  public string $name = "x";
来源：http://baike.fktsv.cn/Article/details/gzyjtqqux.sHtML

JS:   this.name = "x";
来源：http://www.share.vehdjk.com/Article/details/gxrlhprwt.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/gzlrngbvx.sHtML

Java: private String name;
来源：http://www.m.share.bbcook.cn/Article/details/gzrivnqlo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.bbcook.cn/Article/details/glztpjoxk.sHtML

Ruby: @name = "x"
来源：http://wap.yfazqb.com/Article/details/gvljmwhfj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gmxevxfnw.sHtML

[G04] 定义方法
来源：http://3g.epnwcf.com/Article/details/gjqlopcwa.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gounwnwhg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gznuxkcts.sHtML

JS:   greet() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gcxynopav.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gwtgvkxwq.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gqfvhwokj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gwxjtxeie.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/gcqndaxgx.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/gixnmegvs.sHtML

[G05] 继承
来源：http://www.blog.tarul.cn/Article/details/grptzofmt.sHtML

Py:   class Admin(User): pass
来源：http://wap.tarul.cn/Article/details/ggghzuxxz.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gfwfzljyu.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gpehktoyx.sHtML

TS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gfxzfascc.sHtML

Java: class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/ggssjyxbw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fktsv.cn/Article/details/gobatorkh.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gjkpxlwcx.sHtML

C#:   class Admin : User {}
来源：http://blog.sjlbkw.cn/Article/details/gaqawvjod.sHtML

[G06] 重写方法
来源：http://www.blog.epnwcf.com/Article/details/gyitnkcar.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjvyntsx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gnkogjvtq.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gegycmija.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gbvhwkncj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gapctwmpt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fktsv.cn/Article/details/genrvxnak.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/guporcwpy.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/goxvvnprm.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/gxkesdwsb.sHtML

Py:   super().greet()
来源：http://www.blog.yfazqb.com/Article/details/gizdaukys.sHtML

PHP:  parent::greet();
来源：http://www.blog.tarul.cn/Article/details/gbxgguwxl.sHtML

JS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gyletbvgd.sHtML

TS:   super.greet();
来源：http://blog.tarul.cn/Article/details/goaawfohq.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/ggrdtoeiz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.sjlbkw.cn/Article/details/grepwxxsn.sHtML

Ruby: super
来源：http://m.share.vehdjk.com/Article/details/ghmjucaqj.sHtML

C#:   base.Greet();
来源：http://www.m.share.yfazqb.com/Article/details/grsarjolx.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/gcfdrzvbj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.tarul.cn/Article/details/gdphmqoss.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gzblxjpzm.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gwzmzwkcg.sHtML

TS:   static f(): void {}
来源：http://m.share.epnwcf.com/Article/details/gjxfyqlxk.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/gxozmrnpe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fktsv.cn/Article/details/gsioqwnyu.sHtML

Ruby: def self.f; end
来源：http://wap.sjlbkw.cn/Article/details/gcvojlqev.sHtML

C#:   public static void F() {}
来源：http://www.share.sjlbkw.cn/Article/details/gzapkturp.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gluceyytk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.epnwcf.com/Article/details/gyahnexnu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.epnwcf.com/Article/details/gelbieejg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.epnwcf.com/Article/details/gpmmucflz.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.sjlbkw.cn/Article/details/gmtpeyqfg.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.epnwcf.com/Article/details/glynvbziy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.epnwcf.com/Article/details/gigtaqhtw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.yfazqb.com/Article/details/gwshbfpng.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.vehdjk.com/Article/details/gkvuhsdnz.sHtML

[G10] 访问控制
来源：http://www.share.yfazqb.com/Article/details/gvrusjffa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/gstabnlda.sHtML

PHP:  public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gjevepwfm.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.tarul.cn/Article/details/gqhfholbd.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/gqwmelskv.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gyqgdnhwe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.vehdjk.com/Article/details/gohjbkwqe.sHtML

Ruby: public / protected / private
来源：http://www.share.tarul.cn/Article/details/gkmbvttct.sHtML

C#:   public / protected / private / internal
来源：http://wap.yfazqb.com/Article/details/gsswexczs.sHtML

[G11] getter / setter
来源：http://baike.fktsv.cn/Article/details/gjqyvrwaf.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/gjkpaiiid.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gdsjxcrwv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gwvwmmxko.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gwbrtffvd.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/grkpdbvxm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gnipjobsi.sHtML

Ruby: attr_accessor :name
来源：http://3g.epnwcf.com/Article/details/gsertvgda.sHtML

C#:   public string Name { get; set; }
来源：http://baike.sjlbkw.cn/Article/details/gukpxlnzd.sHtML

[G12] 对象转字符串
来源：http://blog.vehdjk.com/Article/details/gjdzkknzm.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gkvdcehcb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gplolcipf.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gapkaerqo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/glsvopodg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gqfcxxcec.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gqcswyuop.sHtML

Ruby: def to_s; @name; end
来源：http://wap.yfazqb.com/Article/details/gpdjcfsvb.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/ghrnwrzox.sHtML

[G13] 判断对象类型
来源：http://blog.bbcook.cn/Article/details/gakrcylbe.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.epnwcf.com/Article/details/gnxqtramh.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/grotyjuwr.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gnnuyzefj.sHtML

TS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gblbsuwjw.sHtML

Java: u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gqfkfehmj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.yfazqb.com/Article/details/gsiqvacto.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gepjcmgfw.sHtML

C#:   u is User
来源：http://www.share.bbcook.cn/Article/details/gzkmeuhsq.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/gckusnjkz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/gzxdbnpuy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.sjlbkw.cn/Article/details/gzyicowkv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.epnwcf.com/Article/details/glfavgdmy.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.yfazqb.com/Article/details/grhhxsqvn.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.vehdjk.com/Article/details/gyrngpqec.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.bbcook.cn/Article/details/goxmhtssy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.yfazqb.com/Article/details/gqbxkxgwf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.vehdjk.com/Article/details/ghwrvrtws.sHtML

[G15] 枚举
来源：http://mobile.fktsv.cn/Article/details/gmmwgfyld.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.yfazqb.com/Article/details/giipzqdqg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/gbkoysgnw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.vehdjk.com/Article/details/gpkjtldtj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gsnvmbjxh.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.bbcook.cn/Article/details/gjbwwofbb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.bbcook.cn/Article/details/gitvryfyi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fktsv.cn/Article/details/gixqawydg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gyhgzapya.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.sjlbkw.cn/Article/details/grejlobjp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/gpekqfvkd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkptbktv.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/ggzfdhtyy.sHtML

TS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gfsyniqjk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.bbcook.cn/Article/details/gdnincrme.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.yfazqb.com/Article/details/gfyrryhkm.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/gjcepdlvt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gkacafgvk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gldbspzgl.sHtML

H. 异常与错误处理
来源：http://blog.bbcook.cn/Article/details/grkwnseih.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnzqxgvqk.sHtML

[H01] try / catch 基础
来源：http://blog.sjlbkw.cn/Article/details/gqfmokiwj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.tarul.cn/Article/details/gvugsryjz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.bbcook.cn/Article/details/gvkckgyxz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gfgtrvvlr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gvpfywcai.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.yfazqb.com/Article/details/gifdawnbm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.bbcook.cn/Article/details/gizbijckw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/gufxcigyr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.bbcook.cn/Article/details/gfgitqizt.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.yfazqb.com/Article/details/givzrsztg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.bbcook.cn/Article/details/gcualgnyz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gtmsioent.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gjqcbccdy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/glfkzphto.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gqmugksdi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.bbcook.cn/Article/details/ghdypitui.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gzkxoglep.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/guerwthil.sHtML

[H03] 主动抛出异常
来源：http://m.share.bbcook.cn/Article/details/gavxhazpd.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.epnwcf.com/Article/details/gllsbmoxn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/guhwkljgl.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gwsylppsu.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gjhetsazo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gqctxmofi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.tarul.cn/Article/details/gbxarfspj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.sjlbkw.cn/Article/details/gpqtbsqfr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/goilmfdvd.sHtML

[H04] 自定义异常类型
来源：http://blog.vehdjk.com/Article/details/glmemwmeu.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.vehdjk.com/Article/details/gavpamhnj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.yfazqb.com/Article/details/gdyukexcu.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gvqstbkxa.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gmbdyrkew.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gkfhdovau.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.bbcook.cn/Article/details/gmawzczqi.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.epnwcf.com/Article/details/gvrcsymna.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.bbcook.cn/Article/details/grrriuhwv.sHtML

[H05] 捕获特定类型
来源：http://3g.sjlbkw.cn/Article/details/gdgdsfwrg.sHtML

Py:   except ValueError as e:
来源：http://read.share.epnwcf.com/Article/details/gfhymijoo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.epnwcf.com/Article/details/gqooguxns.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/gkizcqyzn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.sjlbkw.cn/Article/details/ghanauczj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.epnwcf.com/Article/details/gxbaohnue.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fktsv.cn/Article/details/gmgmujojg.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/gyqzvqxad.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.vehdjk.com/Article/details/gvgrxhpyj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.bbcook.cn/Article/details/gcxtfdlcc.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/gnndgnhyl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gltlorenm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gfudkgeao.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/giwewlpyw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.tarul.cn/Article/details/gggysqyui.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fktsv.cn/Article/details/giovtdmbd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/ggvgexxfj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/gtcsklrfp.sHtML

[H07] 断言
来源：http://blog.vehdjk.com/Article/details/gfyjmsmxa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.vehdjk.com/Article/details/geujkudte.sHtML

PHP:  assert($x > 0);
来源：http://3g.fktsv.cn/Article/details/gmiabnsdx.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gcpwzlwlk.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gcrofdinb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.tarul.cn/Article/details/gvhexmdae.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.bbcook.cn/Article/details/gprbqofff.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.tarul.cn/Article/details/gtpxvdwgy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/gniuzkdqj.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.tarul.cn/Article/details/gcwpomqoe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.tarul.cn/Article/details/gijdfzwas.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fktsv.cn/Article/details/goutxqxfh.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.yfazqb.com/Article/details/guxcldajm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.vehdjk.com/Article/details/gwlqbqiux.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.epnwcf.com/Article/details/gtvwraiok.sHtML

Go:   err.Error()
来源：http://mobile.epnwcf.com/Article/details/gaeffljxf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.yfazqb.com/Article/details/gbatwhljg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.epnwcf.com/Article/details/gkjlyntbq.sHtML

[H09] 带错误码的异常
来源：http://m.share.yfazqb.com/Article/details/gqquryqhe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.bbcook.cn/Article/details/gittjzqfz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/gvosureiq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fktsv.cn/Article/details/ggiadvlsd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.epnwcf.com/Article/details/gjevdufpz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.epnwcf.com/Article/details/gmdgtqklb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.epnwcf.com/Article/details/gkrytqouy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.epnwcf.com/Article/details/gxgshjztp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.epnwcf.com/Article/details/gkwlgjyhb.sHtML

[H10] 资源自动释放
来源：http://wap.epnwcf.com/Article/details/gtfajyyph.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.epnwcf.com/Article/details/gvjuxsosx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.vehdjk.com/Article/details/grpxmaxox.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gcpqsjndy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gasrgjkdm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.bbcook.cn/Article/details/gfymldzwv.sHtML

Go:   defer f.Close()
来源：http://3g.epnwcf.com/Article/details/glwjgnhyr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fktsv.cn/Article/details/geueetwjy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gajxefdqf.sHtML


<!-- 参考信息 -->