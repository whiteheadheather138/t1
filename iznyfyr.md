代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/gopykctqq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gsxkvxiyb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/ghhjmqxcz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/grxwrfjrt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fktsv.cn/Article/details/gejztoxjd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fktsv.cn/Article/details/gyajjaeqo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gsztotipo.sHtML

[F04] 追加写入文件
来源：http://www.blog.epnwcf.com/Article/details/gaxhpthrr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.tarul.cn/Article/details/gfwjnfmyr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/ghsgmszvm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gqsjqpquz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gynwnwbzk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/gxlhblwdp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gbtgqovcx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.tarul.cn/Article/details/gqrbkpmva.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.vehdjk.com/Article/details/gcqyhanre.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/gqmenlqej.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.vehdjk.com/Article/details/gyqrvzpoq.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gvnfukuwt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gswtljjtj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gruqbmvsr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gbqqstxid.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.vehdjk.com/Article/details/gbqwbddlf.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gpypvumgd.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.yfazqb.com/Article/details/grjhpherl.sHtML

[F06] 删除文件
来源：http://mobile.bbcook.cn/Article/details/gdiqqhgim.sHtML

Py:   os.remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/guyclxgbz.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/goistkxjm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/glpeootlp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gqbhrmltb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gmsjyxawi.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gxfhmmgzy.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.yfazqb.com/Article/details/gibfaccgv.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/gryanhpjd.sHtML

[F07] 创建目录（含多级）
来源：http://blog.vehdjk.com/Article/details/gpdebonqc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gmdncoerh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.yfazqb.com/Article/details/glwpygugz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gixcwxsln.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gberzoucp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.bbcook.cn/Article/details/giwuyjmdt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.bbcook.cn/Article/details/gqvamdtqg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.bbcook.cn/Article/details/guscusmwl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/gqodkkzad.sHtML

[F08] 遍历目录
来源：http://baike.fktsv.cn/Article/details/gwyolsmgo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/gzqyyfryv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.epnwcf.com/Article/details/gpmftbdxf.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/grfnpcwby.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gbxkbpprr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gakqanvmu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.epnwcf.com/Article/details/grtjcsplo.sHtML

Ruby: Dir.children("dir")
来源：http://wap.sjlbkw.cn/Article/details/gaktxbfkv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.tarul.cn/Article/details/gapalzbcx.sHtML

[F09] 获取文件大小
来源：http://www.blog.epnwcf.com/Article/details/gdkxkvksv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gurwdlqtx.sHtML

PHP:  filesize("a.txt");
来源：http://blog.yfazqb.com/Article/details/gspwduxvh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gfldkudzq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gyhfmvsnv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gswfiyogt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.epnwcf.com/Article/details/gfxysskch.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gheeqsfgj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.bbcook.cn/Article/details/gbrzrwgfv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.sjlbkw.cn/Article/details/glvondunx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gzhecjxov.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gdltgmebw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/guyryalxq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gqebcpzql.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fktsv.cn/Article/details/gvwnmcpot.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gietysxlt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gaxzmjvrg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gsllzopkv.sHtML

[F11] 复制与移动文件
来源：http://baike.tarul.cn/Article/details/gmgjqvozw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gpfinecpg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.sjlbkw.cn/Article/details/gokfoubnl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gfhyipgdh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gviybscsd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.yfazqb.com/Article/details/gwzdejnxt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.epnwcf.com/Article/details/gcrvnvjvd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/guepgpxai.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.epnwcf.com/Article/details/gqwbgquhd.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/gjlfkhfvb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.tarul.cn/Article/details/guaoucdzt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.yfazqb.com/Article/details/gbpkfbdah.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.bbcook.cn/Article/details/gawsmejze.sHtML

TS:   // 同上
来源：http://blog.epnwcf.com/Article/details/gcokydmom.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.epnwcf.com/Article/details/grccxqzmx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.bbcook.cn/Article/details/givqhhzmw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.vehdjk.com/Article/details/gyrmcidds.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.tarul.cn/Article/details/gjawfinmp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gyqbsyoov.sHtML

G. 面向对象
来源：http://wap.epnwcf.com/Article/details/gykjdiatd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gybzyjhtq.sHtML

[G01] 定义类
来源：http://www.share.epnwcf.com/Article/details/gmckanchw.sHtML

Py:   class User: pass
来源：http://wap.tarul.cn/Article/details/gzuarikbw.sHtML

PHP:  class User {}
来源：http://wap.vehdjk.com/Article/details/ghizqclck.sHtML

JS:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/ggkqqnxkf.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/galpzpplp.sHtML

Java: class User {}
来源：http://3g.sjlbkw.cn/Article/details/gqfbsqajm.sHtML

Go:   type User struct { Name string }
来源：http://read.share.yfazqb.com/Article/details/glaygnrod.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/gnfftzwqu.sHtML

C#:   class User {}
来源：http://blog.epnwcf.com/Article/details/gujigmoog.sHtML

[G02] 构造函数
来源：http://wap.sjlbkw.cn/Article/details/gudyhkslb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.vehdjk.com/Article/details/gmhnqeciw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fktsv.cn/Article/details/gjobblnen.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gpycpzdko.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.sjlbkw.cn/Article/details/gtcxjwbbk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gjwubpuhf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.vehdjk.com/Article/details/gyqehlufs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.vehdjk.com/Article/details/gqtgnvxlt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gobawhanr.sHtML

[G03] 实例属性
来源：http://wap.vehdjk.com/Article/details/glvxocfsc.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/ggwoazyci.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gppgdmpvn.sHtML

JS:   this.name = "x";
来源：http://www.blog.epnwcf.com/Article/details/gjvnkfjnf.sHtML

TS:   name: string = "x";
来源：http://baike.fktsv.cn/Article/details/gltlxyjtb.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/gniairiuc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.epnwcf.com/Article/details/gixmbjtef.sHtML

Ruby: @name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/gykjvoiel.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/guztyyehw.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/gugdowjlu.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/gbvnharsh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gwcaldxhd.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gdszbjusf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gbupiiqud.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gljcyuuzk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gtbehojer.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/ghccgcxqw.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/glvrtgupk.sHtML

[G05] 继承
来源：http://mobile.epnwcf.com/Article/details/gymfahhnw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/gztbgibat.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/glphtxmqs.sHtML

JS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/ggdqrtvdz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gstzyvhoe.sHtML

Java: class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gggkqdcfn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.tarul.cn/Article/details/giqtqctix.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/gtlrbxfko.sHtML

C#:   class Admin : User {}
来源：http://read.share.vehdjk.com/Article/details/gpisfnifo.sHtML

[G06] 重写方法
来源：http://www.m.share.tarul.cn/Article/details/gwevzcrmo.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.vehdjk.com/Article/details/gcjrjemvh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gqydhzapy.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gtqjadcjq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gtnpzfcbq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gcrxjygrx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.sjlbkw.cn/Article/details/ghwrruavt.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.vehdjk.com/Article/details/gefxowolc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.tarul.cn/Article/details/gxiybplqo.sHtML

[G07] 调用父类方法
来源：http://www.share.fktsv.cn/Article/details/gqbskchyj.sHtML

Py:   super().greet()
来源：http://www.share.bbcook.cn/Article/details/gergdxhoj.sHtML

PHP:  parent::greet();
来源：http://wap.vehdjk.com/Article/details/gfbatwrdw.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gemyonqqz.sHtML

TS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gqlqnwqhq.sHtML

Java: super.greet();
来源：http://read.share.vehdjk.com/Article/details/ggoidkyqu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.tarul.cn/Article/details/gjxgccnqy.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gainxxemo.sHtML

C#:   base.Greet();
来源：http://www.blog.vehdjk.com/Article/details/gubzldxjk.sHtML

[G08] 静态方法与属性
来源：http://blog.fktsv.cn/Article/details/gastrjafh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.sjlbkw.cn/Article/details/gstjhkbqo.sHtML

PHP:  public static function f() {}
来源：http://mobile.yfazqb.com/Article/details/gbirkplay.sHtML

JS:   static f() {}
来源：http://read.share.vehdjk.com/Article/details/gtupchtur.sHtML

TS:   static f(): void {}
来源：http://blog.vehdjk.com/Article/details/gfumuphnz.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/gtrgkxsdm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.tarul.cn/Article/details/gxteadcbo.sHtML

Ruby: def self.f; end
来源：http://read.share.epnwcf.com/Article/details/gfdoyrsko.sHtML

C#:   public static void F() {}
来源：http://www.blog.bbcook.cn/Article/details/gyoxxbfml.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.bbcook.cn/Article/details/gxxtetrfk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/gxnwiutyr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.yfazqb.com/Article/details/gjjfzmvwf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.tarul.cn/Article/details/gvvlrlzhf.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.epnwcf.com/Article/details/gdaeqsvcu.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.vehdjk.com/Article/details/gmnddytpp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.sjlbkw.cn/Article/details/gotdqzyfh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/geuyfaxkw.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.yfazqb.com/Article/details/gkwjjcuyy.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/gdpgckreo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.bbcook.cn/Article/details/gpebqjrom.sHtML

PHP:  public / protected / private
来源：http://read.share.fktsv.cn/Article/details/ggsarsunq.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.bbcook.cn/Article/details/gvsodotgf.sHtML

TS:   public / protected / private
来源：http://wap.epnwcf.com/Article/details/gbkgdntje.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.bbcook.cn/Article/details/gzatdexdp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/ghqxhudgp.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gdupxcgfr.sHtML

C#:   public / protected / private / internal
来源：http://wap.vehdjk.com/Article/details/giqokfqfg.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gatvxhfgl.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fktsv.cn/Article/details/gsxqpojcp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/gdrlnqdln.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gkomcsbyj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gkvjcplhf.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gielcqlin.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gcackqzsm.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/ggzgrepag.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.bbcook.cn/Article/details/gquasjgsk.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/grdkwossa.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gdlhateac.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/ggbiskgta.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gvjkbwiei.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gyeszfoey.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.tarul.cn/Article/details/gghceoqqu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/ggaqzfusl.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.bbcook.cn/Article/details/gidmlphpz.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.vehdjk.com/Article/details/gunquntoh.sHtML

[G13] 判断对象类型
来源：http://mobile.tarul.cn/Article/details/ghcipdvca.sHtML

Py:   isinstance(u, User)
来源：http://blog.fktsv.cn/Article/details/gcjdcrtlh.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gjyaubeeu.sHtML

JS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gkkwbnvrl.sHtML

TS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gygdfbgxg.sHtML

Java: u instanceof User
来源：http://3g.yfazqb.com/Article/details/gjcocfhyx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/gfzpwsepz.sHtML

Ruby: u.is_a?(User)
来源：http://3g.tarul.cn/Article/details/gyldwcqds.sHtML

C#:   u is User
来源：http://m.share.fktsv.cn/Article/details/gxgdzccwi.sHtML

[G14] 数据类 / record
来源：http://www.share.tarul.cn/Article/details/gmfrvozyg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.sjlbkw.cn/Article/details/gmrhwpbfi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.vehdjk.com/Article/details/ghdzhsxwa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.yfazqb.com/Article/details/gphzoatne.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fktsv.cn/Article/details/gwscrcfbw.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvapbmdlq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gbbqkfjxr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.bbcook.cn/Article/details/gzrsjogbk.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.tarul.cn/Article/details/giwxpcjwr.sHtML

[G15] 枚举
来源：http://www.blog.tarul.cn/Article/details/gqovoahjl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/grfwyoqxn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.epnwcf.com/Article/details/gcsgelzwi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.epnwcf.com/Article/details/gcffcopgc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/gnmmibzsj.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gmhnmnxjq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.bbcook.cn/Article/details/gejcthuxq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.yfazqb.com/Article/details/ghpuuwibl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gpwsgsdol.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/gsjshnazm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.tarul.cn/Article/details/gsfzephkx.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fktsv.cn/Article/details/ghfumhdyt.sHtML

JS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/grxohfhbr.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gihmxywei.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/glhnpefmk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/ginvuwncu.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.yfazqb.com/Article/details/gzozichvz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gvgsnwioa.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmbfmuwya.sHtML

H. 异常与错误处理
来源：http://m.share.fktsv.cn/Article/details/gzjitftnm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gziczwjmy.sHtML

[H01] try / catch 基础
来源：http://wap.fktsv.cn/Article/details/gjyvjxzrs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/gqabjraqg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.vehdjk.com/Article/details/getdopbsj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gfgbgqdmg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gkljtvslu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.yfazqb.com/Article/details/gehzutnoi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fktsv.cn/Article/details/grabntmkx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.sjlbkw.cn/Article/details/gpkyiwwmb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/gagwniorr.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fktsv.cn/Article/details/gunvdpgfa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.epnwcf.com/Article/details/gyrhjqguo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gavbswaoj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gwcxijrmj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/ghabgxijt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/goaswskng.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.epnwcf.com/Article/details/gqzdrekou.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fktsv.cn/Article/details/gjdywejdh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gsixxyymx.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/gduueuzvh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.yfazqb.com/Article/details/gzsmlkqlk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gzmsgpuvl.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/gtachljij.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/gltrsxdkx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gvgymuvut.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/gyqtnngdj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.sjlbkw.cn/Article/details/gehropyfy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/guzqonosv.sHtML

[H04] 自定义异常类型
来源：http://www.share.tarul.cn/Article/details/gigttziye.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.sjlbkw.cn/Article/details/gifnfrlsl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/ghcuevzyd.sHtML

JS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/ggeioghzc.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.bbcook.cn/Article/details/gldtbhwrx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/gioddlsza.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.sjlbkw.cn/Article/details/godpymxki.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gjwgysomg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.vehdjk.com/Article/details/gsbhdraxd.sHtML

[H05] 捕获特定类型
来源：http://3g.sjlbkw.cn/Article/details/gfrxiiuxu.sHtML

Py:   except ValueError as e:
来源：http://www.blog.sjlbkw.cn/Article/details/gpkydmhcl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.vehdjk.com/Article/details/glhldlsmd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gipylrmaf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.vehdjk.com/Article/details/glczzgqgw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fktsv.cn/Article/details/gpkoqgvig.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.sjlbkw.cn/Article/details/gbzbmfizy.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.sjlbkw.cn/Article/details/geejbkvdu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/gyiaikunf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.sjlbkw.cn/Article/details/gmbdlsqtt.sHtML

Py:   value = d.get("k") or default
来源：http://wap.tarul.cn/Article/details/gbvnjfpbb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gyojahpin.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.tarul.cn/Article/details/gfoczpbkp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.bbcook.cn/Article/details/gomrflmcf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.tarul.cn/Article/details/gqnuxacnk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/gxyysfrbv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.vehdjk.com/Article/details/gocdltjst.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gwgexxujj.sHtML

[H07] 断言
来源：http://blog.fktsv.cn/Article/details/gabpeqgkn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.epnwcf.com/Article/details/gdocgfnrw.sHtML

PHP:  assert($x > 0);
来源：http://www.share.epnwcf.com/Article/details/goegtjhbr.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/grxyrhzdf.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.yfazqb.com/Article/details/guitvxzmy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fktsv.cn/Article/details/ghfcwskqu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.bbcook.cn/Article/details/gdpbkknoa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.yfazqb.com/Article/details/gjnxykkvz.sHtML


<!-- 参考信息 -->