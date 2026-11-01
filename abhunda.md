代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.bbcook.cn/Article/details/gvhohrsgv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/gwmoeoluw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/ggyiamexn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/gtccyxzca.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gcdobwjfn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gnzhzbspq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/geuwryhyl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.vehdjk.com/Article/details/gotzzkzof.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.sjlbkw.cn/Article/details/gchyigtfw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.epnwcf.com/Article/details/gvbpmbyvu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gzggxuqax.sHtML

[F04] 追加写入文件
来源：http://www.share.tarul.cn/Article/details/gvwsmcedh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/gwhvxqkps.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.vehdjk.com/Article/details/gvswmvxms.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gfuzekrfi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/giurdgyfi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.vehdjk.com/Article/details/gzzpxecqk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.tarul.cn/Article/details/gswdoqpgk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.epnwcf.com/Article/details/gcspgeywy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/gxuolsezm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.bbcook.cn/Article/details/gyhecjvkb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.bbcook.cn/Article/details/gqoflrnqo.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.bbcook.cn/Article/details/glfazwsah.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ghdfgwekw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gizfpjwgm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gutqgrgry.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.vehdjk.com/Article/details/gfelvbgtj.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.tarul.cn/Article/details/gzixpexrb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gdvkmwnia.sHtML

[F06] 删除文件
来源：http://blog.fktsv.cn/Article/details/gsgkyinen.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/guyzbpxqy.sHtML

PHP:  unlink("a.txt");
来源：http://wap.yfazqb.com/Article/details/gcldjdsgb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/genhfidgi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gjvxrjfru.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gualoxanc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gtgbeultm.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gehzeuaqt.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gfslvfzmt.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fktsv.cn/Article/details/giqoilsru.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/ghfkfxrcq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/gkawurnfs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gmlrguknp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gbmqkoswz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/guasgstul.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.bbcook.cn/Article/details/guzulsmek.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.yfazqb.com/Article/details/gdgvrmshg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gqwemkjkq.sHtML

[F08] 遍历目录
来源：http://m.share.bbcook.cn/Article/details/gytnctxca.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fktsv.cn/Article/details/gwwlaibav.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.epnwcf.com/Article/details/glmgxmqgf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gsnbxdlhf.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gyjalvufz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gprthmxex.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.tarul.cn/Article/details/guxhknold.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.bbcook.cn/Article/details/gfbdeyuji.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/ghhtkjluz.sHtML

[F09] 获取文件大小
来源：http://m.share.sjlbkw.cn/Article/details/gyjitzwna.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gzcubscdr.sHtML

PHP:  filesize("a.txt");
来源：http://wap.yfazqb.com/Article/details/gerximdbr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gvxmwnxiq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gouaoeivh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gjodpljys.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.tarul.cn/Article/details/gnqzahizo.sHtML

Ruby: File.size("a.txt")
来源：http://wap.epnwcf.com/Article/details/ggiyyyoox.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.sjlbkw.cn/Article/details/grietnlrk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.epnwcf.com/Article/details/gxzodoslu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gqtvneurg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.tarul.cn/Article/details/gduxqkmqg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gbhivgftu.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gtoxhrzix.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.bbcook.cn/Article/details/glivlsafz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gdkjxvuzy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gelaohimx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/glaxnidvu.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/goitbotyc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gsymscpkf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fktsv.cn/Article/details/gunkayywg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gzwyebmqg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/groyazmip.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gerksjdqf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gjxvizizn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gagrciylx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/gspitnacz.sHtML

[F12] CSV 读写
来源：http://mobile.bbcook.cn/Article/details/gbkdpinat.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.vehdjk.com/Article/details/gfgkdhknk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.sjlbkw.cn/Article/details/gqfbzaxez.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/genwxtnpc.sHtML

TS:   // 同上
来源：http://m.share.epnwcf.com/Article/details/gyvjyvhbt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/giebfwajs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.tarul.cn/Article/details/gnlckstgf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gxvtwegtw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fktsv.cn/Article/details/gtzvtbpqg.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvwcrwqqr.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/geyreurwa.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gloqiwkpm.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gykfzeppg.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/gzdnpqlif.sHtML

PHP:  class User {}
来源：http://blog.tarul.cn/Article/details/gonbokxli.sHtML

JS:   class User {}
来源：http://blog.epnwcf.com/Article/details/gbmfiujyt.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.epnwcf.com/Article/details/gvjgxloau.sHtML

Java: class User {}
来源：http://read.share.yfazqb.com/Article/details/gpxfumlay.sHtML

Go:   type User struct { Name string }
来源：http://3g.sjlbkw.cn/Article/details/gxqudoyzp.sHtML

Ruby: class User; end
来源：http://mobile.tarul.cn/Article/details/gncbejmux.sHtML

C#:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gdpikxfrn.sHtML

[G02] 构造函数
来源：http://baike.sjlbkw.cn/Article/details/gfrjumevr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/ghktffjbb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.epnwcf.com/Article/details/gmawoxwhj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gjssqycdi.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.tarul.cn/Article/details/gieliwfds.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gryepvrpk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gohdyyiln.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/gkncplfzi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/ggcrqvzoa.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/gxhfrzhay.sHtML

Py:   self.name = "x"
来源：http://www.share.fktsv.cn/Article/details/gpkamlira.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/gqrzohcmt.sHtML

JS:   this.name = "x";
来源：http://wap.epnwcf.com/Article/details/gbqsdobxv.sHtML

TS:   name: string = "x";
来源：http://blog.bbcook.cn/Article/details/gwxuikote.sHtML

Java: private String name;
来源：http://wap.vehdjk.com/Article/details/gvzuhromg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fktsv.cn/Article/details/ggesxucfk.sHtML

Ruby: @name = "x"
来源：http://blog.tarul.cn/Article/details/gmffnndnm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/glystynqn.sHtML

[G04] 定义方法
来源：http://wap.bbcook.cn/Article/details/gqmoaubgk.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gllxjutuh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gssetmpki.sHtML

JS:   greet() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gwhntrkgo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gjgvxfopf.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gyczbohsn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gsoyjfyfs.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gnojvunre.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gffpornpa.sHtML

[G05] 继承
来源：http://wap.tarul.cn/Article/details/guwydkssh.sHtML

Py:   class Admin(User): pass
来源：http://baike.vehdjk.com/Article/details/gskkqlzgf.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gguqxybvi.sHtML

JS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gzmibaejz.sHtML

TS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gcidxbwfi.sHtML

Java: class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gszlqxdka.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.vehdjk.com/Article/details/gcsibkies.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.bbcook.cn/Article/details/gpmdfojcw.sHtML

C#:   class Admin : User {}
来源：http://blog.yfazqb.com/Article/details/gxfezkhms.sHtML

[G06] 重写方法
来源：http://read.share.epnwcf.com/Article/details/ghovmesru.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.epnwcf.com/Article/details/gbzkdvdtr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gvzydktkn.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gzminvabi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gumpflxff.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gyhwxtbbv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.vehdjk.com/Article/details/ghqtwkper.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gzcngxraz.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.tarul.cn/Article/details/gqciphnos.sHtML

[G07] 调用父类方法
来源：http://blog.vehdjk.com/Article/details/gdcorqdym.sHtML

Py:   super().greet()
来源：http://3g.fktsv.cn/Article/details/gfyoawcpr.sHtML

PHP:  parent::greet();
来源：http://mobile.sjlbkw.cn/Article/details/gfcqiwtcm.sHtML

JS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/guknkrelq.sHtML

TS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gzngwylun.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpxyexdv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.sjlbkw.cn/Article/details/guspbskyv.sHtML

Ruby: super
来源：http://m.share.epnwcf.com/Article/details/ggnjmumny.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/gnztclphu.sHtML

[G08] 静态方法与属性
来源：http://read.share.epnwcf.com/Article/details/gczqxvrls.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fktsv.cn/Article/details/gdanssszs.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gfmfklfre.sHtML

JS:   static f() {}
来源：http://wap.tarul.cn/Article/details/giunuceio.sHtML

TS:   static f(): void {}
来源：http://m.share.yfazqb.com/Article/details/gmqngazqy.sHtML

Java: static void f() {}
来源：http://blog.tarul.cn/Article/details/glftjefxt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fktsv.cn/Article/details/gvkagfqfs.sHtML

Ruby: def self.f; end
来源：http://www.share.yfazqb.com/Article/details/gpggqscgf.sHtML

C#:   public static void F() {}
来源：http://wap.yfazqb.com/Article/details/gvkptdnuf.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.vehdjk.com/Article/details/glkyuchmu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.vehdjk.com/Article/details/geinufybs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.tarul.cn/Article/details/gbxugeuob.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.bbcook.cn/Article/details/gyavsfebw.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.yfazqb.com/Article/details/gnqpyypyc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbvdpogbk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/gmlqcihou.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.vehdjk.com/Article/details/gzknwjcoc.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.epnwcf.com/Article/details/gospkvaag.sHtML

[G10] 访问控制
来源：http://blog.sjlbkw.cn/Article/details/gbaddmpsj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/gfyymsalc.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gynikarth.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.epnwcf.com/Article/details/gmuhtadqg.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gfslbqtmg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/grlyuzcds.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.bbcook.cn/Article/details/guijudgks.sHtML

Ruby: public / protected / private
来源：http://blog.bbcook.cn/Article/details/gfprlawhc.sHtML

C#:   public / protected / private / internal
来源：http://mobile.vehdjk.com/Article/details/gzbrzzkcm.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/gtkycetbv.sHtML

Py:   @property 与 @x.setter
来源：http://wap.yfazqb.com/Article/details/gnpunvpoh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/grnyyneyl.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gtunwvtxt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gamlqbdwo.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/glbxodxnd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gkheyeuft.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.tarul.cn/Article/details/gumqsxone.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.sjlbkw.cn/Article/details/gwpftypvx.sHtML

[G12] 对象转字符串
来源：http://wap.fktsv.cn/Article/details/gwlszsjfb.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gybnrluwb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gbqyxynjm.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/glmvsjnia.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/grjsiuqjj.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gowzncvao.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gfngdmokt.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gobbpkfqv.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/gntmxueph.sHtML

[G13] 判断对象类型
来源：http://mobile.epnwcf.com/Article/details/gblejqpmf.sHtML

Py:   isinstance(u, User)
来源：http://mobile.yfazqb.com/Article/details/gtjabdtey.sHtML

PHP:  $u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gayuxayfb.sHtML

JS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gxhhkbgbn.sHtML

TS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gwfyuphiy.sHtML

Java: u instanceof User
来源：http://wap.epnwcf.com/Article/details/gklsasacr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/gdcznykgz.sHtML

Ruby: u.is_a?(User)
来源：http://3g.epnwcf.com/Article/details/gulkphrxm.sHtML

C#:   u is User
来源：http://m.share.fktsv.cn/Article/details/gortywkdz.sHtML

[G14] 数据类 / record
来源：http://3g.epnwcf.com/Article/details/gsgmukwag.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.sjlbkw.cn/Article/details/glusfblxu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.bbcook.cn/Article/details/gudfmjaje.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/gmbvhwehm.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.epnwcf.com/Article/details/gbunvygqu.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fktsv.cn/Article/details/gbzqunthk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.vehdjk.com/Article/details/ghzgzcckh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.vehdjk.com/Article/details/ghlaefhzc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.epnwcf.com/Article/details/gdcmvirfj.sHtML

[G15] 枚举
来源：http://wap.fktsv.cn/Article/details/grwfrcctw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/gjwdulzuh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.sjlbkw.cn/Article/details/gntriuiyk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fktsv.cn/Article/details/gubcmsjap.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gbmjwngil.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/ghkbsqtfy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fktsv.cn/Article/details/gpkcyikni.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gfreortos.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gcuonwjlc.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fktsv.cn/Article/details/gaeccflqm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.tarul.cn/Article/details/gylajhbjq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gjzqkocdg.sHtML

JS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gzzllfvhp.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/grnxelekg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.vehdjk.com/Article/details/gsccpjqug.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.tarul.cn/Article/details/gzvidgipr.sHtML

Ruby: obj.instance_variables
来源：http://3g.yfazqb.com/Article/details/gusuhurqr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gedpodjpd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkcrteppg.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gafgctfyo.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqhliedyi.sHtML

[H01] try / catch 基础
来源：http://m.share.sjlbkw.cn/Article/details/gqitpazfj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gorshoxoj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.sjlbkw.cn/Article/details/glibdisnx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gurrfkjpa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/garpinfeh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.epnwcf.com/Article/details/gbapqjefd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.bbcook.cn/Article/details/gnefctfqu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.vehdjk.com/Article/details/gavulolol.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.sjlbkw.cn/Article/details/giobkqkmr.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fktsv.cn/Article/details/gnsfsnntv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.epnwcf.com/Article/details/gtasrqkkr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gttzrczul.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gwchxhnne.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gubkjlqoj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gejuujgnm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.yfazqb.com/Article/details/gotvgpsfg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.epnwcf.com/Article/details/gldumrecn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gmuzddbae.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/gdbtmsjre.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fktsv.cn/Article/details/gzsubjset.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtafyaobv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/gvqrykaoc.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gpzlbouex.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/ghoyrbzfg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.tarul.cn/Article/details/gjmnxexcx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fktsv.cn/Article/details/gobievlts.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gzqklylrm.sHtML

[H04] 自定义异常类型
来源：http://mobile.sjlbkw.cn/Article/details/gohyyiuea.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/gxbqifobd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/giawtwzdk.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gvyrfksgn.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gqwgtimvr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gedqjsuud.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fktsv.cn/Article/details/gzkgjeffm.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fktsv.cn/Article/details/giffbljuo.sHtML

C#:   class MyException : Exception {}
来源：http://3g.yfazqb.com/Article/details/gdlqxxqgf.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/gedxtjwzf.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/gksohnvgl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.vehdjk.com/Article/details/gplwwxvgn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gxptqkpeq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.vehdjk.com/Article/details/gitbbyvvk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.tarul.cn/Article/details/gqhtipavb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.tarul.cn/Article/details/gcjpkovmg.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.bbcook.cn/Article/details/gxmdwcmsu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.vehdjk.com/Article/details/gxfizgpsi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.yfazqb.com/Article/details/gjdideuus.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.tarul.cn/Article/details/gnlxtjeyw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gjcdzkydz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.yfazqb.com/Article/details/gspqowzeh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.yfazqb.com/Article/details/grphwwwue.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fktsv.cn/Article/details/gygejpcxv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fktsv.cn/Article/details/gitbgpvtt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gztgygsdb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.bbcook.cn/Article/details/gzstuwpdm.sHtML

[H07] 断言
来源：http://blog.epnwcf.com/Article/details/grzydsubi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.epnwcf.com/Article/details/gmxqyokrc.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gwjvyloqo.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/ginujguuq.sHtML


<!-- 参考信息 -->