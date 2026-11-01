代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.vehdjk.com/Article/details/gyxdwzwli.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/glwgtdzrl.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gdqhtwzwg.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gzuozwjdg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gaxcjngvu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.bbcook.cn/Article/details/gwersgyqn.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gdojhhhcx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gewmoyqcq.sHtML

[F09] 获取文件大小
来源：http://www.m.share.vehdjk.com/Article/details/ghzppsqau.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gncjipihj.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gdogleyhz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gbwbuhexf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gqwhssjql.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gxxfmknfc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.yfazqb.com/Article/details/gkbtppidk.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fktsv.cn/Article/details/gpptctkcw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.vehdjk.com/Article/details/gykyapbwt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fktsv.cn/Article/details/gyfaixlbv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gclpppwgr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fktsv.cn/Article/details/gksofomyq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gquxkxwhb.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/gjqbvqmph.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.epnwcf.com/Article/details/gndcsxgxu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/ggylqnwrv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gpcjlxayx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/giqsobzgv.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.epnwcf.com/Article/details/gqrsvkfub.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/glthohckt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gtctalhxs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/ghgryxsuo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gvbvovcut.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.yfazqb.com/Article/details/gutfjjwrd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.sjlbkw.cn/Article/details/gsfiotkoy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gupeqdjsq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.yfazqb.com/Article/details/godvccteb.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gleremrpn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.epnwcf.com/Article/details/gstuuzodg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.vehdjk.com/Article/details/govwuhgnz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.tarul.cn/Article/details/gofkeehhm.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/gtujxawwf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.vehdjk.com/Article/details/gzzaojume.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.bbcook.cn/Article/details/gijmepuvf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.tarul.cn/Article/details/gkyrohkrh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fktsv.cn/Article/details/gkgkwmjww.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gktaawwoa.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/gtaetvazw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnoscngub.sHtML

[G01] 定义类
来源：http://mobile.vehdjk.com/Article/details/gfzawzbkh.sHtML

Py:   class User: pass
来源：http://www.m.share.yfazqb.com/Article/details/gmvwfaift.sHtML

PHP:  class User {}
来源：http://blog.sjlbkw.cn/Article/details/gukrirypj.sHtML

JS:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gnkvrlmji.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/gzxnpupvc.sHtML

Java: class User {}
来源：http://mobile.tarul.cn/Article/details/ggcbbxqqc.sHtML

Go:   type User struct { Name string }
来源：http://m.share.epnwcf.com/Article/details/gqiueymmu.sHtML

Ruby: class User; end
来源：http://www.m.share.bbcook.cn/Article/details/gxwbpfmum.sHtML

C#:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gaulnzhwh.sHtML

[G02] 构造函数
来源：http://wap.bbcook.cn/Article/details/gtmglmtqz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fktsv.cn/Article/details/gyejpitrr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.yfazqb.com/Article/details/gjlsakjur.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gkqxgksvg.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.sjlbkw.cn/Article/details/grwxrhukb.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gzxlpaoso.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.tarul.cn/Article/details/gqthvirev.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.bbcook.cn/Article/details/gncesyqna.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fktsv.cn/Article/details/gplwwfepo.sHtML

[G03] 实例属性
来源：http://3g.yfazqb.com/Article/details/ghcrlyhku.sHtML

Py:   self.name = "x"
来源：http://3g.fktsv.cn/Article/details/gkcsgucvg.sHtML

PHP:  public string $name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gzhzhwhfp.sHtML

JS:   this.name = "x";
来源：http://3g.yfazqb.com/Article/details/gvimmnbvk.sHtML

TS:   name: string = "x";
来源：http://www.m.share.tarul.cn/Article/details/gokkdmswv.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/gouwblsys.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.tarul.cn/Article/details/gszdkfreb.sHtML

Ruby: @name = "x"
来源：http://mobile.tarul.cn/Article/details/grdvxcbea.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gicdruotz.sHtML

[G04] 定义方法
来源：http://www.share.bbcook.cn/Article/details/gyysuvdzu.sHtML

Py:   def greet(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gludgpkyz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gaemmxmuk.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/giylynytz.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/ggvyiipnr.sHtML

Java: String greet() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gcgpyjvgw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gvnwadgdt.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gkuhtnena.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.tarul.cn/Article/details/gjrlamsrr.sHtML

[G05] 继承
来源：http://www.blog.tarul.cn/Article/details/gwwarsiyw.sHtML

Py:   class Admin(User): pass
来源：http://read.share.tarul.cn/Article/details/ggtdluaik.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gychnbqqe.sHtML

JS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gqoiyhwpi.sHtML

TS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gxstwvrkn.sHtML

Java: class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gztvfznve.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gorbgoxxe.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.yfazqb.com/Article/details/ghihvdebd.sHtML

C#:   class Admin : User {}
来源：http://www.blog.vehdjk.com/Article/details/gpjupmjpq.sHtML

[G06] 重写方法
来源：http://3g.sjlbkw.cn/Article/details/ghmebsutx.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/gpfiqefsn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gbefspdwn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gnxbwksdz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gdcethngv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gpfguxxcb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.epnwcf.com/Article/details/gazddqgov.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.epnwcf.com/Article/details/gnvfzblzg.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gmvbwfidg.sHtML

[G07] 调用父类方法
来源：http://3g.fktsv.cn/Article/details/gcoytygcy.sHtML

Py:   super().greet()
来源：http://baike.epnwcf.com/Article/details/gouzruakb.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/gjcywrfqe.sHtML

JS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/grjcejwxj.sHtML

TS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/grzuciaxj.sHtML

Java: super.greet();
来源：http://wap.sjlbkw.cn/Article/details/ggaxpntyq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.bbcook.cn/Article/details/gxjnmveiq.sHtML

Ruby: super
来源：http://mobile.bbcook.cn/Article/details/gvfamlwkb.sHtML

C#:   base.Greet();
来源：http://www.blog.bbcook.cn/Article/details/gpgmplgcn.sHtML

[G08] 静态方法与属性
来源：http://blog.tarul.cn/Article/details/guzocrdxl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.tarul.cn/Article/details/gjbrcwzwt.sHtML

PHP:  public static function f() {}
来源：http://www.blog.tarul.cn/Article/details/gvittvbym.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/ggueqaeno.sHtML

TS:   static f(): void {}
来源：http://www.blog.fktsv.cn/Article/details/goilihtrh.sHtML

Java: static void f() {}
来源：http://www.blog.yfazqb.com/Article/details/givlbwygz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fktsv.cn/Article/details/gclaoaxwg.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gkrqpufjl.sHtML

C#:   public static void F() {}
来源：http://3g.sjlbkw.cn/Article/details/gnysibpze.sHtML

[G09] 接口 / 抽象类
来源：http://wap.tarul.cn/Article/details/gcwtodimc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.bbcook.cn/Article/details/gbcfgwlsw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/geclrfzcm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gyjcnuvzp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.vehdjk.com/Article/details/gzskuvuwi.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.bbcook.cn/Article/details/gdagafhjx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gzhyxoeui.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.sjlbkw.cn/Article/details/glunycvky.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.tarul.cn/Article/details/gqcclmqus.sHtML

[G10] 访问控制
来源：http://blog.epnwcf.com/Article/details/girlocwau.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/galsqulye.sHtML

PHP:  public / protected / private
来源：http://m.share.tarul.cn/Article/details/ghtokkkxc.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/gksaewdgv.sHtML

TS:   public / protected / private
来源：http://wap.bbcook.cn/Article/details/gjwpmzkua.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.bbcook.cn/Article/details/gxmkzfgyl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.yfazqb.com/Article/details/gkipeinqx.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gpntrlcof.sHtML

C#:   public / protected / private / internal
来源：http://wap.epnwcf.com/Article/details/gsthjbiwl.sHtML

[G11] getter / setter
来源：http://3g.yfazqb.com/Article/details/gytagmkyq.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.epnwcf.com/Article/details/gbdhxogfd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/genagmesp.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gtamrufvu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gppkegpnw.sHtML

Java: public String getName() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gmwgoylsd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gzgvjroie.sHtML

Ruby: attr_accessor :name
来源：http://www.share.vehdjk.com/Article/details/gjaejbmdc.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/gnoujwfsj.sHtML

[G12] 对象转字符串
来源：http://blog.sjlbkw.cn/Article/details/gljlmljtk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyrltovj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gtzpweelp.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gbfjszsuq.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gebwqriiy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/giggylfnz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gcysdqcrh.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/gkitducjs.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/glronyiok.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gjnsvewki.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.yfazqb.com/Article/details/grfbhwqnz.sHtML

PHP:  $u instanceof User
来源：http://blog.vehdjk.com/Article/details/gmqjzkanb.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gwjwygzuq.sHtML

TS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gjcalixvh.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gaqozofit.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fktsv.cn/Article/details/gnoiilrzm.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.tarul.cn/Article/details/gglxzxhac.sHtML

C#:   u is User
来源：http://www.share.fktsv.cn/Article/details/ggikjxssk.sHtML

[G14] 数据类 / record
来源：http://wap.fktsv.cn/Article/details/gozoppiyo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.sjlbkw.cn/Article/details/gfrgeacpn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/gtxyzqatk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fktsv.cn/Article/details/gsmxbrlec.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.sjlbkw.cn/Article/details/gpftnhqjy.sHtML

Java: record User(String name, int age) {}
来源：http://3g.vehdjk.com/Article/details/gyzimzchr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/ggxgxabla.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fktsv.cn/Article/details/gvsdxlvpc.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fktsv.cn/Article/details/grhcdtgjc.sHtML

[G15] 枚举
来源：http://3g.yfazqb.com/Article/details/gescmqxkl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/gvkapplvm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.epnwcf.com/Article/details/gnilalqdk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.vehdjk.com/Article/details/gnyqcjrpk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gkrtlhmio.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/gjqiwrhvu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.bbcook.cn/Article/details/gpujllozz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.epnwcf.com/Article/details/glyjaabov.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gvebotfen.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fktsv.cn/Article/details/gxbuuiaud.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.sjlbkw.cn/Article/details/gwjyzoihc.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.vehdjk.com/Article/details/gcnlhooyp.sHtML

JS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gpheoxuxz.sHtML

TS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gzvpukjeg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/gxneiszlb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/goznttvwz.sHtML

Ruby: obj.instance_variables
来源：http://read.share.epnwcf.com/Article/details/gqtnumber.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gsjuxykti.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gsgufwdtu.sHtML

H. 异常与错误处理
来源：http://www.blog.yfazqb.com/Article/details/gscbfyjqf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtqepfwok.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/gcwidnreo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.vehdjk.com/Article/details/gbgyovdxc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/gdlkkbcme.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gksdokihs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gynwwqtye.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.tarul.cn/Article/details/gbccpouyn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/gwnvuqrwn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/goxnbkwax.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.sjlbkw.cn/Article/details/gogxlrkcy.sHtML

[H02] finally / ensure 收尾
来源：http://blog.vehdjk.com/Article/details/gisioqjgp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.bbcook.cn/Article/details/ggykcmzpa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/goirpxlkz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gtmqgddiq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gllaprtla.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gwyooihqb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.epnwcf.com/Article/details/gshcmorcj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.bbcook.cn/Article/details/gktrwlwoi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gzhgsbsth.sHtML

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/gpxytnrbh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gshsydgew.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gzvcrpyfb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gkhmdqrwv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/glwkkcymz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gnhzozkpu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/gyzszgyiz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.sjlbkw.cn/Article/details/gkluehdmm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gaysemkvy.sHtML

[H04] 自定义异常类型
来源：http://mobile.vehdjk.com/Article/details/ghtgovkmg.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.sjlbkw.cn/Article/details/gyyfrauwl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/ggmwdczlw.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gfvqdlsga.sHtML

TS:   class MyError extends Error {}
来源：http://3g.epnwcf.com/Article/details/gkxxnlrso.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/ghxwxenly.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/gcfinyhga.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fktsv.cn/Article/details/gfzvswost.sHtML

C#:   class MyException : Exception {}
来源：http://3g.vehdjk.com/Article/details/gqvbisxjf.sHtML

[H05] 捕获特定类型
来源：http://3g.epnwcf.com/Article/details/gjxuhvydd.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/glbybtizl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/gvraubfqc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/goggtccly.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/glfofyzxu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.vehdjk.com/Article/details/gwcjiuqjc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.bbcook.cn/Article/details/gthhfkjxs.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.vehdjk.com/Article/details/gvkfgppsv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.epnwcf.com/Article/details/gsmjlvupb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fktsv.cn/Article/details/griuaateu.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fktsv.cn/Article/details/gmcgigkxq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/gswysqcdg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gjiyedsxl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/gjjkklvbf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.yfazqb.com/Article/details/gjxgdimnc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.sjlbkw.cn/Article/details/grufsaiov.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fktsv.cn/Article/details/gqlhplqot.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/gqfoajnza.sHtML

[H07] 断言
来源：http://www.blog.epnwcf.com/Article/details/gmydbeikx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.epnwcf.com/Article/details/gkbsxjxae.sHtML

PHP:  assert($x > 0);
来源：http://www.share.bbcook.cn/Article/details/gvkccbxgo.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/ggycbswiu.sHtML

TS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gshqfxyxx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.epnwcf.com/Article/details/goyjgyrjk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.sjlbkw.cn/Article/details/gxndygtrc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.vehdjk.com/Article/details/gqhadujyp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gfrdzdlzq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.bbcook.cn/Article/details/gagmcugfn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/guzzpsgmu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.tarul.cn/Article/details/gxdqfjfds.sHtML

JS:   e.message;  e.stack
来源：http://blog.sjlbkw.cn/Article/details/gkthcubsm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.yfazqb.com/Article/details/gzsvqsixu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.yfazqb.com/Article/details/gsksqzoay.sHtML

Go:   err.Error()
来源：http://www.share.yfazqb.com/Article/details/gbfzbthlt.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.yfazqb.com/Article/details/gsikfxyxv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fktsv.cn/Article/details/gajzsniua.sHtML

[H09] 带错误码的异常
来源：http://mobile.sjlbkw.cn/Article/details/gvbgdnvar.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/gdhfpobof.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.epnwcf.com/Article/details/gzvubsjaa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.yfazqb.com/Article/details/gvkwjfzkt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fktsv.cn/Article/details/gjeqntpuh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.sjlbkw.cn/Article/details/ggvexdxwe.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.sjlbkw.cn/Article/details/gzhlnmxhs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gqnkxxvzq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fktsv.cn/Article/details/gvqlaxioh.sHtML

[H10] 资源自动释放
来源：http://baike.yfazqb.com/Article/details/gjcmbwvwe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.tarul.cn/Article/details/gpizfockv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.epnwcf.com/Article/details/grlrhojgi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.tarul.cn/Article/details/gurzyqmkk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.vehdjk.com/Article/details/glemjgdbo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/gslnthcsr.sHtML

Go:   defer f.Close()
来源：http://mobile.tarul.cn/Article/details/guagzsvcf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.yfazqb.com/Article/details/gkhnvgqfv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/grnymozwz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gbawwdrmj.sHtML

I. 正则表达式
来源：http://m.share.yfazqb.com/Article/details/gsyriawuc.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqvaplwgs.sHtML

[I01] 判断是否匹配
来源：http://www.share.bbcook.cn/Article/details/gzvbdddxq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.epnwcf.com/Article/details/glnoambqy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gemqrodcm.sHtML

JS:   /\d+/.test(s)
来源：http://blog.sjlbkw.cn/Article/details/ggycicfwv.sHtML

TS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gbetxzygs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.tarul.cn/Article/details/gddwwqnkf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gerkvduia.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gvbqmqsad.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.epnwcf.com/Article/details/ggkspgdid.sHtML

[I02] 提取所有匹配
来源：http://baike.bbcook.cn/Article/details/gqxqdoekc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.vehdjk.com/Article/details/gqubyhtgi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gaqmvvcfm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fktsv.cn/Article/details/gjeomsppw.sHtML


<!-- 参考信息 -->