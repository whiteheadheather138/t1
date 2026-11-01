代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/gwxtwvacx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/gthjbwfff.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/gfubmvjpn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.tarul.cn/Article/details/gvecuygff.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.yfazqb.com/Article/details/gyukyhgsh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.yfazqb.com/Article/details/gloeycehv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gflporrhe.sHtML

[F08] 遍历目录
来源：http://www.share.sjlbkw.cn/Article/details/ghppfzibb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fktsv.cn/Article/details/ghftccwgy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.yfazqb.com/Article/details/gqeehbokh.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gkwmegzyb.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/ginfudjud.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/glqrfrkdt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fktsv.cn/Article/details/gcvaaukls.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.sjlbkw.cn/Article/details/ggtiobftd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.yfazqb.com/Article/details/ghatxhoeg.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gryosbyuh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gggmiidtn.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gegvppxmn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gkikhpzhc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gahvbmmfi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/ggolafmai.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.yfazqb.com/Article/details/gcxrqmgyf.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gnscorcwb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.epnwcf.com/Article/details/gpnksajfy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fktsv.cn/Article/details/gafoncgpe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gsafhravx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/gbdshgaps.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gbbdfdjzo.sHtML

TS:   path.extname("a.txt")
来源：http://baike.bbcook.cn/Article/details/gikoltftp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fktsv.cn/Article/details/gxydwmqcg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/giiihcbej.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gnfevzpid.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gwypjldis.sHtML

[F11] 复制与移动文件
来源：http://3g.sjlbkw.cn/Article/details/grtdovqmv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gxuhpmtta.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.bbcook.cn/Article/details/ghwvvsczg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjnzyiieq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/graprdyon.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/gmchbtmmq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcwdiyhw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gbjilrmij.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.bbcook.cn/Article/details/gapesnacg.sHtML

[F12] CSV 读写
来源：http://read.share.sjlbkw.cn/Article/details/gdtrqzibs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.bbcook.cn/Article/details/gbcxjpxfz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.vehdjk.com/Article/details/gnawobjvp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.tarul.cn/Article/details/gfhnqsilo.sHtML

TS:   // 同上
来源：http://www.share.yfazqb.com/Article/details/gdhotwsvi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.bbcook.cn/Article/details/gmfgvphna.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.vehdjk.com/Article/details/gisnsdfhv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.yfazqb.com/Article/details/gnmzzohqt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/gdmkprrgk.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gebvgmtrw.sHtML

G. 面向对象
来源：http://wap.fktsv.cn/Article/details/gvziauakk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvpsqvfpj.sHtML

[G01] 定义类
来源：http://mobile.vehdjk.com/Article/details/gtsytwivs.sHtML

Py:   class User: pass
来源：http://3g.tarul.cn/Article/details/gghyuwksr.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gatgpdppo.sHtML

JS:   class User {}
来源：http://baike.tarul.cn/Article/details/gwhdhmukt.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/gwmkschcm.sHtML

Java: class User {}
来源：http://www.blog.bbcook.cn/Article/details/gzqzrwjhv.sHtML

Go:   type User struct { Name string }
来源：http://m.share.yfazqb.com/Article/details/gknuynelg.sHtML

Ruby: class User; end
来源：http://blog.bbcook.cn/Article/details/gktrobfte.sHtML

C#:   class User {}
来源：http://read.share.epnwcf.com/Article/details/goohrjhzt.sHtML

[G02] 构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gwrdofpli.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/gbuhnkkyk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/gkbkcgbil.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gsfwmqpla.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.epnwcf.com/Article/details/ggzloydtf.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gpbtwtpls.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gzlmjshrl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fktsv.cn/Article/details/gcibszeoj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gdxqenzgn.sHtML

[G03] 实例属性
来源：http://baike.epnwcf.com/Article/details/gfumytnbt.sHtML

Py:   self.name = "x"
来源：http://blog.fktsv.cn/Article/details/guumdmvck.sHtML

PHP:  public string $name = "x";
来源：http://blog.epnwcf.com/Article/details/gkzsqagdl.sHtML

JS:   this.name = "x";
来源：http://wap.fktsv.cn/Article/details/gzrqprsbm.sHtML

TS:   name: string = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gdsaavxit.sHtML

Java: private String name;
来源：http://www.blog.fktsv.cn/Article/details/gswrcrmyz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.epnwcf.com/Article/details/gresrbgiu.sHtML

Ruby: @name = "x"
来源：http://www.share.yfazqb.com/Article/details/gkaefmjxw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.vehdjk.com/Article/details/ggmkehvzo.sHtML

[G04] 定义方法
来源：http://www.share.sjlbkw.cn/Article/details/giollkjqq.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gwocoqlgk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gejgkique.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/godzrxgyi.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gtckwtusn.sHtML

Java: String greet() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/grxuywebm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gnsuhqavf.sHtML

Ruby: def greet; @name; end
来源：http://blog.epnwcf.com/Article/details/gbcjlqwny.sHtML

C#:   public string Greet() => Name;
来源：http://baike.tarul.cn/Article/details/gwxvdtdpt.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/gtmnesilc.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gbqiiccnj.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gymqwneme.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gpdhzgqgf.sHtML

TS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gmqeklodv.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gghdwzszo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.epnwcf.com/Article/details/gsmhztfkq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.epnwcf.com/Article/details/gcotejprq.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fktsv.cn/Article/details/gokbzhmgw.sHtML

[G06] 重写方法
来源：http://read.share.tarul.cn/Article/details/ghieypdji.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.vehdjk.com/Article/details/gnokndblw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gvsbceggr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gebnphhni.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gjachkhff.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gzqjtglux.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.sjlbkw.cn/Article/details/gzevkuzyb.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.yfazqb.com/Article/details/ghrdfayxd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/gjpzdmczr.sHtML

[G07] 调用父类方法
来源：http://www.share.epnwcf.com/Article/details/gwwvrggkg.sHtML

Py:   super().greet()
来源：http://www.share.bbcook.cn/Article/details/gcfdvulxs.sHtML

PHP:  parent::greet();
来源：http://wap.fktsv.cn/Article/details/gncnbjszh.sHtML

JS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gyjoauioq.sHtML

TS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gzfhhireh.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gvokebwuy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.sjlbkw.cn/Article/details/gqxuzlaeq.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gbwjwpiex.sHtML

C#:   base.Greet();
来源：http://www.blog.fktsv.cn/Article/details/gjjuzwmlk.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/gasfomfwd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.yfazqb.com/Article/details/gbjcdbpta.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/gpddxlsgk.sHtML

JS:   static f() {}
来源：http://wap.yfazqb.com/Article/details/glxuhrhuv.sHtML

TS:   static f(): void {}
来源：http://baike.fktsv.cn/Article/details/gtlcuqcbt.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/ghlbsrdvk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gazyzmxpi.sHtML

Ruby: def self.f; end
来源：http://baike.epnwcf.com/Article/details/gkhyappkx.sHtML

C#:   public static void F() {}
来源：http://www.share.sjlbkw.cn/Article/details/giubzfhxt.sHtML

[G09] 接口 / 抽象类
来源：http://3g.epnwcf.com/Article/details/gquapvocw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/ghptvszch.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.sjlbkw.cn/Article/details/gpvguasyq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/gwxzhozqn.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.vehdjk.com/Article/details/gwrcnysov.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/gncnsorpi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fktsv.cn/Article/details/gxiyhbxwa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.bbcook.cn/Article/details/gvivtjzve.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/gaszkqwrs.sHtML

[G10] 访问控制
来源：http://baike.sjlbkw.cn/Article/details/gtntkqhos.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gnhczeuxz.sHtML

PHP:  public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gkqixqiqa.sHtML

JS:   #private 字段；其余公开
来源：http://blog.yfazqb.com/Article/details/gpwpkstvu.sHtML

TS:   public / protected / private
来源：http://wap.bbcook.cn/Article/details/gisjgxksj.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.vehdjk.com/Article/details/gimesufon.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.epnwcf.com/Article/details/gbzzbbssv.sHtML

Ruby: public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gggkdsomk.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.vehdjk.com/Article/details/ggzdfrihz.sHtML

[G11] getter / setter
来源：http://baike.fktsv.cn/Article/details/gqjornwkc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.bbcook.cn/Article/details/gjksckiwx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/guopvrqwq.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gvmxhbnin.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/gaiyuvjyx.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gljsvvhrl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gkfztpeml.sHtML

Ruby: attr_accessor :name
来源：http://baike.vehdjk.com/Article/details/gnhutqlrc.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/gazqmrtlu.sHtML

[G12] 对象转字符串
来源：http://blog.fktsv.cn/Article/details/gdkyonaog.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/gxclxhmzk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gihvhmusg.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gpfjgubwo.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gpmuhzpom.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gxzobkbil.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gntcmpnok.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/gmzgzqcgb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/glrmgkaqb.sHtML

[G13] 判断对象类型
来源：http://www.m.share.tarul.cn/Article/details/gclgmrugx.sHtML

Py:   isinstance(u, User)
来源：http://www.share.bbcook.cn/Article/details/gwgbxdeoy.sHtML

PHP:  $u instanceof User
来源：http://mobile.yfazqb.com/Article/details/ghpglwcgz.sHtML

JS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/ghkbmcgcf.sHtML

TS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gmnbwhnpg.sHtML

Java: u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gzkeenuzo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/gpgkmqkwp.sHtML

Ruby: u.is_a?(User)
来源：http://3g.epnwcf.com/Article/details/gzpxifdxs.sHtML

C#:   u is User
来源：http://m.share.tarul.cn/Article/details/gaextdnbj.sHtML

[G14] 数据类 / record
来源：http://read.share.epnwcf.com/Article/details/gltbxvjoa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.epnwcf.com/Article/details/grkkturkp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.yfazqb.com/Article/details/gpozfpbul.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.sjlbkw.cn/Article/details/gqfamlbkm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.epnwcf.com/Article/details/gjuvnmcms.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/gzhadcyfl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fktsv.cn/Article/details/gnqvxvipp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.tarul.cn/Article/details/glfkcnckj.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.vehdjk.com/Article/details/gczrhknxh.sHtML

[G15] 枚举
来源：http://www.blog.fktsv.cn/Article/details/gtlueawkh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.epnwcf.com/Article/details/gkhkdvtyc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/ggcrvuhsz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.vehdjk.com/Article/details/govnzhkou.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/gcinkvzds.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.sjlbkw.cn/Article/details/gmfzvduyq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.yfazqb.com/Article/details/gngjnctbf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.sjlbkw.cn/Article/details/gargjyutt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gepywrzca.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.bbcook.cn/Article/details/gjsjaqyfn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fktsv.cn/Article/details/ghzccwdck.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.vehdjk.com/Article/details/gexwysshm.sHtML

JS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gcbhlqasi.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gvmpvrlys.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.epnwcf.com/Article/details/gljdtjaii.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fktsv.cn/Article/details/gsmhufywo.sHtML

Ruby: obj.instance_variables
来源：http://3g.fktsv.cn/Article/details/gosfdadjy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gurbuseki.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghqhepnna.sHtML

H. 异常与错误处理
来源：http://www.share.bbcook.cn/Article/details/gsaabmpzm.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjdkcunbu.sHtML

[H01] try / catch 基础
来源：http://baike.epnwcf.com/Article/details/gmledkcqb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.yfazqb.com/Article/details/gvqazrhke.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.vehdjk.com/Article/details/gbnjqyyiz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gbahqklkk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/ggcjehdel.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/gaegtsqkv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.bbcook.cn/Article/details/gsyzfdoqj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.sjlbkw.cn/Article/details/gqsesumbz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/genoczgdi.sHtML

[H02] finally / ensure 收尾
来源：http://wap.sjlbkw.cn/Article/details/gnlugfzma.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.sjlbkw.cn/Article/details/gnvgfqrya.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gkckoforx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gqznebzaq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gqvbblosf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/goiyeettt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.bbcook.cn/Article/details/gaamtvlol.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.epnwcf.com/Article/details/gsyvpeajt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gcltmlsfp.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/gyzwwqeqw.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.vehdjk.com/Article/details/gbepiryuj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gelgrjguo.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gsvycycks.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gubgmsnuy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gtsqsysdl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fktsv.cn/Article/details/gzqwxdddu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.epnwcf.com/Article/details/gmsajmsga.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gebmjpdxc.sHtML

[H04] 自定义异常类型
来源：http://blog.tarul.cn/Article/details/gvvqwkccp.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.bbcook.cn/Article/details/gquvtflla.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.bbcook.cn/Article/details/gmjqxgwda.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gqspgjrlr.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/gcovmiwgh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gpnudweks.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.tarul.cn/Article/details/gscgfrkiu.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.sjlbkw.cn/Article/details/gfctrrznc.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/geixwzltm.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.vehdjk.com/Article/details/gvjgnpmxp.sHtML

Py:   except ValueError as e:
来源：http://blog.epnwcf.com/Article/details/gnbzqtbxw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.sjlbkw.cn/Article/details/gukrvjgmz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gnnfngfyd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/gahpdxqnh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.tarul.cn/Article/details/gccameobc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/grkdjgeyk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.bbcook.cn/Article/details/gagtwotho.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/grjgghvpo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/gjyrxzqsl.sHtML

Py:   value = d.get("k") or default
来源：http://blog.tarul.cn/Article/details/glpszndpp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/grmcvcurv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gyvzfzodn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/geqzqtxyp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fktsv.cn/Article/details/grngaotem.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.yfazqb.com/Article/details/gepjdnyln.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.epnwcf.com/Article/details/gzdbxhvyy.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.epnwcf.com/Article/details/gqwnljsil.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gysqfltmz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.vehdjk.com/Article/details/gffmjjbgc.sHtML

PHP:  assert($x > 0);
来源：http://read.share.tarul.cn/Article/details/gpteweoeb.sHtML

JS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gvekygeqc.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gjfiqixes.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gnxphysti.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.epnwcf.com/Article/details/grlngsqjt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fktsv.cn/Article/details/gkacveqwm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gufsjgzyy.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.bbcook.cn/Article/details/glwpwtzbf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.yfazqb.com/Article/details/gflrffewh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fktsv.cn/Article/details/gcfnuljhr.sHtML

JS:   e.message;  e.stack
来源：http://m.share.bbcook.cn/Article/details/goziguekq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/gluuiegpi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/giopswafe.sHtML

Go:   err.Error()
来源：http://www.blog.yfazqb.com/Article/details/gdpslmrxe.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gtgoccvxl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.sjlbkw.cn/Article/details/gsmfsdptl.sHtML

[H09] 带错误码的异常
来源：http://www.share.yfazqb.com/Article/details/gudulcwhw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.bbcook.cn/Article/details/gqaunhjgf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.epnwcf.com/Article/details/gswnignvz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjbrvnnr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.yfazqb.com/Article/details/gcjqklrtp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.bbcook.cn/Article/details/gzkergvcj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fktsv.cn/Article/details/gceaiimag.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.vehdjk.com/Article/details/gzebabupp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.epnwcf.com/Article/details/gkadtxput.sHtML

[H10] 资源自动释放
来源：http://m.share.epnwcf.com/Article/details/gdgfwsnfa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.epnwcf.com/Article/details/gtjtqglcb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.sjlbkw.cn/Article/details/gtzkoapfw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gqteyjyke.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gpkwcqvbe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.epnwcf.com/Article/details/gcocabgmy.sHtML

Go:   defer f.Close()
来源：http://3g.yfazqb.com/Article/details/gwrrqnvzj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.vehdjk.com/Article/details/ggblaiamw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.bbcook.cn/Article/details/gcngfxwjg.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkojikpvu.sHtML

I. 正则表达式
来源：http://www.share.epnwcf.com/Article/details/gdaqzqqym.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gyskmhqly.sHtML

[I01] 判断是否匹配
来源：http://read.share.vehdjk.com/Article/details/gvxexewyt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gkskciivj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.vehdjk.com/Article/details/gedotnths.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.yfazqb.com/Article/details/gjjjaxnmx.sHtML

TS:   /\d+/.test(s)
来源：http://3g.bbcook.cn/Article/details/gobsztbnb.sHtML


<!-- 参考信息 -->