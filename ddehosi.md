代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.bbcook.cn/Article/details/gmbyzndke.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/gpzgnewbq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gewjwoqyv.sHtML

[F04] 追加写入文件
来源：http://mobile.sjlbkw.cn/Article/details/ggpwniwye.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/giyewtvfh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fktsv.cn/Article/details/gzxwrptjh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gscgsehwl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gvnnpqynx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.sjlbkw.cn/Article/details/gviyufpds.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.tarul.cn/Article/details/gswuthwnh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.yfazqb.com/Article/details/gnittbgll.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.epnwcf.com/Article/details/goktwgxul.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.yfazqb.com/Article/details/gkvddvyrw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/guokoohzx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/ggksgbtid.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gvvjshhsr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gfldbwpdy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gxmfuvpfd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.sjlbkw.cn/Article/details/gsohwyvmi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/glicwsbpl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.tarul.cn/Article/details/gfsjxotvi.sHtML

[F06] 删除文件
来源：http://www.share.bbcook.cn/Article/details/gntabhlul.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/grzldjhto.sHtML

PHP:  unlink("a.txt");
来源：http://wap.yfazqb.com/Article/details/gqaweklhb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/guflaqrln.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gmuxwinkj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/giwodxkbv.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gsxclnpmm.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.vehdjk.com/Article/details/gtegyyito.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gsvlzrepp.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fktsv.cn/Article/details/gtairlxaq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gbysotfll.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.sjlbkw.cn/Article/details/gjjyxkanh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gmhjgcbuo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gwaayehxk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.bbcook.cn/Article/details/gxosyvfii.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.sjlbkw.cn/Article/details/gsbjiqota.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/guhsbrtjf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fktsv.cn/Article/details/gbfegaxrs.sHtML

[F08] 遍历目录
来源：http://baike.vehdjk.com/Article/details/ghexzuvoi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.bbcook.cn/Article/details/gvuaeihob.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.epnwcf.com/Article/details/gtnwcqluk.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gpmsxbbfo.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gevzucoge.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gphgnseum.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gvnvtxvrq.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.vehdjk.com/Article/details/gfdlomzgr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.bbcook.cn/Article/details/gahunegaw.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/gxbledcvd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.vehdjk.com/Article/details/gsigvmttt.sHtML

PHP:  filesize("a.txt");
来源：http://baike.tarul.cn/Article/details/gdnxnjdjq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gctoxwcug.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/grygmbhyr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gewkukqik.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.epnwcf.com/Article/details/gvuftyvxm.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gkzgqooaj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fktsv.cn/Article/details/gqioarlcb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fktsv.cn/Article/details/gvtfnklfe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/grrnmkhrd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gecefnvhf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ghxzkptdo.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gxaxuqhbg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.sjlbkw.cn/Article/details/gmqdemcyv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/grpztzalr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gowcvlfof.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gzhvgmqwh.sHtML

[F11] 复制与移动文件
来源：http://wap.vehdjk.com/Article/details/gycjbylzm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gamdnjcuv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.yfazqb.com/Article/details/gxijwehfk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gmbtqnmso.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gykduciyk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/ggambujjd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gwahymyfn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gizvxiust.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.tarul.cn/Article/details/gcmijpldj.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/gnrsejixh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fktsv.cn/Article/details/gkrkcosnq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/gbhbbkzss.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.bbcook.cn/Article/details/gmrztiqua.sHtML

TS:   // 同上
来源：http://baike.fktsv.cn/Article/details/guhqnttyc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/giijznvrk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/gcsoetryn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gnayrclcz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/goffyliwa.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvyxxqder.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/geprkflqv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gyjghgdrh.sHtML

[G01] 定义类
来源：http://www.m.share.tarul.cn/Article/details/gtkmkatqf.sHtML

Py:   class User: pass
来源：http://wap.tarul.cn/Article/details/gghfebmky.sHtML

PHP:  class User {}
来源：http://baike.yfazqb.com/Article/details/gbmejwqon.sHtML

JS:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gifwgosdb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.yfazqb.com/Article/details/gzkeqwhoe.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/gbvpducqb.sHtML

Go:   type User struct { Name string }
来源：http://blog.tarul.cn/Article/details/gsyccybmy.sHtML

Ruby: class User; end
来源：http://blog.fktsv.cn/Article/details/ggcpmagqt.sHtML

C#:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/goagqmqwg.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/gpljdmojg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.yfazqb.com/Article/details/gufdtscdj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/gncsvhokt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/gvqhkzcjh.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.epnwcf.com/Article/details/gxfhakrls.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggorwpotu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.epnwcf.com/Article/details/gterhwyut.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/grpcuftkj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gghyicmbx.sHtML

[G03] 实例属性
来源：http://wap.fktsv.cn/Article/details/gecwbkykk.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/grlkhtxtv.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gxeancnip.sHtML

JS:   this.name = "x";
来源：http://wap.tarul.cn/Article/details/gtylmgzms.sHtML

TS:   name: string = "x";
来源：http://m.share.yfazqb.com/Article/details/gdhdvmeyp.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/gjecavywe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/goncwflym.sHtML

Ruby: @name = "x"
来源：http://wap.bbcook.cn/Article/details/gesztszif.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/guupizmew.sHtML

[G04] 定义方法
来源：http://wap.tarul.cn/Article/details/gznwjorty.sHtML

Py:   def greet(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gyrtnntww.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gqbzeuxse.sHtML

JS:   greet() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/ggjqlcimk.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gmfmyjaiw.sHtML

Java: String greet() { return name; }
来源：http://read.share.yfazqb.com/Article/details/guetlqcde.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gtklahnzj.sHtML

Ruby: def greet; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gnnijwuan.sHtML

C#:   public string Greet() => Name;
来源：http://blog.epnwcf.com/Article/details/goxqsaxyd.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gdklhuvnk.sHtML

Py:   class Admin(User): pass
来源：http://baike.vehdjk.com/Article/details/gtqwujrhp.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/glyeurrzk.sHtML

JS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gncnpdscy.sHtML

TS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gjeumoeld.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gizstvezc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsmxlahv.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gifxtpvnj.sHtML

C#:   class Admin : User {}
来源：http://read.share.tarul.cn/Article/details/gcqbaapna.sHtML

[G06] 重写方法
来源：http://www.blog.yfazqb.com/Article/details/gvlvqvxfj.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/gjxepzpns.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gxadjovhl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gczrhmkfl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gyldyldov.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gptrpcilq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.epnwcf.com/Article/details/gnlncfnmt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fktsv.cn/Article/details/gmafqhzfq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.vehdjk.com/Article/details/gefkcykjc.sHtML

[G07] 调用父类方法
来源：http://read.share.yfazqb.com/Article/details/gvrfnheek.sHtML

Py:   super().greet()
来源：http://www.share.tarul.cn/Article/details/gsmytswlx.sHtML

PHP:  parent::greet();
来源：http://blog.fktsv.cn/Article/details/gwercampx.sHtML

JS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gtxxewpvu.sHtML

TS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gqbppugxu.sHtML

Java: super.greet();
来源：http://baike.epnwcf.com/Article/details/giojdcyjf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/gqldgyxje.sHtML

Ruby: super
来源：http://www.m.share.vehdjk.com/Article/details/gnmdzisjp.sHtML

C#:   base.Greet();
来源：http://m.share.tarul.cn/Article/details/gwkegbjfq.sHtML

[G08] 静态方法与属性
来源：http://m.share.tarul.cn/Article/details/gczyzudko.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.vehdjk.com/Article/details/ggielkekt.sHtML

PHP:  public static function f() {}
来源：http://blog.bbcook.cn/Article/details/gpciwcicg.sHtML

JS:   static f() {}
来源：http://mobile.epnwcf.com/Article/details/gqzywsyhr.sHtML

TS:   static f(): void {}
来源：http://www.m.share.bbcook.cn/Article/details/grkncwlsu.sHtML

Java: static void f() {}
来源：http://read.share.fktsv.cn/Article/details/guvwqpxny.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/ghrllkqbb.sHtML

Ruby: def self.f; end
来源：http://blog.epnwcf.com/Article/details/gswyyxnek.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/ghcueczir.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/guhhcdnwm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.bbcook.cn/Article/details/gfnaudlml.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.bbcook.cn/Article/details/gxtsjrxym.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/gdjqyedgc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.vehdjk.com/Article/details/gwlrnphji.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.bbcook.cn/Article/details/gifxorpoi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.sjlbkw.cn/Article/details/gaakgppfn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fktsv.cn/Article/details/gnsytjcnt.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/grwguezio.sHtML

[G10] 访问控制
来源：http://m.share.sjlbkw.cn/Article/details/gutjpobhu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.sjlbkw.cn/Article/details/gbzyyyubv.sHtML

PHP:  public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/grehvxnay.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.epnwcf.com/Article/details/gyftevesx.sHtML

TS:   public / protected / private
来源：http://blog.bbcook.cn/Article/details/glpeniema.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/gzocgdggr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fktsv.cn/Article/details/gzlomeead.sHtML

Ruby: public / protected / private
来源：http://blog.bbcook.cn/Article/details/gqzuoojeg.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fktsv.cn/Article/details/gfcjgmwvz.sHtML

[G11] getter / setter
来源：http://m.share.fktsv.cn/Article/details/giideifrm.sHtML

Py:   @property 与 @x.setter
来源：http://blog.sjlbkw.cn/Article/details/gwrnqturv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/givayvlap.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gxaqbfjtq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gzxmlzysk.sHtML

Java: public String getName() { return name; }
来源：http://blog.yfazqb.com/Article/details/gnswacuae.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gerhuyxai.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fktsv.cn/Article/details/ggagptwsv.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fktsv.cn/Article/details/gotmqdrik.sHtML

[G12] 对象转字符串
来源：http://baike.vehdjk.com/Article/details/gxbmapaha.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/ggbajipwa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/godmwqcha.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/ggfqnmsyh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gowrxyssz.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gexrtrjzn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gvpyycgda.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.yfazqb.com/Article/details/gybwbitzw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/ghoskbdlz.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gtdasbzus.sHtML

Py:   isinstance(u, User)
来源：http://mobile.tarul.cn/Article/details/gwicfobyg.sHtML

PHP:  $u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gfhevenuw.sHtML

JS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/glcjtxgwo.sHtML

TS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/gumwgtzwu.sHtML

Java: u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/ghnnkhxzl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.bbcook.cn/Article/details/gdhrvxclj.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/glldakbaj.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/ggdonpwfc.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/gzpbsddyb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.vehdjk.com/Article/details/ghclvrmgh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.tarul.cn/Article/details/gdytbqwvv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.bbcook.cn/Article/details/gzxmiuzyf.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fktsv.cn/Article/details/gbeimpbtl.sHtML

Java: record User(String name, int age) {}
来源：http://baike.yfazqb.com/Article/details/guqzgvdot.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gokxvhkxl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fktsv.cn/Article/details/gihnklmbb.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.bbcook.cn/Article/details/gulnejprh.sHtML

[G15] 枚举
来源：http://m.share.bbcook.cn/Article/details/gqhynslom.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gfcxupnvp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.bbcook.cn/Article/details/gxwwlbgyj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.epnwcf.com/Article/details/gkicxwpvz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gwyntmtsc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fktsv.cn/Article/details/gxzkrcqsk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.epnwcf.com/Article/details/gethrzbbg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.yfazqb.com/Article/details/gariclahu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/gabbweejp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fktsv.cn/Article/details/gjprzsbsc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.vehdjk.com/Article/details/gpixfcrlz.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.sjlbkw.cn/Article/details/gpbswghvf.sHtML

JS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gpkvangrt.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gaejdapbu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.sjlbkw.cn/Article/details/gfcenvcud.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.bbcook.cn/Article/details/gnvpampvm.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fktsv.cn/Article/details/gpsyxqxsm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/giowwbnmx.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtaqdqphs.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gnlmkakud.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gembdiryo.sHtML

[H01] try / catch 基础
来源：http://mobile.vehdjk.com/Article/details/ghzaywoqt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.vehdjk.com/Article/details/gdrmjxshw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.vehdjk.com/Article/details/gqskfblgb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gowthxbbl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/glnzbxoyt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.vehdjk.com/Article/details/gqjvendrz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.tarul.cn/Article/details/gteldvxwq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fktsv.cn/Article/details/gsvndyujv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.yfazqb.com/Article/details/ghwxhjkmp.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.bbcook.cn/Article/details/gwiduceel.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.sjlbkw.cn/Article/details/gooaqnebe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gjitwgxie.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gmbljatrt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/getsbeflg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/ghoyirdlf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.tarul.cn/Article/details/gilqfqcaj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.sjlbkw.cn/Article/details/giyblrjdg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gwutjfagy.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/ghnhddcsg.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.vehdjk.com/Article/details/gliqtcvkn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gpzcfnqwo.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/gvhshpqvg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gtredgtjs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/ghkrayuyi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.bbcook.cn/Article/details/gluobqkcu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gboyhjzpq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gqnqgjsxm.sHtML

[H04] 自定义异常类型
来源：http://blog.bbcook.cn/Article/details/gooblrygr.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.sjlbkw.cn/Article/details/gcgesqufr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/gouvchlor.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gpukfdazr.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gkeasrasc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gyueuwdge.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.bbcook.cn/Article/details/grdihxfyl.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.bbcook.cn/Article/details/gnfsdfcgj.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.vehdjk.com/Article/details/gjysrqbmc.sHtML

[H05] 捕获特定类型
来源：http://read.share.bbcook.cn/Article/details/gfuiiucnz.sHtML

Py:   except ValueError as e:
来源：http://read.share.fktsv.cn/Article/details/gvsesgwkx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.yfazqb.com/Article/details/gljmpxkjb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gutecqotv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gwegrmcmb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.vehdjk.com/Article/details/gaxjexshs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.sjlbkw.cn/Article/details/gqkslloly.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.sjlbkw.cn/Article/details/gfunlquwa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.bbcook.cn/Article/details/ghuxawgko.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.epnwcf.com/Article/details/gpvcqdrrz.sHtML

Py:   value = d.get("k") or default
来源：http://blog.sjlbkw.cn/Article/details/gcwvzuzev.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gnbtrizic.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gpjaslmwx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/ggylvppkc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fktsv.cn/Article/details/gxysxrgqk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.sjlbkw.cn/Article/details/ghqmsdjrq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.sjlbkw.cn/Article/details/gpzkzmrsy.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.tarul.cn/Article/details/gnpqxnepq.sHtML

[H07] 断言
来源：http://m.share.sjlbkw.cn/Article/details/gchgpkjfx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.tarul.cn/Article/details/gbrahqrpw.sHtML

PHP:  assert($x > 0);
来源：http://www.share.epnwcf.com/Article/details/gvqduixhg.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gxqkxtczl.sHtML

TS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gdqigxilx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/gxuvsczie.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.vehdjk.com/Article/details/gdpvasrqv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.bbcook.cn/Article/details/gdlkwxbwo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/gxbnhyrfl.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.vehdjk.com/Article/details/gfhgzoipc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.sjlbkw.cn/Article/details/gknilqlwa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.tarul.cn/Article/details/gigdadkbt.sHtML


<!-- 参考信息 -->