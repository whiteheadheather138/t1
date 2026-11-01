代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.tarul.cn/Article/details/ghxjsohhu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gspkqdmrn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gvoqnwpoa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.yfazqb.com/Article/details/grnsnhfkg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.tarul.cn/Article/details/gyyecreke.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/gimcfsqtd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/gaxzktybk.sHtML

[F08] 遍历目录
来源：http://www.m.share.tarul.cn/Article/details/gdyfovcoh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/guwxvbzvh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gnwbressj.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gipxjhjdt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gklmtudbi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gaybzwfdg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.epnwcf.com/Article/details/gbarouenp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/gdipqbhoa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.tarul.cn/Article/details/gdsdidnas.sHtML

[F09] 获取文件大小
来源：http://wap.fktsv.cn/Article/details/gvyjkqisv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gueofpwft.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gdmrblxub.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/gaaxnevcg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gipmvvyvk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gaccdfpmg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.tarul.cn/Article/details/gkmbnoedf.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gpukqqyqm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fktsv.cn/Article/details/gxcjlpnoo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fktsv.cn/Article/details/gsdcjyjpk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gfcmiimvm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.epnwcf.com/Article/details/gkukixxoq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/ggqtqaqwq.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gipsraguz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.sjlbkw.cn/Article/details/gxxtfsnui.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/ghutppnam.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gmpdtbeaj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gvormzdqb.sHtML

[F11] 复制与移动文件
来源：http://blog.tarul.cn/Article/details/gbzqirguq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gxtdsneif.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gumjctdxk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gkzuyavfb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gqvnfbwjb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gqupvehvi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/gfqqyayyx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gjffuvbhw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.epnwcf.com/Article/details/gfsnxincb.sHtML

[F12] CSV 读写
来源：http://3g.fktsv.cn/Article/details/gombmohpi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.sjlbkw.cn/Article/details/ggfskxjzf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fktsv.cn/Article/details/gjhklling.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.tarul.cn/Article/details/gsxmnfuit.sHtML

TS:   // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gybiqvxpf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/gosvijpbg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.tarul.cn/Article/details/gjhsdizaa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.epnwcf.com/Article/details/gciaojwkc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.yfazqb.com/Article/details/gldtuorsp.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gtlwodifx.sHtML

G. 面向对象
来源：http://3g.fktsv.cn/Article/details/gwbiliwus.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdotxhpsp.sHtML

[G01] 定义类
来源：http://wap.bbcook.cn/Article/details/gkzdzzpjm.sHtML

Py:   class User: pass
来源：http://read.share.sjlbkw.cn/Article/details/gqlrijdsg.sHtML

PHP:  class User {}
来源：http://blog.bbcook.cn/Article/details/gxytzlpbp.sHtML

JS:   class User {}
来源：http://3g.fktsv.cn/Article/details/gtcsnongl.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.tarul.cn/Article/details/glhrneznl.sHtML

Java: class User {}
来源：http://m.share.bbcook.cn/Article/details/glbjjhgjt.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/gkeexbxyl.sHtML

Ruby: class User; end
来源：http://www.m.share.yfazqb.com/Article/details/gsqctuipb.sHtML

C#:   class User {}
来源：http://3g.yfazqb.com/Article/details/gtqnnlygb.sHtML

[G02] 构造函数
来源：http://read.share.sjlbkw.cn/Article/details/ghdvzvucp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.sjlbkw.cn/Article/details/giuabtkdk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.yfazqb.com/Article/details/ggshhvhxt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gtchbewkf.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.vehdjk.com/Article/details/gsxaorueh.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gmdsfkwqo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.epnwcf.com/Article/details/gdkffxqav.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.yfazqb.com/Article/details/gpdwupkyu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.tarul.cn/Article/details/gztjoanqq.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/gbgywpusw.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gansgagga.sHtML

PHP:  public string $name = "x";
来源：http://blog.fktsv.cn/Article/details/gkthwradl.sHtML

JS:   this.name = "x";
来源：http://3g.fktsv.cn/Article/details/gbqeaurvh.sHtML

TS:   name: string = "x";
来源：http://baike.yfazqb.com/Article/details/gpuufrdzz.sHtML

Java: private String name;
来源：http://www.blog.tarul.cn/Article/details/gbpuweubn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.bbcook.cn/Article/details/gpfzgbigb.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/gudpyhjjm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.sjlbkw.cn/Article/details/gwiojdkyh.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/gamzipehs.sHtML

Py:   def greet(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gmsdtdzcs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gqshqvaln.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gvyxgbfmt.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gmcakghpv.sHtML

Java: String greet() { return name; }
来源：http://baike.fktsv.cn/Article/details/ggmzctilq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gqxogdkax.sHtML

Ruby: def greet; @name; end
来源：http://wap.fktsv.cn/Article/details/gowtjpwzc.sHtML

C#:   public string Greet() => Name;
来源：http://baike.epnwcf.com/Article/details/gowoeyuwt.sHtML

[G05] 继承
来源：http://3g.vehdjk.com/Article/details/gmniaeboc.sHtML

Py:   class Admin(User): pass
来源：http://baike.vehdjk.com/Article/details/gcnzvalar.sHtML

PHP:  class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/ghqyvzdyc.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gbydchvsh.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gqrtmrsex.sHtML

Java: class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gpctjgtnp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.epnwcf.com/Article/details/glgkxvmjy.sHtML

Ruby: class Admin < User; end
来源：http://baike.fktsv.cn/Article/details/gufunftca.sHtML

C#:   class Admin : User {}
来源：http://wap.sjlbkw.cn/Article/details/gqdveppll.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gobruswue.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.tarul.cn/Article/details/glmfisdth.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gkyumsvii.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/glrrifiob.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpscnsju.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gqjztxxzi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.vehdjk.com/Article/details/gppwzjoqb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.bbcook.cn/Article/details/glljsdnez.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.sjlbkw.cn/Article/details/gumvfbypn.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/gsossnnln.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/goqcwyewi.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gtrabiolk.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gbmmxxkps.sHtML

TS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/godnsvnrq.sHtML

Java: super.greet();
来源：http://baike.fktsv.cn/Article/details/gktaelxig.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.tarul.cn/Article/details/gbnbbvdeu.sHtML

Ruby: super
来源：http://blog.bbcook.cn/Article/details/gvvrcirgw.sHtML

C#:   base.Greet();
来源：http://www.blog.tarul.cn/Article/details/gbawcnwsw.sHtML

[G08] 静态方法与属性
来源：http://mobile.sjlbkw.cn/Article/details/guswrevdi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fktsv.cn/Article/details/gxdxxfvbn.sHtML

PHP:  public static function f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gxqwxpzrr.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/glmsmjjdk.sHtML

TS:   static f(): void {}
来源：http://wap.fktsv.cn/Article/details/gxyagseuw.sHtML

Java: static void f() {}
来源：http://www.share.vehdjk.com/Article/details/gtkqahbbs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.bbcook.cn/Article/details/gasvbcsqq.sHtML

Ruby: def self.f; end
来源：http://m.share.sjlbkw.cn/Article/details/gaafgnojl.sHtML

C#:   public static void F() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbdxeiemj.sHtML

[G09] 接口 / 抽象类
来源：http://baike.epnwcf.com/Article/details/gcgedxbah.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.vehdjk.com/Article/details/gqkwddkcp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fktsv.cn/Article/details/gepvctbwm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/gwitgrwcr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.vehdjk.com/Article/details/gctiziqhi.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gqaynmmcx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/gvuewfaga.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/gwtmbjfoc.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fktsv.cn/Article/details/gmqgbvyvu.sHtML

[G10] 访问控制
来源：http://wap.fktsv.cn/Article/details/grxvgujzz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.epnwcf.com/Article/details/gzlcukecn.sHtML

PHP:  public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gpffkrjrf.sHtML

JS:   #private 字段；其余公开
来源：http://3g.bbcook.cn/Article/details/gtmmazjso.sHtML

TS:   public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gvjrnsyts.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.tarul.cn/Article/details/gmpaxdjfr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fktsv.cn/Article/details/gbmmggepn.sHtML

Ruby: public / protected / private
来源：http://wap.tarul.cn/Article/details/gvlmtvwwf.sHtML

C#:   public / protected / private / internal
来源：http://3g.bbcook.cn/Article/details/gvdrzmcds.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/gwfngjyxo.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.tarul.cn/Article/details/gwvdlkzjg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gcvovxflu.sHtML

JS:   get name() { return this._name; }
来源：http://baike.tarul.cn/Article/details/gamnasfwo.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gttrlxzgx.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gsjcnpueo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gbnpndijc.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.sjlbkw.cn/Article/details/gohuegchk.sHtML

C#:   public string Name { get; set; }
来源：http://baike.tarul.cn/Article/details/gmpsviapg.sHtML

[G12] 对象转字符串
来源：http://baike.yfazqb.com/Article/details/gegikzitd.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gxcttnhod.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gkdfkmqbn.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gsdizskjw.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/ghmpvdxpn.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fktsv.cn/Article/details/grbrdapsn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/grcizihbg.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/gciozrlrz.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.yfazqb.com/Article/details/gzejsdypf.sHtML

[G13] 判断对象类型
来源：http://www.share.vehdjk.com/Article/details/gyxavrzty.sHtML

Py:   isinstance(u, User)
来源：http://baike.tarul.cn/Article/details/gvqrtnyui.sHtML

PHP:  $u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gvflndvwx.sHtML

JS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gfnqqfgyq.sHtML

TS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gijncolji.sHtML

Java: u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gvyhnwsvh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/gyuofcnge.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.tarul.cn/Article/details/geygmxqox.sHtML

C#:   u is User
来源：http://blog.vehdjk.com/Article/details/gtatgwgyo.sHtML

[G14] 数据类 / record
来源：http://baike.yfazqb.com/Article/details/gfovinyvq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.yfazqb.com/Article/details/grbgfpday.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.sjlbkw.cn/Article/details/gfjctzacu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/giooqowgr.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gdyyapkqw.sHtML

Java: record User(String name, int age) {}
来源：http://3g.bbcook.cn/Article/details/gummtrequ.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.sjlbkw.cn/Article/details/gqhjizwyq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/gqifiacyd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/giulfppjr.sHtML

[G15] 枚举
来源：http://www.blog.bbcook.cn/Article/details/gzkciwmrz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.sjlbkw.cn/Article/details/gxnbteznu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fktsv.cn/Article/details/gsmqwcvzw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.sjlbkw.cn/Article/details/gtmrcxttn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gpycoxaxw.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fktsv.cn/Article/details/gfwwitmvw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.tarul.cn/Article/details/gykheooln.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.sjlbkw.cn/Article/details/gagtclctx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gpezfodeo.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.yfazqb.com/Article/details/gkaxyuonp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.epnwcf.com/Article/details/gibrjmboe.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/gekzzctrx.sHtML

JS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/ggdhlzsqh.sHtML

TS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gwnxkkzlr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqopmbwji.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.bbcook.cn/Article/details/glxtprpjz.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fktsv.cn/Article/details/gtyxtsyhu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gxagpjbfd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpmonarrs.sHtML

H. 异常与错误处理
来源：http://www.share.epnwcf.com/Article/details/gezpybsih.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqotwabao.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/gqflouwzf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fktsv.cn/Article/details/gfhnjayxo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.vehdjk.com/Article/details/glpaenzcx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gtkyndzes.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gyekudmmi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.sjlbkw.cn/Article/details/goibikcql.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.tarul.cn/Article/details/gpyvklkcg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/gxxzpesdf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.vehdjk.com/Article/details/gwdjknuuw.sHtML

[H02] finally / ensure 收尾
来源：http://wap.epnwcf.com/Article/details/gxofpweql.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.yfazqb.com/Article/details/gxujdinku.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gztieflkj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/grebknpsg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gusptgigv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gswuinjzp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.tarul.cn/Article/details/gainivwce.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.sjlbkw.cn/Article/details/gwxopqsnr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gmxwmnmcq.sHtML

[H03] 主动抛出异常
来源：http://read.share.bbcook.cn/Article/details/gjepybavs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.yfazqb.com/Article/details/gsdlpaync.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/govwovfnz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/guahnbmsp.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gyxasspnf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gbwuvbhyp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.vehdjk.com/Article/details/gwmpryfnd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.epnwcf.com/Article/details/gkgjlwdbd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gehdldeed.sHtML

[H04] 自定义异常类型
来源：http://3g.vehdjk.com/Article/details/gnfnmehhi.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fktsv.cn/Article/details/gynzqkmtf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/grvcnewga.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gavhmamts.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gqchtultc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/gaexsnigg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.bbcook.cn/Article/details/gtgmotgqm.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.sjlbkw.cn/Article/details/gtrakvntt.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.sjlbkw.cn/Article/details/gnjubltaa.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/gezmwgqql.sHtML

Py:   except ValueError as e:
来源：http://3g.bbcook.cn/Article/details/getbnpuac.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.tarul.cn/Article/details/gquzotwtr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gntsgpmgr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/gxoqcorlq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.yfazqb.com/Article/details/getvcltul.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.bbcook.cn/Article/details/gicsctrou.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.vehdjk.com/Article/details/gglymhybn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/gwzaebecy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.epnwcf.com/Article/details/ghsyrbkxd.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.epnwcf.com/Article/details/gfalpdibk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gylfvaeyb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gxfexmqhl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/glvjatlhn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.sjlbkw.cn/Article/details/gfrhefaao.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.epnwcf.com/Article/details/gfesehuus.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.epnwcf.com/Article/details/gigecknmi.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.tarul.cn/Article/details/guzddveiv.sHtML

[H07] 断言
来源：http://wap.yfazqb.com/Article/details/gzjziyzct.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.epnwcf.com/Article/details/gvumftcgk.sHtML

PHP:  assert($x > 0);
来源：http://blog.tarul.cn/Article/details/guxwwofud.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gbwzylvce.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/geecuyqip.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fktsv.cn/Article/details/gdcqoicnf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.bbcook.cn/Article/details/gttkytxqa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.yfazqb.com/Article/details/gjgkjcyto.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gpjkqqace.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.bbcook.cn/Article/details/gykzubxjz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.sjlbkw.cn/Article/details/gkjlrsaqi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.yfazqb.com/Article/details/guwooflww.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.epnwcf.com/Article/details/ggaxhgyxd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.epnwcf.com/Article/details/gnjswdgxv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.bbcook.cn/Article/details/gypxbjunt.sHtML

Go:   err.Error()
来源：http://wap.tarul.cn/Article/details/gazkprksk.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.epnwcf.com/Article/details/ggmpsbvyc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.tarul.cn/Article/details/gvyhoudbv.sHtML

[H09] 带错误码的异常
来源：http://www.share.sjlbkw.cn/Article/details/gonevcxss.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/gqocdfcfq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.sjlbkw.cn/Article/details/gxyvbossh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gextboipy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.yfazqb.com/Article/details/gcxflitks.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.tarul.cn/Article/details/gwgwguzpk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.tarul.cn/Article/details/gwufvpbul.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fktsv.cn/Article/details/gmhjefllf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.sjlbkw.cn/Article/details/gcgqkdvap.sHtML

[H10] 资源自动释放
来源：http://baike.sjlbkw.cn/Article/details/gpoihcevc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.yfazqb.com/Article/details/gkounforz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.sjlbkw.cn/Article/details/gupbaphzl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gxprwybfl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.bbcook.cn/Article/details/ghsiekskk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.epnwcf.com/Article/details/gqydfegvc.sHtML

Go:   defer f.Close()
来源：http://mobile.sjlbkw.cn/Article/details/gwodpzovg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.tarul.cn/Article/details/glpqsohxk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.epnwcf.com/Article/details/ggugjnwtr.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtkmacaaj.sHtML

I. 正则表达式
来源：http://www.share.fktsv.cn/Article/details/gpqtlovlh.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzytpfhmd.sHtML

[I01] 判断是否匹配
来源：http://read.share.sjlbkw.cn/Article/details/ghyagjmjc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.sjlbkw.cn/Article/details/gtqkyxdbr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.yfazqb.com/Article/details/gcdeptbzu.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/ghnzvlrrx.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/gmmlzrovw.sHtML


<!-- 参考信息 -->