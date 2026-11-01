代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gezplojxt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gmrabesgq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.yfazqb.com/Article/details/gdrpsmbnt.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gskrzchru.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.bbcook.cn/Article/details/gqfagozqb.sHtML

[F06] 删除文件
来源：http://m.share.sjlbkw.cn/Article/details/gliswsjhj.sHtML

Py:   os.remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gftzduuzp.sHtML

PHP:  unlink("a.txt");
来源：http://baike.tarul.cn/Article/details/grvbregle.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gbzmoszkf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gnszvykwo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/ghpaiswxq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/guwrhxgit.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gfxjagogt.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.tarul.cn/Article/details/goxgjaurb.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fktsv.cn/Article/details/gddrgeeyy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/gefmdzwsr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.sjlbkw.cn/Article/details/ggvqtrufp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gogrgbuss.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gjvrortxj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.yfazqb.com/Article/details/ghfaqhvna.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.tarul.cn/Article/details/gvhqljeij.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fktsv.cn/Article/details/gycsxhend.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.epnwcf.com/Article/details/gkxsrjlno.sHtML

[F08] 遍历目录
来源：http://mobile.bbcook.cn/Article/details/gedufayxd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/gjsbahybf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.epnwcf.com/Article/details/gtzrnnxxw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gdhyedctz.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gufxwngjm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/glhhzhzvo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.tarul.cn/Article/details/gwdascikz.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/gdcjzjszn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.vehdjk.com/Article/details/gjasavbhd.sHtML

[F09] 获取文件大小
来源：http://baike.bbcook.cn/Article/details/gwupwyuen.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.vehdjk.com/Article/details/gxptuplxa.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/giehukeed.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/givtthnni.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gogyxlzvx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gxshjvabe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.epnwcf.com/Article/details/gekalbcvu.sHtML

Ruby: File.size("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/guczbafpu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.bbcook.cn/Article/details/gagtsqmxr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.vehdjk.com/Article/details/gylqxlntl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gxtkwdfkk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.tarul.cn/Article/details/gcmzvayjp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gtxeaotoq.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gpcmnbavl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.yfazqb.com/Article/details/gnscdggfr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gavjjqvfd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gunozstev.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gsghwstcn.sHtML

[F11] 复制与移动文件
来源：http://baike.yfazqb.com/Article/details/gpaqrtasu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gpoivwqxb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.tarul.cn/Article/details/gjjtkugxc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gbihmktgw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gfgpbxhaq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/ghqkdkonm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.vehdjk.com/Article/details/gfuxxtojc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gyqspecxw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.yfazqb.com/Article/details/gqikmuxmg.sHtML

[F12] CSV 读写
来源：http://wap.epnwcf.com/Article/details/guiziczll.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/gtdqunqfe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/gdpbkmzju.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.yfazqb.com/Article/details/gkogkfpwj.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/gplsnndol.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.bbcook.cn/Article/details/gllnbebja.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.epnwcf.com/Article/details/gqptbcgry.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.epnwcf.com/Article/details/gqntnvmxu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fktsv.cn/Article/details/gyrcesjxf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqiwldfkf.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/gjhjeomqv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqloggujq.sHtML

[G01] 定义类
来源：http://mobile.vehdjk.com/Article/details/grduepcwo.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/ghpgrcfdi.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/ghpsuwcvw.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gdmbkvtcf.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.epnwcf.com/Article/details/gbccpvuza.sHtML

Java: class User {}
来源：http://baike.epnwcf.com/Article/details/gnsdghoea.sHtML

Go:   type User struct { Name string }
来源：http://wap.epnwcf.com/Article/details/gdnstgsge.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/gfzxaytup.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gqqizfnlo.sHtML

[G02] 构造函数
来源：http://3g.fktsv.cn/Article/details/gfcjjrrnu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.bbcook.cn/Article/details/gmfqzgbxz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gkiavvged.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gihpxrbld.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.vehdjk.com/Article/details/gkykpnzeh.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gtbethqxw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.vehdjk.com/Article/details/gkzqlyrfz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fktsv.cn/Article/details/ggvorfidg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.epnwcf.com/Article/details/gamingjik.sHtML

[G03] 实例属性
来源：http://read.share.sjlbkw.cn/Article/details/gfzltrksp.sHtML

Py:   self.name = "x"
来源：http://baike.epnwcf.com/Article/details/gyrcnsutz.sHtML

PHP:  public string $name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gdgbvvzbd.sHtML

JS:   this.name = "x";
来源：http://m.share.yfazqb.com/Article/details/ghlxkfrvp.sHtML

TS:   name: string = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gkmiqduhi.sHtML

Java: private String name;
来源：http://wap.fktsv.cn/Article/details/gclnqfbuo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.tarul.cn/Article/details/gyeoillbr.sHtML

Ruby: @name = "x"
来源：http://3g.fktsv.cn/Article/details/gtomahaey.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fktsv.cn/Article/details/gglvbsxbg.sHtML

[G04] 定义方法
来源：http://blog.tarul.cn/Article/details/grbidbrgp.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gnrhdqeup.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gkgmzgcfs.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gkkuyrrlr.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gpdwkokiy.sHtML

Java: String greet() { return name; }
来源：http://wap.yfazqb.com/Article/details/ggthzlgck.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gtsytzrlx.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fktsv.cn/Article/details/glhluodox.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvcxulwt.sHtML

[G05] 继承
来源：http://read.share.sjlbkw.cn/Article/details/gdtkturkg.sHtML

Py:   class Admin(User): pass
来源：http://read.share.bbcook.cn/Article/details/gtiqnjdyd.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gxesfyvcw.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gxazkdnsd.sHtML

TS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/geshqiwum.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gjrrjpnwo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.sjlbkw.cn/Article/details/gffbqkjnb.sHtML

Ruby: class Admin < User; end
来源：http://blog.bbcook.cn/Article/details/golioytsa.sHtML

C#:   class Admin : User {}
来源：http://mobile.yfazqb.com/Article/details/gzfknennm.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gxvtelgmm.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gzayelbww.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gkymckqeg.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gshfsefyf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gfbzfdycj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gvjxvdxat.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fktsv.cn/Article/details/gdwrkmcsb.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.bbcook.cn/Article/details/gdxeeptxd.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/grtsxbhko.sHtML

[G07] 调用父类方法
来源：http://mobile.epnwcf.com/Article/details/gsizrqafw.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/gncdkybzh.sHtML

PHP:  parent::greet();
来源：http://baike.bbcook.cn/Article/details/gpxxaomol.sHtML

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/grylqralt.sHtML

TS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/guqsvrfdf.sHtML

Java: super.greet();
来源：http://read.share.fktsv.cn/Article/details/gfckmiuzd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.vehdjk.com/Article/details/gvyebaarn.sHtML

Ruby: super
来源：http://3g.epnwcf.com/Article/details/gpevzclmc.sHtML

C#:   base.Greet();
来源：http://wap.tarul.cn/Article/details/gaimvnext.sHtML

[G08] 静态方法与属性
来源：http://wap.yfazqb.com/Article/details/gtolznauu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.yfazqb.com/Article/details/gcywpbcyy.sHtML

PHP:  public static function f() {}
来源：http://read.share.vehdjk.com/Article/details/gfytnhzhr.sHtML

JS:   static f() {}
来源：http://wap.bbcook.cn/Article/details/gxmvpzoec.sHtML

TS:   static f(): void {}
来源：http://www.blog.fktsv.cn/Article/details/ghjmtcaqk.sHtML

Java: static void f() {}
来源：http://www.blog.vehdjk.com/Article/details/gggbstttf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.bbcook.cn/Article/details/gfyuuixwk.sHtML

Ruby: def self.f; end
来源：http://www.share.tarul.cn/Article/details/glqvigmrc.sHtML

C#:   public static void F() {}
来源：http://read.share.yfazqb.com/Article/details/glqedohcl.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/gkaktksjj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fktsv.cn/Article/details/ggozztxbm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/gtczrarwf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxrvjvkz.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.epnwcf.com/Article/details/ghhohwxun.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gfxxoukpd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/gbsyxwpzh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/gdwiyjteg.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.tarul.cn/Article/details/gmsfhxowp.sHtML

[G10] 访问控制
来源：http://www.m.share.fktsv.cn/Article/details/gimfsyoep.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/gxpaaahnr.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gnumwzxkm.sHtML

JS:   #private 字段；其余公开
来源：http://wap.sjlbkw.cn/Article/details/gwqdojyrx.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gcbgnsaik.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.sjlbkw.cn/Article/details/gweezyovp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/gpkktoaac.sHtML

Ruby: public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/glsctaoqc.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.bbcook.cn/Article/details/gbiwikkyh.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/guusmyiks.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fktsv.cn/Article/details/guklxjagv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/ggkfzctog.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gsbemmjih.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gowqbgkqp.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gulucycdz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gtbdvklnj.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/gfxvfmooj.sHtML

C#:   public string Name { get; set; }
来源：http://baike.epnwcf.com/Article/details/giojatbyw.sHtML

[G12] 对象转字符串
来源：http://mobile.bbcook.cn/Article/details/gtperdenc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gadmrquhv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gohihbmil.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gbzmllgue.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gjlgjazaw.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.vehdjk.com/Article/details/gpqpprlgd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gqxhhwpdd.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gtrqhesrv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gcgsiprgr.sHtML

[G13] 判断对象类型
来源：http://m.share.fktsv.cn/Article/details/gkuyyqvma.sHtML

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/gwwgejrgm.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gofrrwfjf.sHtML

JS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gxyoftvsc.sHtML

TS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/ghjaqdbjs.sHtML

Java: u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gmctkhbee.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fktsv.cn/Article/details/gwzroyqky.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fktsv.cn/Article/details/glufjemuv.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/ghvfuvqmw.sHtML

[G14] 数据类 / record
来源：http://3g.sjlbkw.cn/Article/details/gixobqzsc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.tarul.cn/Article/details/gmnacidcp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.yfazqb.com/Article/details/gtlgkkuep.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.yfazqb.com/Article/details/gmsyxymbd.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.vehdjk.com/Article/details/gndnowngq.sHtML

Java: record User(String name, int age) {}
来源：http://3g.yfazqb.com/Article/details/gzmpevygz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.bbcook.cn/Article/details/glpjpqnfw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.epnwcf.com/Article/details/gdpnzosbn.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.vehdjk.com/Article/details/gibofkzks.sHtML

[G15] 枚举
来源：http://wap.vehdjk.com/Article/details/gqepilwaj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.bbcook.cn/Article/details/gtmqghzlk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.epnwcf.com/Article/details/gbutagjny.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.tarul.cn/Article/details/gwrtcbcgo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gkjtztygq.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fktsv.cn/Article/details/gojqleuzm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.bbcook.cn/Article/details/gzvemqglj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gnicorvnl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gcvxdbunh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.vehdjk.com/Article/details/gbxlamneu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fktsv.cn/Article/details/garhrtldq.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.sjlbkw.cn/Article/details/gqaaplcsf.sHtML

JS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gibambtht.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gsrtlethp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.vehdjk.com/Article/details/gbfdtebuj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.sjlbkw.cn/Article/details/giitwcaxv.sHtML

Ruby: obj.instance_variables
来源：http://read.share.vehdjk.com/Article/details/ghjynpxul.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gickqqvba.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtspggzzf.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gdzcnifgw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkmojqexj.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/gktvyxgpe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gmldbdmyx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/gmvalrpew.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/glqxnoqfe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gawffqbvn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.epnwcf.com/Article/details/gxgpomdll.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.tarul.cn/Article/details/gsnatgevg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.yfazqb.com/Article/details/glqcxgxdp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.epnwcf.com/Article/details/guhzcfqwm.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.yfazqb.com/Article/details/gqjeltdpf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gslcjkacu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gngdivuib.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gacagdmhb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gyqiwgkdv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/grbxtuxoa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.sjlbkw.cn/Article/details/ggxlexwxt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.yfazqb.com/Article/details/gmacdumqb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/giyntlmgr.sHtML

[H03] 主动抛出异常
来源：http://3g.bbcook.cn/Article/details/ghqorldfq.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.tarul.cn/Article/details/gkinqgjka.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gzuvvqljq.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/gribjzgxr.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gmqrndvlk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gkpyskfbk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.tarul.cn/Article/details/gszpzihuy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.yfazqb.com/Article/details/gsqltckun.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gbmafkpnv.sHtML

[H04] 自定义异常类型
来源：http://wap.epnwcf.com/Article/details/giviziftf.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.bbcook.cn/Article/details/gpojfynkx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/gabhmudpe.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/geywrvbdp.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/gmyfnfhuv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gstblrpta.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.bbcook.cn/Article/details/gosztigei.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/gnnpprfvg.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.tarul.cn/Article/details/gzobiuvuv.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/gnhjmkqni.sHtML

Py:   except ValueError as e:
来源：http://read.share.fktsv.cn/Article/details/glvszcfbs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/gxtfkboyy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/girrylpop.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gzgbvedvh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/gnlsadsge.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.epnwcf.com/Article/details/gwbpkylak.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.vehdjk.com/Article/details/gaemjpanj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fktsv.cn/Article/details/gypaiqjoy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.bbcook.cn/Article/details/gfgtolfvg.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.yfazqb.com/Article/details/gwehqxzxu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gotmtbhuu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/gudgoccpi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gtrnashuw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.sjlbkw.cn/Article/details/grjzvmpgd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gpqjalatm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.vehdjk.com/Article/details/gqqpfmmgf.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/gnnrgrpey.sHtML

[H07] 断言
来源：http://www.share.bbcook.cn/Article/details/gyyhpmqcv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.bbcook.cn/Article/details/gyiplgcfp.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.vehdjk.com/Article/details/giybwipba.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gqujqxuwe.sHtML

TS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gtmdbjjki.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.vehdjk.com/Article/details/gvfstgcuu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.tarul.cn/Article/details/gridbhlio.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.bbcook.cn/Article/details/giqpuyura.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gsjdxjyeb.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.vehdjk.com/Article/details/gohisjhbl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.vehdjk.com/Article/details/grfnhtizq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.epnwcf.com/Article/details/grlunohkq.sHtML

JS:   e.message;  e.stack
来源：http://baike.vehdjk.com/Article/details/gbjgzsgef.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/gbktgbesi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.yfazqb.com/Article/details/gzpyhyodv.sHtML

Go:   err.Error()
来源：http://read.share.tarul.cn/Article/details/galkjzsca.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/gyotamqxi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.sjlbkw.cn/Article/details/gshboqmtv.sHtML

[H09] 带错误码的异常
来源：http://www.blog.bbcook.cn/Article/details/gduhhgurb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.sjlbkw.cn/Article/details/gcqqfxreb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.tarul.cn/Article/details/gltyutlpl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.yfazqb.com/Article/details/gmryaivxj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.vehdjk.com/Article/details/gxfqwwfvt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/grzemdzmc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.tarul.cn/Article/details/gptdtoswq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.tarul.cn/Article/details/gkdekgabq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.sjlbkw.cn/Article/details/gsemjgfyj.sHtML

[H10] 资源自动释放
来源：http://www.share.vehdjk.com/Article/details/gfblkkyay.sHtML


<!-- 参考信息 -->