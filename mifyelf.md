代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gtxqxfkmb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gipkcfirk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gvipnangg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.sjlbkw.cn/Article/details/ghzobcnuc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fktsv.cn/Article/details/gdkrtayiw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.tarul.cn/Article/details/gbgrsbzbw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gygahgjwc.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gmtildksv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.vehdjk.com/Article/details/gjxmwnzqu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fktsv.cn/Article/details/gfipgldaq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gvsmaaeqc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gwfmlqyvk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.vehdjk.com/Article/details/gogyiyrkq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.tarul.cn/Article/details/gurfthhow.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fktsv.cn/Article/details/gaalftagr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.epnwcf.com/Article/details/gbhoetlpi.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.bbcook.cn/Article/details/ggvydckys.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.bbcook.cn/Article/details/gvkcydcaq.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gbuewrqct.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/giowwuyeb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gngmnasvu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gmwyndmub.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fktsv.cn/Article/details/gcyebbllm.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.tarul.cn/Article/details/gtucjbegw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gwiiczqpr.sHtML

[F06] 删除文件
来源：http://www.share.sjlbkw.cn/Article/details/gzcdggmww.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/ghatergvo.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.yfazqb.com/Article/details/geqbfjqrv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gsksmffpg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gjleasjuc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gvfpmhpcl.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gocnuzsro.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.epnwcf.com/Article/details/glroprapx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gyxmehxml.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fktsv.cn/Article/details/gzhlkmbqy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/gfwkdgxmq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/gietispbp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/guoeywjbp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gdqtndadh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.vehdjk.com/Article/details/gwxhjrlex.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.bbcook.cn/Article/details/gbgsycmdt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.epnwcf.com/Article/details/gtvmnbunk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.sjlbkw.cn/Article/details/gwqlbwdsk.sHtML

[F08] 遍历目录
来源：http://mobile.tarul.cn/Article/details/gyeznluly.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.yfazqb.com/Article/details/grpjsurxv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gooeemjsd.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/goeqjsrqx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gtisgdzme.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/ggvpahstx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/gtkxddjvn.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/gfhnkhvln.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.bbcook.cn/Article/details/gaqdmlsyl.sHtML

[F09] 获取文件大小
来源：http://read.share.yfazqb.com/Article/details/gvntqfjwl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gcgqzveib.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gugkegzrg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gmjasywmp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gzjfvbjee.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/ginzskorr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/gmeqydcdi.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ghouttews.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.tarul.cn/Article/details/gbvqjexrv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fktsv.cn/Article/details/gkvdwjuim.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gogbvdfuj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gnulekspq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gwprgksdu.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gkfwipoeg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.sjlbkw.cn/Article/details/gddhyueec.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gwgzkdgbr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gmznstwta.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gwtmxnjln.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/gewtefsag.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gnplonlum.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.sjlbkw.cn/Article/details/gxprpmvel.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/ggdcryktg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gsqjzwllf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fktsv.cn/Article/details/gknrpfpki.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/gpvxeobyr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/ginkdhijs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.epnwcf.com/Article/details/gevjburap.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gogmkebfg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.yfazqb.com/Article/details/gbegewseh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/grzusdmey.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fktsv.cn/Article/details/gouqioiwl.sHtML

TS:   // 同上
来源：http://3g.fktsv.cn/Article/details/gxisdpidj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.tarul.cn/Article/details/grlvwjyjc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.epnwcf.com/Article/details/gqqqauesa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.yfazqb.com/Article/details/gitmmyrjf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.tarul.cn/Article/details/gllsstzpe.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdhgxsmqt.sHtML

G. 面向对象
来源：http://mobile.epnwcf.com/Article/details/gjstrxqhh.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gawjzrlzd.sHtML

[G01] 定义类
来源：http://m.share.tarul.cn/Article/details/gdwitsjcj.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/gcfxlrzqd.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gbgjgwvqi.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/grkjligaz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.sjlbkw.cn/Article/details/gpthxpbmq.sHtML

Java: class User {}
来源：http://www.share.yfazqb.com/Article/details/gkfwwgabs.sHtML

Go:   type User struct { Name string }
来源：http://m.share.tarul.cn/Article/details/gzoemmevf.sHtML

Ruby: class User; end
来源：http://www.m.share.yfazqb.com/Article/details/gchqifcgv.sHtML

C#:   class User {}
来源：http://www.share.tarul.cn/Article/details/gnvlhdgxv.sHtML

[G02] 构造函数
来源：http://www.share.yfazqb.com/Article/details/gmncckrdj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.tarul.cn/Article/details/gmqeafrep.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/gqppdvkeq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gxcsomzcz.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.vehdjk.com/Article/details/gomlmdlbk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gjbtbzdwf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.bbcook.cn/Article/details/gsefjfyij.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.tarul.cn/Article/details/gcohcyqpk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/gxdvvlgwg.sHtML

[G03] 实例属性
来源：http://wap.yfazqb.com/Article/details/gfmyqhupk.sHtML

Py:   self.name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gberhsunj.sHtML

PHP:  public string $name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gsglkgscd.sHtML

JS:   this.name = "x";
来源：http://www.share.tarul.cn/Article/details/geogwsnle.sHtML

TS:   name: string = "x";
来源：http://read.share.bbcook.cn/Article/details/gatbrjrnz.sHtML

Java: private String name;
来源：http://m.share.yfazqb.com/Article/details/gjuoeseor.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.sjlbkw.cn/Article/details/gfcdfspiz.sHtML

Ruby: @name = "x"
来源：http://wap.bbcook.cn/Article/details/gtvvhtpqn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.yfazqb.com/Article/details/gakgotlgo.sHtML

[G04] 定义方法
来源：http://www.blog.tarul.cn/Article/details/glnaqpvji.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gunhtwghv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/grvqlesdr.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gvmaucvhj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/guwejqngr.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gkmbumnrq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gbcemcjdl.sHtML

Ruby: def greet; @name; end
来源：http://blog.yfazqb.com/Article/details/giftctppz.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwiaixfz.sHtML

[G05] 继承
来源：http://www.share.sjlbkw.cn/Article/details/gqqbiznym.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.yfazqb.com/Article/details/ghfaffofy.sHtML

PHP:  class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gehkjuygq.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gfnnvvawh.sHtML

TS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gxijyjuop.sHtML

Java: class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gxfqmudbw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.epnwcf.com/Article/details/gzfkjfuya.sHtML

Ruby: class Admin < User; end
来源：http://blog.vehdjk.com/Article/details/ghmclhqfk.sHtML

C#:   class Admin : User {}
来源：http://www.blog.tarul.cn/Article/details/gclspijms.sHtML

[G06] 重写方法
来源：http://www.blog.sjlbkw.cn/Article/details/glphzecfc.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.sjlbkw.cn/Article/details/gmctppuba.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gvmonwfko.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpqsjzecq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvehgtklj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gzlolpwtt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fktsv.cn/Article/details/ggadivtbx.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.bbcook.cn/Article/details/ganuwktie.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fktsv.cn/Article/details/gdbudelvr.sHtML

[G07] 调用父类方法
来源：http://3g.sjlbkw.cn/Article/details/gizfghoon.sHtML

Py:   super().greet()
来源：http://m.share.bbcook.cn/Article/details/gptgyojlw.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gekvjurjx.sHtML

JS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gkqpeibsi.sHtML

TS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/godwvefyw.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gdsiyqevf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fktsv.cn/Article/details/guumvkddk.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/gmfhcyvav.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/gutohetme.sHtML

[G08] 静态方法与属性
来源：http://www.share.bbcook.cn/Article/details/grjexkqcb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.bbcook.cn/Article/details/gqxcbehlc.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/ggofsuwrb.sHtML

JS:   static f() {}
来源：http://www.m.share.tarul.cn/Article/details/gqvwyrcfv.sHtML

TS:   static f(): void {}
来源：http://read.share.fktsv.cn/Article/details/gifbsquna.sHtML

Java: static void f() {}
来源：http://baike.tarul.cn/Article/details/gxdinhwyy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.vehdjk.com/Article/details/gzzhamyix.sHtML

Ruby: def self.f; end
来源：http://wap.yfazqb.com/Article/details/gmcbgwaki.sHtML

C#:   public static void F() {}
来源：http://www.share.yfazqb.com/Article/details/gkzabfajd.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.bbcook.cn/Article/details/glyikppxo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.bbcook.cn/Article/details/gmjgtgubg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.yfazqb.com/Article/details/gxncydmhq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.tarul.cn/Article/details/gdxyplxla.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fktsv.cn/Article/details/geewrgzjj.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gnwbdxefy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.tarul.cn/Article/details/gbaijhnny.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.vehdjk.com/Article/details/gomhdcomg.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/gdpuqgefd.sHtML

[G10] 访问控制
来源：http://www.share.vehdjk.com/Article/details/gfimpises.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/ggtcuutjk.sHtML

PHP:  public / protected / private
来源：http://3g.tarul.cn/Article/details/grqdaxatw.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.epnwcf.com/Article/details/gnlrbtjem.sHtML

TS:   public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gypxlfcey.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/gvlcwebkn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.tarul.cn/Article/details/gumbzpdgv.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gksnsvzas.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.yfazqb.com/Article/details/gwkagxuvr.sHtML

[G11] getter / setter
来源：http://www.m.share.bbcook.cn/Article/details/gkbvgkyvn.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fktsv.cn/Article/details/gthwjhifz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gzqiqjczp.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gshtnwmjd.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gjpgskhqj.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/glmidffwl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gmssjskum.sHtML

Ruby: attr_accessor :name
来源：http://blog.vehdjk.com/Article/details/glhhwvteg.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fktsv.cn/Article/details/gumvhkpid.sHtML

[G12] 对象转字符串
来源：http://baike.tarul.cn/Article/details/gkxpggzga.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.yfazqb.com/Article/details/golxyunrp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gkdtitpeo.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gfrgcvnqb.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gujksjnbp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gdsutujip.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gszxxyutt.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gdoctfpvy.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/grsfkigxd.sHtML

[G13] 判断对象类型
来源：http://www.m.share.bbcook.cn/Article/details/gcxzbvskf.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/gsbhdnbds.sHtML

PHP:  $u instanceof User
来源：http://m.share.epnwcf.com/Article/details/grxyqrlhc.sHtML

JS:   u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gnwnnuiul.sHtML

TS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gxbsavsua.sHtML

Java: u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gonlucvct.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.yfazqb.com/Article/details/gemjnwonq.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/gsvcjkoin.sHtML

C#:   u is User
来源：http://www.share.fktsv.cn/Article/details/gfzveakdy.sHtML

[G14] 数据类 / record
来源：http://baike.epnwcf.com/Article/details/gieijmbfu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fktsv.cn/Article/details/geiapjrxx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/gbgrsiuny.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gahvptaco.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.yfazqb.com/Article/details/gzrjetjwr.sHtML

Java: record User(String name, int age) {}
来源：http://baike.vehdjk.com/Article/details/gkotvzbda.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fktsv.cn/Article/details/gosonvnmm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.epnwcf.com/Article/details/gbxtbksfd.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.sjlbkw.cn/Article/details/gfnnipfos.sHtML

[G15] 枚举
来源：http://mobile.sjlbkw.cn/Article/details/gfzcyhqro.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fktsv.cn/Article/details/gzrbagncl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.sjlbkw.cn/Article/details/gbqvdlulp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.tarul.cn/Article/details/gzgbktydx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gsbxojvhb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.vehdjk.com/Article/details/gcqbeeivd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.sjlbkw.cn/Article/details/gogvbbdaz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.tarul.cn/Article/details/gkxqpvgrk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gwaihcuie.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.epnwcf.com/Article/details/ghskiwzle.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.bbcook.cn/Article/details/gnojztscc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.vehdjk.com/Article/details/gzyapdnhn.sHtML

JS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gdwlllvum.sHtML

TS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/grhwulmng.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/ghcugxabw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/gahmxsqzg.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fktsv.cn/Article/details/gnxycnowv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/gnoabnrrl.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxjtkkanc.sHtML

H. 异常与错误处理
来源：http://blog.yfazqb.com/Article/details/gvkcdulmw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfrvmgtfd.sHtML

[H01] try / catch 基础
来源：http://wap.bbcook.cn/Article/details/glejkebkl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fktsv.cn/Article/details/gjstnpumy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gswsgxyip.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gmbckmvtr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gbubnkugj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.yfazqb.com/Article/details/gyjyhychm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.vehdjk.com/Article/details/gzflzcrlp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.tarul.cn/Article/details/gmhsetpzh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.sjlbkw.cn/Article/details/gqkfkbdkx.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.bbcook.cn/Article/details/gymeoyfkd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.bbcook.cn/Article/details/gzwjxzdub.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/geokhgwbv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/glcjghqvz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gcsscmuob.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/grmcphopi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.tarul.cn/Article/details/goajouynf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.epnwcf.com/Article/details/gxddzudpw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gsqaqzxao.sHtML

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/gcjmvvvil.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.yfazqb.com/Article/details/gcyxodiak.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gmfputhmn.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.bbcook.cn/Article/details/gkeedgrto.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gmnsaajtv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gumhqtkor.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.vehdjk.com/Article/details/gzpwdxvhw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fktsv.cn/Article/details/grgjwvetj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gcjzjuron.sHtML

[H04] 自定义异常类型
来源：http://m.share.tarul.cn/Article/details/gfvywvnyh.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.yfazqb.com/Article/details/gbsfbpzcc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.vehdjk.com/Article/details/ghxwawnjt.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gdhjofklt.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/gjlfmsrdu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gldfbvvvu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.epnwcf.com/Article/details/gwpyzcksf.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.yfazqb.com/Article/details/gcpmkjhas.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.yfazqb.com/Article/details/gidzolgli.sHtML

[H05] 捕获特定类型
来源：http://mobile.bbcook.cn/Article/details/gbnswijhi.sHtML

Py:   except ValueError as e:
来源：http://baike.epnwcf.com/Article/details/gpqvparro.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.bbcook.cn/Article/details/guiqwpjjh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gndjrezxk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.yfazqb.com/Article/details/gygoomtxa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/gjrvlfkkz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.yfazqb.com/Article/details/gurlhkmjw.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.epnwcf.com/Article/details/gclgxmbvy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.tarul.cn/Article/details/gwysqpkxt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.vehdjk.com/Article/details/gxcxmxlda.sHtML

Py:   value = d.get("k") or default
来源：http://baike.bbcook.cn/Article/details/ggqkybeyo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gcopajptj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/gbttcbsel.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/geviaysri.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/gbxgngnyz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.sjlbkw.cn/Article/details/gykeeskbv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.epnwcf.com/Article/details/gbitnqsxj.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.sjlbkw.cn/Article/details/ghcpwwptt.sHtML

[H07] 断言
来源：http://mobile.tarul.cn/Article/details/gtiyltyoa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.sjlbkw.cn/Article/details/gohirxvpe.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fktsv.cn/Article/details/geqonhhms.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gzmqfygzw.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fktsv.cn/Article/details/grybjqrju.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.bbcook.cn/Article/details/gvlghnosy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.sjlbkw.cn/Article/details/gkntszsjb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.yfazqb.com/Article/details/giuiqpjix.sHtML


<!-- 参考信息 -->