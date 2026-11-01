代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/gpjvkoynf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/gurlvbfnd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gfnorwyjc.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gaupnnewk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/gquedxmsz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.vehdjk.com/Article/details/gskurppin.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/glkysukql.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/ghktuvkcp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.epnwcf.com/Article/details/gxpdcpyad.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.vehdjk.com/Article/details/gnpsqcmun.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/gmbhhhhmf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fktsv.cn/Article/details/gjlkaysek.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.yfazqb.com/Article/details/gutnsptpt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fktsv.cn/Article/details/geuqbyhuo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gakdhjzmi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gioxvkzft.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gqbvyntde.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gbzzrkevt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.epnwcf.com/Article/details/gbopycpeo.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gqueuuhtl.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gzjeifxql.sHtML

[F06] 删除文件
来源：http://mobile.bbcook.cn/Article/details/gnzqkrlnz.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gpirgmflz.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.yfazqb.com/Article/details/goadahotf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/guvyuytgd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/guwnxgqjp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gkzwtfore.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gcbmihepi.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjjaryxx.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gmnupkdnk.sHtML

[F07] 创建目录（含多级）
来源：http://blog.tarul.cn/Article/details/gfibgkmag.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gmvjwekog.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.bbcook.cn/Article/details/gvhdqoxsv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gsznslvve.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/gcsfqmvkj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.epnwcf.com/Article/details/gbumxqtkn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.yfazqb.com/Article/details/gjcvzgtrc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fktsv.cn/Article/details/geemhdsnq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.sjlbkw.cn/Article/details/gzfgutcxu.sHtML

[F08] 遍历目录
来源：http://blog.epnwcf.com/Article/details/gxdlhzlfx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.sjlbkw.cn/Article/details/gxceurtsv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/gpiqwwatm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gwkfqvobl.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gfrniidao.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/gbadtjfff.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gyfrxadbd.sHtML

Ruby: Dir.children("dir")
来源：http://3g.bbcook.cn/Article/details/gqxplblxy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.sjlbkw.cn/Article/details/gpzpommge.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/glflpivfb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gidjiadgf.sHtML

PHP:  filesize("a.txt");
来源：http://wap.vehdjk.com/Article/details/gxhnryeee.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gzjifcwoq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.tarul.cn/Article/details/geersgtqw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gdhnzhkvd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.vehdjk.com/Article/details/gjnecpxux.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/geqgrplfr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.epnwcf.com/Article/details/gsalbzvzc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/gqyaajxiv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gfpguzbtv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fktsv.cn/Article/details/gnapggswb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/ggthlchnk.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gryopyuzu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gquzxroyv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gsqillsor.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gkbljnury.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjveuczxe.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gjbxjfhum.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gwxbkjziw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtgaymms.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gknbrbyku.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gdaprxcou.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.tarul.cn/Article/details/gltosmoed.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/gzivlyxxr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/golavwobp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.tarul.cn/Article/details/gsrpfkydx.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/gqirsfvoo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fktsv.cn/Article/details/gtqtfjjas.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/gguxyjmye.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.sjlbkw.cn/Article/details/gmsczwver.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gxvuglmkk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.yfazqb.com/Article/details/gvoirtzkd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gfcnpburt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.tarul.cn/Article/details/gkrszidda.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.epnwcf.com/Article/details/gvqbssecn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glfdhopgw.sHtML

G. 面向对象
来源：http://www.blog.yfazqb.com/Article/details/gbaiwtgrt.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjbqrddoc.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/gaetqfmgd.sHtML

Py:   class User: pass
来源：http://www.m.share.vehdjk.com/Article/details/gghsfvcpf.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/gucrxkqsr.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gphyanryt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/glawuachx.sHtML

Java: class User {}
来源：http://wap.yfazqb.com/Article/details/gynppksqy.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.vehdjk.com/Article/details/gbakoobfm.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gxnhqlvmb.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gvdhwanbd.sHtML

[G02] 构造函数
来源：http://blog.fktsv.cn/Article/details/gfoqtgfvr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.epnwcf.com/Article/details/ggtwnupmo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.sjlbkw.cn/Article/details/gmqjwliam.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gvncmbxcy.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.tarul.cn/Article/details/gxsqfcbzr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/guruvmdlo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.yfazqb.com/Article/details/giexrkmvx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.bbcook.cn/Article/details/ggpuwkqki.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gefrhqwyr.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/gayaeuyfn.sHtML

Py:   self.name = "x"
来源：http://www.blog.bbcook.cn/Article/details/grkfzunfn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gyxofigld.sHtML

JS:   this.name = "x";
来源：http://www.share.fktsv.cn/Article/details/gcoabxgnz.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/gldgdanxo.sHtML

Java: private String name;
来源：http://www.share.sjlbkw.cn/Article/details/gkljokvvp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gjasxiamc.sHtML

Ruby: @name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/gdqiwbrxz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.tarul.cn/Article/details/gofiybioi.sHtML

[G04] 定义方法
来源：http://www.share.epnwcf.com/Article/details/gkkmqqzfh.sHtML

Py:   def greet(self): return self.name
来源：http://3g.vehdjk.com/Article/details/gpuvxrfjk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gfkfnjqbb.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gvmdhjfva.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gazttzska.sHtML

Java: String greet() { return name; }
来源：http://baike.yfazqb.com/Article/details/goalvcejl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gpcvoqsal.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/ghrkllsef.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fktsv.cn/Article/details/gcinvazcr.sHtML

[G05] 继承
来源：http://mobile.yfazqb.com/Article/details/gbbrecaom.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/gvpdmjqsw.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gwzaoqgto.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/ggpkrgasa.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gncjylhtg.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gzaphphbn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.bbcook.cn/Article/details/gxlaikeyu.sHtML

Ruby: class Admin < User; end
来源：http://3g.vehdjk.com/Article/details/ghwddxiia.sHtML

C#:   class Admin : User {}
来源：http://www.share.vehdjk.com/Article/details/gbdeuzoob.sHtML

[G06] 重写方法
来源：http://3g.epnwcf.com/Article/details/gidkcxtge.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.sjlbkw.cn/Article/details/gqmrikeom.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gtnjinebh.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gklcviptp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gevuyahha.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gxebfktub.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.vehdjk.com/Article/details/gddanhpfy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/gcyhjgpmh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.sjlbkw.cn/Article/details/govcptwxz.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/gyssurulf.sHtML

Py:   super().greet()
来源：http://www.blog.sjlbkw.cn/Article/details/gwvawnjvq.sHtML

PHP:  parent::greet();
来源：http://www.blog.fktsv.cn/Article/details/gtzkxofrr.sHtML

JS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gukutojnu.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gukbeslag.sHtML

Java: super.greet();
来源：http://wap.epnwcf.com/Article/details/gtsdmzwue.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.tarul.cn/Article/details/gnsjjhibt.sHtML

Ruby: super
来源：http://mobile.yfazqb.com/Article/details/gwwusgxut.sHtML

C#:   base.Greet();
来源：http://read.share.vehdjk.com/Article/details/gotsnjegp.sHtML

[G08] 静态方法与属性
来源：http://www.share.yfazqb.com/Article/details/gyjnrjltp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.vehdjk.com/Article/details/gncevtpyd.sHtML

PHP:  public static function f() {}
来源：http://www.blog.bbcook.cn/Article/details/gwwawahlb.sHtML

JS:   static f() {}
来源：http://wap.fktsv.cn/Article/details/grujgvxkr.sHtML

TS:   static f(): void {}
来源：http://m.share.vehdjk.com/Article/details/gwynzodfs.sHtML

Java: static void f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gcfolxbcx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.vehdjk.com/Article/details/gvuyaagpa.sHtML

Ruby: def self.f; end
来源：http://mobile.bbcook.cn/Article/details/gisldsnrq.sHtML

C#:   public static void F() {}
来源：http://read.share.tarul.cn/Article/details/gwrcqxwmc.sHtML

[G09] 接口 / 抽象类
来源：http://blog.yfazqb.com/Article/details/gpnxaxhew.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.sjlbkw.cn/Article/details/gbfmgzqkq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fktsv.cn/Article/details/gxubppyhx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.vehdjk.com/Article/details/gisrfjpri.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gqiagljwh.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gddlohtpk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.vehdjk.com/Article/details/ghmiatykv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.epnwcf.com/Article/details/gvpesenuh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gylgcaaee.sHtML

[G10] 访问控制
来源：http://baike.tarul.cn/Article/details/gwydpsxfh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.yfazqb.com/Article/details/gqqyhglvn.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gjtrcncoh.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fktsv.cn/Article/details/gnkgentnk.sHtML

TS:   public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gttngivbx.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.vehdjk.com/Article/details/gyofxqtov.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gjdqdhfsb.sHtML

Ruby: public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gabuqjlbg.sHtML

C#:   public / protected / private / internal
来源：http://m.share.vehdjk.com/Article/details/gzwubaehm.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/ghofhftgi.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.tarul.cn/Article/details/gkrxhtyyv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gfnavwwdk.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/gbxworpvu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gwzeswsut.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gmabcfhuu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/glbppixil.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.epnwcf.com/Article/details/gdncrjzoe.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.vehdjk.com/Article/details/gwfxmbtcu.sHtML

[G12] 对象转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gyghjoett.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gmdeayvqg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gmpaezoul.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gjohftpon.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gysgixyex.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.tarul.cn/Article/details/gbdbgswii.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gimmcpxhw.sHtML

Ruby: def to_s; @name; end
来源：http://blog.yfazqb.com/Article/details/gzmdzocdo.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/gypdelaob.sHtML

[G13] 判断对象类型
来源：http://wap.yfazqb.com/Article/details/gspdodxco.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fktsv.cn/Article/details/ghuyabgix.sHtML

PHP:  $u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gqwsanjje.sHtML

JS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gkqxvnbzg.sHtML

TS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gpwosmnao.sHtML

Java: u instanceof User
来源：http://blog.vehdjk.com/Article/details/ggrzfzrdw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/gwndtffhi.sHtML

Ruby: u.is_a?(User)
来源：http://wap.epnwcf.com/Article/details/gobnuhfgi.sHtML

C#:   u is User
来源：http://wap.tarul.cn/Article/details/grewciabr.sHtML

[G14] 数据类 / record
来源：http://baike.vehdjk.com/Article/details/gjehfutze.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.vehdjk.com/Article/details/ghyytuvnz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.epnwcf.com/Article/details/gpuomdsqg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/gwgtwadze.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.sjlbkw.cn/Article/details/gyrhbwxti.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.yfazqb.com/Article/details/gjkjiizih.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.tarul.cn/Article/details/grioxbqej.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.yfazqb.com/Article/details/gzqofthih.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.epnwcf.com/Article/details/gbmjrinit.sHtML

[G15] 枚举
来源：http://www.m.share.bbcook.cn/Article/details/gvzvbvjyc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.tarul.cn/Article/details/giborbyzr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.tarul.cn/Article/details/gudzulhhc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.sjlbkw.cn/Article/details/gtncwwpaj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gbiidadve.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.tarul.cn/Article/details/gwmwvecrr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.yfazqb.com/Article/details/gjbasekxf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.sjlbkw.cn/Article/details/gecbqdbfd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gcawscafl.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/gxrswbzav.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.sjlbkw.cn/Article/details/grdmmhlqp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fktsv.cn/Article/details/gjyqtjdvl.sHtML

JS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gjkrbazuq.sHtML

TS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gerejhjaf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.vehdjk.com/Article/details/gduizqiml.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.epnwcf.com/Article/details/ggebnosef.sHtML

Ruby: obj.instance_variables
来源：http://www.share.vehdjk.com/Article/details/gljujbahq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/gamnhpxei.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gldteiowk.sHtML

H. 异常与错误处理
来源：http://baike.bbcook.cn/Article/details/gqycfomfp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwxooovtm.sHtML

[H01] try / catch 基础
来源：http://www.share.epnwcf.com/Article/details/ggdolmbdw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/gmhpeycdj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/grauyspem.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gwiixwwzc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gyqqzaxkb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.yfazqb.com/Article/details/gsmtfzvwx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.sjlbkw.cn/Article/details/giuksrqkx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.bbcook.cn/Article/details/gsjikeapg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.epnwcf.com/Article/details/gqnhwoija.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fktsv.cn/Article/details/gjsabrirb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.epnwcf.com/Article/details/giikvwmcs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gatudfwgj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gwjrxetod.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gufvrhkpa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gzavbxkxj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.sjlbkw.cn/Article/details/gskmxghcz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.tarul.cn/Article/details/gmobhkhxm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.tarul.cn/Article/details/geqmxqfwd.sHtML

[H03] 主动抛出异常
来源：http://www.blog.epnwcf.com/Article/details/giuzvtebz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.vehdjk.com/Article/details/gnivzkcqs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gsbvdvwuu.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gkrhunyml.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/giwgfvath.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gnhfekorr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.yfazqb.com/Article/details/gzbwcwepv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.sjlbkw.cn/Article/details/givzcwscd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gbliwtvcl.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/ghohpgyzz.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.vehdjk.com/Article/details/gilwbmgdw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/gtetsidaj.sHtML

JS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/guvnwexkv.sHtML

TS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gjthgqsli.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fktsv.cn/Article/details/gryzsgfrz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.vehdjk.com/Article/details/gohioglbr.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fktsv.cn/Article/details/gerlsksxq.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.sjlbkw.cn/Article/details/gnkscmfjf.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.bbcook.cn/Article/details/gjuklpbiw.sHtML

Py:   except ValueError as e:
来源：http://read.share.tarul.cn/Article/details/gslmopegf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.yfazqb.com/Article/details/gnfumhzlm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/guvwqlhil.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gemrfxclm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.epnwcf.com/Article/details/gswmsktzj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fktsv.cn/Article/details/gmmplvney.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fktsv.cn/Article/details/gbtudbwap.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.epnwcf.com/Article/details/gbethxidi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.yfazqb.com/Article/details/gqvbtxfiy.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fktsv.cn/Article/details/gsbjfpgck.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gfjyodbyg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gksjrukoi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gicoznqyh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.epnwcf.com/Article/details/gphqbmmkp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.sjlbkw.cn/Article/details/guyukufct.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.yfazqb.com/Article/details/gnefllcno.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/gpvjojtgz.sHtML

[H07] 断言
来源：http://baike.bbcook.cn/Article/details/gljroiovg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.sjlbkw.cn/Article/details/geptqnerx.sHtML

PHP:  assert($x > 0);
来源：http://wap.yfazqb.com/Article/details/ginoevaec.sHtML

JS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/ghticictb.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gggjnoojv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.epnwcf.com/Article/details/gtyavaprs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.vehdjk.com/Article/details/gnpkmoert.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.bbcook.cn/Article/details/gzfhwneyw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gaebfnbrj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.yfazqb.com/Article/details/gjrwoaevg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.yfazqb.com/Article/details/grhtybcwm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.epnwcf.com/Article/details/gyzaxyjky.sHtML


<!-- 参考信息 -->