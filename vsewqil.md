代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gvgcbthnf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gaujgtmyr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gzcaxvxjt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.vehdjk.com/Article/details/gytrrpjue.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.epnwcf.com/Article/details/gwepbnudk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gmttuwwyk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/guehplmqy.sHtML

[F04] 追加写入文件
来源：http://mobile.yfazqb.com/Article/details/gyvsmjnog.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fktsv.cn/Article/details/gwqavuqhh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.vehdjk.com/Article/details/gaoffwblf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/golxiqksh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gxzpbjuat.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gaefbykbs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.bbcook.cn/Article/details/gfnadlhbz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fktsv.cn/Article/details/gfvoswooc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.vehdjk.com/Article/details/gdniejlas.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gjmvdnhju.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.sjlbkw.cn/Article/details/gpwzfsodm.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/gfszocghm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gpuqsdkwe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gjgcuwowv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gxmdgskzo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/gdyqighyr.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gqjpnnxhb.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.tarul.cn/Article/details/gkmkumxii.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhhzmxgu.sHtML

Py:   os.remove("a.txt")
来源：http://baike.tarul.cn/Article/details/ghnxqeyzy.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/ghzdibjvh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gnbjvbnvx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gpqxzhruy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/guxvmgcdk.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gvaqnsntq.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.epnwcf.com/Article/details/glnjaztjw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gnstnogjk.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/gjcyaixsi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.tarul.cn/Article/details/gnsqljvae.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.tarul.cn/Article/details/gdummnlqu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gpicnelih.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gmqglvuzv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.epnwcf.com/Article/details/ggedrxhno.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/gsstuqeok.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.vehdjk.com/Article/details/gatgujaum.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.vehdjk.com/Article/details/geccebpqn.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/gcvmqybza.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.bbcook.cn/Article/details/gfaglupdj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.bbcook.cn/Article/details/gbjjbxhzo.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gvffqmxxl.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gbeyjmauf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/ggmqlrhjr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.vehdjk.com/Article/details/grkzumlol.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.yfazqb.com/Article/details/gxmiiqmiy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gvleraktm.sHtML

[F09] 获取文件大小
来源：http://www.share.tarul.cn/Article/details/gstulnjuy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gtwcpjwfp.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gmjqjmqew.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gwnolpruf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/globiqtne.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/grcedemym.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.vehdjk.com/Article/details/gflwlqllp.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gmboqmeqm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.sjlbkw.cn/Article/details/gzqgcioyw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fktsv.cn/Article/details/ggiftqgqx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gmilknqdl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.yfazqb.com/Article/details/gzblfboue.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/ggkwgradr.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fktsv.cn/Article/details/gkhqezqiy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.vehdjk.com/Article/details/grjcuoeup.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gdcytwiba.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gyfajmbba.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gnmrkflvz.sHtML

[F11] 复制与移动文件
来源：http://www.share.vehdjk.com/Article/details/gfeksrnuf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gdpkdozwx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gbbtxxixe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/glvlajjqw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/grdmzontd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.epnwcf.com/Article/details/grmdpfuee.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.sjlbkw.cn/Article/details/gbfdvwtex.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gcqtuuekl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.yfazqb.com/Article/details/gfuykmelq.sHtML

[F12] CSV 读写
来源：http://mobile.fktsv.cn/Article/details/gieutibou.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fktsv.cn/Article/details/ggtezbbdl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.yfazqb.com/Article/details/gmbrygdmf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gdbpcgrll.sHtML

TS:   // 同上
来源：http://m.share.epnwcf.com/Article/details/gkcfssytv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gtaoovmzt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gmbsopcxl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.tarul.cn/Article/details/gyljyyhab.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.sjlbkw.cn/Article/details/gecjbjplb.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gliysaqqo.sHtML

G. 面向对象
来源：http://mobile.epnwcf.com/Article/details/gldqkbaja.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/guphraqzp.sHtML

[G01] 定义类
来源：http://baike.sjlbkw.cn/Article/details/geurwjyed.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/gqwzbbxqf.sHtML

PHP:  class User {}
来源：http://www.share.bbcook.cn/Article/details/gdsxpbggy.sHtML

JS:   class User {}
来源：http://m.share.bbcook.cn/Article/details/guztejjbz.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/gcmawozma.sHtML

Java: class User {}
来源：http://read.share.bbcook.cn/Article/details/gymrhxnle.sHtML

Go:   type User struct { Name string }
来源：http://read.share.sjlbkw.cn/Article/details/gmllccwjz.sHtML

Ruby: class User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gdnmcqlen.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gtxahcsgl.sHtML

[G02] 构造函数
来源：http://www.blog.yfazqb.com/Article/details/geyworgur.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gnhtxuaqv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.sjlbkw.cn/Article/details/gxdkkjcqg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gsfxacnqb.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.tarul.cn/Article/details/gbhmnkbov.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gjbmvgvby.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.sjlbkw.cn/Article/details/gnfrlzmuu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.sjlbkw.cn/Article/details/gdkpmkbhb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.tarul.cn/Article/details/gmofnicso.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/gafptovkd.sHtML

Py:   self.name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/getkwjwrb.sHtML

PHP:  public string $name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gaxlprwad.sHtML

JS:   this.name = "x";
来源：http://blog.tarul.cn/Article/details/gtodzrsvh.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gchtppnyh.sHtML

Java: private String name;
来源：http://www.share.tarul.cn/Article/details/geabrayka.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gfiirkosu.sHtML

Ruby: @name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gojmkwhsh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.tarul.cn/Article/details/gyudlczlh.sHtML

[G04] 定义方法
来源：http://mobile.epnwcf.com/Article/details/gjsjipcjn.sHtML

Py:   def greet(self): return self.name
来源：http://3g.tarul.cn/Article/details/gpkrohmxp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gkxiqbkku.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gnoxuppxl.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gsetevqef.sHtML

Java: String greet() { return name; }
来源：http://wap.yfazqb.com/Article/details/gwslmqlhg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/glcdwumnf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.vehdjk.com/Article/details/govkdjveb.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gjwuruffg.sHtML

[G05] 继承
来源：http://3g.bbcook.cn/Article/details/grrgdogfy.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gyguzfhol.sHtML

PHP:  class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/grzbhqfyl.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gmrstqism.sHtML

TS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gavccdhmv.sHtML

Java: class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gouavqrir.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.tarul.cn/Article/details/gkbdvsxnx.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fktsv.cn/Article/details/gzfoounbg.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/gpihbguin.sHtML

[G06] 重写方法
来源：http://www.m.share.fktsv.cn/Article/details/gfcbgpcjn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.bbcook.cn/Article/details/gjykiucab.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gbdyjouil.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/giejptdmh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gqxhuagig.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/ghukfatcq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.vehdjk.com/Article/details/gcnywashy.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fktsv.cn/Article/details/gxecfiqmv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.tarul.cn/Article/details/gtxprdyuv.sHtML

[G07] 调用父类方法
来源：http://read.share.sjlbkw.cn/Article/details/gxzinhvne.sHtML

Py:   super().greet()
来源：http://www.share.epnwcf.com/Article/details/gbuuiaocy.sHtML

PHP:  parent::greet();
来源：http://www.share.sjlbkw.cn/Article/details/gicdvoqga.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gxggpokcm.sHtML

TS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gvyepvgxi.sHtML

Java: super.greet();
来源：http://wap.yfazqb.com/Article/details/gpafjfqec.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.sjlbkw.cn/Article/details/gjgvqolxv.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gmqwefazk.sHtML

C#:   base.Greet();
来源：http://mobile.vehdjk.com/Article/details/ggkmevwkz.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/guusvdzhz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.vehdjk.com/Article/details/gexehhuyx.sHtML

PHP:  public static function f() {}
来源：http://read.share.epnwcf.com/Article/details/gsjgqgzga.sHtML

JS:   static f() {}
来源：http://read.share.epnwcf.com/Article/details/glwhtfesh.sHtML

TS:   static f(): void {}
来源：http://mobile.vehdjk.com/Article/details/gsyktqswr.sHtML

Java: static void f() {}
来源：http://baike.fktsv.cn/Article/details/gqdxgdczp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.bbcook.cn/Article/details/gbiglgfwt.sHtML

Ruby: def self.f; end
来源：http://baike.fktsv.cn/Article/details/gplxbqqmq.sHtML

C#:   public static void F() {}
来源：http://wap.bbcook.cn/Article/details/gmrjomoff.sHtML

[G09] 接口 / 抽象类
来源：http://wap.sjlbkw.cn/Article/details/grswizhkz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.vehdjk.com/Article/details/gwwyqibgh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/gjmdtsbxi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.vehdjk.com/Article/details/gbhedkaty.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdfnphbuu.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.bbcook.cn/Article/details/gyohedwlk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.sjlbkw.cn/Article/details/gdsixoupx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.bbcook.cn/Article/details/gcrqcwwep.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.bbcook.cn/Article/details/gsalemome.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/gjxwqecrt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.vehdjk.com/Article/details/gbhdzbsmt.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gywrrliey.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.yfazqb.com/Article/details/gpyfhbvsc.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/geiwcbqjh.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.vehdjk.com/Article/details/grhyvqkmw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gctjguhyr.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gxaaueqcf.sHtML

C#:   public / protected / private / internal
来源：http://www.share.tarul.cn/Article/details/gazwapvcp.sHtML

[G11] getter / setter
来源：http://read.share.yfazqb.com/Article/details/gyjllqigi.sHtML

Py:   @property 与 @x.setter
来源：http://baike.tarul.cn/Article/details/gxigqvidz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gyvlfljeq.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gmbsloiey.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gbnsstfzr.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/glmplsbei.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gkymfszcl.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/graxdgonh.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.sjlbkw.cn/Article/details/gtjvpjwqp.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/gcgwobxih.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/ghkdjrteo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gpnkbljsx.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gfjfymbzk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/ghcogewoe.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.yfazqb.com/Article/details/guchahgos.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gkbgrdgzs.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.tarul.cn/Article/details/gloggybuw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gvydffhbb.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/gmqkhidwj.sHtML

Py:   isinstance(u, User)
来源：http://3g.vehdjk.com/Article/details/gdbkgbffn.sHtML

PHP:  $u instanceof User
来源：http://mobile.tarul.cn/Article/details/gwgztzbor.sHtML

JS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/gahdsokdy.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gppltdpgi.sHtML

Java: u instanceof User
来源：http://blog.vehdjk.com/Article/details/gglvumpkk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.bbcook.cn/Article/details/ghtsengdv.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.tarul.cn/Article/details/gstjabsys.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/gounfaodh.sHtML

[G14] 数据类 / record
来源：http://m.share.tarul.cn/Article/details/goskxwpew.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.tarul.cn/Article/details/geewtyzok.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gaupoddvl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.bbcook.cn/Article/details/gjskoqvzl.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.bbcook.cn/Article/details/gsrwbzoae.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fktsv.cn/Article/details/gvkdjmddf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gtziscmpz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.bbcook.cn/Article/details/gssmtqvra.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqmxckme.sHtML

[G15] 枚举
来源：http://baike.yfazqb.com/Article/details/gzovluckp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/ggivkwtjy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fktsv.cn/Article/details/gsnlbhzbo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.yfazqb.com/Article/details/gkbdjjkqi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/gneeiihpa.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.vehdjk.com/Article/details/gxreysbqi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.tarul.cn/Article/details/gvrslnumi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fktsv.cn/Article/details/govrzubue.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gznjhevxd.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.epnwcf.com/Article/details/gqonkujca.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.epnwcf.com/Article/details/gkezyzxkh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.vehdjk.com/Article/details/gizosokzj.sHtML

JS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gpimdybwe.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/giluzbemg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.bbcook.cn/Article/details/gunzjsfgi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fktsv.cn/Article/details/grljadtyb.sHtML

Ruby: obj.instance_variables
来源：http://www.share.epnwcf.com/Article/details/gkttlpqqc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/gjjqknlxq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggomdduto.sHtML

H. 异常与错误处理
来源：http://blog.tarul.cn/Article/details/grfncpoxm.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtqiqgzwr.sHtML

[H01] try / catch 基础
来源：http://3g.epnwcf.com/Article/details/gtqhvjunq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gbbetikoc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/gjvfdowot.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gusfckrav.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gmhdsvgce.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.yfazqb.com/Article/details/gjerpawij.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.vehdjk.com/Article/details/gjpfiydsq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.vehdjk.com/Article/details/gezpxzbke.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.bbcook.cn/Article/details/gamiuhfkr.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fktsv.cn/Article/details/gmuhfvcvg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.sjlbkw.cn/Article/details/gdtnqdnty.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gbndbgyal.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gbreltxhc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gxvqkciqn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gvuduaowi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.vehdjk.com/Article/details/gyfukvabd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.yfazqb.com/Article/details/grovazqli.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gzpiogzyu.sHtML

[H03] 主动抛出异常
来源：http://wap.bbcook.cn/Article/details/gwfmvetmi.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fktsv.cn/Article/details/gudbtgtvl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gcjsgfgai.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/goefywdvn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gwamvywni.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gzspxpwgt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.yfazqb.com/Article/details/gypylsedr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.yfazqb.com/Article/details/gzaauvnqu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/ghwkmzfys.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/gjqhapmxr.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.epnwcf.com/Article/details/gfkruomqv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/gwognrdre.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gqafsfslr.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gffavzggw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gttjfjngu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.yfazqb.com/Article/details/gwpojeasl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fktsv.cn/Article/details/gxahszndm.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.sjlbkw.cn/Article/details/gvfjtubvt.sHtML

[H05] 捕获特定类型
来源：http://read.share.sjlbkw.cn/Article/details/gcpbynout.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/glcorqzpg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.vehdjk.com/Article/details/glwfrussh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gxdmhjpte.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/gxgvluqon.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/gzgygnkig.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.vehdjk.com/Article/details/gnngbrozr.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.vehdjk.com/Article/details/gwawtihyt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.sjlbkw.cn/Article/details/gcahbmxqc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.vehdjk.com/Article/details/gxvsbxxqf.sHtML

Py:   value = d.get("k") or default
来源：http://blog.yfazqb.com/Article/details/guywpkjkq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gqyaosqbp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gajncwizu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.yfazqb.com/Article/details/gulihxccb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.tarul.cn/Article/details/gqmgsxzcj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.bbcook.cn/Article/details/grmovgbjn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.bbcook.cn/Article/details/gvjcmfhhc.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/gosvlfuzx.sHtML

[H07] 断言
来源：http://m.share.fktsv.cn/Article/details/gadwbpooq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.bbcook.cn/Article/details/gxjakztdd.sHtML

PHP:  assert($x > 0);
来源：http://read.share.vehdjk.com/Article/details/ghpbokrls.sHtML

JS:   console.assert(x > 0);
来源：http://blog.sjlbkw.cn/Article/details/gdwujqvcb.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gvuhlfvsa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fktsv.cn/Article/details/gjfbwopic.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.tarul.cn/Article/details/gktqkfqlq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.bbcook.cn/Article/details/gnlmweihm.sHtML


<!-- 参考信息 -->