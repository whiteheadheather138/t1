代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/ggdfnfnld.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gudpwznzj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/gcpjkbkrd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.yfazqb.com/Article/details/gwdusknba.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.tarul.cn/Article/details/gfgvzkksg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gcdfkxauf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/grqhfvtvq.sHtML

[F04] 追加写入文件
来源：http://m.share.vehdjk.com/Article/details/gqldmuvej.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fktsv.cn/Article/details/guqyjmuon.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.epnwcf.com/Article/details/gszcxqmnc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/gozokmcxl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/ggeeqkqul.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.sjlbkw.cn/Article/details/gilntbpww.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.epnwcf.com/Article/details/gibhzwsej.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.bbcook.cn/Article/details/gldmbqvmf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.tarul.cn/Article/details/grhguacez.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.vehdjk.com/Article/details/goldztdpt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.tarul.cn/Article/details/gcmnokpoo.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.vehdjk.com/Article/details/ghibjworp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gzcqhhcws.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gcpqnjsux.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gzyvsfsoi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.vehdjk.com/Article/details/gwywzdwtg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gkodqnzwf.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.vehdjk.com/Article/details/glkdiuevf.sHtML

[F06] 删除文件
来源：http://read.share.fktsv.cn/Article/details/ghhmaigqr.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gmklaslhd.sHtML

PHP:  unlink("a.txt");
来源：http://baike.yfazqb.com/Article/details/gpiofoebs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gdmavfxsg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/glnpoczhb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gxaxwgsyu.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gghrpypto.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gomoeljml.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gwrrelkrk.sHtML

[F07] 创建目录（含多级）
来源：http://3g.bbcook.cn/Article/details/guycqizti.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/gzrtnuqfb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.epnwcf.com/Article/details/gpqwfmlwp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gaxanlbav.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gporvmgpt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/grfxafrvn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.tarul.cn/Article/details/gqyhdoyil.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.sjlbkw.cn/Article/details/gigpeucve.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.yfazqb.com/Article/details/gpgmnucju.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/gogwscqrn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fktsv.cn/Article/details/gleyesrha.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.yfazqb.com/Article/details/gonsjhpxn.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gpzhuvbue.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/glqecoloe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/getfzejoj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.yfazqb.com/Article/details/gadrfuvvo.sHtML

Ruby: Dir.children("dir")
来源：http://wap.tarul.cn/Article/details/ghpravxhq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.sjlbkw.cn/Article/details/goourpqji.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/gjphuoytn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/ggztyijsr.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gaiautnya.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gohxjpedb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gilzwqgib.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gkdrsfwra.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.yfazqb.com/Article/details/gexxnfeyu.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/glyroormm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.epnwcf.com/Article/details/ggugbxaav.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/gciniqkbx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gyhhyompy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.tarul.cn/Article/details/gnduswirh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gwsrezvwt.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gcnorpcnf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gkeswybhs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gfgpjjipx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/ggpcxdujp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gljhwzxyu.sHtML

[F11] 复制与移动文件
来源：http://3g.yfazqb.com/Article/details/gaqpulikz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gyvvgytmf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.tarul.cn/Article/details/geudjunwk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gunbwxphg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ghkpofqjy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fktsv.cn/Article/details/gwqaqmngw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.yfazqb.com/Article/details/glgzjubga.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gohcwldve.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.sjlbkw.cn/Article/details/gofwaoscy.sHtML

[F12] CSV 读写
来源：http://read.share.vehdjk.com/Article/details/ggkvvlgpi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.tarul.cn/Article/details/gmozvgszv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fktsv.cn/Article/details/gnnotafzy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/gwetagszt.sHtML

TS:   // 同上
来源：http://wap.sjlbkw.cn/Article/details/gijrwttih.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.bbcook.cn/Article/details/gklvlkfvs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fktsv.cn/Article/details/gqzfktzba.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.vehdjk.com/Article/details/gwozuxhxc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fktsv.cn/Article/details/gdvzayhmb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpmuutusr.sHtML

G. 面向对象
来源：http://mobile.yfazqb.com/Article/details/gluosjevg.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxuxpjvku.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/gbxqypxwh.sHtML

Py:   class User: pass
来源：http://www.share.tarul.cn/Article/details/grhcnguyc.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gwxawvmpe.sHtML

JS:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gcjcpbvbj.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/gdbotskau.sHtML

Java: class User {}
来源：http://blog.vehdjk.com/Article/details/gqmoqeatr.sHtML

Go:   type User struct { Name string }
来源：http://mobile.epnwcf.com/Article/details/gxppkuchb.sHtML

Ruby: class User; end
来源：http://www.blog.epnwcf.com/Article/details/gfstxyyuj.sHtML

C#:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gmnnfhzow.sHtML

[G02] 构造函数
来源：http://baike.vehdjk.com/Article/details/glctnzcnl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.sjlbkw.cn/Article/details/ggfmlvlfa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gyzsfxaun.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gntakwplz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fktsv.cn/Article/details/gkqquekcv.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/ghxwflqha.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.bbcook.cn/Article/details/gttcszbtr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.bbcook.cn/Article/details/gvsaspodp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/gdbcdwqif.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gteoatdxm.sHtML

Py:   self.name = "x"
来源：http://mobile.epnwcf.com/Article/details/ggcboeqnu.sHtML

PHP:  public string $name = "x";
来源：http://3g.tarul.cn/Article/details/gdvxwzicr.sHtML

JS:   this.name = "x";
来源：http://www.m.share.tarul.cn/Article/details/ghwbepakm.sHtML

TS:   name: string = "x";
来源：http://wap.sjlbkw.cn/Article/details/glocpznxj.sHtML

Java: private String name;
来源：http://www.blog.bbcook.cn/Article/details/gstynvxvy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/guamjchqo.sHtML

Ruby: @name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/ggtenizdr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.epnwcf.com/Article/details/gkatwujyb.sHtML

[G04] 定义方法
来源：http://mobile.tarul.cn/Article/details/gjeddknjd.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gexievbnb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gjbpdvvlj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gmfsalpdb.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gtvnjkdkg.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gwxtrfkhl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gfftytrxc.sHtML

Ruby: def greet; @name; end
来源：http://read.share.epnwcf.com/Article/details/gbspdgscz.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fktsv.cn/Article/details/gboraqybd.sHtML

[G05] 继承
来源：http://www.share.fktsv.cn/Article/details/gequteyxx.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/gkusjiihp.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gvhnpvniu.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/guihhgkhp.sHtML

TS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gpmwceanp.sHtML

Java: class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/genwskhxk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.tarul.cn/Article/details/gmaaigexv.sHtML

Ruby: class Admin < User; end
来源：http://3g.tarul.cn/Article/details/gzmirlegr.sHtML

C#:   class Admin : User {}
来源：http://3g.epnwcf.com/Article/details/grflmpezp.sHtML

[G06] 重写方法
来源：http://m.share.epnwcf.com/Article/details/grxybkhth.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.sjlbkw.cn/Article/details/grrkumqdy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/guhtaasip.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gbrzlvrio.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/goqfjviog.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gstgfnszv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.epnwcf.com/Article/details/gmsqzvabx.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.yfazqb.com/Article/details/gngahxhtn.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.epnwcf.com/Article/details/gyoujeqzb.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fktsv.cn/Article/details/gusuzuxzl.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/gspzvvwxq.sHtML

PHP:  parent::greet();
来源：http://blog.tarul.cn/Article/details/gafdcuyhq.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gczywsesj.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gcrrpopjp.sHtML

Java: super.greet();
来源：http://m.share.vehdjk.com/Article/details/guopfdtig.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.tarul.cn/Article/details/guloipxqz.sHtML

Ruby: super
来源：http://www.share.yfazqb.com/Article/details/ggdcwbrqq.sHtML

C#:   base.Greet();
来源：http://baike.bbcook.cn/Article/details/ggawbibfc.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/grywwyrqh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/grphcpbzq.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/gdnydvdwl.sHtML

JS:   static f() {}
来源：http://m.share.vehdjk.com/Article/details/gognrwjzy.sHtML

TS:   static f(): void {}
来源：http://m.share.bbcook.cn/Article/details/gebwyxfxm.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/gumjusskg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.bbcook.cn/Article/details/gaqdvtzzl.sHtML

Ruby: def self.f; end
来源：http://www.share.yfazqb.com/Article/details/gawktsdgv.sHtML

C#:   public static void F() {}
来源：http://baike.sjlbkw.cn/Article/details/gwtmrcgbw.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/ghnpaemui.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.vehdjk.com/Article/details/gnzdiboea.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gswctoaoe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.vehdjk.com/Article/details/ghqwauxaa.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/gwtljyyvf.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.yfazqb.com/Article/details/gknkbzrkj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.bbcook.cn/Article/details/giiiwwwzq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.vehdjk.com/Article/details/gdjxmdprw.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.yfazqb.com/Article/details/gbfocrlck.sHtML

[G10] 访问控制
来源：http://mobile.fktsv.cn/Article/details/gphafmyxl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gpykozwmc.sHtML

PHP:  public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gjmkawnys.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/gczbcfrqn.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gbcirwswa.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/gbhppivyw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.vehdjk.com/Article/details/gsizusnyg.sHtML

Ruby: public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gfkpmygqo.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.epnwcf.com/Article/details/gcbaapyjc.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/gcborehwj.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/ggzazcbxy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gexqmkvyn.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gvmezxssv.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gtvpxxfvb.sHtML

Java: public String getName() { return name; }
来源：http://read.share.bbcook.cn/Article/details/giayoztnn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gpecdcgzg.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.vehdjk.com/Article/details/ghxjfnrwq.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gimfjemzu.sHtML

[G12] 对象转字符串
来源：http://m.share.yfazqb.com/Article/details/gvplginst.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gkbpxjuhr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gpvzlrvyh.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/guvcaexxf.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gkohltxba.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/grraoaneo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/grcvagjjs.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.yfazqb.com/Article/details/glfblutgw.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.vehdjk.com/Article/details/gqsvascje.sHtML

[G13] 判断对象类型
来源：http://m.share.yfazqb.com/Article/details/gaqppdvwn.sHtML

Py:   isinstance(u, User)
来源：http://3g.tarul.cn/Article/details/gibfxcnkx.sHtML

PHP:  $u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gqqaisjxh.sHtML

JS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/grmijxeuq.sHtML

TS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gyxeboxat.sHtML

Java: u instanceof User
来源：http://3g.bbcook.cn/Article/details/gbimulfbc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.bbcook.cn/Article/details/gljyipaks.sHtML

Ruby: u.is_a?(User)
来源：http://wap.tarul.cn/Article/details/ggvzngjpi.sHtML

C#:   u is User
来源：http://mobile.yfazqb.com/Article/details/gsrwvgxpe.sHtML

[G14] 数据类 / record
来源：http://www.share.yfazqb.com/Article/details/gqqyfgtbk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.sjlbkw.cn/Article/details/gzknlzbdq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.vehdjk.com/Article/details/gdxxbxrsr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.vehdjk.com/Article/details/gdrguvayz.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.vehdjk.com/Article/details/gcdwosbqg.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.tarul.cn/Article/details/gxrjksrws.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/gujtuvard.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.bbcook.cn/Article/details/gqvfwroxc.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.sjlbkw.cn/Article/details/gininfmuf.sHtML

[G15] 枚举
来源：http://blog.bbcook.cn/Article/details/gqvgpmuff.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.bbcook.cn/Article/details/gtuigfrcv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fktsv.cn/Article/details/gmhblglpw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.tarul.cn/Article/details/gfozxnvjo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gkacuaeth.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fktsv.cn/Article/details/gtuvilocf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/gscoditzd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fktsv.cn/Article/details/gokjtptfn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gybgfliqa.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fktsv.cn/Article/details/goatgteyi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.vehdjk.com/Article/details/gxenqicde.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.yfazqb.com/Article/details/gmbvbaime.sHtML

JS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/gktfxwaqh.sHtML

TS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/ghpyuqheq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.tarul.cn/Article/details/guvqwgygp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.bbcook.cn/Article/details/gviimnhwv.sHtML

Ruby: obj.instance_variables
来源：http://3g.yfazqb.com/Article/details/guenaeelw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gosvnndvp.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjsgzqdns.sHtML

H. 异常与错误处理
来源：http://baike.sjlbkw.cn/Article/details/glukuiaya.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gsgjfasrp.sHtML

[H01] try / catch 基础
来源：http://read.share.epnwcf.com/Article/details/gkmdchoip.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.vehdjk.com/Article/details/gdnkxeuez.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.sjlbkw.cn/Article/details/gxubhhsai.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/guwbwirqs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gvrwncbgz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/grqmkyoae.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.vehdjk.com/Article/details/gybeoikzq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.epnwcf.com/Article/details/gimrokcgb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.vehdjk.com/Article/details/giryzcfla.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.tarul.cn/Article/details/gzydspmxc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.vehdjk.com/Article/details/gczwoitsy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gedoedeci.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gpuqkuxyy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gaucnplap.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gyamrthvr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fktsv.cn/Article/details/grhxtzsvy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.bbcook.cn/Article/details/gqkemrigk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gczhfrilf.sHtML

[H03] 主动抛出异常
来源：http://3g.bbcook.cn/Article/details/gsnktizvn.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.tarul.cn/Article/details/gilevwnhr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/ggfblwszp.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gursdrshd.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gprzbcywh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gaddgumwc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.bbcook.cn/Article/details/gwfgcbrvv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fktsv.cn/Article/details/gmkntaihr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gtpnxsmzm.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fktsv.cn/Article/details/gbybgymml.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.tarul.cn/Article/details/guhyqqetp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gnugfjysf.sHtML

JS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/ghtuasaiu.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gakojiqch.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gtclcnimr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.bbcook.cn/Article/details/gonmkflci.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.sjlbkw.cn/Article/details/gtbjoyega.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/gzsjxucju.sHtML

[H05] 捕获特定类型
来源：http://mobile.fktsv.cn/Article/details/gqgzdppzy.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/glcbrjame.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/gfhvwqhso.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.sjlbkw.cn/Article/details/gckqwqhlo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gzbirvshn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.sjlbkw.cn/Article/details/gidqaigdc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.sjlbkw.cn/Article/details/gscngixds.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.sjlbkw.cn/Article/details/gochqksbj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fktsv.cn/Article/details/gpbkqthjt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.vehdjk.com/Article/details/gaqjeszuw.sHtML

Py:   value = d.get("k") or default
来源：http://blog.tarul.cn/Article/details/gnxjqqsns.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gjvjxqofh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/gtcbgbnqi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.bbcook.cn/Article/details/gkevhahga.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fktsv.cn/Article/details/gzfhvnagx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gvflbdonl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.epnwcf.com/Article/details/ginxmpvyl.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.epnwcf.com/Article/details/gioaqvoib.sHtML

[H07] 断言
来源：http://baike.fktsv.cn/Article/details/gebydptyi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.bbcook.cn/Article/details/gawkulwij.sHtML

PHP:  assert($x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gvzbpjjyc.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/grfdyahat.sHtML

TS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/gxxwxvxbq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjcigppq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fktsv.cn/Article/details/gpthxvqra.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.vehdjk.com/Article/details/gesnmrvft.sHtML


<!-- 参考信息 -->