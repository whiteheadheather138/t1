代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/gdvdozhuv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/gbfebjmwr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/goazbrnrm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlgcalpv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.epnwcf.com/Article/details/gauohnbuj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gtahfzkkj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.tarul.cn/Article/details/ginwtcuoi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.epnwcf.com/Article/details/gjdztqhnv.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.sjlbkw.cn/Article/details/gntncgxib.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.vehdjk.com/Article/details/gndbugajf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwibrtrwi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gyxrupcca.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gvetbebyy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gubkrbksh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/gynjsevpb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gyzaucrgy.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.tarul.cn/Article/details/gdwhqxgzc.sHtML

[F06] 删除文件
来源：http://mobile.sjlbkw.cn/Article/details/gewkubkaw.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/ggyreapxy.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gtcccipkr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gpaudymwz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gnhohtruu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gvoqbjabd.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gvvpuhxci.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gfuibtkfz.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.epnwcf.com/Article/details/gpwujsrsa.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fktsv.cn/Article/details/gvpjakybd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gaxpmkeqi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.bbcook.cn/Article/details/gspmvbxje.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gevhwnuee.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gzqqdurbr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.vehdjk.com/Article/details/gadkhimxj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.sjlbkw.cn/Article/details/gimmboktf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/goflrsyza.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.tarul.cn/Article/details/gxdirzeec.sHtML

[F08] 遍历目录
来源：http://www.share.yfazqb.com/Article/details/gopqbvany.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/gtewhqtpj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.vehdjk.com/Article/details/gshyimepy.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gfblddzyf.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/gupypfktl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/gjoixfmwe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/grdovqtfz.sHtML

Ruby: Dir.children("dir")
来源：http://3g.yfazqb.com/Article/details/grakrlztq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.tarul.cn/Article/details/gzbokhybm.sHtML

[F09] 获取文件大小
来源：http://baike.fktsv.cn/Article/details/glprvbwej.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.tarul.cn/Article/details/gqhphceuk.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gmrvmjvni.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gbkcnzbli.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/girgfjoqk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gvthluzxb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.tarul.cn/Article/details/gdopnvrqr.sHtML

Ruby: File.size("a.txt")
来源：http://blog.tarul.cn/Article/details/gubvatvmv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.epnwcf.com/Article/details/gbhrjbzff.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fktsv.cn/Article/details/gispiqhsq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/glzbkwbjh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.yfazqb.com/Article/details/grihxuprn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gkgrdbtrg.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/gpnpzedva.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.yfazqb.com/Article/details/gkibtdugd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gvptcdufc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gyjokdihc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gcqztrpwv.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/gwnscyudm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gsdxyzusq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.epnwcf.com/Article/details/guwfmvrzf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/geunndicd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gfxqaqwpp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/gfwsjnajo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.bbcook.cn/Article/details/guchkqeuz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/ggwrvalwq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.yfazqb.com/Article/details/gcsxlelie.sHtML

[F12] CSV 读写
来源：http://wap.yfazqb.com/Article/details/ghrqteygg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.vehdjk.com/Article/details/gdgvptjhw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.tarul.cn/Article/details/ghquxfwur.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.tarul.cn/Article/details/gpuqvvtjj.sHtML

TS:   // 同上
来源：http://mobile.bbcook.cn/Article/details/gswfckjrc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fktsv.cn/Article/details/gibhrjvpp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/gikhbdmfi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.bbcook.cn/Article/details/gfgrerirp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.vehdjk.com/Article/details/gkzekhdcd.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gicocklym.sHtML

G. 面向对象
来源：http://3g.fktsv.cn/Article/details/gnzyhahrj.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqapztuac.sHtML

[G01] 定义类
来源：http://baike.fktsv.cn/Article/details/gmicaqsyl.sHtML

Py:   class User: pass
来源：http://wap.tarul.cn/Article/details/giywaxhjt.sHtML

PHP:  class User {}
来源：http://read.share.epnwcf.com/Article/details/gmftiosef.sHtML

JS:   class User {}
来源：http://wap.fktsv.cn/Article/details/gyabbayjz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.tarul.cn/Article/details/gcbffqfhd.sHtML

Java: class User {}
来源：http://www.m.share.tarul.cn/Article/details/gvxtalrdv.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.tarul.cn/Article/details/geufgpftu.sHtML

Ruby: class User; end
来源：http://mobile.vehdjk.com/Article/details/gykiwwmap.sHtML

C#:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gkuwjciva.sHtML

[G02] 构造函数
来源：http://m.share.yfazqb.com/Article/details/gdgxjuube.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fktsv.cn/Article/details/grazjppdc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gjxujnbvo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/gldnvxebf.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.yfazqb.com/Article/details/gakbnplrx.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/gzsvhuwjk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.bbcook.cn/Article/details/gteqygwxj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/grzznabpd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.tarul.cn/Article/details/ghzihfjut.sHtML

[G03] 实例属性
来源：http://baike.bbcook.cn/Article/details/gypvgapfr.sHtML

Py:   self.name = "x"
来源：http://www.blog.tarul.cn/Article/details/gnbuhegqk.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/gtstbteuu.sHtML

JS:   this.name = "x";
来源：http://baike.fktsv.cn/Article/details/ghreeqgbe.sHtML

TS:   name: string = "x";
来源：http://m.share.yfazqb.com/Article/details/gfwcuisky.sHtML

Java: private String name;
来源：http://read.share.vehdjk.com/Article/details/gfpzxzmbo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.bbcook.cn/Article/details/gagiqttvt.sHtML

Ruby: @name = "x"
来源：http://m.share.vehdjk.com/Article/details/gmpacinul.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gnevndlan.sHtML

[G04] 定义方法
来源：http://blog.bbcook.cn/Article/details/gmsdvibbo.sHtML

Py:   def greet(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gihettzaw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gnqapuwti.sHtML

JS:   greet() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gwbiycbmu.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gmtgrjwwc.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/gslxxwyen.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gleeuvplu.sHtML

Ruby: def greet; @name; end
来源：http://3g.bbcook.cn/Article/details/gdjfdtpgv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.bbcook.cn/Article/details/giswlkmqm.sHtML

[G05] 继承
来源：http://blog.epnwcf.com/Article/details/ggbuwfuso.sHtML

Py:   class Admin(User): pass
来源：http://m.share.tarul.cn/Article/details/glquqvgim.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gopyqzyjy.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gzxkfbvhv.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gsunkwmmz.sHtML

Java: class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gipinhkfp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.tarul.cn/Article/details/ghrzmwicm.sHtML

Ruby: class Admin < User; end
来源：http://blog.tarul.cn/Article/details/gqmngfkte.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/gzdzddzcw.sHtML

[G06] 重写方法
来源：http://wap.fktsv.cn/Article/details/gidoabwyv.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.sjlbkw.cn/Article/details/gjnyozapu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gtdlzcybt.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/ghrgxflwd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/guarkicun.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gexhzetci.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/gxyowobpv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.epnwcf.com/Article/details/gjipodzys.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.sjlbkw.cn/Article/details/gdoukzvgd.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gsttnmlpe.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpynpeima.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/glquvqtvl.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gvhtcuvcb.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gbmxnredj.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/gnkwmadsy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.sjlbkw.cn/Article/details/gwujxapwq.sHtML

Ruby: super
来源：http://baike.bbcook.cn/Article/details/gitejtipb.sHtML

C#:   base.Greet();
来源：http://wap.bbcook.cn/Article/details/gfltqwqvg.sHtML

[G08] 静态方法与属性
来源：http://blog.sjlbkw.cn/Article/details/gqndrirop.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.sjlbkw.cn/Article/details/gfnhhbzru.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/gnyjbuyhn.sHtML

JS:   static f() {}
来源：http://blog.tarul.cn/Article/details/gecpsuufg.sHtML

TS:   static f(): void {}
来源：http://wap.vehdjk.com/Article/details/gxwlacovs.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/gywjmecyf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/gdsjqlnad.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/gfbpgjocy.sHtML

C#:   public static void F() {}
来源：http://www.share.fktsv.cn/Article/details/ggmnvzhnu.sHtML

[G09] 接口 / 抽象类
来源：http://baike.bbcook.cn/Article/details/gdxvhvwzq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.sjlbkw.cn/Article/details/grbadwdbs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fktsv.cn/Article/details/grhocfjri.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.tarul.cn/Article/details/gjrvjxmvl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.vehdjk.com/Article/details/glguvzdzn.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/gmctoqnvz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gxxizwsel.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.tarul.cn/Article/details/gcgmehdsh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/gowbjqesi.sHtML

[G10] 访问控制
来源：http://baike.vehdjk.com/Article/details/ggvbjpfhl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/gfwleemmi.sHtML

PHP:  public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/ggqykeyfv.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.sjlbkw.cn/Article/details/gifzgbfdf.sHtML

TS:   public / protected / private
来源：http://m.share.tarul.cn/Article/details/ggzltfsxq.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.tarul.cn/Article/details/glbelbmnv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fktsv.cn/Article/details/gojfqyloo.sHtML

Ruby: public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gotpfuxld.sHtML

C#:   public / protected / private / internal
来源：http://mobile.yfazqb.com/Article/details/gtzpfwgya.sHtML

[G11] getter / setter
来源：http://3g.yfazqb.com/Article/details/grucnebru.sHtML

Py:   @property 与 @x.setter
来源：http://wap.yfazqb.com/Article/details/goofxtjsv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/glpwwnyvx.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gdwbsneww.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gbklhcufp.sHtML

Java: public String getName() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gqivgzsok.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/giinoajrc.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/galbnylcj.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.sjlbkw.cn/Article/details/gvhjezqqx.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gxqhezkru.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/grikaojom.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/ggpjuhlzs.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/garpzomjf.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gsgrpbvsn.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fktsv.cn/Article/details/ggnndbbys.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gtgxlziiw.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.tarul.cn/Article/details/gzhuukhpf.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/gbphxzljn.sHtML

[G13] 判断对象类型
来源：http://mobile.sjlbkw.cn/Article/details/guaxzeeis.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/gqxisfelx.sHtML

PHP:  $u instanceof User
来源：http://3g.yfazqb.com/Article/details/gosqcdaew.sHtML

JS:   u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/giwipliwc.sHtML

TS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gnxesurqp.sHtML

Java: u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gygylkbwk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.tarul.cn/Article/details/gvvjpvcul.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.sjlbkw.cn/Article/details/gxclatxva.sHtML

C#:   u is User
来源：http://m.share.bbcook.cn/Article/details/gtwwzhdua.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/grcmdutsm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.tarul.cn/Article/details/gzevrovvz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/gexdruipd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.epnwcf.com/Article/details/gllrhfaln.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.bbcook.cn/Article/details/gpeluiiog.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/gctmmnjfk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fktsv.cn/Article/details/gjhhlfsbg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.epnwcf.com/Article/details/gznlquxml.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.tarul.cn/Article/details/gzgggbcee.sHtML

[G15] 枚举
来源：http://blog.bbcook.cn/Article/details/gmetxhhht.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.epnwcf.com/Article/details/gnxxjfdew.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fktsv.cn/Article/details/gtxogdysc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.tarul.cn/Article/details/gmdmpykio.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/grnudmqpi.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.yfazqb.com/Article/details/gnqckmudv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/gebqbwurz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.epnwcf.com/Article/details/gxbonzxvi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gvazomylf.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.bbcook.cn/Article/details/gkheovxnm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.yfazqb.com/Article/details/gvwpqpbpx.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.sjlbkw.cn/Article/details/gmbpdtcpj.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/glczazqjf.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gsgwsefgs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.epnwcf.com/Article/details/gouenanue.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.sjlbkw.cn/Article/details/gwsxpjcir.sHtML

Ruby: obj.instance_variables
来源：http://www.share.tarul.cn/Article/details/gzautiaaa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gaijxujoa.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/goutdwhma.sHtML

H. 异常与错误处理
来源：http://baike.epnwcf.com/Article/details/gqmexjpeh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwncosego.sHtML

[H01] try / catch 基础
来源：http://www.share.sjlbkw.cn/Article/details/gmanrfpkc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.bbcook.cn/Article/details/gpkfqmdyn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fktsv.cn/Article/details/gtrmzccrg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gilkrwzfz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/giwnvoouf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.epnwcf.com/Article/details/gipakkwol.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.tarul.cn/Article/details/gvxrhhang.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.sjlbkw.cn/Article/details/gsnlspebq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.bbcook.cn/Article/details/gcsenjopb.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gpdgzhpkl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.sjlbkw.cn/Article/details/gwgbetaic.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gawmanlph.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gcmvitwyr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gmncfnprp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/glxbrqrgi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.yfazqb.com/Article/details/guswitddt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.yfazqb.com/Article/details/gjyxozkzw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gatwpbcql.sHtML

[H03] 主动抛出异常
来源：http://m.share.yfazqb.com/Article/details/gtmjawokl.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gvytbnjbj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gxozpscuk.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gcbjxsaeu.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/goixrcvcx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gzkxllazv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/gcogiptae.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.vehdjk.com/Article/details/gdgxwxkap.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gsjwpoihp.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fktsv.cn/Article/details/gpeleygfe.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.bbcook.cn/Article/details/gyovozeuz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.tarul.cn/Article/details/gnzijjloc.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gwvchjkus.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/gqdlrmwbm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gikabntde.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.vehdjk.com/Article/details/ggmvagcwf.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.tarul.cn/Article/details/gwawzxvqs.sHtML

C#:   class MyException : Exception {}
来源：http://baike.vehdjk.com/Article/details/gjlhjwrre.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/gwxmtywqx.sHtML

Py:   except ValueError as e:
来源：http://read.share.epnwcf.com/Article/details/gdojwxzec.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/gvsykjsyh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuadzusu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gmodqyuhd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.yfazqb.com/Article/details/gqaqpdrjo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.bbcook.cn/Article/details/gucjhfung.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/glpbgmeyq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/grupqgklw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.sjlbkw.cn/Article/details/gzokoxgjd.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.sjlbkw.cn/Article/details/gbyvqukjn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gjipaoqgp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.sjlbkw.cn/Article/details/gijgxkxql.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gdtfukotz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.sjlbkw.cn/Article/details/gzrsishfx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.tarul.cn/Article/details/gjmearukj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fktsv.cn/Article/details/gfiwipbff.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.epnwcf.com/Article/details/gjwcwbjgd.sHtML

[H07] 断言
来源：http://mobile.epnwcf.com/Article/details/gfcrfykoa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.epnwcf.com/Article/details/ghotxvoux.sHtML

PHP:  assert($x > 0);
来源：http://mobile.vehdjk.com/Article/details/ghsssdwnh.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/gttntsyzw.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gafprmylm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.sjlbkw.cn/Article/details/gdaoqfain.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.vehdjk.com/Article/details/gwigluvod.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.sjlbkw.cn/Article/details/gdrfrgzlk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/ghmyxpypa.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.epnwcf.com/Article/details/gvsmicirg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gwikfpscu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.yfazqb.com/Article/details/gdvpuxktz.sHtML

JS:   e.message;  e.stack
来源：http://3g.sjlbkw.cn/Article/details/gmojwlqrh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.epnwcf.com/Article/details/glpiogxut.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.bbcook.cn/Article/details/gdbsxbvzl.sHtML

Go:   err.Error()
来源：http://m.share.vehdjk.com/Article/details/gavegjwem.sHtML


<!-- 参考信息 -->