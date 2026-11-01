代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gsuncdgms.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/ginypuley.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gvmbjjndl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gdrqpnayn.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gkzwdmvyo.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/geosjdqnz.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.bbcook.cn/Article/details/ghocnywek.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/gjqruvhvd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.epnwcf.com/Article/details/gxbgngnlr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gskcdadtt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gkojfolnd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.vehdjk.com/Article/details/gyzuvthoo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.tarul.cn/Article/details/grsecamvw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fktsv.cn/Article/details/gkruqccwd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/gainhgome.sHtML

[F08] 遍历目录
来源：http://www.m.share.epnwcf.com/Article/details/gvxjdvkdm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.yfazqb.com/Article/details/guzuksyey.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gvzhtmxbf.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gyabkaifo.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/ggjunfeyd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gdkkcoiai.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fktsv.cn/Article/details/gtllqiece.sHtML

Ruby: Dir.children("dir")
来源：http://3g.yfazqb.com/Article/details/gztppoqvq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/glzhxdvhd.sHtML

[F09] 获取文件大小
来源：http://www.m.share.vehdjk.com/Article/details/gzrwmtlrp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gutdpnrxg.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gbfutlmef.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gsxwergwn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gpqyoomer.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gniyrofom.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.sjlbkw.cn/Article/details/gmdbkampj.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/grhmlmlza.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fktsv.cn/Article/details/gmytldpan.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.tarul.cn/Article/details/guzsjllor.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/grzifrvfr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.epnwcf.com/Article/details/guxvrlsxe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gihtvkmdj.sHtML

TS:   path.extname("a.txt")
来源：http://blog.tarul.cn/Article/details/gisoenjon.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/gmygjqucs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gstzedyye.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gyifkaxxv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/glbftmwby.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gjmpgezsc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gyrstwgbz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/gyvlvcdeb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gmaprjcvf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gnoihyemj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.tarul.cn/Article/details/gfbciobyl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.bbcook.cn/Article/details/gtxihutsz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gkejgaygp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.tarul.cn/Article/details/glhnqwjyf.sHtML

[F12] CSV 读写
来源：http://mobile.vehdjk.com/Article/details/gndojaxkv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.vehdjk.com/Article/details/ggyfghjqx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.tarul.cn/Article/details/gcsrhtybu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.epnwcf.com/Article/details/gtkciohmf.sHtML

TS:   // 同上
来源：http://mobile.bbcook.cn/Article/details/gsyrbswzl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.epnwcf.com/Article/details/glgcvzoqd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.sjlbkw.cn/Article/details/genygsfyg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gwpwvxgiy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.tarul.cn/Article/details/goifkwxpe.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gptxvhcqj.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gznhisuoi.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggiicoglb.sHtML

[G01] 定义类
来源：http://www.m.share.vehdjk.com/Article/details/giaywsqih.sHtML

Py:   class User: pass
来源：http://mobile.bbcook.cn/Article/details/guthpkgjz.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/ghjqlimqc.sHtML

JS:   class User {}
来源：http://baike.epnwcf.com/Article/details/grrcnorri.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fktsv.cn/Article/details/ggnjwwwkq.sHtML

Java: class User {}
来源：http://www.blog.bbcook.cn/Article/details/ghbjthbaa.sHtML

Go:   type User struct { Name string }
来源：http://mobile.vehdjk.com/Article/details/gbgeythbi.sHtML

Ruby: class User; end
来源：http://read.share.vehdjk.com/Article/details/gljmuwvjk.sHtML

C#:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/geixwdbsi.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gxayaymjv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.sjlbkw.cn/Article/details/gvngznlaz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.bbcook.cn/Article/details/gibkvkxyv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/goxawyuat.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.vehdjk.com/Article/details/gjaemiueb.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gremzdtug.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.epnwcf.com/Article/details/guwnschyi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/gxmyaiuov.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.bbcook.cn/Article/details/ghsjpepfq.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/glyijseqj.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gdpqmqkja.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/gvndeqwic.sHtML

JS:   this.name = "x";
来源：http://blog.vehdjk.com/Article/details/gcbodgjgd.sHtML

TS:   name: string = "x";
来源：http://www.blog.fktsv.cn/Article/details/genalwpur.sHtML

Java: private String name;
来源：http://www.m.share.epnwcf.com/Article/details/gxghyqiyz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/gcuzhnkbh.sHtML

Ruby: @name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gcwwfueww.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.epnwcf.com/Article/details/gcgcelerz.sHtML

[G04] 定义方法
来源：http://read.share.tarul.cn/Article/details/gtrswdqci.sHtML

Py:   def greet(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gibrfygni.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/guctovzhr.sHtML

JS:   greet() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gdjnljalz.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gycxqxshx.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpmgoqjm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gacuoojjy.sHtML

Ruby: def greet; @name; end
来源：http://m.share.yfazqb.com/Article/details/gkilccpjy.sHtML

C#:   public string Greet() => Name;
来源：http://wap.tarul.cn/Article/details/ghtvvhgrt.sHtML

[G05] 继承
来源：http://baike.fktsv.cn/Article/details/grxfskfwm.sHtML

Py:   class Admin(User): pass
来源：http://blog.tarul.cn/Article/details/grurtgdny.sHtML

PHP:  class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gioshqukn.sHtML

JS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gwmcsaudk.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gyiakgirl.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gefunfclo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gsvmzmirx.sHtML

Ruby: class Admin < User; end
来源：http://m.share.bbcook.cn/Article/details/gunevntpz.sHtML

C#:   class Admin : User {}
来源：http://mobile.fktsv.cn/Article/details/grveqxmpw.sHtML

[G06] 重写方法
来源：http://www.share.sjlbkw.cn/Article/details/gzdoiypgx.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.bbcook.cn/Article/details/gszimiqxg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gaumpcbbg.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gqinmdkfq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gbcxfdusl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gsgbbjvcj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.tarul.cn/Article/details/glsfpqoqk.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.tarul.cn/Article/details/gfxbjchrq.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fktsv.cn/Article/details/gozamybsd.sHtML

[G07] 调用父类方法
来源：http://wap.epnwcf.com/Article/details/gwjglgegk.sHtML

Py:   super().greet()
来源：http://blog.tarul.cn/Article/details/gjyeobcbg.sHtML

PHP:  parent::greet();
来源：http://baike.bbcook.cn/Article/details/glyseibrv.sHtML

JS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gdzwzbkzr.sHtML

TS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/goyqjyiei.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/gpjswtudq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/gavklbxwg.sHtML

Ruby: super
来源：http://www.m.share.tarul.cn/Article/details/gdvqsfyjx.sHtML

C#:   base.Greet();
来源：http://m.share.epnwcf.com/Article/details/gomjjvpvc.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/gcsziigfy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.bbcook.cn/Article/details/gpejkerit.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gdpsrozro.sHtML

JS:   static f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gusrkjaql.sHtML

TS:   static f(): void {}
来源：http://wap.bbcook.cn/Article/details/gfsvlheyw.sHtML

Java: static void f() {}
来源：http://mobile.vehdjk.com/Article/details/gkwqdnlua.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.bbcook.cn/Article/details/gfjpagosc.sHtML

Ruby: def self.f; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvjnfrhg.sHtML

C#:   public static void F() {}
来源：http://m.share.bbcook.cn/Article/details/gwsuixsrc.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.yfazqb.com/Article/details/gswyuouod.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.yfazqb.com/Article/details/gjcyhmbtt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gmuinjhup.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fktsv.cn/Article/details/gefvbgjkn.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.yfazqb.com/Article/details/gadjaqkeo.sHtML

Java: interface Shape { double area(); }
来源：http://wap.vehdjk.com/Article/details/gnifqmmjz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gidcqixnn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.tarul.cn/Article/details/gvhqrsszi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fktsv.cn/Article/details/gbsghmapk.sHtML

[G10] 访问控制
来源：http://3g.fktsv.cn/Article/details/ghdlewbyx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.epnwcf.com/Article/details/gtvkfawvw.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gbsofwlmc.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.vehdjk.com/Article/details/galzxagnx.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gapcxwubu.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.tarul.cn/Article/details/gkfjksrfd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.vehdjk.com/Article/details/gwcpfobsy.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gmgxhigmy.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.yfazqb.com/Article/details/gqperccsy.sHtML

[G11] getter / setter
来源：http://blog.epnwcf.com/Article/details/gsjiahyvx.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fktsv.cn/Article/details/gmqdxdgit.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/giiuqkmkt.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/ggzikhzje.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/grrvvqslf.sHtML

Java: public String getName() { return name; }
来源：http://3g.epnwcf.com/Article/details/ggmnqdcqr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gfdratwng.sHtML

Ruby: attr_accessor :name
来源：http://3g.tarul.cn/Article/details/gwgkfblzd.sHtML

C#:   public string Name { get; set; }
来源：http://baike.yfazqb.com/Article/details/gclxqgsar.sHtML

[G12] 对象转字符串
来源：http://read.share.vehdjk.com/Article/details/gwgunwbhi.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gwtjyogaw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gsrxcqspr.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/ggcwazzpm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwahlgnl.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.vehdjk.com/Article/details/ggiyjdhfu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gbklsghpe.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/gjhfiuabp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gruscmlaz.sHtML

[G13] 判断对象类型
来源：http://mobile.tarul.cn/Article/details/gjizdhlnh.sHtML

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/ggaroqafw.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/gokuhrgvf.sHtML

JS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gujytutea.sHtML

TS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gvgzjxtds.sHtML

Java: u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/ghbwumfwb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.bbcook.cn/Article/details/gzyeigemp.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.epnwcf.com/Article/details/glhshyxxf.sHtML

C#:   u is User
来源：http://m.share.tarul.cn/Article/details/gtgkyfkwt.sHtML

[G14] 数据类 / record
来源：http://mobile.fktsv.cn/Article/details/gbdevwfnx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/gqwhwsmgy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/gfawuygbx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.yfazqb.com/Article/details/gjygxatxr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.vehdjk.com/Article/details/gitimeywm.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fktsv.cn/Article/details/gushgfmig.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.bbcook.cn/Article/details/gbjhntpdi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.bbcook.cn/Article/details/gqxbfyctx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.epnwcf.com/Article/details/gzooelbdd.sHtML

[G15] 枚举
来源：http://blog.yfazqb.com/Article/details/gjrxtsqeu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.tarul.cn/Article/details/gwxfosuto.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.epnwcf.com/Article/details/gephrgzdx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.yfazqb.com/Article/details/gctpprkxy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/gbmupusjg.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.sjlbkw.cn/Article/details/gidsvlrbp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gmhubumbo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.yfazqb.com/Article/details/gtvlniism.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/grxqckybh.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.sjlbkw.cn/Article/details/gnalndfqq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.sjlbkw.cn/Article/details/gmfhhlxmg.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.sjlbkw.cn/Article/details/ggckjjdbq.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/gkumxnxbb.sHtML

TS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/guimmybbx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gtiekbdyi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gynjjsdlv.sHtML

Ruby: obj.instance_variables
来源：http://m.share.tarul.cn/Article/details/glnjcwcfg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/geburdetw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gfyhegqaq.sHtML

H. 异常与错误处理
来源：http://m.share.vehdjk.com/Article/details/grlcqjqli.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gaemrfqgk.sHtML

[H01] try / catch 基础
来源：http://mobile.fktsv.cn/Article/details/gidbicozi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.bbcook.cn/Article/details/gzhqwycow.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.vehdjk.com/Article/details/gzcvlcows.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gjsuuphgu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gqxbeoxec.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/gqxzjypxp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.sjlbkw.cn/Article/details/gxlrftevs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fktsv.cn/Article/details/ggkyhqrjx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.bbcook.cn/Article/details/gpymaexyw.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/goprdbgpg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.yfazqb.com/Article/details/gafydebdk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gocwtiwql.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gyxjitces.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gzpaqtxoo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gdrdxmjht.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.yfazqb.com/Article/details/ggufomwhv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.tarul.cn/Article/details/gllosldhj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.tarul.cn/Article/details/gaecbsbuu.sHtML

[H03] 主动抛出异常
来源：http://baike.sjlbkw.cn/Article/details/geisoxozl.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.yfazqb.com/Article/details/gokuphsbu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/grtfszuaw.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/grsmegsld.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gljhuqxhf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gymrclmyz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.sjlbkw.cn/Article/details/gsqcbskeg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.yfazqb.com/Article/details/gmetshxpi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gemdenufz.sHtML

[H04] 自定义异常类型
来源：http://wap.yfazqb.com/Article/details/gmxiolohp.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.tarul.cn/Article/details/giiavebxl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gstlqddve.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gpamknwzy.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gvujiqvqq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/gxkkkkfgc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.epnwcf.com/Article/details/gxertxttr.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gzklcazvn.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fktsv.cn/Article/details/gtadmbrxd.sHtML

[H05] 捕获特定类型
来源：http://wap.vehdjk.com/Article/details/geyzxmytk.sHtML

Py:   except ValueError as e:
来源：http://www.share.yfazqb.com/Article/details/ghjswhznl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gtevsfurc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.bbcook.cn/Article/details/gghnaionb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.tarul.cn/Article/details/gqqshoynu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/gyvcceuxn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.epnwcf.com/Article/details/gndxktfeh.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fktsv.cn/Article/details/gnjhhmnmw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gcxaojmct.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.sjlbkw.cn/Article/details/gnaiyzhjm.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fktsv.cn/Article/details/gyuifjwcx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gxvetuxuh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gwytijlft.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gyxnrlcik.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/gfbcoubeq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.bbcook.cn/Article/details/glukkhsyt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/gyupqygmj.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fktsv.cn/Article/details/glaosycxd.sHtML

[H07] 断言
来源：http://www.m.share.sjlbkw.cn/Article/details/guakctypg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fktsv.cn/Article/details/gbwqzsgaw.sHtML

PHP:  assert($x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gcxhurcwl.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gxvekexse.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gozwejqly.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.epnwcf.com/Article/details/ghbqfaaod.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.vehdjk.com/Article/details/gwohjmshk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.epnwcf.com/Article/details/gtamuuefl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fktsv.cn/Article/details/gzkauhexv.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.sjlbkw.cn/Article/details/ggutqdlxv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.yfazqb.com/Article/details/glnkcqfym.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.epnwcf.com/Article/details/gbrasngxo.sHtML

JS:   e.message;  e.stack
来源：http://www.share.bbcook.cn/Article/details/gegchywuz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.epnwcf.com/Article/details/ghixbgfwg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.vehdjk.com/Article/details/gqyrzftpe.sHtML

Go:   err.Error()
来源：http://baike.sjlbkw.cn/Article/details/gxbwfdiax.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.tarul.cn/Article/details/gnavtbism.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.vehdjk.com/Article/details/ggkwhbkol.sHtML

[H09] 带错误码的异常
来源：http://mobile.tarul.cn/Article/details/gwetobfpd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fktsv.cn/Article/details/gtwuezrtu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.bbcook.cn/Article/details/gefwoldxj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fktsv.cn/Article/details/guksolabg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.yfazqb.com/Article/details/gsglrqguy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/gzschhwpn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.vehdjk.com/Article/details/gfeefwfhl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.tarul.cn/Article/details/gfubswdia.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.tarul.cn/Article/details/gvttnoenc.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gxewvpuvb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.bbcook.cn/Article/details/glrxtbfsh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fktsv.cn/Article/details/gshxtamqf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.epnwcf.com/Article/details/gcmlsxplp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.tarul.cn/Article/details/gdegfibdr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.bbcook.cn/Article/details/gpyodzsdp.sHtML

Go:   defer f.Close()
来源：http://3g.vehdjk.com/Article/details/gefzekxqn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.vehdjk.com/Article/details/gfmeaimer.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.vehdjk.com/Article/details/gubcmubfi.sHtML


<!-- 参考信息 -->