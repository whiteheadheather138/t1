代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.epnwcf.com/Article/details/gkrypxqrf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/gsudshwfo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gztykubfw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.bbcook.cn/Article/details/goekswaxf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpvfqtmr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.tarul.cn/Article/details/guivtenal.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.tarul.cn/Article/details/ghpapxkjv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.yfazqb.com/Article/details/gayeybksz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.tarul.cn/Article/details/gnotegvnl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.tarul.cn/Article/details/ggiuafeob.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gedhyiast.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gureckcfy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/ggcgisikx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gffuasafy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.epnwcf.com/Article/details/grbspapac.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fktsv.cn/Article/details/gsypvhuxz.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.bbcook.cn/Article/details/gtmcwadtg.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/gkrroxnos.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gaepsakui.sHtML

PHP:  unlink("a.txt");
来源：http://wap.epnwcf.com/Article/details/giltekrfn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gpqjxlxnb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/glvooaaow.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gvehkwwut.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gpioodcyt.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.yfazqb.com/Article/details/gvncdzwyr.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.yfazqb.com/Article/details/ghegghxvp.sHtML

[F07] 创建目录（含多级）
来源：http://3g.vehdjk.com/Article/details/gwpgcbdzz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gpahdafvo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fktsv.cn/Article/details/grvqhhnre.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gcqydzhbh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gfsccsojg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.sjlbkw.cn/Article/details/gdbdogzed.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.tarul.cn/Article/details/gckubrjrb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fktsv.cn/Article/details/gmpgmodmk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.vehdjk.com/Article/details/glxqcunio.sHtML

[F08] 遍历目录
来源：http://blog.yfazqb.com/Article/details/gzuxhkrkw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/gcjgwwxqe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.tarul.cn/Article/details/gvizntfpr.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gfpcooyok.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/ggtzhdmcy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/genfhomvf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.bbcook.cn/Article/details/gcrickfvc.sHtML

Ruby: Dir.children("dir")
来源：http://baike.epnwcf.com/Article/details/grlfwqvqj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.bbcook.cn/Article/details/gdlvpotjx.sHtML

[F09] 获取文件大小
来源：http://m.share.sjlbkw.cn/Article/details/gyuwktect.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gnmgvfhcq.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gqupdevac.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gtoxlyfnr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gpgltqimy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gbfdedxdq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.epnwcf.com/Article/details/gfslkyexh.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gieseuitl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fktsv.cn/Article/details/grhhectlk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/gkmytoadk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gyzudlkeb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/ggfnztdoe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gsrwftidq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.vehdjk.com/Article/details/govtlopnv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.yfazqb.com/Article/details/gphwrtxxs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gqmorgimp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gvxvmynuu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gwikcbkwy.sHtML

[F11] 复制与移动文件
来源：http://blog.yfazqb.com/Article/details/gwbbmgyca.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gullgodbw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.vehdjk.com/Article/details/gamjhdkhn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gyrcqexxb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gctroiotn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.bbcook.cn/Article/details/ghzspenei.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.sjlbkw.cn/Article/details/gejhbzovz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gycwrvcdw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/gufggetve.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/gbbzwvbdl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/gkccoisfr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.yfazqb.com/Article/details/garhdvdse.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.yfazqb.com/Article/details/gjchjqixb.sHtML

TS:   // 同上
来源：http://m.share.bbcook.cn/Article/details/gwllgzsuu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gdttlxjja.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.yfazqb.com/Article/details/gegiredfr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.tarul.cn/Article/details/gfdmrybcq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.yfazqb.com/Article/details/gwczzxunt.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghdteixrb.sHtML

G. 面向对象
来源：http://3g.sjlbkw.cn/Article/details/gowvbqjns.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gyeipoayd.sHtML

[G01] 定义类
来源：http://www.blog.epnwcf.com/Article/details/gqharecmn.sHtML

Py:   class User: pass
来源：http://3g.sjlbkw.cn/Article/details/gvciasmtk.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/glmaeotwr.sHtML

JS:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gsxswbwbr.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/guecmgvza.sHtML

Java: class User {}
来源：http://www.blog.bbcook.cn/Article/details/gqnnrkyqt.sHtML

Go:   type User struct { Name string }
来源：http://www.share.tarul.cn/Article/details/grbykqpyy.sHtML

Ruby: class User; end
来源：http://www.share.fktsv.cn/Article/details/ggprbcgpg.sHtML

C#:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gjrrfseul.sHtML

[G02] 构造函数
来源：http://m.share.yfazqb.com/Article/details/gesphdidz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/gpmlhvmgu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.yfazqb.com/Article/details/glvgbrmcy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gmoucqkgg.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.sjlbkw.cn/Article/details/gwbvrsktc.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gyanmggdy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.tarul.cn/Article/details/gedqessgn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fktsv.cn/Article/details/geilnbuha.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gwappidcy.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/gbmrrhuxm.sHtML

Py:   self.name = "x"
来源：http://wap.vehdjk.com/Article/details/gvlngysad.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/ghxdzhllu.sHtML

JS:   this.name = "x";
来源：http://www.share.tarul.cn/Article/details/gnaynlava.sHtML

TS:   name: string = "x";
来源：http://3g.vehdjk.com/Article/details/gmrjvastk.sHtML

Java: private String name;
来源：http://blog.sjlbkw.cn/Article/details/gvkhqxtpt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.tarul.cn/Article/details/gmwspivxw.sHtML

Ruby: @name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/gsknmdbje.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.epnwcf.com/Article/details/ghdjxrdrk.sHtML

[G04] 定义方法
来源：http://read.share.vehdjk.com/Article/details/gflqrekba.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/ghwzurwsm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gcslizcbz.sHtML

JS:   greet() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gjaokmnnq.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gorapulye.sHtML

Java: String greet() { return name; }
来源：http://baike.vehdjk.com/Article/details/gjjotiqzy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gjdzkagwa.sHtML

Ruby: def greet; @name; end
来源：http://baike.vehdjk.com/Article/details/gukcnkfyb.sHtML

C#:   public string Greet() => Name;
来源：http://wap.tarul.cn/Article/details/gttyjcruy.sHtML

[G05] 继承
来源：http://m.share.fktsv.cn/Article/details/gckyqqqbz.sHtML

Py:   class Admin(User): pass
来源：http://mobile.vehdjk.com/Article/details/gejluzdbd.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmetqltot.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gbgljrsli.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gmhzyiafl.sHtML

Java: class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gdguwxsyw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.bbcook.cn/Article/details/gxzsqeqrc.sHtML

Ruby: class Admin < User; end
来源：http://www.share.yfazqb.com/Article/details/gwvittbzn.sHtML

C#:   class Admin : User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkksggzst.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gbeloweqe.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/gsrehxuro.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gbzjmmqef.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gikxofely.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gpsgabbtz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gtoyabqbw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.epnwcf.com/Article/details/gwiwbfihp.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.epnwcf.com/Article/details/gkwptkubi.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.vehdjk.com/Article/details/gwribpsto.sHtML

[G07] 调用父类方法
来源：http://baike.bbcook.cn/Article/details/gxheidgxe.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/gihvtsubz.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gonlomgyg.sHtML

JS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gibawnmbg.sHtML

TS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gbjuaskai.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gmiicnrdw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fktsv.cn/Article/details/gmxiultke.sHtML

Ruby: super
来源：http://blog.epnwcf.com/Article/details/glgoenutj.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/gpyovgzhn.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/gkwwhlvmt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.vehdjk.com/Article/details/gcznzqqpp.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/guzcsgomb.sHtML

JS:   static f() {}
来源：http://m.share.tarul.cn/Article/details/gtmhzknzb.sHtML

TS:   static f(): void {}
来源：http://read.share.tarul.cn/Article/details/gqghzeyui.sHtML

Java: static void f() {}
来源：http://www.share.epnwcf.com/Article/details/gjqataxcf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.epnwcf.com/Article/details/gykjggrlt.sHtML

Ruby: def self.f; end
来源：http://read.share.fktsv.cn/Article/details/gpzncgpcy.sHtML

C#:   public static void F() {}
来源：http://www.share.fktsv.cn/Article/details/gfujzpvrn.sHtML

[G09] 接口 / 抽象类
来源：http://3g.vehdjk.com/Article/details/gadnracmj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fktsv.cn/Article/details/glhbghqcw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.bbcook.cn/Article/details/gqjivojnt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.vehdjk.com/Article/details/gchoiytdx.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.epnwcf.com/Article/details/ggsvsqhsp.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fktsv.cn/Article/details/gezrfryxk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.vehdjk.com/Article/details/gtuuktipm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/gymjeglbv.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/ghthxyrld.sHtML

[G10] 访问控制
来源：http://mobile.tarul.cn/Article/details/gvluuujld.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.epnwcf.com/Article/details/gblrwcdcl.sHtML

PHP:  public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gutehbtfi.sHtML

JS:   #private 字段；其余公开
来源：http://baike.sjlbkw.cn/Article/details/gzxlddxxb.sHtML

TS:   public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/graxtobdq.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.epnwcf.com/Article/details/geteljgus.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/gyitmyntv.sHtML

Ruby: public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gzsuzigxu.sHtML

C#:   public / protected / private / internal
来源：http://baike.sjlbkw.cn/Article/details/gwmujbrqi.sHtML

[G11] getter / setter
来源：http://wap.tarul.cn/Article/details/glcuaghvw.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.bbcook.cn/Article/details/gfpxmlmwx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gwdapknge.sHtML

JS:   get name() { return this._name; }
来源：http://blog.yfazqb.com/Article/details/ghlyazqbf.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gohdsckvr.sHtML

Java: public String getName() { return name; }
来源：http://3g.epnwcf.com/Article/details/ggytmvwjc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/grkwpiudd.sHtML

Ruby: attr_accessor :name
来源：http://www.share.vehdjk.com/Article/details/gexzjyeuq.sHtML

C#:   public string Name { get; set; }
来源：http://3g.vehdjk.com/Article/details/gkdokzjge.sHtML

[G12] 对象转字符串
来源：http://m.share.tarul.cn/Article/details/gzhtyogye.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gfvflrnom.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gbcpnhihh.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gipwrltjs.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gupvpjqhp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gguzsadwb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gbfsvgiqo.sHtML

Ruby: def to_s; @name; end
来源：http://3g.bbcook.cn/Article/details/ghaqrcxca.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/grxzrymtm.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/grkrchkav.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fktsv.cn/Article/details/gynlrrrml.sHtML

PHP:  $u instanceof User
来源：http://mobile.epnwcf.com/Article/details/ghnxxwmmc.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gfkhydvsp.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gluxdkpej.sHtML

Java: u instanceof User
来源：http://baike.vehdjk.com/Article/details/ggxazbyjr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.yfazqb.com/Article/details/gyukqhymf.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.vehdjk.com/Article/details/guxpywvqb.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/grtytkdzn.sHtML

[G14] 数据类 / record
来源：http://blog.epnwcf.com/Article/details/gyhdugdgx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.epnwcf.com/Article/details/gkzncmjii.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.epnwcf.com/Article/details/gjxqqshlg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.yfazqb.com/Article/details/gpzmdovhn.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.sjlbkw.cn/Article/details/gxxntbgpk.sHtML

Java: record User(String name, int age) {}
来源：http://blog.bbcook.cn/Article/details/gtzcnlyfp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/glossoyge.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.tarul.cn/Article/details/gidfrnjvw.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.vehdjk.com/Article/details/gozrcoadc.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/gfybaszrb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.sjlbkw.cn/Article/details/grrnlkijj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/gttouwtkj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.yfazqb.com/Article/details/grpoedmha.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gnqoocskt.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.sjlbkw.cn/Article/details/gsoycplab.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.epnwcf.com/Article/details/gvuiboscv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fktsv.cn/Article/details/gqtmonvcc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gpcichpgr.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.tarul.cn/Article/details/golcgdeoc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.epnwcf.com/Article/details/ghygpvhni.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fktsv.cn/Article/details/ghefivhrf.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gydbvqxcr.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gorqbwlqv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/gbbdmhyyo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/gllsdaphp.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gciqmvadh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gpgwbdfum.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/giiloolgl.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gsrqdnimj.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gdpveubml.sHtML

[H01] try / catch 基础
来源：http://blog.fktsv.cn/Article/details/giayhhykq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/gmpaincfi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.bbcook.cn/Article/details/gpwutmvkr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gmtrpdbau.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gbmooerpp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fktsv.cn/Article/details/gcqphzpyj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.sjlbkw.cn/Article/details/gaqgnfryv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/gydpplwvu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.yfazqb.com/Article/details/gmcczhnir.sHtML

[H02] finally / ensure 收尾
来源：http://wap.vehdjk.com/Article/details/gxtqvzfbo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gukkxphjn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gagdfhiwy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gpcevautn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbnxjplb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gpvjmkwlg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/grmlqoved.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/gepqvddas.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/glyxximhz.sHtML

[H03] 主动抛出异常
来源：http://www.share.yfazqb.com/Article/details/gyhmqvboq.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.yfazqb.com/Article/details/gwizakhub.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gswfgqytr.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/grggxmivn.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gorjytvwc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/grtfdanuo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/gpwwodlsg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.sjlbkw.cn/Article/details/gvsdfzrzp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gaxcjpigg.sHtML

[H04] 自定义异常类型
来源：http://www.blog.yfazqb.com/Article/details/gqskdksxq.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.yfazqb.com/Article/details/ghtfbjgiv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gufxslzus.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gouftfmka.sHtML

TS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gzeezelgy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gqnerprgn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.vehdjk.com/Article/details/gmlhvilfj.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.yfazqb.com/Article/details/gfbffwjzh.sHtML

C#:   class MyException : Exception {}
来源：http://blog.vehdjk.com/Article/details/gnimrvuvj.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gydybtoco.sHtML

Py:   except ValueError as e:
来源：http://wap.tarul.cn/Article/details/gkiftdelg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.tarul.cn/Article/details/gsytejfle.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gdqykyfxw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/gyhqidbld.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.sjlbkw.cn/Article/details/gvjnaugee.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.bbcook.cn/Article/details/gdkxkxadw.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.vehdjk.com/Article/details/gfzcyofft.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbmeqlvd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.tarul.cn/Article/details/gqjnmojqn.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.sjlbkw.cn/Article/details/gofkfwent.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/guxvkqaey.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/gfurqkyqs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gkdoboszx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.epnwcf.com/Article/details/gzkqmlqlp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.sjlbkw.cn/Article/details/ghpaucztb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.sjlbkw.cn/Article/details/gukttprrb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gbpkshekk.sHtML

[H07] 断言
来源：http://wap.bbcook.cn/Article/details/gxyjqjhzs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.epnwcf.com/Article/details/geicbroos.sHtML

PHP:  assert($x > 0);
来源：http://blog.yfazqb.com/Article/details/ggshheeam.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gotvofrjo.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gesxiozmt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fktsv.cn/Article/details/gclyjhqve.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.yfazqb.com/Article/details/gpxuhfadk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.tarul.cn/Article/details/gojffrkhq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gbfewgykt.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.sjlbkw.cn/Article/details/gnvokiamd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.sjlbkw.cn/Article/details/gdgylemje.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.sjlbkw.cn/Article/details/gphtgdvek.sHtML

JS:   e.message;  e.stack
来源：http://m.share.tarul.cn/Article/details/ggpttwpzc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.vehdjk.com/Article/details/gdywhvlxn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.tarul.cn/Article/details/gqlgbgoho.sHtML

Go:   err.Error()
来源：http://wap.epnwcf.com/Article/details/gunjxvcbr.sHtML


<!-- 参考信息 -->