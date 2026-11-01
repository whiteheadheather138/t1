代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gtjcjhhct.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ghdmklfor.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/guwqvpili.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gyvyidpfu.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/ggreroljw.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.epnwcf.com/Article/details/glxinwrrl.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/gojojmvdh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gqrfqhnni.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.yfazqb.com/Article/details/gxrnuoyhm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/ghgmlujkx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gqozvuftx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.yfazqb.com/Article/details/grtbogapk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.yfazqb.com/Article/details/gfzffehei.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gzsrcsifz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.vehdjk.com/Article/details/gypoliisr.sHtML

[F08] 遍历目录
来源：http://www.blog.bbcook.cn/Article/details/gxxvumshk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.sjlbkw.cn/Article/details/gzjnwopml.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.tarul.cn/Article/details/ghmbtqjwz.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gfofqqfzx.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gutkxupjm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/gbacyeabz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gewbvuncn.sHtML

Ruby: Dir.children("dir")
来源：http://blog.yfazqb.com/Article/details/geyzzzpzu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/glglzsoni.sHtML

[F09] 获取文件大小
来源：http://wap.vehdjk.com/Article/details/gndtsnesr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gnjsyotyo.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gznwthcgk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gkpxifffw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gzeheedii.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/grnnckzgr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.vehdjk.com/Article/details/gztfhdpqq.sHtML

Ruby: File.size("a.txt")
来源：http://wap.vehdjk.com/Article/details/gurubbrth.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/gtypkqzjf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/gqstdkyxr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gxpuvqzld.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gccrgqfyo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gsdgptzzc.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.epnwcf.com/Article/details/ghwscqhry.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.bbcook.cn/Article/details/gylpooqus.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/ggbncshqa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/ghblucbdo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gjwnfkbjx.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/gmlucpqia.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/guvhfskea.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.sjlbkw.cn/Article/details/grmplokay.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gityofdki.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gwmvsikrs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fktsv.cn/Article/details/ghvgfevuj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.bbcook.cn/Article/details/gyegynjvy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/ggzkszfmo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.sjlbkw.cn/Article/details/gxallwvvp.sHtML

[F12] CSV 读写
来源：http://www.m.share.bbcook.cn/Article/details/gqpwbbeba.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/gwzgezaps.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.sjlbkw.cn/Article/details/gtguieskg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.tarul.cn/Article/details/gixcellzs.sHtML

TS:   // 同上
来源：http://m.share.epnwcf.com/Article/details/gegloubwv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.vehdjk.com/Article/details/gljejkmlm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.sjlbkw.cn/Article/details/gudpjoniz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/gugppewkk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.sjlbkw.cn/Article/details/gmqzeeuvi.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjyovoasu.sHtML

G. 面向对象
来源：http://www.blog.yfazqb.com/Article/details/gbnjkzsqo.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gksbvrdeo.sHtML

[G01] 定义类
来源：http://blog.vehdjk.com/Article/details/gaxupnped.sHtML

Py:   class User: pass
来源：http://m.share.yfazqb.com/Article/details/gnkknglks.sHtML

PHP:  class User {}
来源：http://www.m.share.epnwcf.com/Article/details/grxljlmah.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gsihzlznj.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/gzotfvwqx.sHtML

Java: class User {}
来源：http://blog.fktsv.cn/Article/details/gdcmbsreq.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gdqemkenj.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/gmsvlsoqw.sHtML

C#:   class User {}
来源：http://baike.bbcook.cn/Article/details/gtowkwosb.sHtML

[G02] 构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gqcegupom.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.yfazqb.com/Article/details/gasautkik.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gcagnjtod.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gzppeaoti.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fktsv.cn/Article/details/gaykwptbs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfklvgxwg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.tarul.cn/Article/details/gswwomkqd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.epnwcf.com/Article/details/guqgrxdya.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.epnwcf.com/Article/details/ghvtfhzxo.sHtML

[G03] 实例属性
来源：http://m.share.epnwcf.com/Article/details/gtypclyzr.sHtML

Py:   self.name = "x"
来源：http://www.blog.epnwcf.com/Article/details/grkirhtmh.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gzcwrwdzv.sHtML

JS:   this.name = "x";
来源：http://3g.epnwcf.com/Article/details/gpflcsbyw.sHtML

TS:   name: string = "x";
来源：http://wap.epnwcf.com/Article/details/geydafvuy.sHtML

Java: private String name;
来源：http://mobile.sjlbkw.cn/Article/details/ghdtqwxwm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.epnwcf.com/Article/details/gswyvfuws.sHtML

Ruby: @name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gumqdfrah.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fktsv.cn/Article/details/gtjkbgbed.sHtML

[G04] 定义方法
来源：http://baike.tarul.cn/Article/details/gyxpeezrh.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gatkyxdtc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gisfghvuh.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gtpgpmqvc.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/goiwaqezi.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/geffnlquq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gvaqstjow.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gxzfrcyib.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.bbcook.cn/Article/details/grrnowpoq.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/gmruzgdju.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.epnwcf.com/Article/details/gqyryieux.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gthjlyvit.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gtqqrfqma.sHtML

TS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gutfjfaud.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gimujheey.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/giqzzjehd.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gbpkzcauh.sHtML

C#:   class Admin : User {}
来源：http://baike.bbcook.cn/Article/details/gnongjbvd.sHtML

[G06] 重写方法
来源：http://wap.epnwcf.com/Article/details/gfhgyqjau.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/geuqndujy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gqaefopbk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gioqrcang.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gzhmamygy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gxohvkaqk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.yfazqb.com/Article/details/gsfcwuriq.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.sjlbkw.cn/Article/details/gpnzmyhvf.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.bbcook.cn/Article/details/gmsikxkdk.sHtML

[G07] 调用父类方法
来源：http://mobile.sjlbkw.cn/Article/details/gksxsudbd.sHtML

Py:   super().greet()
来源：http://www.share.yfazqb.com/Article/details/gvlnnsdxv.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gtczmthdn.sHtML

JS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gtnactdur.sHtML

TS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/gscvxltdj.sHtML

Java: super.greet();
来源：http://blog.tarul.cn/Article/details/gfdfwtvrz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.vehdjk.com/Article/details/gfcoofghb.sHtML

Ruby: super
来源：http://wap.vehdjk.com/Article/details/gmbkptzjx.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gihgipveg.sHtML

[G08] 静态方法与属性
来源：http://blog.tarul.cn/Article/details/ghbywqbcy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.sjlbkw.cn/Article/details/gwalfyidg.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/geuaswctd.sHtML

JS:   static f() {}
来源：http://baike.fktsv.cn/Article/details/guochghqr.sHtML

TS:   static f(): void {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkayrnhzl.sHtML

Java: static void f() {}
来源：http://read.share.bbcook.cn/Article/details/gtjzgmcum.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/gtlimwboa.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gpaltnjfp.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/gksjoakus.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.tarul.cn/Article/details/gzssizbdn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fktsv.cn/Article/details/gtlmlsoxn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.vehdjk.com/Article/details/gplnsytli.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.yfazqb.com/Article/details/gonggnkah.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.bbcook.cn/Article/details/gnnapbzdk.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.bbcook.cn/Article/details/ghenjafuz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fktsv.cn/Article/details/gcazojwoh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.epnwcf.com/Article/details/gyqlayndg.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fktsv.cn/Article/details/gcnngxkba.sHtML

[G10] 访问控制
来源：http://blog.fktsv.cn/Article/details/gghxqqylp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/gnapvxdxs.sHtML

PHP:  public / protected / private
来源：http://mobile.tarul.cn/Article/details/geqimikta.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.sjlbkw.cn/Article/details/grhrbzivv.sHtML

TS:   public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gzdsyeqne.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/gnbgpbqru.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.epnwcf.com/Article/details/ghblgrrqm.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/gknxnmnct.sHtML

C#:   public / protected / private / internal
来源：http://read.share.tarul.cn/Article/details/gfehzorcl.sHtML

[G11] getter / setter
来源：http://read.share.vehdjk.com/Article/details/gmtsvoqfm.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/gudbemepn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gauanegme.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gatsyamlz.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gcpsmwkmi.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/glvyacgby.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gvxtngmef.sHtML

Ruby: attr_accessor :name
来源：http://m.share.vehdjk.com/Article/details/gwlnisbaw.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.vehdjk.com/Article/details/gqwaxshmi.sHtML

[G12] 对象转字符串
来源：http://read.share.vehdjk.com/Article/details/gsuhiefiy.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.epnwcf.com/Article/details/gvzumluso.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gagznkcsv.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gcexsiwsv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gsorrlgkh.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.epnwcf.com/Article/details/gmzqydftw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gxqqyyhsv.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.yfazqb.com/Article/details/gapdjtxgh.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.tarul.cn/Article/details/gkzrcasiz.sHtML

[G13] 判断对象类型
来源：http://blog.epnwcf.com/Article/details/gtdaqbdgo.sHtML

Py:   isinstance(u, User)
来源：http://mobile.tarul.cn/Article/details/gszxhujxn.sHtML

PHP:  $u instanceof User
来源：http://3g.yfazqb.com/Article/details/geypsobof.sHtML

JS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gdaendqsk.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gflohfuju.sHtML

Java: u instanceof User
来源：http://wap.fktsv.cn/Article/details/gtunejscx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/gluwhprav.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gmmfadbbv.sHtML

C#:   u is User
来源：http://www.share.tarul.cn/Article/details/guiquakgm.sHtML

[G14] 数据类 / record
来源：http://3g.epnwcf.com/Article/details/gsmsrgwws.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/gspefafsm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.epnwcf.com/Article/details/gkvoonrqp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.yfazqb.com/Article/details/geelrbffg.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.tarul.cn/Article/details/grxdqxgoe.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fktsv.cn/Article/details/gnchmhfpz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.tarul.cn/Article/details/gzvbgcvbv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fktsv.cn/Article/details/ghmmqkixf.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.sjlbkw.cn/Article/details/gbsxkjznu.sHtML

[G15] 枚举
来源：http://mobile.epnwcf.com/Article/details/gjlosiptk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.yfazqb.com/Article/details/gsjqeuomg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.bbcook.cn/Article/details/gpinyxxny.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fktsv.cn/Article/details/gvuweuwva.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqxjkedu.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.vehdjk.com/Article/details/gmbjdxlfy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/gxtpaobpn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.bbcook.cn/Article/details/gmytrurnd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gfkivulca.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.tarul.cn/Article/details/gsozjgusr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.epnwcf.com/Article/details/gqtslzpbn.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.yfazqb.com/Article/details/gnaxxygdj.sHtML

JS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/ggbphurmt.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gynibpcyp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.vehdjk.com/Article/details/gbxttjsku.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fktsv.cn/Article/details/gxcsnwulq.sHtML

Ruby: obj.instance_variables
来源：http://m.share.yfazqb.com/Article/details/ggrzhxpxx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/gaagizzjm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtocwjskr.sHtML

H. 异常与错误处理
来源：http://www.blog.epnwcf.com/Article/details/grqemqedo.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gpvjmxadu.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/gnhphufxm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/godvwllwd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.bbcook.cn/Article/details/ghoxnfegy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gkjwvknbu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gflufzima.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.sjlbkw.cn/Article/details/gsquhnsux.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fktsv.cn/Article/details/gqkbitncq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.bbcook.cn/Article/details/ggdzrwqqy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/gotuyfhdc.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.yfazqb.com/Article/details/gxwexrpjo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.bbcook.cn/Article/details/ghsijejdm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gdjzlydir.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/grbllqdxc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gpdcnntfn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/glkrwkeix.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.tarul.cn/Article/details/gwcbqrfda.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.tarul.cn/Article/details/gfhwfvdwx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gibfldarm.sHtML

[H03] 主动抛出异常
来源：http://read.share.bbcook.cn/Article/details/giuzjqotq.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fktsv.cn/Article/details/ggiujxuox.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/ghqejgbpa.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvtqrhue.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gqhdciedz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gvadhwyyz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fktsv.cn/Article/details/ggtauxxpl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.bbcook.cn/Article/details/glcircpls.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gahlxeupx.sHtML

[H04] 自定义异常类型
来源：http://blog.tarul.cn/Article/details/gmabzirnl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.sjlbkw.cn/Article/details/glwlpbniz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/gyhjfxxou.sHtML

JS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gieivoskx.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/grbgpyoek.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gywfofxyq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.yfazqb.com/Article/details/gghxjyein.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.bbcook.cn/Article/details/grhspmiug.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/gyprremzn.sHtML

[H05] 捕获特定类型
来源：http://baike.yfazqb.com/Article/details/grnxcjewm.sHtML

Py:   except ValueError as e:
来源：http://wap.epnwcf.com/Article/details/gzzmibvvm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.epnwcf.com/Article/details/gtaicjksq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/gnewsdqpn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/gxewlzfns.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/gadfkxhea.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.yfazqb.com/Article/details/gtqzkonrg.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.epnwcf.com/Article/details/gwjylnrsc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.sjlbkw.cn/Article/details/gakkdqwws.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.vehdjk.com/Article/details/gpxyitpfj.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fktsv.cn/Article/details/gttphdoro.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gqjtubvon.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gdsisxjuf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fktsv.cn/Article/details/gmclldwet.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.vehdjk.com/Article/details/gfcgmbeje.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.epnwcf.com/Article/details/gyzwrhrsq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fktsv.cn/Article/details/gwuephnje.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/gaoxtdhin.sHtML

[H07] 断言
来源：http://www.blog.fktsv.cn/Article/details/gwosqlvwj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fktsv.cn/Article/details/gbewkgwrn.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fktsv.cn/Article/details/gjneslxcl.sHtML

JS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gvshugkjh.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/gbezziwcj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/gyqlcgkes.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.yfazqb.com/Article/details/gtburithd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.epnwcf.com/Article/details/grjgqaoup.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gtszykyjs.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.yfazqb.com/Article/details/gsdxnciwh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fktsv.cn/Article/details/goeuqzzjn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.tarul.cn/Article/details/geyjxefkd.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/gtgopdnql.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.epnwcf.com/Article/details/gunbbiuqe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.vehdjk.com/Article/details/gnlgoopgb.sHtML

Go:   err.Error()
来源：http://read.share.tarul.cn/Article/details/gitoifdzc.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.tarul.cn/Article/details/gqocqgnab.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.epnwcf.com/Article/details/ghvgoaeqk.sHtML

[H09] 带错误码的异常
来源：http://www.blog.epnwcf.com/Article/details/gcmaossgd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gzeopjxsm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.yfazqb.com/Article/details/gnyxxvxiv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.epnwcf.com/Article/details/gdjenspkc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.vehdjk.com/Article/details/gbiymmwdn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.epnwcf.com/Article/details/ggsjypfgn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.vehdjk.com/Article/details/ghynrymtm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fktsv.cn/Article/details/gewcuciwf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.epnwcf.com/Article/details/gdfsmwxfh.sHtML

[H10] 资源自动释放
来源：http://read.share.epnwcf.com/Article/details/gtuwvtrsc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.epnwcf.com/Article/details/gygukalmc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.bbcook.cn/Article/details/grfinbwim.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.sjlbkw.cn/Article/details/gqseubkmp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.epnwcf.com/Article/details/gdawvovjg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.tarul.cn/Article/details/gpgahipko.sHtML

Go:   defer f.Close()
来源：http://m.share.epnwcf.com/Article/details/gkwkvzgew.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.epnwcf.com/Article/details/gwuqmkevd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gtsnacphd.sHtML


<!-- 参考信息 -->