代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.vehdjk.com/Article/details/ghibtcmdo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gyueldpld.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/ghuzsmnrs.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fktsv.cn/Article/details/ghonolikm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.epnwcf.com/Article/details/gwgmtcymz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.sjlbkw.cn/Article/details/gnlpcqjxi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gtbrpblbb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gyueprydn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.tarul.cn/Article/details/gaafmjhiu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fktsv.cn/Article/details/grdjzvqur.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.yfazqb.com/Article/details/gtsfwkhaj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.tarul.cn/Article/details/gtaxdgbbv.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.vehdjk.com/Article/details/goflbhdaz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/glkmeihma.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.bbcook.cn/Article/details/gasheaunt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gjsxkiuyg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gqyokpnjw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gdpvrtwzh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/gofkswxeg.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.tarul.cn/Article/details/ghgjzizdw.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.tarul.cn/Article/details/gxoxswbrv.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/gqylnapdd.sHtML

Py:   os.remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gfvmgrgxh.sHtML

PHP:  unlink("a.txt");
来源：http://3g.tarul.cn/Article/details/gycxeafpo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gtsedcluj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/glmdxhftu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gfnowgwcy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gwbxnbyir.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.bbcook.cn/Article/details/gamcdpnmx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gafxgbubk.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.tarul.cn/Article/details/gkiuahlil.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.vehdjk.com/Article/details/gpjfuakiw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.bbcook.cn/Article/details/gzhhbjerz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gylxgrymt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.tarul.cn/Article/details/goufnzgbq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.tarul.cn/Article/details/glxmezgmx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/gkwddwrfk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fktsv.cn/Article/details/gdnhvsafw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.vehdjk.com/Article/details/giszeeghq.sHtML

[F08] 遍历目录
来源：http://read.share.epnwcf.com/Article/details/grclkknte.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.sjlbkw.cn/Article/details/gtlquavku.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/grqlpngnl.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/giypywcxz.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gmncsqorg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gbkmnkxpn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.epnwcf.com/Article/details/grstomdlw.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.bbcook.cn/Article/details/glyoxtpjk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.bbcook.cn/Article/details/gjbmqnwrs.sHtML

[F09] 获取文件大小
来源：http://3g.vehdjk.com/Article/details/gnersupyz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.epnwcf.com/Article/details/goibldpez.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gzunlvsbn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gxxguwnhn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gbtyfgeix.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gyybtzjxw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fktsv.cn/Article/details/gwnfjxaxl.sHtML

Ruby: File.size("a.txt")
来源：http://baike.bbcook.cn/Article/details/ghbcezvjj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.tarul.cn/Article/details/gugawwdrq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fktsv.cn/Article/details/gbxxavbmc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gwvhpzngg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gefiuwool.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gitzswslv.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/gqibfcwvr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fktsv.cn/Article/details/gphoaevev.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gjpruewps.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/guxxfrfws.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gmwpcazlj.sHtML

[F11] 复制与移动文件
来源：http://www.blog.epnwcf.com/Article/details/gejifjdtz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gzchlyzmu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gcpcdjbrk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/ggcqptvzr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gvbomefgp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.bbcook.cn/Article/details/gpqdpoulx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.vehdjk.com/Article/details/grvhtgdqm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gvvfeoppw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.yfazqb.com/Article/details/gjcgfyfop.sHtML

[F12] CSV 读写
来源：http://m.share.yfazqb.com/Article/details/gkefebntc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fktsv.cn/Article/details/gffrfhcyr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.epnwcf.com/Article/details/gcpexegwx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.bbcook.cn/Article/details/gipzynucb.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/gvxmvmmwq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/glkemdkat.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.yfazqb.com/Article/details/gfwzxicaa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.tarul.cn/Article/details/gciiwwovp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/gmuomabkq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gxxthhtoz.sHtML

G. 面向对象
来源：http://baike.epnwcf.com/Article/details/gzwrzwkod.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghljyljes.sHtML

[G01] 定义类
来源：http://3g.tarul.cn/Article/details/gcnoohnqk.sHtML

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/gfyhrzzbl.sHtML

PHP:  class User {}
来源：http://wap.vehdjk.com/Article/details/gldhqpwot.sHtML

JS:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gvikozzag.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fktsv.cn/Article/details/gqepsquog.sHtML

Java: class User {}
来源：http://blog.yfazqb.com/Article/details/gqkfbjbyq.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/ghlynasmn.sHtML

Ruby: class User; end
来源：http://www.m.share.bbcook.cn/Article/details/gfbolmwap.sHtML

C#:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gvnfmkdbc.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gozbstzpc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.epnwcf.com/Article/details/gcjzceetf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.epnwcf.com/Article/details/gsszmifwf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/grrltuasn.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fktsv.cn/Article/details/gwpkvmxbq.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gpxeuuzrn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.tarul.cn/Article/details/ginvdtbvw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.tarul.cn/Article/details/gatehbhgn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gonclosax.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/gkeclspnr.sHtML

Py:   self.name = "x"
来源：http://baike.epnwcf.com/Article/details/gmegqixrz.sHtML

PHP:  public string $name = "x";
来源：http://mobile.bbcook.cn/Article/details/gyiwkbbbw.sHtML

JS:   this.name = "x";
来源：http://wap.yfazqb.com/Article/details/gmllyjabw.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/gorxwiezp.sHtML

Java: private String name;
来源：http://baike.tarul.cn/Article/details/gncozxnhx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.vehdjk.com/Article/details/ghftinler.sHtML

Ruby: @name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gktglyrzx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.bbcook.cn/Article/details/gsyomsgmo.sHtML

[G04] 定义方法
来源：http://baike.epnwcf.com/Article/details/gclgdmurd.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gpewijpob.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gebdpzmtm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gorfmrvdm.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gsmcmojir.sHtML

Java: String greet() { return name; }
来源：http://3g.vehdjk.com/Article/details/gpplmcnts.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gfegoxvlh.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fktsv.cn/Article/details/goktuudwr.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gsjnxfvbg.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/gobtfckba.sHtML

Py:   class Admin(User): pass
来源：http://wap.tarul.cn/Article/details/gkbscybal.sHtML

PHP:  class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/glsbvfjop.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxjijojxu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gcedbqypl.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gmaonfkag.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.yfazqb.com/Article/details/gibjvqzgl.sHtML

Ruby: class Admin < User; end
来源：http://blog.fktsv.cn/Article/details/gstwpkjxw.sHtML

C#:   class Admin : User {}
来源：http://www.blog.tarul.cn/Article/details/gaysibqyn.sHtML

[G06] 重写方法
来源：http://3g.yfazqb.com/Article/details/gbbvfujui.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fktsv.cn/Article/details/ghschvyep.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gxgmawchp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gocdpqqwr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/goleczaej.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/ggjfdhroz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gupdmskyg.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.tarul.cn/Article/details/gguoeewnb.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.tarul.cn/Article/details/gmtloxozs.sHtML

[G07] 调用父类方法
来源：http://www.m.share.vehdjk.com/Article/details/goefcsish.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/gqxutkpmh.sHtML

PHP:  parent::greet();
来源：http://wap.vehdjk.com/Article/details/ghwkwktbr.sHtML

JS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gyrvbrpvp.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gfobvzcck.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/gzimkuqnc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.epnwcf.com/Article/details/gtiovjiuo.sHtML

Ruby: super
来源：http://m.share.tarul.cn/Article/details/gmnhjsthd.sHtML

C#:   base.Greet();
来源：http://baike.yfazqb.com/Article/details/gbxlvghza.sHtML

[G08] 静态方法与属性
来源：http://www.share.vehdjk.com/Article/details/gcsauxyil.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.epnwcf.com/Article/details/gwkrtiyrd.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhptlrms.sHtML

JS:   static f() {}
来源：http://3g.epnwcf.com/Article/details/gwtdkixdk.sHtML

TS:   static f(): void {}
来源：http://wap.fktsv.cn/Article/details/ganyrucgq.sHtML

Java: static void f() {}
来源：http://m.share.fktsv.cn/Article/details/gsiviexlm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.tarul.cn/Article/details/gdqajkgox.sHtML

Ruby: def self.f; end
来源：http://read.share.epnwcf.com/Article/details/gypzjmems.sHtML

C#:   public static void F() {}
来源：http://3g.tarul.cn/Article/details/grpmojghy.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.epnwcf.com/Article/details/gvfilcvmp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.sjlbkw.cn/Article/details/gpahnxcat.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.sjlbkw.cn/Article/details/gixxuwchk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gkxkqsflx.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.vehdjk.com/Article/details/gucqdulbm.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.sjlbkw.cn/Article/details/ghvfjvtud.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.vehdjk.com/Article/details/gpbtvdwns.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.tarul.cn/Article/details/gwupxrytg.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.sjlbkw.cn/Article/details/gvatmuaox.sHtML

[G10] 访问控制
来源：http://blog.bbcook.cn/Article/details/gtkgflxkc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.tarul.cn/Article/details/gayzarhlq.sHtML

PHP:  public / protected / private
来源：http://wap.tarul.cn/Article/details/gffgnhzlx.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.epnwcf.com/Article/details/gwfyfxlvt.sHtML

TS:   public / protected / private
来源：http://wap.bbcook.cn/Article/details/gumhdsvkm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.sjlbkw.cn/Article/details/gsxwzlqzr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.sjlbkw.cn/Article/details/gnvfhqfhp.sHtML

Ruby: public / protected / private
来源：http://wap.fktsv.cn/Article/details/gmbwgkzkz.sHtML

C#:   public / protected / private / internal
来源：http://blog.epnwcf.com/Article/details/ggprcnztv.sHtML

[G11] getter / setter
来源：http://wap.vehdjk.com/Article/details/glhaviqaw.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.yfazqb.com/Article/details/guxvrfqna.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gwsckkgws.sHtML

JS:   get name() { return this._name; }
来源：http://baike.vehdjk.com/Article/details/gpkmqeufh.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gemkjgqol.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gbouwexug.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gjclrfvjh.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/ggfvvpcif.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.tarul.cn/Article/details/gchseacgn.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gqumuorfd.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gubfkuquu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gzixstyty.sHtML

JS:   toString() { return this.name; }
来源：http://wap.tarul.cn/Article/details/goinnmjyg.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gzeiokgka.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gzattrbnb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/ggjldimbm.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.epnwcf.com/Article/details/gpzwciryf.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.tarul.cn/Article/details/ggdamokap.sHtML

[G13] 判断对象类型
来源：http://blog.epnwcf.com/Article/details/gwskxhdpc.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/gwbekbiho.sHtML

PHP:  $u instanceof User
来源：http://blog.tarul.cn/Article/details/gvcylucgt.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gogyrlxzl.sHtML

TS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/ghwacmqmw.sHtML

Java: u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gsaqhlxey.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.epnwcf.com/Article/details/gkqvhnxml.sHtML

Ruby: u.is_a?(User)
来源：http://blog.sjlbkw.cn/Article/details/glnaveyoa.sHtML

C#:   u is User
来源：http://mobile.vehdjk.com/Article/details/gqgjngivh.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/gzqllzwtp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gzsbkysyv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.epnwcf.com/Article/details/gnktpfmeb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/gtudgncki.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fktsv.cn/Article/details/gdwgmsvpl.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.vehdjk.com/Article/details/gutydwwmi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.sjlbkw.cn/Article/details/gwakrnojm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.epnwcf.com/Article/details/gntawjoch.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.vehdjk.com/Article/details/ghtpeskvl.sHtML

[G15] 枚举
来源：http://read.share.fktsv.cn/Article/details/gfroolhsi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.tarul.cn/Article/details/gfcwvfegi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcnyvkfam.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.sjlbkw.cn/Article/details/gaawvxvar.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/ggppudrer.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.epnwcf.com/Article/details/gfidzeyww.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.yfazqb.com/Article/details/gmxnyukyw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.tarul.cn/Article/details/geqbvqcil.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gfizhuqsb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.epnwcf.com/Article/details/gzbecawpt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.sjlbkw.cn/Article/details/gttbulftn.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.vehdjk.com/Article/details/gmepzdwnw.sHtML

JS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gkbblmlwx.sHtML

TS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/gdoktflsi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.epnwcf.com/Article/details/gdauullgy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.vehdjk.com/Article/details/gwnqvsevq.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gmynanqxk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.tarul.cn/Article/details/gvhyklwbm.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcvvgvqiv.sHtML

H. 异常与错误处理
来源：http://www.share.epnwcf.com/Article/details/gfwefupvl.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpibqdlgn.sHtML

[H01] try / catch 基础
来源：http://www.m.share.sjlbkw.cn/Article/details/gpybfqguc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.yfazqb.com/Article/details/gccibyhlo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.bbcook.cn/Article/details/gqrnckoak.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gcrnuydkv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gwieiaorq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.vehdjk.com/Article/details/grmejqtzn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.tarul.cn/Article/details/gcelktgzm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.vehdjk.com/Article/details/gxkbbxqoq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.vehdjk.com/Article/details/gbtxoeamd.sHtML

[H02] finally / ensure 收尾
来源：http://baike.vehdjk.com/Article/details/grvgunhxy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.yfazqb.com/Article/details/ggliopkja.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/glavzbwxe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gqqoohorz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gpsiuynon.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gkldhsvdn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.epnwcf.com/Article/details/gatxwzdul.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.bbcook.cn/Article/details/grviutsfw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gxjjhgkct.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/geieqljca.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/gzhrpuclv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gzmfjuvvw.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gbqgyafmr.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gxzmbguhl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gfqomkkow.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/gzohvwaza.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/giyzkjoki.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gcttaasao.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/gsdefrwdj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.tarul.cn/Article/details/guwizbqiv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gkzzfjxrg.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gyxduvkav.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gdxacmuyg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gslgihyer.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.tarul.cn/Article/details/gsbsaybxu.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.tarul.cn/Article/details/gznkhrtml.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.yfazqb.com/Article/details/gqlpkpeis.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/gyluuepxz.sHtML

Py:   except ValueError as e:
来源：http://baike.sjlbkw.cn/Article/details/gizmavzbf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.epnwcf.com/Article/details/gumgkenqb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/ghczgxjmc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/ginxrlnta.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.sjlbkw.cn/Article/details/gzfbeubni.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fktsv.cn/Article/details/gkecmjqrs.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.tarul.cn/Article/details/grryxaglt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gndgwfbdg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.sjlbkw.cn/Article/details/ghzerzrhr.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.bbcook.cn/Article/details/gcqdpvkeg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gfvgvdcce.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gzhszbarj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gvytqszco.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.vehdjk.com/Article/details/gdncqvsiv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gmfrqnnjv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.sjlbkw.cn/Article/details/gfcssdbod.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.bbcook.cn/Article/details/gsrocfegb.sHtML

[H07] 断言
来源：http://www.share.yfazqb.com/Article/details/gystzkuqj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.epnwcf.com/Article/details/gpnacszmh.sHtML

PHP:  assert($x > 0);
来源：http://m.share.tarul.cn/Article/details/ganwryptx.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gsmbeumgm.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fktsv.cn/Article/details/gmykpuejy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.tarul.cn/Article/details/gghitgowt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fktsv.cn/Article/details/gsxgnhkby.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.sjlbkw.cn/Article/details/ghqkdinhm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gybfjustw.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fktsv.cn/Article/details/gzylbkvhj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fktsv.cn/Article/details/guucxbkfa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.tarul.cn/Article/details/gluxmdzyc.sHtML


<!-- 参考信息 -->