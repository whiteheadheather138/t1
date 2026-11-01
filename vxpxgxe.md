代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.tarul.cn/Article/details/gfzbqoyus.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.epnwcf.com/Article/details/gijvvmvgj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/goajntxvd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gdhtqygzj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fktsv.cn/Article/details/gsxncqwzt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fktsv.cn/Article/details/gtzlgyyhp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/gspvrwckb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.vehdjk.com/Article/details/glfmunhpb.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/gciphfxdd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.bbcook.cn/Article/details/gmtrhobsu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gywstgaih.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gcptnxnxn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/ggtoifouk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gzphuhmfe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fktsv.cn/Article/details/gyzflxsoq.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/guhnyeybk.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.tarul.cn/Article/details/gifbcieqb.sHtML

[F06] 删除文件
来源：http://www.share.yfazqb.com/Article/details/gbglqviee.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gcxrljnta.sHtML

PHP:  unlink("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gnzqavswj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gurkhqbus.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gvpxthjnr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gotyhujri.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gedlorxrb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gaynqueko.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.vehdjk.com/Article/details/gecpckksk.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.bbcook.cn/Article/details/gmemihldl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gvpmcuvnk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.vehdjk.com/Article/details/gpkwkevlu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/givswtomv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gskysmjpu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.vehdjk.com/Article/details/gnsunqisu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.sjlbkw.cn/Article/details/gvxjnughu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.bbcook.cn/Article/details/gnbcxnvcl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.sjlbkw.cn/Article/details/gkfprmmvu.sHtML

[F08] 遍历目录
来源：http://www.blog.sjlbkw.cn/Article/details/ghumilflv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.vehdjk.com/Article/details/gsiwxqnyl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/gsubmlapa.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/grdjffzyl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gxapmuvwc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gfevbtgeh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.sjlbkw.cn/Article/details/gauqxxiuw.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/grudwaign.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gczgezijc.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/gliuhdryo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/guwtlzfob.sHtML

PHP:  filesize("a.txt");
来源：http://wap.yfazqb.com/Article/details/gacucukkk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gwflcrlmw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/geupftavp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/ghozxksnl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/gkznxdtnm.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gpvxhmbio.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.bbcook.cn/Article/details/gkqozpgwn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fktsv.cn/Article/details/gjzvohnyk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gsiuuddjn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.tarul.cn/Article/details/gsnufeixl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gkzaxhaaz.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gvfyfpelb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.yfazqb.com/Article/details/geooitdyz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gotjabpnr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gakjtsoge.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gpytxwslp.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/gekcumiyb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gfmxdkfly.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.vehdjk.com/Article/details/gxccctrls.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gkticvmls.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gwcazutnv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fktsv.cn/Article/details/gwcaiouzk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.yfazqb.com/Article/details/gcywfhdqc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gistjvjnt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/gvtotowtu.sHtML

[F12] CSV 读写
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcncpcmy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.bbcook.cn/Article/details/gignfrvlw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.tarul.cn/Article/details/gbuciruzc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.tarul.cn/Article/details/gxikorxfu.sHtML

TS:   // 同上
来源：http://www.share.yfazqb.com/Article/details/grnuboofm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.bbcook.cn/Article/details/gzmjpkgit.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.epnwcf.com/Article/details/gfqlplgqw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.yfazqb.com/Article/details/gbzttyals.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/ghyrkfbyo.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/getjcosyz.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/gwctebxbu.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grsxdrkeg.sHtML

[G01] 定义类
来源：http://blog.epnwcf.com/Article/details/guqklaewn.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/gfxemxiau.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/goitvpndt.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gmtbnajdc.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/ggzbhscia.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gxxpzjrpk.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/grgazlatf.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/gbqkusspj.sHtML

C#:   class User {}
来源：http://read.share.tarul.cn/Article/details/gkzhrtopw.sHtML

[G02] 构造函数
来源：http://blog.sjlbkw.cn/Article/details/gmxepmkpx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.bbcook.cn/Article/details/glsrddspv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.yfazqb.com/Article/details/gppzyfsld.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gkenwcnfm.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.vehdjk.com/Article/details/gottkislo.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gabgiwecd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.bbcook.cn/Article/details/gsgqtuvbe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.yfazqb.com/Article/details/gxxqnuoyn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.yfazqb.com/Article/details/gcfdzjsat.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/gwolknhfg.sHtML

Py:   self.name = "x"
来源：http://mobile.vehdjk.com/Article/details/gpxdggdhs.sHtML

PHP:  public string $name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gbjkqinqe.sHtML

JS:   this.name = "x";
来源：http://www.share.vehdjk.com/Article/details/gdfzoqgaq.sHtML

TS:   name: string = "x";
来源：http://read.share.tarul.cn/Article/details/gstiwwxiq.sHtML

Java: private String name;
来源：http://baike.yfazqb.com/Article/details/gizvvmabb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/goqhxbypv.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/gtovwwfkp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.tarul.cn/Article/details/giwksujom.sHtML

[G04] 定义方法
来源：http://www.m.share.vehdjk.com/Article/details/gxxthdfjm.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/glxgpviwn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gbyvguphh.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gudeclmyy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gpticgekc.sHtML

Java: String greet() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gadlqitju.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/grkjsscim.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gyusfuqhc.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.yfazqb.com/Article/details/gxffvbhwa.sHtML

[G05] 继承
来源：http://blog.sjlbkw.cn/Article/details/gykjwjjfq.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fktsv.cn/Article/details/gazrvujlr.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gjuanbynd.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gmelynbks.sHtML

TS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gvsxjlkxy.sHtML

Java: class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gvdykxfrw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.epnwcf.com/Article/details/guepitqyt.sHtML

Ruby: class Admin < User; end
来源：http://m.share.bbcook.cn/Article/details/gyonqqhje.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/galywpehn.sHtML

[G06] 重写方法
来源：http://3g.tarul.cn/Article/details/ghhfqlggj.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/gvedociij.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gudexbdil.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/ggdsdglyf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gywcgvkcg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/ghgxkcsva.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.sjlbkw.cn/Article/details/gxeeswgag.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fktsv.cn/Article/details/gfloxasya.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.vehdjk.com/Article/details/gmasarykj.sHtML

[G07] 调用父类方法
来源：http://www.share.yfazqb.com/Article/details/gftqlojny.sHtML

Py:   super().greet()
来源：http://baike.sjlbkw.cn/Article/details/gnkvdhekn.sHtML

PHP:  parent::greet();
来源：http://mobile.yfazqb.com/Article/details/grnucsxdy.sHtML

JS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/geprfxhqv.sHtML

TS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gpehikmso.sHtML

Java: super.greet();
来源：http://3g.fktsv.cn/Article/details/geroekkdk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.sjlbkw.cn/Article/details/gpayufukp.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/gxwrznmxe.sHtML

C#:   base.Greet();
来源：http://blog.yfazqb.com/Article/details/gymrcxaol.sHtML

[G08] 静态方法与属性
来源：http://read.share.epnwcf.com/Article/details/goshcrhin.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.yfazqb.com/Article/details/gbpmjofxg.sHtML

PHP:  public static function f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gghglfmez.sHtML

JS:   static f() {}
来源：http://wap.yfazqb.com/Article/details/ghbocdjmw.sHtML

TS:   static f(): void {}
来源：http://www.share.tarul.cn/Article/details/gwpwvtfbv.sHtML

Java: static void f() {}
来源：http://mobile.tarul.cn/Article/details/ggchorpfs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.yfazqb.com/Article/details/gedldvfoz.sHtML

Ruby: def self.f; end
来源：http://3g.fktsv.cn/Article/details/gnezmkvma.sHtML

C#:   public static void F() {}
来源：http://www.share.sjlbkw.cn/Article/details/gjgykdfvl.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.tarul.cn/Article/details/gekmrbvsi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/giozcolum.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.vehdjk.com/Article/details/gaobupaic.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/ghwjylxai.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/gxmlejejn.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.vehdjk.com/Article/details/gycxwokcg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.bbcook.cn/Article/details/gikyzrukk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.epnwcf.com/Article/details/gmwfmyyef.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/gbblyghje.sHtML

[G10] 访问控制
来源：http://blog.sjlbkw.cn/Article/details/gwwcfoyzs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.bbcook.cn/Article/details/gwhghpjju.sHtML

PHP:  public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbqbymhk.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.yfazqb.com/Article/details/gjqmguzij.sHtML

TS:   public / protected / private
来源：http://wap.vehdjk.com/Article/details/gbfrszilc.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.epnwcf.com/Article/details/gglmvxwfb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.vehdjk.com/Article/details/gadrjkzqj.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gvpokirnz.sHtML

C#:   public / protected / private / internal
来源：http://3g.tarul.cn/Article/details/glufpxtxd.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gdbwvobxl.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fktsv.cn/Article/details/gttkjgurx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/ghratpusr.sHtML

JS:   get name() { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gjzoewtwr.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.tarul.cn/Article/details/gilsoovml.sHtML

Java: public String getName() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gvsbeqjab.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/guevirrga.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/grwkumpas.sHtML

C#:   public string Name { get; set; }
来源：http://3g.sjlbkw.cn/Article/details/gfnvnbxyh.sHtML

[G12] 对象转字符串
来源：http://m.share.bbcook.cn/Article/details/gnuxokoxq.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gukrccafo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gkpmvwnbq.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gruhnshrm.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gnlfkmnhp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gzgfjmcsw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gvsviiwln.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.tarul.cn/Article/details/gspusxwyc.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/gaqayznxd.sHtML

[G13] 判断对象类型
来源：http://blog.sjlbkw.cn/Article/details/gybfmqyvu.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fktsv.cn/Article/details/goaytbihm.sHtML

PHP:  $u instanceof User
来源：http://wap.tarul.cn/Article/details/gpmjzkxnh.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gmxkayueh.sHtML

TS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/glqzzdbwo.sHtML

Java: u instanceof User
来源：http://baike.bbcook.cn/Article/details/gmpbpztym.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.yfazqb.com/Article/details/gzqqccfvx.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/gitsbunez.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/gxobdfruv.sHtML

[G14] 数据类 / record
来源：http://read.share.sjlbkw.cn/Article/details/gdxdolbqu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.sjlbkw.cn/Article/details/gtrfgtevi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fktsv.cn/Article/details/gdvjxjspm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.epnwcf.com/Article/details/gipkfkvzq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fktsv.cn/Article/details/gljbcfdap.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fktsv.cn/Article/details/gkxffphom.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.sjlbkw.cn/Article/details/gfyvawzfh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/gqxforcbf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/gehryllnn.sHtML

[G15] 枚举
来源：http://mobile.tarul.cn/Article/details/gcpkpxokr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/glqqbwcbz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.vehdjk.com/Article/details/glzhcoiqi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gndohtwtb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gtkpyccuo.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.yfazqb.com/Article/details/gcddzxjor.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.yfazqb.com/Article/details/gcefvwaai.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.sjlbkw.cn/Article/details/gcgfapwdv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gvkchrewz.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.bbcook.cn/Article/details/gxkpmopsu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fktsv.cn/Article/details/gypjsaffu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.vehdjk.com/Article/details/gmnvyacna.sHtML

JS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gzvwngkdr.sHtML

TS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/grjgwdwsl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.bbcook.cn/Article/details/gfmsyhgiq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.epnwcf.com/Article/details/gxhaswvkz.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/ghdkugkqs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.tarul.cn/Article/details/geivlrhti.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gujuvisyy.sHtML

H. 异常与错误处理
来源：http://m.share.yfazqb.com/Article/details/giisiubmk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghviupakg.sHtML

[H01] try / catch 基础
来源：http://read.share.sjlbkw.cn/Article/details/gdtthrbgo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fktsv.cn/Article/details/gfjpurgvc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.sjlbkw.cn/Article/details/gozyyordn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gsjxxykbh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.vehdjk.com/Article/details/gdibdrbjv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.vehdjk.com/Article/details/gpbkfzdiv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.yfazqb.com/Article/details/gffgaebos.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/gdeszrovr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fktsv.cn/Article/details/gqfawhahb.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fktsv.cn/Article/details/gplyxfqzt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.yfazqb.com/Article/details/gowjaeznf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gxmtlfavk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gvyoqevkf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gbjqtdrop.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gzjiwrkml.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fktsv.cn/Article/details/gbkyhjsff.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.bbcook.cn/Article/details/gchiildyv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/glpqimshz.sHtML

[H03] 主动抛出异常
来源：http://3g.epnwcf.com/Article/details/grvjrvmad.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.epnwcf.com/Article/details/gjcqpowhs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/ggtcfcbvy.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gdxpevzwj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/goyrehahx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/glggimlze.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fktsv.cn/Article/details/gukwifjdl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.vehdjk.com/Article/details/gzzdtezuu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gmzwlkdvo.sHtML

[H04] 自定义异常类型
来源：http://3g.fktsv.cn/Article/details/gdxanlckk.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.vehdjk.com/Article/details/ggeclyazf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gdbhefanh.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.bbcook.cn/Article/details/gvvhckamx.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/gyzhibmer.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gownrerkp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.sjlbkw.cn/Article/details/gapnfqdzm.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.vehdjk.com/Article/details/gjxsjlybf.sHtML

C#:   class MyException : Exception {}
来源：http://wap.epnwcf.com/Article/details/gxizyngut.sHtML

[H05] 捕获特定类型
来源：http://wap.epnwcf.com/Article/details/gagwwbtjw.sHtML

Py:   except ValueError as e:
来源：http://read.share.bbcook.cn/Article/details/gpqdievfn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.epnwcf.com/Article/details/gemxaxheh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gjhixspso.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/gpqwbxwkn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.yfazqb.com/Article/details/gdrneveft.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.tarul.cn/Article/details/gqyqhdgqg.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.bbcook.cn/Article/details/gxximwfty.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fktsv.cn/Article/details/grhacdqbt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/gyhdmzgfj.sHtML

Py:   value = d.get("k") or default
来源：http://wap.tarul.cn/Article/details/gajmrthcx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gklyeswzt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gpsogwzos.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gqoqkfnmo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/gxjxxsijr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fktsv.cn/Article/details/glnlgbetn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.yfazqb.com/Article/details/gunhztoke.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.tarul.cn/Article/details/gvhtfwmdd.sHtML

[H07] 断言
来源：http://3g.tarul.cn/Article/details/giexhqehr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.tarul.cn/Article/details/gpwggrfcw.sHtML

PHP:  assert($x > 0);
来源：http://blog.tarul.cn/Article/details/gkthaoxta.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gultgvtds.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gcmrtvilg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.yfazqb.com/Article/details/gondheajr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.sjlbkw.cn/Article/details/gwmihlbum.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.epnwcf.com/Article/details/gymozyhxb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gygptotcl.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.vehdjk.com/Article/details/gfhmwqkmr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.vehdjk.com/Article/details/gurebmwbt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fktsv.cn/Article/details/gunwzwzca.sHtML

JS:   e.message;  e.stack
来源：http://www.share.epnwcf.com/Article/details/glhcwtqig.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.bbcook.cn/Article/details/gwtnhuqih.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.bbcook.cn/Article/details/gpppvygrf.sHtML

Go:   err.Error()
来源：http://read.share.tarul.cn/Article/details/gwcckrjom.sHtML


<!-- 参考信息 -->