代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/gvwhfxhki.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gmvjjsimv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gpxvmgoje.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.yfazqb.com/Article/details/gkrqqbpmz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.vehdjk.com/Article/details/gnpvwvgeg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.epnwcf.com/Article/details/gloxgjwsk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.vehdjk.com/Article/details/grzyseaxk.sHtML

[F08] 遍历目录
来源：http://www.blog.vehdjk.com/Article/details/gmutlneba.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.epnwcf.com/Article/details/gjzezrqkw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.vehdjk.com/Article/details/gszwuvioe.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/gtfyularx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gfkzfygjf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/gesdpavop.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.epnwcf.com/Article/details/gzmcjeznu.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.sjlbkw.cn/Article/details/guuashkah.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.yfazqb.com/Article/details/gncoicxcb.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/glkfqcdxg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gprgtclbg.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gomvwfblp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gymbmltld.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gjroabooz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/glddtioch.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fktsv.cn/Article/details/guhqmpqqa.sHtML

Ruby: File.size("a.txt")
来源：http://blog.tarul.cn/Article/details/gijymosjf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.bbcook.cn/Article/details/ghwahbyzj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gyiqsgjrv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gngybtgjg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fktsv.cn/Article/details/guxlvotbx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/govnjpjhb.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gineimuxg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.vehdjk.com/Article/details/gpjbpkokq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gifwcslnq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gcjgpdqxw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gosgheksx.sHtML

[F11] 复制与移动文件
来源：http://blog.tarul.cn/Article/details/gkvuigkyi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gubgzmhxa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/ggigtfqnr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gqrgmvcvv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gzolfpgoj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.epnwcf.com/Article/details/gzscpksyz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.epnwcf.com/Article/details/gkvqbjatk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gnewsmgdo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.yfazqb.com/Article/details/gajkybnkh.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/gglougsjm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.tarul.cn/Article/details/gefpbhykj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.yfazqb.com/Article/details/grdvsltcz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/gieibyhhz.sHtML

TS:   // 同上
来源：http://read.share.fktsv.cn/Article/details/gjtpjviqe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.vehdjk.com/Article/details/giakafixo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fktsv.cn/Article/details/gazcwfjja.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.bbcook.cn/Article/details/gibkiipou.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.epnwcf.com/Article/details/gtjjplufl.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvqazgmpm.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/gjqcjigbk.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/guklmxavq.sHtML

[G01] 定义类
来源：http://www.blog.epnwcf.com/Article/details/gznxqvjvq.sHtML

Py:   class User: pass
来源：http://read.share.bbcook.cn/Article/details/grhzcrdog.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/guwnmfvli.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gujtmrhvh.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.sjlbkw.cn/Article/details/gwqqlsecg.sHtML

Java: class User {}
来源：http://www.blog.fktsv.cn/Article/details/gvkfkkxaq.sHtML

Go:   type User struct { Name string }
来源：http://blog.tarul.cn/Article/details/gsjeayujc.sHtML

Ruby: class User; end
来源：http://blog.vehdjk.com/Article/details/glnebaurw.sHtML

C#:   class User {}
来源：http://wap.fktsv.cn/Article/details/ginspscob.sHtML

[G02] 构造函数
来源：http://www.blog.epnwcf.com/Article/details/goghckcdc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.vehdjk.com/Article/details/gbcyamqbd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/ghxcmyeqv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gxafcohbi.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.tarul.cn/Article/details/gojwvuzhi.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gwfqpcjex.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/goptggjka.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.tarul.cn/Article/details/grgtylhdy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.yfazqb.com/Article/details/gkbuljtwz.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/gnipsjdxn.sHtML

Py:   self.name = "x"
来源：http://wap.tarul.cn/Article/details/ghucbuheq.sHtML

PHP:  public string $name = "x";
来源：http://3g.yfazqb.com/Article/details/gfpxsclxy.sHtML

JS:   this.name = "x";
来源：http://read.share.epnwcf.com/Article/details/gceccqmlj.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/gyvlxazfk.sHtML

Java: private String name;
来源：http://blog.tarul.cn/Article/details/gmubnqbhb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.yfazqb.com/Article/details/gxzwuafuz.sHtML

Ruby: @name = "x"
来源：http://m.share.vehdjk.com/Article/details/ghjeqbabj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gunefvuqq.sHtML

[G04] 定义方法
来源：http://read.share.epnwcf.com/Article/details/gdrfgmcgt.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gapoalhhd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/geoiqztuy.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gztbxhase.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/grigjomur.sHtML

Java: String greet() { return name; }
来源：http://m.share.tarul.cn/Article/details/gmzwsavkt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gcqyjdbwk.sHtML

Ruby: def greet; @name; end
来源：http://www.share.epnwcf.com/Article/details/gjwnaneud.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gpotrtgyk.sHtML

[G05] 继承
来源：http://blog.yfazqb.com/Article/details/grqwtfvau.sHtML

Py:   class Admin(User): pass
来源：http://www.share.epnwcf.com/Article/details/gowthltvm.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gvprgecbf.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gztpqffyn.sHtML

TS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gtueeudlw.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/geqbewiyk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gpcxpjkvl.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gycnmvsbh.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/gdbscyngp.sHtML

[G06] 重写方法
来源：http://blog.tarul.cn/Article/details/gxagrgawo.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/gcwrsjudt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gdyrxtfgp.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gvmxqgyml.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gkmwrlxfx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gnbslmhoa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fktsv.cn/Article/details/goqiitvth.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.yfazqb.com/Article/details/gqvzkirfz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fktsv.cn/Article/details/gyulhtqka.sHtML

[G07] 调用父类方法
来源：http://3g.yfazqb.com/Article/details/gsdkjwzyx.sHtML

Py:   super().greet()
来源：http://www.share.epnwcf.com/Article/details/gfsjwjina.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gwzzolkgx.sHtML

JS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gxjmrljcq.sHtML

TS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gxltynhqr.sHtML

Java: super.greet();
来源：http://www.share.fktsv.cn/Article/details/gkipsptvf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/gskillpys.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gzdemufvi.sHtML

C#:   base.Greet();
来源：http://www.share.tarul.cn/Article/details/goqmwdbjf.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/gxhoblqxi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.bbcook.cn/Article/details/gpgnygubd.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gqypioghl.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gncgqhedx.sHtML

TS:   static f(): void {}
来源：http://m.share.bbcook.cn/Article/details/gdpuxvczt.sHtML

Java: static void f() {}
来源：http://baike.yfazqb.com/Article/details/gdmulbrgu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.sjlbkw.cn/Article/details/gyyruagwb.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fktsv.cn/Article/details/gtzuunitv.sHtML

C#:   public static void F() {}
来源：http://m.share.tarul.cn/Article/details/gdrbquhak.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.tarul.cn/Article/details/ghddpdbju.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.vehdjk.com/Article/details/gnonfzuzv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.vehdjk.com/Article/details/gfgpoazbx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fktsv.cn/Article/details/guvpswwgx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.vehdjk.com/Article/details/gpvvcewqx.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/gbuhjaleh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fktsv.cn/Article/details/giznfzzvs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/gnqcrxyir.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.epnwcf.com/Article/details/gtnjlzqhi.sHtML

[G10] 访问控制
来源：http://mobile.vehdjk.com/Article/details/gctybonqe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.sjlbkw.cn/Article/details/geadtiqrr.sHtML

PHP:  public / protected / private
来源：http://m.share.epnwcf.com/Article/details/ggmwqjwdi.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.epnwcf.com/Article/details/gbghauyjf.sHtML

TS:   public / protected / private
来源：http://wap.yfazqb.com/Article/details/gbhisuael.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fktsv.cn/Article/details/glxfbcocy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.epnwcf.com/Article/details/ginyozjdv.sHtML

Ruby: public / protected / private
来源：http://3g.yfazqb.com/Article/details/gkgtigjko.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.vehdjk.com/Article/details/gyvinuvgq.sHtML

[G11] getter / setter
来源：http://baike.sjlbkw.cn/Article/details/gtngdxjxu.sHtML

Py:   @property 与 @x.setter
来源：http://3g.tarul.cn/Article/details/gpczsowki.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gdqkjkgop.sHtML

JS:   get name() { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gdcovewek.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gennjspyy.sHtML

Java: public String getName() { return name; }
来源：http://3g.yfazqb.com/Article/details/guqntxnmk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gpzqfhtou.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/gsqzqqfbx.sHtML

C#:   public string Name { get; set; }
来源：http://blog.sjlbkw.cn/Article/details/gfucptwqe.sHtML

[G12] 对象转字符串
来源：http://wap.epnwcf.com/Article/details/gdofrpycn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/guqiacxhg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gprngxqcd.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gzojjdijk.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gddcamyvi.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gbtrmkncy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gzansikwp.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.epnwcf.com/Article/details/gqrhhkipu.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gmqyfgrio.sHtML

[G13] 判断对象类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhhhdyxw.sHtML

Py:   isinstance(u, User)
来源：http://blog.fktsv.cn/Article/details/gqomxcqoy.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/grxmtlnsn.sHtML

JS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/glstokgmd.sHtML

TS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gvpfklyfw.sHtML

Java: u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gyarvthih.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.yfazqb.com/Article/details/ggpjxlkqn.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/gtmuujplx.sHtML

C#:   u is User
来源：http://baike.sjlbkw.cn/Article/details/gowifeupa.sHtML

[G14] 数据类 / record
来源：http://www.blog.sjlbkw.cn/Article/details/glxwgwneg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/gdhaswkum.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gvjguuxqq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.vehdjk.com/Article/details/gvranixlg.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.vehdjk.com/Article/details/gacolczyv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.bbcook.cn/Article/details/gkguntozb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.tarul.cn/Article/details/ghxegomkk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/gscztmdor.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/geowovchn.sHtML

[G15] 枚举
来源：http://www.share.bbcook.cn/Article/details/gbqyhgmgt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/gqedswnof.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.vehdjk.com/Article/details/gotmrghmr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fktsv.cn/Article/details/glwozvywm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gtcozwykw.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.bbcook.cn/Article/details/gkriynzwu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.sjlbkw.cn/Article/details/gfqjpigks.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.tarul.cn/Article/details/gfdiuhmcu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gbrjmytuh.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.tarul.cn/Article/details/gxrxczhnc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/grbcmolfk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.epnwcf.com/Article/details/gsjwaamzx.sHtML

JS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gylennwyj.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/glpqyouda.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.bbcook.cn/Article/details/gmqkglcgm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.epnwcf.com/Article/details/glarryiou.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.bbcook.cn/Article/details/giivmupee.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gzhbbmshc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gelvxpkls.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/gzohcjkrm.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvcytlfej.sHtML

[H01] try / catch 基础
来源：http://www.share.bbcook.cn/Article/details/gcqbjizmx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.epnwcf.com/Article/details/gmvhpawrr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/gebzlqscw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gnzqqspzv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gtcdusfzu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.tarul.cn/Article/details/gngipavzq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.sjlbkw.cn/Article/details/gzcominpy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/gurizbwvy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.tarul.cn/Article/details/gnoogmtpm.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/gqyrsbqnd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.epnwcf.com/Article/details/gvpugenjp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/geqspeada.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/glgtjoehq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gfykxfvbv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gdgxjbktl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.tarul.cn/Article/details/gjnqhuzkp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.vehdjk.com/Article/details/gvjbbrdyl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gvhrguukj.sHtML

[H03] 主动抛出异常
来源：http://blog.bbcook.cn/Article/details/gfnwetqve.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.epnwcf.com/Article/details/gthwbfbum.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gmywnhnkc.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gvimptlyx.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/ggirxbmra.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gjfqicjar.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fktsv.cn/Article/details/gwcantihr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/gbumfydis.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/ggoctwfli.sHtML

[H04] 自定义异常类型
来源：http://3g.vehdjk.com/Article/details/ghwlgbuvq.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.vehdjk.com/Article/details/gwgqiyzbb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gqwcaymvr.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/ggvgylupc.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gpkytmnse.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/geocnkvcq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.epnwcf.com/Article/details/gnauykpry.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fktsv.cn/Article/details/gewovvkrs.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fktsv.cn/Article/details/ghwgsxkza.sHtML

[H05] 捕获特定类型
来源：http://baike.bbcook.cn/Article/details/gwdwtkpyg.sHtML

Py:   except ValueError as e:
来源：http://blog.fktsv.cn/Article/details/gmghlgfad.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fktsv.cn/Article/details/gyokdptov.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/gywadctup.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gnuybhadg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.bbcook.cn/Article/details/glxenxwai.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.yfazqb.com/Article/details/gsrxutnkk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.bbcook.cn/Article/details/grfvtenos.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fktsv.cn/Article/details/godoyqyaf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.vehdjk.com/Article/details/gojsmrvzo.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.vehdjk.com/Article/details/gcbagtwcq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/gzolnfkgw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/gfsterihz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.vehdjk.com/Article/details/gmzjgcvqx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/gwzojdghb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.sjlbkw.cn/Article/details/gindgqhol.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fktsv.cn/Article/details/ggzekjhlq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gtlowzjfd.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdyoxwpu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.epnwcf.com/Article/details/gvvpyolhp.sHtML

PHP:  assert($x > 0);
来源：http://mobile.epnwcf.com/Article/details/gihabtqac.sHtML

JS:   console.assert(x > 0);
来源：http://3g.tarul.cn/Article/details/gceoktscs.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.tarul.cn/Article/details/gtluvdwqo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.yfazqb.com/Article/details/gwotgeeod.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fktsv.cn/Article/details/gnosjhmir.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.yfazqb.com/Article/details/ghlipfbpv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gloudycew.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.vehdjk.com/Article/details/gqpjrkosz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.epnwcf.com/Article/details/gmpbmthxq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.epnwcf.com/Article/details/grztlcnij.sHtML

JS:   e.message;  e.stack
来源：http://m.share.epnwcf.com/Article/details/gvvipvajj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.bbcook.cn/Article/details/glnibtfjs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.bbcook.cn/Article/details/gmwuftcim.sHtML

Go:   err.Error()
来源：http://www.blog.vehdjk.com/Article/details/gastrnnfr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.tarul.cn/Article/details/gbfmapnes.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fktsv.cn/Article/details/gnrylmfvy.sHtML

[H09] 带错误码的异常
来源：http://read.share.tarul.cn/Article/details/gdzrqemfg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.yfazqb.com/Article/details/gqynkrrsa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.tarul.cn/Article/details/gbrqgyldr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/gozyrcqtw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.epnwcf.com/Article/details/gcrjukgsy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fktsv.cn/Article/details/giwznxtrx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.sjlbkw.cn/Article/details/gtjvxnzqj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.bbcook.cn/Article/details/gukclrkia.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.vehdjk.com/Article/details/gshtcfhvh.sHtML

[H10] 资源自动释放
来源：http://read.share.vehdjk.com/Article/details/ggopcoigk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.vehdjk.com/Article/details/gczfutnhh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fktsv.cn/Article/details/gohdgbrkq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gwaxzmmkc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.vehdjk.com/Article/details/glnkkomfs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gkcxndaxs.sHtML

Go:   defer f.Close()
来源：http://wap.fktsv.cn/Article/details/ghzqsvtef.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.yfazqb.com/Article/details/gpevenmhc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.tarul.cn/Article/details/gqnzxyoyx.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/givcfrzez.sHtML

I. 正则表达式
来源：http://read.share.yfazqb.com/Article/details/gfdrsylzl.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/galqdpitg.sHtML

[I01] 判断是否匹配
来源：http://mobile.vehdjk.com/Article/details/gsokjijxe.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/guajbvbhp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.tarul.cn/Article/details/gmdyekekz.sHtML

JS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/grpcpvuak.sHtML

TS:   /\d+/.test(s)
来源：http://3g.yfazqb.com/Article/details/gwxtjftpd.sHtML


<!-- 参考信息 -->