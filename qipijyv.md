代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.bbcook.cn/Article/details/glehszkbm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.epnwcf.com/Article/details/gyztaazfs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/ghbxivrwu.sHtML

[F04] 追加写入文件
来源：http://mobile.tarul.cn/Article/details/ghjvnpafy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.bbcook.cn/Article/details/gmxcolvlw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.sjlbkw.cn/Article/details/gtqakiidn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gustppdhu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/ggqidwpve.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fktsv.cn/Article/details/goxwzactz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.tarul.cn/Article/details/gtxtkdbcb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/grrmyqwhc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.yfazqb.com/Article/details/gcwrimfgz.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.tarul.cn/Article/details/gbobreerm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.epnwcf.com/Article/details/gvdvlrtvw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gnewwiaer.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gfelqcljm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gafiejghd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gjzvuegwq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/gswvrdcme.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.bbcook.cn/Article/details/guydwmroz.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gzmswwanx.sHtML

[F06] 删除文件
来源：http://baike.epnwcf.com/Article/details/gerinsbae.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/geujtbapl.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/gvguogekp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gxhxmeaij.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gwusornxp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/ggyebftnm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gczsgyzhc.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.tarul.cn/Article/details/gebsmojzx.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.epnwcf.com/Article/details/guwlmkohd.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.yfazqb.com/Article/details/gcgsrvmdz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gkpppvihx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.tarul.cn/Article/details/gjnoiifvl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/grlpqjxhv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gxnndlref.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.epnwcf.com/Article/details/gtrdeabyd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.epnwcf.com/Article/details/grzqxrmes.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.vehdjk.com/Article/details/ghvwignwk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.yfazqb.com/Article/details/gmgbsnzrb.sHtML

[F08] 遍历目录
来源：http://blog.sjlbkw.cn/Article/details/gbkbwmzok.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.epnwcf.com/Article/details/gkwkooygx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/grctwzqpj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gaibogzdj.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/gldrnlnoo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gtnybxulo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gswidtpoi.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gqwzdlgil.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fktsv.cn/Article/details/ghrvdrdom.sHtML

[F09] 获取文件大小
来源：http://3g.bbcook.cn/Article/details/gurmadyaz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/ghwkdnmds.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gplmqlqkv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gcjocyaxo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gadfjyffh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/grcpdkrlf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.vehdjk.com/Article/details/gpvailhna.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gmibrllzd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gjwpmkaag.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fktsv.cn/Article/details/gmwdyeqfe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gbzzkudya.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/ggxhtkpdm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gdxfnzrdi.sHtML

TS:   path.extname("a.txt")
来源：http://blog.bbcook.cn/Article/details/gjpjrityv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fktsv.cn/Article/details/gvwhipiiy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gsfkaryhs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gmzmysxpa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gxxqysncd.sHtML

[F11] 复制与移动文件
来源：http://blog.vehdjk.com/Article/details/gjlxgltas.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gctcxhbqh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.epnwcf.com/Article/details/gjjzdlsed.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gcorwopql.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gurmwnncn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.bbcook.cn/Article/details/gpzatwohn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.tarul.cn/Article/details/gxxfqxxsl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gjhaeaxef.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.bbcook.cn/Article/details/giyxdsijn.sHtML

[F12] CSV 读写
来源：http://www.m.share.bbcook.cn/Article/details/gprzyqdqw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gscflufxo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.tarul.cn/Article/details/grdbueefb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/gesclsqff.sHtML

TS:   // 同上
来源：http://3g.bbcook.cn/Article/details/gkrncgwta.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.epnwcf.com/Article/details/glkgrllxj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.tarul.cn/Article/details/gzkidzmlx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.bbcook.cn/Article/details/gglvjqhxm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.yfazqb.com/Article/details/gjngueqsr.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gysazjteq.sHtML

G. 面向对象
来源：http://mobile.bbcook.cn/Article/details/gnwmsyzag.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gszmiipqs.sHtML

[G01] 定义类
来源：http://www.share.epnwcf.com/Article/details/gqhiglefc.sHtML

Py:   class User: pass
来源：http://mobile.vehdjk.com/Article/details/gpjvlpbae.sHtML

PHP:  class User {}
来源：http://www.share.tarul.cn/Article/details/gxxylhcff.sHtML

JS:   class User {}
来源：http://m.share.epnwcf.com/Article/details/gtbjejngb.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.yfazqb.com/Article/details/gycnwtmgd.sHtML

Java: class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gnjcytooc.sHtML

Go:   type User struct { Name string }
来源：http://www.share.yfazqb.com/Article/details/gmqspokdm.sHtML

Ruby: class User; end
来源：http://read.share.yfazqb.com/Article/details/gdlcjxwun.sHtML

C#:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gkrpheqiy.sHtML

[G02] 构造函数
来源：http://blog.epnwcf.com/Article/details/gkalayjln.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/ghrgreodt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.yfazqb.com/Article/details/gwhyusrrs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gsnwvlxwk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/grebupalm.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/glpsdfsrn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gtkaeclkp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.epnwcf.com/Article/details/gwoyqdyqj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gfycytecn.sHtML

[G03] 实例属性
来源：http://m.share.bbcook.cn/Article/details/gyfetpglo.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gtkcbwcxc.sHtML

PHP:  public string $name = "x";
来源：http://mobile.vehdjk.com/Article/details/goinbihzj.sHtML

JS:   this.name = "x";
来源：http://m.share.tarul.cn/Article/details/gwxegaons.sHtML

TS:   name: string = "x";
来源：http://www.m.share.bbcook.cn/Article/details/geqmfihrs.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/gelrnjeox.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.tarul.cn/Article/details/gdurtjaxl.sHtML

Ruby: @name = "x"
来源：http://m.share.fktsv.cn/Article/details/geobwghat.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.bbcook.cn/Article/details/gzyaysrgc.sHtML

[G04] 定义方法
来源：http://wap.fktsv.cn/Article/details/grcrqveav.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gtyladcvk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/geewktoal.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gsycpkozn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gwvyuthik.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gupeyptbm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gzkftsehj.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/gveboymbr.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gzpartxgx.sHtML

[G05] 继承
来源：http://wap.tarul.cn/Article/details/gzvplaopv.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/ghgzlyest.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/ggcqzdxxt.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gfxewulij.sHtML

TS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/ghtytfdbf.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/grgugttpj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.yfazqb.com/Article/details/gmuldjvus.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fktsv.cn/Article/details/gxltbfioh.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/gibnftgxf.sHtML

[G06] 重写方法
来源：http://www.blog.fktsv.cn/Article/details/gvrgbyaoa.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.tarul.cn/Article/details/gtkcmxtzw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/ggwgesuxh.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gswejzjsj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gfcntshqk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gnjtfnkdz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.vehdjk.com/Article/details/gjvivjsrd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fktsv.cn/Article/details/gworvvsbj.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gxdlbhxea.sHtML

[G07] 调用父类方法
来源：http://read.share.vehdjk.com/Article/details/gawsglxji.sHtML

Py:   super().greet()
来源：http://mobile.yfazqb.com/Article/details/gqolhixyz.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/gpohrfuza.sHtML

JS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gwjakjcno.sHtML

TS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gebqwupky.sHtML

Java: super.greet();
来源：http://baike.tarul.cn/Article/details/gxrllcpgv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.epnwcf.com/Article/details/gdspxyeuz.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/godgqdjod.sHtML

C#:   base.Greet();
来源：http://m.share.tarul.cn/Article/details/gfntfqite.sHtML

[G08] 静态方法与属性
来源：http://wap.yfazqb.com/Article/details/gtjixampd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/gizkrjcbl.sHtML

PHP:  public static function f() {}
来源：http://m.share.yfazqb.com/Article/details/gwtbpmcjd.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/geilvtaem.sHtML

TS:   static f(): void {}
来源：http://m.share.vehdjk.com/Article/details/gnfoscorq.sHtML

Java: static void f() {}
来源：http://wap.bbcook.cn/Article/details/gcbeqsmlh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.bbcook.cn/Article/details/gpanxlnbq.sHtML

Ruby: def self.f; end
来源：http://read.share.tarul.cn/Article/details/gtiwkngyb.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/giyxkrkwq.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/grjyjirkk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.sjlbkw.cn/Article/details/gdkyermvs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.tarul.cn/Article/details/gghozqjwz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.tarul.cn/Article/details/gjfijdtpn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.epnwcf.com/Article/details/gjkgdggep.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.tarul.cn/Article/details/ggpmlitdt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gbkmvhphg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.tarul.cn/Article/details/gxdlesahy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.yfazqb.com/Article/details/gewpgneqv.sHtML

[G10] 访问控制
来源：http://mobile.vehdjk.com/Article/details/gwcuvvwvh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.bbcook.cn/Article/details/gzpqbixay.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gngvjwkac.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.vehdjk.com/Article/details/gfnsyilgk.sHtML

TS:   public / protected / private
来源：http://3g.epnwcf.com/Article/details/gworfobnh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.sjlbkw.cn/Article/details/gqvpgaxte.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.yfazqb.com/Article/details/gemswqkoy.sHtML

Ruby: public / protected / private
来源：http://wap.yfazqb.com/Article/details/gctgmtykx.sHtML

C#:   public / protected / private / internal
来源：http://baike.fktsv.cn/Article/details/getbqqlrs.sHtML

[G11] getter / setter
来源：http://read.share.epnwcf.com/Article/details/gnrchagnk.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.yfazqb.com/Article/details/gphvveipj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/ggwxspumj.sHtML

JS:   get name() { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gvwdpigus.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gmkanmndx.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gepscrani.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/grhksvyku.sHtML

Ruby: attr_accessor :name
来源：http://mobile.epnwcf.com/Article/details/gbjtifyhv.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/gqiixyqht.sHtML

[G12] 对象转字符串
来源：http://mobile.vehdjk.com/Article/details/gvrcttqgk.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gxlcwkkqu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gokdsocee.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gvmvhppmw.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gxtkvhtrc.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.epnwcf.com/Article/details/ggchseuws.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gjnkyjlmg.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.vehdjk.com/Article/details/gdxynmrih.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.vehdjk.com/Article/details/giyagyfby.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/ghxxvmcqd.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.tarul.cn/Article/details/giycyiylu.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gcxeolfxi.sHtML

JS:   u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gvfiyyshw.sHtML

TS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gobidcfwy.sHtML

Java: u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyzewumy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.tarul.cn/Article/details/gwyebbupg.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/gmgjygkgg.sHtML

C#:   u is User
来源：http://www.m.share.bbcook.cn/Article/details/gzrezlkwl.sHtML

[G14] 数据类 / record
来源：http://www.share.epnwcf.com/Article/details/ggtgzqdvc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.bbcook.cn/Article/details/gaoxyctzt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.sjlbkw.cn/Article/details/gkvzapwms.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.vehdjk.com/Article/details/gdseuzckc.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.tarul.cn/Article/details/gskwmdzno.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fktsv.cn/Article/details/gkivxwwcq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.vehdjk.com/Article/details/gfrzfsaql.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.bbcook.cn/Article/details/ghqwrglaa.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/glpsrabxh.sHtML

[G15] 枚举
来源：http://m.share.epnwcf.com/Article/details/gvvpwhkzy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.bbcook.cn/Article/details/gpzfthtxy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/gsjybjyyh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.yfazqb.com/Article/details/gjuwiqqtp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/gmvxlesbw.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.yfazqb.com/Article/details/gqwxcmqwf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.sjlbkw.cn/Article/details/grlvneccu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.vehdjk.com/Article/details/giqorpnea.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gzbtbyban.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.epnwcf.com/Article/details/gityeyrsf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.epnwcf.com/Article/details/gxysbyblq.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.yfazqb.com/Article/details/gscknwmas.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gldobypvy.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gfwfscvur.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.sjlbkw.cn/Article/details/gltbjegfl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/giiclmjcs.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.yfazqb.com/Article/details/ghisfcbwr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gshehuvqk.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gujuhilrv.sHtML

H. 异常与错误处理
来源：http://read.share.bbcook.cn/Article/details/gbfovttzk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/glvyongcy.sHtML

[H01] try / catch 基础
来源：http://blog.fktsv.cn/Article/details/gcwaqhrcj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fktsv.cn/Article/details/gihgywwni.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.sjlbkw.cn/Article/details/gvthkzxei.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwngarsma.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/ghxfhqjic.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.tarul.cn/Article/details/gjnoxgdog.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.tarul.cn/Article/details/gmjizhvlw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/gfehpaina.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/goxawqpdv.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.bbcook.cn/Article/details/gjavwqvnt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.epnwcf.com/Article/details/gezslbjsg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/ghvmkjuqs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gtdktqcaf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gkrhligqs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gjehdjrnf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.epnwcf.com/Article/details/glqguzkvf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.epnwcf.com/Article/details/gfbawiwaw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/grknwxnps.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/gnnvypejt.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.sjlbkw.cn/Article/details/geafdnttz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gugpyjdzj.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gzssilewo.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gbtfyuayp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gegczmzvx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/gmmegchpn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.tarul.cn/Article/details/gvrkjixom.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gajlntaou.sHtML

[H04] 自定义异常类型
来源：http://blog.yfazqb.com/Article/details/gdgtfezow.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.tarul.cn/Article/details/gzgfxyudl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gxlfiscdb.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/ghuitgjuy.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/gcpznwmgv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/gopggbdwk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/gcomivzgr.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.epnwcf.com/Article/details/guhdpdhaj.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fktsv.cn/Article/details/gpbhcdsfy.sHtML

[H05] 捕获特定类型
来源：http://wap.vehdjk.com/Article/details/gljkphgaa.sHtML

Py:   except ValueError as e:
来源：http://www.blog.yfazqb.com/Article/details/gmdxrlltr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.bbcook.cn/Article/details/gwrljbvtc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gseokayfu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gombuxgti.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.epnwcf.com/Article/details/gmohbcbcf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.bbcook.cn/Article/details/gdmosrfwo.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.bbcook.cn/Article/details/gtulmppun.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gqwvvlmqr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fktsv.cn/Article/details/gwbxxyjkx.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.sjlbkw.cn/Article/details/gfwhfhrti.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.epnwcf.com/Article/details/ghkoarmyj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gjhzhfnae.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gdwijtalm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.bbcook.cn/Article/details/ggkmzhgzg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.sjlbkw.cn/Article/details/gduqlzhxn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.bbcook.cn/Article/details/gqvdgjpfi.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/gzemqqtcc.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gkfegfliz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.tarul.cn/Article/details/gzpstfias.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gchaivkwm.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gqcmhjtse.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/ggjixrnru.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fktsv.cn/Article/details/gcchzpihz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.vehdjk.com/Article/details/ggloiwnrj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.epnwcf.com/Article/details/gfgaybaow.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gdwxpqjyh.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.yfazqb.com/Article/details/gmogqnbst.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.sjlbkw.cn/Article/details/gulwrbufu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fktsv.cn/Article/details/gyutrtqzp.sHtML


<!-- 参考信息 -->