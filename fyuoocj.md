代发 wailian999

C#:   File.Exists("a.txt")
来源：http://m.share.yfazqb.com/Article/details/ghgvbirhy.sHtML

[F06] 删除文件
来源：http://read.share.vehdjk.com/Article/details/gwajtngii.sHtML

Py:   os.remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/ghdeiqhba.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/gslicxksz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gdpclzeio.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/glulrocud.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gcmfrumzl.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gmvfbrmxk.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.bbcook.cn/Article/details/gogebzuzf.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gnulnnkyy.sHtML

[F07] 创建目录（含多级）
来源：http://baike.vehdjk.com/Article/details/gwqlzrjjj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/glhrafmft.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fktsv.cn/Article/details/gnmozhgof.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/gviqbamqa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gdhxlmxeg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.vehdjk.com/Article/details/gumioinde.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.sjlbkw.cn/Article/details/gzkzgfekj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.sjlbkw.cn/Article/details/gwhbemlum.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.tarul.cn/Article/details/gzpkcsgyt.sHtML

[F08] 遍历目录
来源：http://wap.sjlbkw.cn/Article/details/gidknxuad.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsuvpiac.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fktsv.cn/Article/details/gdviyhisj.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gxcoplaaw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gcofmwupe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gyagzjjfp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.vehdjk.com/Article/details/gjojhphiw.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fktsv.cn/Article/details/groohotcl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/gzctgabrp.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gawksicvp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gnoidouoi.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/ggrfkdmch.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gfhmkeolk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gqabcoksh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gqucumrgn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.epnwcf.com/Article/details/gxpmceuvj.sHtML

Ruby: File.size("a.txt")
来源：http://3g.bbcook.cn/Article/details/gyuafnbyb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.epnwcf.com/Article/details/gycohxadw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.tarul.cn/Article/details/giftolgca.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gsyjaisvd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/gctmklwat.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gfawmdmil.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fktsv.cn/Article/details/gfcyzhkhb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.yfazqb.com/Article/details/glayidxqa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/grwkmbmco.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gylisxbzj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gpbkrablj.sHtML

[F11] 复制与移动文件
来源：http://www.blog.tarul.cn/Article/details/gqeycqnur.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/glqdumznm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gyituzoxz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/ggwfrlfwa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gbyasudgn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gavlprbfi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.vehdjk.com/Article/details/gzwjbppbx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gkhrgunfq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gdlcehicr.sHtML

[F12] CSV 读写
来源：http://m.share.vehdjk.com/Article/details/gbnfccequ.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.tarul.cn/Article/details/gsmyohpxy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.yfazqb.com/Article/details/gbmmspahk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fktsv.cn/Article/details/gnwwtrbwq.sHtML

TS:   // 同上
来源：http://mobile.sjlbkw.cn/Article/details/grhopjlon.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gxkjyyrnp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.sjlbkw.cn/Article/details/giezckeah.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.tarul.cn/Article/details/gelfwblog.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/grnnhefdg.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gfbqdmbby.sHtML

G. 面向对象
来源：http://blog.epnwcf.com/Article/details/ggnychgys.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtwueslzd.sHtML

[G01] 定义类
来源：http://www.blog.fktsv.cn/Article/details/gxgkzesmt.sHtML

Py:   class User: pass
来源：http://www.blog.yfazqb.com/Article/details/gkhovscxg.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/gwzcszqfo.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gfyzvamhu.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/gtukicpzz.sHtML

Java: class User {}
来源：http://wap.tarul.cn/Article/details/gpicdceyf.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/gtfabfwpp.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gqlvtlpgu.sHtML

C#:   class User {}
来源：http://baike.vehdjk.com/Article/details/gxgwzsihl.sHtML

[G02] 构造函数
来源：http://www.blog.vehdjk.com/Article/details/grmwcltbv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gresvvdae.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/gxmbsipkq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gasvahwbl.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/gbtcpdmbr.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gvaabnrqp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.yfazqb.com/Article/details/gilksduqf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fktsv.cn/Article/details/gpaxasfvr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/grqvzjmrh.sHtML

[G03] 实例属性
来源：http://baike.epnwcf.com/Article/details/gfxdcmhhb.sHtML

Py:   self.name = "x"
来源：http://www.blog.tarul.cn/Article/details/gmpjzlhvv.sHtML

PHP:  public string $name = "x";
来源：http://blog.yfazqb.com/Article/details/gpnxzgxor.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gbejuvrgc.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/gfrfbavga.sHtML

Java: private String name;
来源：http://www.m.share.fktsv.cn/Article/details/gvzzoxsvv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/grxmmlqts.sHtML

Ruby: @name = "x"
来源：http://mobile.epnwcf.com/Article/details/gibqemymw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.vehdjk.com/Article/details/geyhhxqgy.sHtML

[G04] 定义方法
来源：http://www.share.sjlbkw.cn/Article/details/gniucwgys.sHtML

Py:   def greet(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gggsvhxvw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gfycsomjr.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/geaxnutry.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gsgfsecnc.sHtML

Java: String greet() { return name; }
来源：http://3g.vehdjk.com/Article/details/ghhrczbat.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gogejzfxi.sHtML

Ruby: def greet; @name; end
来源：http://read.share.epnwcf.com/Article/details/gdthslnpq.sHtML

C#:   public string Greet() => Name;
来源：http://wap.bbcook.cn/Article/details/gnbexpdiu.sHtML

[G05] 继承
来源：http://blog.yfazqb.com/Article/details/gbgunjjqu.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.bbcook.cn/Article/details/gszridcca.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gejofzmgf.sHtML

JS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gsvhraghf.sHtML

TS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gbdajyqqt.sHtML

Java: class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gmzqhdiks.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.epnwcf.com/Article/details/gsfohjmsc.sHtML

Ruby: class Admin < User; end
来源：http://blog.epnwcf.com/Article/details/ggnrhrcac.sHtML

C#:   class Admin : User {}
来源：http://blog.sjlbkw.cn/Article/details/gnpekvwyi.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/gcwgdxcxm.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.tarul.cn/Article/details/goqiscnvn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gdujpqcfb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/ggscuwsqo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/guueheuzw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gginkefna.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gpmnsjepi.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.epnwcf.com/Article/details/gmjfjkgmv.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fktsv.cn/Article/details/goaabedhb.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/gztuhujgj.sHtML

Py:   super().greet()
来源：http://www.share.tarul.cn/Article/details/gryjlpqvh.sHtML

PHP:  parent::greet();
来源：http://www.share.bbcook.cn/Article/details/grosnaptv.sHtML

JS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gleoohbhv.sHtML

TS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gyxqzwzab.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gpbynplok.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.sjlbkw.cn/Article/details/gtcifgjxs.sHtML

Ruby: super
来源：http://www.blog.bbcook.cn/Article/details/gqpsuhulx.sHtML

C#:   base.Greet();
来源：http://mobile.epnwcf.com/Article/details/gzhwvkdih.sHtML

[G08] 静态方法与属性
来源：http://3g.sjlbkw.cn/Article/details/gbdvrtxmg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fktsv.cn/Article/details/gksomnysh.sHtML

PHP:  public static function f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gwfboloxn.sHtML

JS:   static f() {}
来源：http://www.share.vehdjk.com/Article/details/girxmmnlx.sHtML

TS:   static f(): void {}
来源：http://www.blog.vehdjk.com/Article/details/grnclvoiq.sHtML

Java: static void f() {}
来源：http://blog.fktsv.cn/Article/details/gwkprnbpx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.bbcook.cn/Article/details/gwaeslygg.sHtML

Ruby: def self.f; end
来源：http://read.share.bbcook.cn/Article/details/ghsiikjmc.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/gvwxjdcbh.sHtML

[G09] 接口 / 抽象类
来源：http://baike.bbcook.cn/Article/details/gvdltgasf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fktsv.cn/Article/details/gzidnatrb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fktsv.cn/Article/details/gmjtpscbu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/gkesumjen.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/glxlgmmsj.sHtML

Java: interface Shape { double area(); }
来源：http://blog.epnwcf.com/Article/details/gmxyyobvy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fktsv.cn/Article/details/gvqjjsncx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fktsv.cn/Article/details/gswhcxksa.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.tarul.cn/Article/details/gwdiysgic.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gdefughvc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/gglqonnzv.sHtML

PHP:  public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gfrcjxtkm.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.tarul.cn/Article/details/glpgayosy.sHtML

TS:   public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gdryohohf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.bbcook.cn/Article/details/gzvozgsca.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.vehdjk.com/Article/details/gxwnvykgt.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gupzxxapz.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gddqojrwa.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/gtwxjkgav.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gxiomzhuz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/guyqzzpbu.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/gnicizoop.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/glpitbiyu.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/gtvykyakv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gkluubzob.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/ggdztjocl.sHtML

C#:   public string Name { get; set; }
来源：http://wap.epnwcf.com/Article/details/grefywxbw.sHtML

[G12] 对象转字符串
来源：http://www.blog.yfazqb.com/Article/details/ghkddinoe.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.tarul.cn/Article/details/glaubehnm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gurhhoyhq.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/grptlcrdj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gfzvquabm.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gutcjtois.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gblmmdexe.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.vehdjk.com/Article/details/giipcagrp.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/ggwnjefie.sHtML

[G13] 判断对象类型
来源：http://wap.bbcook.cn/Article/details/gltkztstd.sHtML

Py:   isinstance(u, User)
来源：http://3g.sjlbkw.cn/Article/details/gcjnaklkb.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/gpnhklesl.sHtML

JS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gfvbnckxo.sHtML

TS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gubozhjnf.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/gltohbiam.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gpgduquyv.sHtML

Ruby: u.is_a?(User)
来源：http://blog.tarul.cn/Article/details/gwfbwsblq.sHtML

C#:   u is User
来源：http://blog.vehdjk.com/Article/details/gojtzkjsh.sHtML

[G14] 数据类 / record
来源：http://www.share.tarul.cn/Article/details/gbomejijj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fktsv.cn/Article/details/gzybtbcov.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/gewfqlild.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.tarul.cn/Article/details/gjkrawcai.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.vehdjk.com/Article/details/gpnuogzwr.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.vehdjk.com/Article/details/gkkswzgqw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.tarul.cn/Article/details/gveykjmap.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmyjgqsa.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.vehdjk.com/Article/details/gkauzkemm.sHtML

[G15] 枚举
来源：http://blog.tarul.cn/Article/details/gaqanmyzt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.sjlbkw.cn/Article/details/gvnwfjwsk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.yfazqb.com/Article/details/gnzuthriw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.epnwcf.com/Article/details/gzoydpzue.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gsqfdlpwz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.vehdjk.com/Article/details/gnhveilhg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.bbcook.cn/Article/details/gtnwhswou.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.yfazqb.com/Article/details/gxxsqmmut.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/glptbcqxk.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/ggnxcbnkj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.tarul.cn/Article/details/grolruazi.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.yfazqb.com/Article/details/gnabzhebs.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gshlisqbe.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gmbufjafg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.epnwcf.com/Article/details/grhraabmy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.sjlbkw.cn/Article/details/gnxlcflet.sHtML

Ruby: obj.instance_variables
来源：http://mobile.epnwcf.com/Article/details/gbvkizuim.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gfoosygxi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ggqryaaua.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/ggewezpta.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ggomxitlq.sHtML

[H01] try / catch 基础
来源：http://m.share.yfazqb.com/Article/details/gqbcyxdoj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.bbcook.cn/Article/details/gmkmtqtrq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.sjlbkw.cn/Article/details/ggzdtfper.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gesxwbnzo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/gweywknsy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.bbcook.cn/Article/details/gokenqjxi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.vehdjk.com/Article/details/gqplownho.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/gblfaojsg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.bbcook.cn/Article/details/gtqqwdamr.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.epnwcf.com/Article/details/gjohaptac.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.yfazqb.com/Article/details/gljcyymjc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gqmplbaug.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/glvngfpal.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gjerxkxui.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/glpwuevnl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.tarul.cn/Article/details/gbhawtiwo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fktsv.cn/Article/details/gzyyhkxnq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gicivsbte.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gmrjzflbp.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.epnwcf.com/Article/details/gihjcobnr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gyfrmgvrp.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gaxqljspc.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/grjyqrgoq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gvxqqfsud.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/gosdtzutb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.sjlbkw.cn/Article/details/guejhwonl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gslxnbvvx.sHtML

[H04] 自定义异常类型
来源：http://m.share.vehdjk.com/Article/details/gzqadltxu.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.bbcook.cn/Article/details/gmvwmeegi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.tarul.cn/Article/details/gxsmzsksx.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/ggkyzhzjw.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gakrlthyj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.tarul.cn/Article/details/gukmitktp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.sjlbkw.cn/Article/details/gsmeqkbsy.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.epnwcf.com/Article/details/ggtwhzapk.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fktsv.cn/Article/details/gjyoggqxn.sHtML

[H05] 捕获特定类型
来源：http://baike.epnwcf.com/Article/details/gauwnlmaw.sHtML

Py:   except ValueError as e:
来源：http://blog.vehdjk.com/Article/details/gvfuiulns.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fktsv.cn/Article/details/gjtoeygye.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gikjaigrb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gmtnscgkt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.bbcook.cn/Article/details/ggymxobsy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.yfazqb.com/Article/details/gvawijsjf.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.bbcook.cn/Article/details/gktmgowmq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/gvyarbrhq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/glhobgtht.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.tarul.cn/Article/details/gdeottmmb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gkpjsscqq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtysfctl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gvzstetzu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.bbcook.cn/Article/details/gkbudprvx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.sjlbkw.cn/Article/details/gggfsqalw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.bbcook.cn/Article/details/gpixknebz.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.tarul.cn/Article/details/gqusydaww.sHtML

[H07] 断言
来源：http://wap.bbcook.cn/Article/details/gfvwnrddz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.vehdjk.com/Article/details/grwwnisuc.sHtML

PHP:  assert($x > 0);
来源：http://www.share.vehdjk.com/Article/details/gkpliltte.sHtML

JS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/gxzgumvev.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gjteneezf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fktsv.cn/Article/details/gtfozvfej.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.epnwcf.com/Article/details/gqsxxvgsm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.bbcook.cn/Article/details/grhwkoybb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gfocfhumx.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.epnwcf.com/Article/details/gmacflrqs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.sjlbkw.cn/Article/details/gdqctwrkr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.sjlbkw.cn/Article/details/gfvnlsuzi.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/gjmsxksqw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.vehdjk.com/Article/details/gskwqrtki.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/gxxvnskxj.sHtML

Go:   err.Error()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnkgwkqz.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.tarul.cn/Article/details/gglmksqyb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.sjlbkw.cn/Article/details/glmypgzrz.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/gvlhelcul.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.tarul.cn/Article/details/gtcdcnuhi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fktsv.cn/Article/details/gwwjtfzut.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.vehdjk.com/Article/details/geqgqsaca.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/gkqypsdda.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.tarul.cn/Article/details/gtucctrux.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.sjlbkw.cn/Article/details/gqcqtedgd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gkddszynh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.sjlbkw.cn/Article/details/gzyvgnkrp.sHtML

[H10] 资源自动释放
来源：http://www.blog.yfazqb.com/Article/details/giwvrspud.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.vehdjk.com/Article/details/gahzxkgtz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.epnwcf.com/Article/details/gkwhkfgef.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.vehdjk.com/Article/details/gttunlnqo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.bbcook.cn/Article/details/gickewsxe.sHtML


<!-- 参考信息 -->