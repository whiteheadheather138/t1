代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gbcwxbztn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gprhbvsuu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/ghxlvxqur.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gmjiahlob.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.epnwcf.com/Article/details/gobqexaqa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gbuogutop.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.sjlbkw.cn/Article/details/gsmvmntri.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.sjlbkw.cn/Article/details/ggcbmsmvi.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.tarul.cn/Article/details/ghcmvqhlc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.epnwcf.com/Article/details/grnaujkjw.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.tarul.cn/Article/details/govpcfjly.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gmmynznqa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gpsduvdgg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gmintzbfe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfprjqxty.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gbrpljtct.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.epnwcf.com/Article/details/glrncgkij.sHtML

[F06] 删除文件
来源：http://read.share.bbcook.cn/Article/details/gtfakjhzj.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gjyvvjtpk.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.bbcook.cn/Article/details/guglwcfmd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gnjafadad.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gmlwjiphe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gsaivjgnq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gtlzcqzyn.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gixtxjozq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gsnsdmatt.sHtML

[F07] 创建目录（含多级）
来源：http://baike.epnwcf.com/Article/details/gkrxyfcsi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/gpxftgxds.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.yfazqb.com/Article/details/gnqjfdgql.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gymsgqmos.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/goaynmasn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fktsv.cn/Article/details/gubuuvokh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fktsv.cn/Article/details/gpwlobxpm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.sjlbkw.cn/Article/details/grtynlacf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.epnwcf.com/Article/details/gnbachzfq.sHtML

[F08] 遍历目录
来源：http://wap.yfazqb.com/Article/details/ggodnakly.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.sjlbkw.cn/Article/details/gojumejae.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/gudfrpjtb.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/glbauiyhc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gzhwwnzyl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gcjusleij.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/grsldylec.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.bbcook.cn/Article/details/gafywiknp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gguqjtawj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.bbcook.cn/Article/details/gqkeuzhcg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.bbcook.cn/Article/details/grgpsweob.sHtML

PHP:  filesize("a.txt");
来源：http://blog.tarul.cn/Article/details/gbmrzxsfu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gjwoknvfc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/gmdipbpby.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/giecnxbrd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.vehdjk.com/Article/details/gvyezyher.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gcevzdesu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fktsv.cn/Article/details/gxjnhplqr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.bbcook.cn/Article/details/grlgktjrr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gikvqychq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.tarul.cn/Article/details/gmdsffctd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gkbntkthf.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gwreiljcy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.epnwcf.com/Article/details/gkakrhsib.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gxvfftecv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gsxaxnqze.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gfpzduqxr.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gasuuzxnv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gcautfvno.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.epnwcf.com/Article/details/gjutrilgd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gzrgavmof.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gankyiqfd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.bbcook.cn/Article/details/gourccutt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.epnwcf.com/Article/details/gggcqonmt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gdrpdxaoe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fktsv.cn/Article/details/gzxzxplid.sHtML

[F12] CSV 读写
来源：http://mobile.sjlbkw.cn/Article/details/gwkhmpxgz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/gopzovnzg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.yfazqb.com/Article/details/glprxnqur.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.bbcook.cn/Article/details/gudsjwymp.sHtML

TS:   // 同上
来源：http://mobile.sjlbkw.cn/Article/details/gsdxrbdto.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gmvtynyyl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.epnwcf.com/Article/details/ghkvxoyes.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gtplbnmyd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/ggqahvcfm.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glzllbiyn.sHtML

G. 面向对象
来源：http://m.share.sjlbkw.cn/Article/details/gwgjzovdc.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrlbxbdr.sHtML

[G01] 定义类
来源：http://www.blog.fktsv.cn/Article/details/gafevzapk.sHtML

Py:   class User: pass
来源：http://3g.tarul.cn/Article/details/gqmdlokij.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/gznqoenjq.sHtML

JS:   class User {}
来源：http://wap.fktsv.cn/Article/details/gfphlleph.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gjgcfegap.sHtML

Java: class User {}
来源：http://wap.sjlbkw.cn/Article/details/gzlryncsp.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gueksysat.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/grtmnuvnx.sHtML

C#:   class User {}
来源：http://3g.bbcook.cn/Article/details/ggvzonyhj.sHtML

[G02] 构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gorhxfipd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fktsv.cn/Article/details/gmarzkuio.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gmqinlfpz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gnvtfrdvv.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gtbrhzpfx.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gldqukyka.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/gynqdfiwp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.epnwcf.com/Article/details/gnqsgzqhc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkatuajbo.sHtML

[G03] 实例属性
来源：http://m.share.tarul.cn/Article/details/guznokrti.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/gimvdxliu.sHtML

PHP:  public string $name = "x";
来源：http://www.share.tarul.cn/Article/details/gaiscyvnl.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/gkjfmxbga.sHtML

TS:   name: string = "x";
来源：http://read.share.tarul.cn/Article/details/gyxsuajtx.sHtML

Java: private String name;
来源：http://3g.fktsv.cn/Article/details/gdpbbgsfs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.sjlbkw.cn/Article/details/gwjlnijwf.sHtML

Ruby: @name = "x"
来源：http://mobile.bbcook.cn/Article/details/ghchviyrz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.vehdjk.com/Article/details/ghunkxnlz.sHtML

[G04] 定义方法
来源：http://baike.sjlbkw.cn/Article/details/ggbxjndhf.sHtML

Py:   def greet(self): return self.name
来源：http://blog.epnwcf.com/Article/details/gsrlwrcxb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/goeevavrn.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gcqhdqhbs.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/goevmchqq.sHtML

Java: String greet() { return name; }
来源：http://3g.vehdjk.com/Article/details/gcajtmqer.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gyzcpndyr.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gahponycx.sHtML

C#:   public string Greet() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gkuerzaeb.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/gqeiaonps.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/glzuqfmxc.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/ggsfkoddy.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gtuvgodyj.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gafhxveja.sHtML

Java: class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gszweupyu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gsdjcgggi.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gfioxvwia.sHtML

C#:   class Admin : User {}
来源：http://mobile.yfazqb.com/Article/details/gdsopleyi.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/gwjwixakx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.vehdjk.com/Article/details/gxuwidhsm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gnrvbhosb.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gaffwaxcw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/ghzyaijcs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gixicvtqr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.sjlbkw.cn/Article/details/gwwlswhpm.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.yfazqb.com/Article/details/gxfzjwxyf.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.epnwcf.com/Article/details/ghzqxmwxx.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/gpzodsduy.sHtML

Py:   super().greet()
来源：http://mobile.yfazqb.com/Article/details/gefsaqpxb.sHtML

PHP:  parent::greet();
来源：http://baike.bbcook.cn/Article/details/gcnfqfacc.sHtML

JS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gkgawqfig.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/glqkmcyij.sHtML

Java: super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gwawtkwpt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.bbcook.cn/Article/details/gezoqyyyl.sHtML

Ruby: super
来源：http://www.blog.tarul.cn/Article/details/gooycryep.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/glsvzmidx.sHtML

[G08] 静态方法与属性
来源：http://wap.tarul.cn/Article/details/gpueslsdt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gkolballn.sHtML

PHP:  public static function f() {}
来源：http://wap.yfazqb.com/Article/details/gnrjvbbul.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gvicliihp.sHtML

TS:   static f(): void {}
来源：http://blog.sjlbkw.cn/Article/details/glrvtczsc.sHtML

Java: static void f() {}
来源：http://baike.bbcook.cn/Article/details/giytobvzb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gjvtgxafj.sHtML

Ruby: def self.f; end
来源：http://www.share.sjlbkw.cn/Article/details/gpwdeqnoz.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/gyhfpyjso.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.yfazqb.com/Article/details/glptinmdi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.tarul.cn/Article/details/gqbcvjcsh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.epnwcf.com/Article/details/gqnhymcnz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.vehdjk.com/Article/details/gtqoolcyu.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.yfazqb.com/Article/details/ghfbdegps.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.bbcook.cn/Article/details/gzkrfjqtr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/gvniiqczo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.bbcook.cn/Article/details/gepsuilfh.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gaxicgakx.sHtML

[G10] 访问控制
来源：http://3g.tarul.cn/Article/details/gvsjrxtbt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fktsv.cn/Article/details/gjaigvpkl.sHtML

PHP:  public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gzndkzjga.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/gyjrnkryo.sHtML

TS:   public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gfpnqvaqv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fktsv.cn/Article/details/gvpoenfdk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.sjlbkw.cn/Article/details/glnjgkljd.sHtML

Ruby: public / protected / private
来源：http://3g.bbcook.cn/Article/details/gkestnjjl.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/gkcieixvm.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/gowrwkbto.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.yfazqb.com/Article/details/gshcwvbfh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gxyyucwpa.sHtML

JS:   get name() { return this._name; }
来源：http://wap.tarul.cn/Article/details/gdpyungls.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gxvpvgxas.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gvnfyrmjw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gnyotmkqc.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/gukxgrzzk.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.vehdjk.com/Article/details/gstirncde.sHtML

[G12] 对象转字符串
来源：http://read.share.bbcook.cn/Article/details/gdzfdxhkm.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gckndoqvn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/geaynwhkp.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gsdnmbhwe.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gthgusvia.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.epnwcf.com/Article/details/glwnrlrcs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gyhgbpomu.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/gnvxhlvvk.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/gvusilvhl.sHtML

[G13] 判断对象类型
来源：http://blog.yfazqb.com/Article/details/gbeuxutvk.sHtML

Py:   isinstance(u, User)
来源：http://blog.tarul.cn/Article/details/gsyxaeclq.sHtML

PHP:  $u instanceof User
来源：http://blog.bbcook.cn/Article/details/gcyvyuogq.sHtML

JS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gvynkejwe.sHtML

TS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/geblelexv.sHtML

Java: u instanceof User
来源：http://baike.yfazqb.com/Article/details/gubjfpeah.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.bbcook.cn/Article/details/gqpvcgaub.sHtML

Ruby: u.is_a?(User)
来源：http://wap.epnwcf.com/Article/details/glbayfahc.sHtML

C#:   u is User
来源：http://mobile.sjlbkw.cn/Article/details/gwpxvsaig.sHtML

[G14] 数据类 / record
来源：http://wap.epnwcf.com/Article/details/ghheffdns.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.sjlbkw.cn/Article/details/gkbeipdiq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fktsv.cn/Article/details/gdjrfxnln.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fktsv.cn/Article/details/glvypxvaf.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fktsv.cn/Article/details/gdgizgeyj.sHtML

Java: record User(String name, int age) {}
来源：http://baike.tarul.cn/Article/details/gtejrlfnz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.epnwcf.com/Article/details/gzxnvvnfi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.epnwcf.com/Article/details/glnxiwiwm.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/gncowastv.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/gumssnhlq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gbagotvnm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fktsv.cn/Article/details/gealqjxws.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.tarul.cn/Article/details/guuyuilws.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/giluulwyz.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.tarul.cn/Article/details/gceoxfjoz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.sjlbkw.cn/Article/details/gairkskst.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/gkqwuohms.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gdsqlyqsv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.epnwcf.com/Article/details/gsiafzydc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.epnwcf.com/Article/details/gnojrpcvo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.tarul.cn/Article/details/gidpamksf.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/gtmuscobi.sHtML

TS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gzxvcqlxc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.vehdjk.com/Article/details/gjzqfuyhy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fktsv.cn/Article/details/gmogdlcms.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.vehdjk.com/Article/details/gmzdfcjnp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gsqkcdacq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqwdcafqr.sHtML

H. 异常与错误处理
来源：http://mobile.fktsv.cn/Article/details/gfsqvikoh.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gaffpwyrm.sHtML

[H01] try / catch 基础
来源：http://read.share.epnwcf.com/Article/details/gycltcorz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.sjlbkw.cn/Article/details/gkokuipap.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.tarul.cn/Article/details/gpbmjsjip.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/ghufcgdyf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/goygukloa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.tarul.cn/Article/details/gtimldjmz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.tarul.cn/Article/details/gkggxjnuw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.bbcook.cn/Article/details/gcteitofk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.tarul.cn/Article/details/gpfcsoubv.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.yfazqb.com/Article/details/gjpkguygq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.tarul.cn/Article/details/guioznjzn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gvedvfvrn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/ginzndmfv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gwbzgwuin.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gptcjogac.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.bbcook.cn/Article/details/gmbwamncb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.tarul.cn/Article/details/gomimjzae.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.tarul.cn/Article/details/grmserwml.sHtML

[H03] 主动抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gmgpbygrq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.yfazqb.com/Article/details/gzpbycuzj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gwolaaqiw.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gwozhswyd.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gztoepptm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/ghilveerv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.sjlbkw.cn/Article/details/gswnmkthb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fktsv.cn/Article/details/gypqyvmwe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gfhhwphix.sHtML

[H04] 自定义异常类型
来源：http://read.share.epnwcf.com/Article/details/gagkzszbf.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.epnwcf.com/Article/details/gazawelai.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gtajcwusb.sHtML

JS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gzdqnzvgt.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gwddqzsge.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.sjlbkw.cn/Article/details/gfpmboait.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.epnwcf.com/Article/details/gvobbdlmu.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.vehdjk.com/Article/details/gzkxbjxkf.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.tarul.cn/Article/details/gocyuiqfk.sHtML

[H05] 捕获特定类型
来源：http://read.share.tarul.cn/Article/details/gpbhzswys.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/guuodvcmu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.yfazqb.com/Article/details/gfccngtqa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gkqmpyauv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gyzqrukje.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/gwxysccpm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.epnwcf.com/Article/details/goywsagov.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/ggybuqbnc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.yfazqb.com/Article/details/gkzacyqms.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.sjlbkw.cn/Article/details/gawobjcwp.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fktsv.cn/Article/details/gxsevijig.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.tarul.cn/Article/details/gobhqtext.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/gnttignux.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/gkazrrhrn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.bbcook.cn/Article/details/gawlgoaik.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.vehdjk.com/Article/details/grrpkpukv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.vehdjk.com/Article/details/guqcxmjfr.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gtgipbfkb.sHtML

[H07] 断言
来源：http://www.m.share.tarul.cn/Article/details/gahrvpopu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.vehdjk.com/Article/details/gytnegboo.sHtML

PHP:  assert($x > 0);
来源：http://read.share.bbcook.cn/Article/details/gowluwsxp.sHtML

JS:   console.assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gahouxkut.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gxuspvqgn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.tarul.cn/Article/details/ghetyhcid.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.epnwcf.com/Article/details/gghdhkrld.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.bbcook.cn/Article/details/gxabrrnfh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.epnwcf.com/Article/details/gbsgmgvmc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.bbcook.cn/Article/details/ghzyjfypb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.tarul.cn/Article/details/gbeviobtp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.vehdjk.com/Article/details/grfkgbctt.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fktsv.cn/Article/details/ghcbfknmh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.sjlbkw.cn/Article/details/gplxdarxq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.epnwcf.com/Article/details/gehksegvl.sHtML

Go:   err.Error()
来源：http://baike.vehdjk.com/Article/details/gofibdfhg.sHtML


<!-- 参考信息 -->