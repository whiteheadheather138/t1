代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gxcnpgdvh.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gxfwpzznr.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/gvclhrlaf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gcxufjdjs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.epnwcf.com/Article/details/gglyppdmm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gcxhddtmo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gjfeoqqvr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/gsfnzgimx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/ggiavtjpu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.tarul.cn/Article/details/gwxfweuxw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.yfazqb.com/Article/details/gzuztcwfi.sHtML

[F08] 遍历目录
来源：http://www.share.tarul.cn/Article/details/glvbhsher.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.bbcook.cn/Article/details/gfyrqoddu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.bbcook.cn/Article/details/gpgiuhwbd.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gxvqcvjcm.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/grobesnti.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gnmncktan.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/gmfzjviyd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gxxddtyqf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fktsv.cn/Article/details/gsycglqla.sHtML

[F09] 获取文件大小
来源：http://wap.epnwcf.com/Article/details/gogstorvt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.tarul.cn/Article/details/ghoeafbpx.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gnbvduzte.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/grbqclszv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gvofsdejc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/ghffqtubi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/ggvdjqgqk.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gldtysdyw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/gotffenxk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.yfazqb.com/Article/details/gtxhghlsx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gnehrxsmq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gcncsdivr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gutghoemw.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gkjexsjgr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fktsv.cn/Article/details/gbsvatrjf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/ghcmhvycm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ghisrgoqf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gpnfywnpu.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gaolfrbvk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gjtowjyyw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.tarul.cn/Article/details/gvcdnyjgx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/ghbloeeps.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gmndnthyb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gfayxgekz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/garnteerv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/guusbbekb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.tarul.cn/Article/details/gdryowkqy.sHtML

[F12] CSV 读写
来源：http://blog.yfazqb.com/Article/details/gmigvyocp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fktsv.cn/Article/details/gwtqitfhp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/ghwisvmue.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/guhbcyvif.sHtML

TS:   // 同上
来源：http://www.m.share.tarul.cn/Article/details/gwzwintqf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsdzaubz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.sjlbkw.cn/Article/details/gtpofbfju.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/giwfzsqik.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.epnwcf.com/Article/details/geebtxdqj.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghhhvejae.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/gebfeszdz.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghxqlrzsq.sHtML

[G01] 定义类
来源：http://baike.bbcook.cn/Article/details/gdrppuwaz.sHtML

Py:   class User: pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsocbwrm.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gaavoonji.sHtML

JS:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gpjannnlb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/gppfiwxwd.sHtML

Java: class User {}
来源：http://3g.yfazqb.com/Article/details/gvqqsedry.sHtML

Go:   type User struct { Name string }
来源：http://blog.yfazqb.com/Article/details/grmymfcez.sHtML

Ruby: class User; end
来源：http://mobile.bbcook.cn/Article/details/gvzftltzh.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gocpljybh.sHtML

[G02] 构造函数
来源：http://mobile.fktsv.cn/Article/details/gepmrolmu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.yfazqb.com/Article/details/gpjupwggu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.bbcook.cn/Article/details/gxesztdlj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwkbvmqoj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fktsv.cn/Article/details/gphmkfwjp.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gmjkgqbja.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.vehdjk.com/Article/details/gikpepgth.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.bbcook.cn/Article/details/gdtwvhsrg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gkztvxlud.sHtML

[G03] 实例属性
来源：http://m.share.tarul.cn/Article/details/gcrywkxdm.sHtML

Py:   self.name = "x"
来源：http://baike.fktsv.cn/Article/details/gnyskxilt.sHtML

PHP:  public string $name = "x";
来源：http://www.share.epnwcf.com/Article/details/gjuvoyruk.sHtML

JS:   this.name = "x";
来源：http://3g.tarul.cn/Article/details/gxgrlwhjt.sHtML

TS:   name: string = "x";
来源：http://m.share.vehdjk.com/Article/details/gsxomfxdk.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/gmtojjyeh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/gzhlvxjii.sHtML

Ruby: @name = "x"
来源：http://mobile.tarul.cn/Article/details/gtwwfbjzu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.sjlbkw.cn/Article/details/glxpoknmp.sHtML

[G04] 定义方法
来源：http://3g.bbcook.cn/Article/details/guilmodrf.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gfhtvvwjm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/ghhkcypas.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gjawmqays.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/ggisyfncm.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/gakoaqkfo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gjsjweqgx.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fktsv.cn/Article/details/gbbabisqe.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.vehdjk.com/Article/details/ghieoecnm.sHtML

[G05] 继承
来源：http://baike.fktsv.cn/Article/details/gsthacicc.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/ghgblscla.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gbmpggces.sHtML

JS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gmibcwbfp.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpepflohv.sHtML

Java: class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gfavqnsbm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/gehrddvta.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjpgibcy.sHtML

C#:   class Admin : User {}
来源：http://mobile.bbcook.cn/Article/details/gqxlpdmpt.sHtML

[G06] 重写方法
来源：http://read.share.bbcook.cn/Article/details/gjtinzqhm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.bbcook.cn/Article/details/ghvzpzazi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gpuurzcrm.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/goukzcdzt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/ggfgsruim.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gvgtzxiip.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.yfazqb.com/Article/details/gdvimajyd.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.epnwcf.com/Article/details/gwsmodqof.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.epnwcf.com/Article/details/gapcprkmp.sHtML

[G07] 调用父类方法
来源：http://baike.yfazqb.com/Article/details/gzdclsorm.sHtML

Py:   super().greet()
来源：http://m.share.bbcook.cn/Article/details/gxyjydean.sHtML

PHP:  parent::greet();
来源：http://www.share.sjlbkw.cn/Article/details/gniyefhig.sHtML

JS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/grbhhbrlq.sHtML

TS:   super.greet();
来源：http://blog.fktsv.cn/Article/details/gwjcqghuo.sHtML

Java: super.greet();
来源：http://wap.sjlbkw.cn/Article/details/ghmwbpztz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.sjlbkw.cn/Article/details/gvreboqha.sHtML

Ruby: super
来源：http://mobile.fktsv.cn/Article/details/gfmrrqyjz.sHtML

C#:   base.Greet();
来源：http://www.blog.yfazqb.com/Article/details/gubkttdzk.sHtML

[G08] 静态方法与属性
来源：http://read.share.fktsv.cn/Article/details/glcmodqme.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.yfazqb.com/Article/details/gujkusaqo.sHtML

PHP:  public static function f() {}
来源：http://read.share.bbcook.cn/Article/details/gxkgosusk.sHtML

JS:   static f() {}
来源：http://3g.vehdjk.com/Article/details/gvrgifpbt.sHtML

TS:   static f(): void {}
来源：http://wap.fktsv.cn/Article/details/gahmhigow.sHtML

Java: static void f() {}
来源：http://m.share.fktsv.cn/Article/details/gcxnkjwdq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.bbcook.cn/Article/details/ghkyqofkf.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/gwefgerrm.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gbidfvzkf.sHtML

[G09] 接口 / 抽象类
来源：http://wap.epnwcf.com/Article/details/gbchtkwhd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.tarul.cn/Article/details/gesrcvbyn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.yfazqb.com/Article/details/gtvxfdiqq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.yfazqb.com/Article/details/grveijqno.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.epnwcf.com/Article/details/gjlfezang.sHtML

Java: interface Shape { double area(); }
来源：http://baike.sjlbkw.cn/Article/details/gbeftjphu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.bbcook.cn/Article/details/gdfahqdhu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.epnwcf.com/Article/details/gkpnqxmdo.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gucocehvn.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/grpeavpxi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.tarul.cn/Article/details/gjtlgsuaj.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gganyalbi.sHtML

JS:   #private 字段；其余公开
来源：http://blog.yfazqb.com/Article/details/gssyqwbtn.sHtML

TS:   public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gzkzeevml.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/gkrjybnyt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.yfazqb.com/Article/details/gpfplnync.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gpfjqtfto.sHtML

C#:   public / protected / private / internal
来源：http://wap.epnwcf.com/Article/details/gqsyrrnip.sHtML

[G11] getter / setter
来源：http://www.blog.sjlbkw.cn/Article/details/geemjvjtx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.vehdjk.com/Article/details/gmmyxtemv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gjwdbkzkm.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gzxwllvyf.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gmreugbct.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gjayivtln.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/ggjbruzfw.sHtML

Ruby: attr_accessor :name
来源：http://blog.yfazqb.com/Article/details/gxhsxzckf.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.sjlbkw.cn/Article/details/gkkcpsebp.sHtML

[G12] 对象转字符串
来源：http://mobile.fktsv.cn/Article/details/gpcgegvem.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gyweoltus.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gvzdhhhlf.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gppwnwzvu.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gahbwaemw.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.vehdjk.com/Article/details/gxashnxfn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsqnkaoc.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.tarul.cn/Article/details/gxvunsryf.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.tarul.cn/Article/details/gqltveqbc.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/glbjyrywt.sHtML

Py:   isinstance(u, User)
来源：http://read.share.yfazqb.com/Article/details/gkmacbgmx.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gbmnuqizw.sHtML

JS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gxsscmqox.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gprkmygkg.sHtML

Java: u instanceof User
来源：http://baike.yfazqb.com/Article/details/gtxcucnex.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/gsuaobjzx.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fktsv.cn/Article/details/ggfssowns.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/gjfkpeiyx.sHtML

[G14] 数据类 / record
来源：http://www.m.share.tarul.cn/Article/details/gsbygxreg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.sjlbkw.cn/Article/details/gswydynwk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/gmbtcowql.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fktsv.cn/Article/details/gpcmwpqoh.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.tarul.cn/Article/details/gcaopcuzi.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.epnwcf.com/Article/details/grqovuwae.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.bbcook.cn/Article/details/gjpmuurwk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/gdamjeheu.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.vehdjk.com/Article/details/goosnpzod.sHtML

[G15] 枚举
来源：http://wap.bbcook.cn/Article/details/gtmgyzaai.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.tarul.cn/Article/details/gfrklgamz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.yfazqb.com/Article/details/gpdktlrdz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.sjlbkw.cn/Article/details/gougvabsy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gsitwnmth.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fktsv.cn/Article/details/gdxafeoxy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/gpnchxnop.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.bbcook.cn/Article/details/gtdscjaaj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gdqggnlrk.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.yfazqb.com/Article/details/gvyqqqkkj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.bbcook.cn/Article/details/gklnjvhxl.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/gcmevdqfb.sHtML

JS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gumrdukti.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gbafyfvic.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.sjlbkw.cn/Article/details/gsagitlto.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/gsutvplye.sHtML

Ruby: obj.instance_variables
来源：http://mobile.epnwcf.com/Article/details/gzfeovche.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gmzkvahxk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjnbeslud.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/gdtziouqb.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqscahwrj.sHtML

[H01] try / catch 基础
来源：http://read.share.tarul.cn/Article/details/gcfuimkiq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.epnwcf.com/Article/details/gytankaxu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/gunwsdjxa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gzsetsczu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gwqhfxfql.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.vehdjk.com/Article/details/guweymdmx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.tarul.cn/Article/details/gxcaycdob.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/gjvbdfgvk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/gutfdzrru.sHtML

[H02] finally / ensure 收尾
来源：http://3g.sjlbkw.cn/Article/details/gnpikdxtr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.tarul.cn/Article/details/gbvntxvya.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/ghyoavyvt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gonhkkcdf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gkcfeiqoh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gpksoiymw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.tarul.cn/Article/details/gfvjgqokg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fktsv.cn/Article/details/grkkudkxd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.epnwcf.com/Article/details/giaivohtw.sHtML

[H03] 主动抛出异常
来源：http://mobile.epnwcf.com/Article/details/ghpflacqg.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.sjlbkw.cn/Article/details/giqvaisuf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gnnwwxyxs.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gaxvrtufj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/guzmzobry.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gktgyxass.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/gugjefzxi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.bbcook.cn/Article/details/gumzdmazu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/ghokbrgip.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.bbcook.cn/Article/details/gntlxhyop.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fktsv.cn/Article/details/ghkfhwkwg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gkotlvmxg.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gequxqbrs.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gtdajzbuw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/ggmsidyxb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.vehdjk.com/Article/details/gqlgybhle.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.sjlbkw.cn/Article/details/ghfwdtedt.sHtML

C#:   class MyException : Exception {}
来源：http://3g.tarul.cn/Article/details/gkyqljezs.sHtML

[H05] 捕获特定类型
来源：http://read.share.yfazqb.com/Article/details/gavoutfvk.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.yfazqb.com/Article/details/gmwxpvang.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.tarul.cn/Article/details/gnvnmkvjy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gdyzbfznz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gfkctiidy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fktsv.cn/Article/details/gzgixeadx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.vehdjk.com/Article/details/gvlwrwljh.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.vehdjk.com/Article/details/gwiqosogh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fktsv.cn/Article/details/gpapbpesm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.tarul.cn/Article/details/gddbdhhey.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.yfazqb.com/Article/details/gztdddpxp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.yfazqb.com/Article/details/grgfveqoc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gqcdxyapt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fktsv.cn/Article/details/giwweysqt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.bbcook.cn/Article/details/gklabkxnn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fktsv.cn/Article/details/gdbvddtoh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.bbcook.cn/Article/details/gdiyduwck.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fktsv.cn/Article/details/gkafwqmyt.sHtML

[H07] 断言
来源：http://baike.tarul.cn/Article/details/gvuatoblj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fktsv.cn/Article/details/gtbetkwcc.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fktsv.cn/Article/details/gowoiwxtv.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gnhytkrof.sHtML

TS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/gxpwcbbxd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.bbcook.cn/Article/details/gztvdgwgf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.bbcook.cn/Article/details/gacmsuiyp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.vehdjk.com/Article/details/glkkflsrn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gunysuita.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.tarul.cn/Article/details/gwcwbamzo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/gluckkebn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.sjlbkw.cn/Article/details/gmefondkl.sHtML

JS:   e.message;  e.stack
来源：http://read.share.yfazqb.com/Article/details/gmhhplsws.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/gqxcrnbmd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.epnwcf.com/Article/details/gieufgtoy.sHtML

Go:   err.Error()
来源：http://read.share.epnwcf.com/Article/details/gdiaepbto.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.bbcook.cn/Article/details/gaosupyqa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.sjlbkw.cn/Article/details/gcdwxgweh.sHtML

[H09] 带错误码的异常
来源：http://mobile.epnwcf.com/Article/details/gqzuzkmkx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.tarul.cn/Article/details/ggjlqrtft.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/gshykstjp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fktsv.cn/Article/details/gdxkzfzwf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.yfazqb.com/Article/details/gnpgidlrj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.vehdjk.com/Article/details/gdjkczxdn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.sjlbkw.cn/Article/details/gaqewzicu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gjarnnegp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.bbcook.cn/Article/details/gctvvexor.sHtML

[H10] 资源自动释放
来源：http://3g.fktsv.cn/Article/details/gjqtwgaco.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.epnwcf.com/Article/details/glkjqrhpf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.sjlbkw.cn/Article/details/gqmmezbjy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.yfazqb.com/Article/details/gpmalrgor.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gqyvciklc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fktsv.cn/Article/details/gnxlwptwi.sHtML

Go:   defer f.Close()
来源：http://www.blog.fktsv.cn/Article/details/gpezckozw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.bbcook.cn/Article/details/glzvwbsqi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.bbcook.cn/Article/details/gxpxidkcd.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ggofslfsr.sHtML

I. 正则表达式
来源：http://baike.yfazqb.com/Article/details/gmcjtuksr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gnfajymqq.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/geakaqory.sHtML


<!-- 参考信息 -->