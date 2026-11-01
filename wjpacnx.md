代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.yfazqb.com/Article/details/gwuxsmqkm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/gdmsbrxwo.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.yfazqb.com/Article/details/ginrjgfuz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/goturcdrr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/guxtrlxzf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/giztlcvzo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gaxxcqbzw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gnonqange.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.tarul.cn/Article/details/guvsnoika.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.vehdjk.com/Article/details/gtlniqvlg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/ggeyiurhx.sHtML

[F04] 追加写入文件
来源：http://mobile.bbcook.cn/Article/details/gshdilpdc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gtwaunfpp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.epnwcf.com/Article/details/gbfuwiiyh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gmlbepqqi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/gbiqnmkdz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.yfazqb.com/Article/details/ggkkysuoa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fktsv.cn/Article/details/gqhbblhvn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fktsv.cn/Article/details/gvjckvowk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/gssrnxhbu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gpliqepla.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.tarul.cn/Article/details/gneihunfr.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gkvpjcotx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gsfnjcxdk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ghsilqhpo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gttoayapm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/gijndknww.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gjhhnmmfx.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gratjvgxt.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/godijqiwl.sHtML

Py:   os.remove("a.txt")
来源：http://3g.tarul.cn/Article/details/ggqyagisf.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gdeczprwk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gwrqlehix.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gsazeikgo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gcpcbdwfx.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/ghkfkfymx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gydzqroel.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.bbcook.cn/Article/details/ghuncapip.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/gjjjqybss.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gcmzqevgm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.bbcook.cn/Article/details/gtpcjcnop.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gzuiwlvfg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gmjxwjqxl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/gxsqsextg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/gzmbruocz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.vehdjk.com/Article/details/geshgghzt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.tarul.cn/Article/details/gomxxnggl.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/gqbkgylvb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gnbkrypxq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.bbcook.cn/Article/details/grtikcbta.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/giyfkzlvy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gwzqwpgan.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/ggakwhxxd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gmhonkyfk.sHtML

Ruby: Dir.children("dir")
来源：http://wap.tarul.cn/Article/details/gwjgyfobq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gdehvwguj.sHtML

[F09] 获取文件大小
来源：http://3g.sjlbkw.cn/Article/details/gnyjapvjr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.epnwcf.com/Article/details/govnbxboj.sHtML

PHP:  filesize("a.txt");
来源：http://baike.tarul.cn/Article/details/gxiaurlsx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/gsybhyyuk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gsimvnxzv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gugipicsh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.tarul.cn/Article/details/gqcbrmxwy.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gjhdrdlpa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.vehdjk.com/Article/details/gjxqkdnnf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.yfazqb.com/Article/details/goldakijr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gldskdwxm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.epnwcf.com/Article/details/gwgprxvew.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gwpqqhink.sHtML

TS:   path.extname("a.txt")
来源：http://baike.tarul.cn/Article/details/gaisootgj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.tarul.cn/Article/details/grpuiyizm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gxkohgjry.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gaiqoekma.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gjsuatzjp.sHtML

[F11] 复制与移动文件
来源：http://m.share.tarul.cn/Article/details/grpuzvsxv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gzvbiuxrq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.yfazqb.com/Article/details/ggderrqas.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gpjwuteqm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gzbyzcksj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/gurpnaces.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.bbcook.cn/Article/details/gbptdvras.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gcdrgrrfk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gdaxwxnvo.sHtML

[F12] CSV 读写
来源：http://www.m.share.epnwcf.com/Article/details/gwcjpjtlf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.yfazqb.com/Article/details/gjsheopya.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.sjlbkw.cn/Article/details/gvaoyemez.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.yfazqb.com/Article/details/gymkgzlpv.sHtML

TS:   // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/gstnrbepf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.vehdjk.com/Article/details/gxjadsdya.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/gvbhoipkd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.sjlbkw.cn/Article/details/grlcylhmx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/gvjushtku.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfcxvsior.sHtML

G. 面向对象
来源：http://m.share.bbcook.cn/Article/details/gbdnwjdtc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghelmtyjs.sHtML

[G01] 定义类
来源：http://wap.yfazqb.com/Article/details/gdrgbotik.sHtML

Py:   class User: pass
来源：http://m.share.bbcook.cn/Article/details/ghxgfmjoz.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/gqyomkwrd.sHtML

JS:   class User {}
来源：http://3g.bbcook.cn/Article/details/gqexknndc.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.tarul.cn/Article/details/gsmwblwox.sHtML

Java: class User {}
来源：http://baike.fktsv.cn/Article/details/gmypuzloe.sHtML

Go:   type User struct { Name string }
来源：http://m.share.tarul.cn/Article/details/goqkenpts.sHtML

Ruby: class User; end
来源：http://www.share.bbcook.cn/Article/details/ghogfzhjo.sHtML

C#:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gqkxaxxcg.sHtML

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/gkwqmjpmz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gogrfmzvx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/gkblopitc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/geniqsgpg.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.yfazqb.com/Article/details/gmmvpweny.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzissirul.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.vehdjk.com/Article/details/gcxcdacup.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.sjlbkw.cn/Article/details/gpkizbxxl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.bbcook.cn/Article/details/gexthhznz.sHtML

[G03] 实例属性
来源：http://blog.epnwcf.com/Article/details/gikbtyggd.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gvmqmnpmq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.epnwcf.com/Article/details/gslwpfqxq.sHtML

JS:   this.name = "x";
来源：http://3g.bbcook.cn/Article/details/gxckslahr.sHtML

TS:   name: string = "x";
来源：http://m.share.tarul.cn/Article/details/gfoixkufh.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/gcyyzpuwn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.vehdjk.com/Article/details/gejsgelrt.sHtML

Ruby: @name = "x"
来源：http://m.share.epnwcf.com/Article/details/gqjqrogoy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gcgjlzfxp.sHtML

[G04] 定义方法
来源：http://mobile.vehdjk.com/Article/details/gngmyrfmg.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/goxhmyfpb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/giydcmreh.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gbkhltwji.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gyzzypqas.sHtML

Java: String greet() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gnwjyeoxw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gaghpuotv.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/gptuoyqav.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.yfazqb.com/Article/details/goozordeh.sHtML

[G05] 继承
来源：http://www.m.share.tarul.cn/Article/details/gawltthtk.sHtML

Py:   class Admin(User): pass
来源：http://baike.yfazqb.com/Article/details/gpyvvxnoj.sHtML

PHP:  class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gczyqpkgq.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gqqgyfidw.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/glhntvcfq.sHtML

Java: class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/grdroegtz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gbhwwdmuu.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fktsv.cn/Article/details/gnwswqzoz.sHtML

C#:   class Admin : User {}
来源：http://read.share.fktsv.cn/Article/details/gudfvmjqm.sHtML

[G06] 重写方法
来源：http://blog.vehdjk.com/Article/details/gpxheoldm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.yfazqb.com/Article/details/gphofclod.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/ggptbadks.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gunabgwjw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gygftmjod.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/ggcoxugtl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.epnwcf.com/Article/details/gptnbmgob.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.tarul.cn/Article/details/gblgreyxu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.sjlbkw.cn/Article/details/gmwlushlg.sHtML

[G07] 调用父类方法
来源：http://blog.bbcook.cn/Article/details/gjzafwzya.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/gthxgvnbf.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gwnkqtrki.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gjmwmdkzt.sHtML

TS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gktpauayx.sHtML

Java: super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gobqbkwci.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/glvdzegzj.sHtML

Ruby: super
来源：http://www.blog.bbcook.cn/Article/details/gfzcjvlkt.sHtML

C#:   base.Greet();
来源：http://baike.sjlbkw.cn/Article/details/gnxxgpkgd.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/gvqdrjqqn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.vehdjk.com/Article/details/gnkxowmja.sHtML

PHP:  public static function f() {}
来源：http://mobile.fktsv.cn/Article/details/gfvhjsvie.sHtML

JS:   static f() {}
来源：http://baike.vehdjk.com/Article/details/gexkpwrie.sHtML

TS:   static f(): void {}
来源：http://read.share.yfazqb.com/Article/details/gtebztwvu.sHtML

Java: static void f() {}
来源：http://read.share.tarul.cn/Article/details/gjvqlixjr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.tarul.cn/Article/details/gxczbihmf.sHtML

Ruby: def self.f; end
来源：http://baike.yfazqb.com/Article/details/gxblltmys.sHtML

C#:   public static void F() {}
来源：http://wap.sjlbkw.cn/Article/details/gfuswmvkw.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gxipqofqj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.yfazqb.com/Article/details/gtlnnnkod.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.sjlbkw.cn/Article/details/gubvrvugl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.epnwcf.com/Article/details/gunmedgwz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/gygyabcxx.sHtML

Java: interface Shape { double area(); }
来源：http://3g.epnwcf.com/Article/details/grvbyzgfw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.yfazqb.com/Article/details/gmqnqrpbx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.vehdjk.com/Article/details/gfaghpvls.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gxonnwnsb.sHtML

[G10] 访问控制
来源：http://www.share.fktsv.cn/Article/details/gltgabnpf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/gapqgtjhg.sHtML

PHP:  public / protected / private
来源：http://wap.yfazqb.com/Article/details/gvlhuynyi.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gljwjnsaw.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gxtyuortj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.epnwcf.com/Article/details/goyqzzkhs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.sjlbkw.cn/Article/details/gzwreqqds.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gchxiobro.sHtML

C#:   public / protected / private / internal
来源：http://www.share.bbcook.cn/Article/details/gxzzjoarz.sHtML

[G11] getter / setter
来源：http://baike.bbcook.cn/Article/details/giorfqofy.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/gdylwrcnn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gseptctjr.sHtML

JS:   get name() { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gkpqsoopv.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fktsv.cn/Article/details/gibzqtiqb.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gmtgqqwlt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gstlgwezs.sHtML

Ruby: attr_accessor :name
来源：http://www.share.yfazqb.com/Article/details/gtlkezkzt.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.epnwcf.com/Article/details/gealsrtdz.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/gtfezxizq.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/guvdqomfz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gzrnhmwup.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gocgatzdo.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/grgkqhtze.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gwbtqtnqt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gvtdzbuix.sHtML

Ruby: def to_s; @name; end
来源：http://wap.bbcook.cn/Article/details/gjmnwmcwt.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/gupsmnsvq.sHtML

[G13] 判断对象类型
来源：http://wap.bbcook.cn/Article/details/guceapmzv.sHtML

Py:   isinstance(u, User)
来源：http://baike.bbcook.cn/Article/details/ggrjfshpo.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/glibavpug.sHtML

JS:   u instanceof User
来源：http://wap.tarul.cn/Article/details/gbmmtqgdd.sHtML

TS:   u instanceof User
来源：http://blog.fktsv.cn/Article/details/ggrpwglfx.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/graqlpdbs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.vehdjk.com/Article/details/gvmguwufs.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.tarul.cn/Article/details/gvzjmbtvz.sHtML

C#:   u is User
来源：http://www.blog.vehdjk.com/Article/details/gprfzkzfr.sHtML

[G14] 数据类 / record
来源：http://m.share.fktsv.cn/Article/details/gtgahjqvx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fktsv.cn/Article/details/gclpgvnaq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.vehdjk.com/Article/details/gfppunhyf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.sjlbkw.cn/Article/details/gxljqqjyl.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.vehdjk.com/Article/details/gswlonkae.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.vehdjk.com/Article/details/gqwzqovwz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.sjlbkw.cn/Article/details/gzvjuuurf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.epnwcf.com/Article/details/gexmipmbt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.vehdjk.com/Article/details/geasadndr.sHtML

[G15] 枚举
来源：http://wap.yfazqb.com/Article/details/gmnxapmuy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.yfazqb.com/Article/details/grrhryerb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.vehdjk.com/Article/details/gvniapqsi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gbcozprvo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gvpwjgfiy.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.yfazqb.com/Article/details/ggufsgtea.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.vehdjk.com/Article/details/gtexovsqo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fktsv.cn/Article/details/gkysjqqan.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/guqpiyhbs.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.sjlbkw.cn/Article/details/ginuuptlv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fktsv.cn/Article/details/gdhlusbbr.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.bbcook.cn/Article/details/gqwkeetoy.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gzkiauggs.sHtML

TS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gaqtzvaok.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.vehdjk.com/Article/details/gpfddxehm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/goakapkhy.sHtML

Ruby: obj.instance_variables
来源：http://wap.epnwcf.com/Article/details/gzdsyolfy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/gwlpccriu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkvpbhbzc.sHtML

H. 异常与错误处理
来源：http://m.share.fktsv.cn/Article/details/gqkzxioie.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ggtocjwgu.sHtML

[H01] try / catch 基础
来源：http://www.share.epnwcf.com/Article/details/gbikgncop.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.yfazqb.com/Article/details/gbuhltgrq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbztgwpmo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gdnaljoww.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gjkbdriqr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.tarul.cn/Article/details/gobtagapf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fktsv.cn/Article/details/ghruerndr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/gnhngclnw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.tarul.cn/Article/details/gycnpqnxy.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.tarul.cn/Article/details/gzmdzdeiu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.vehdjk.com/Article/details/grzrxxqmc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gpfehjdjw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gewjncute.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gbehqyfat.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gwckbggpd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.sjlbkw.cn/Article/details/grstyhzbx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.yfazqb.com/Article/details/gwquimutd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gdducgpam.sHtML

[H03] 主动抛出异常
来源：http://wap.bbcook.cn/Article/details/gpvfuxhqd.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.epnwcf.com/Article/details/gpthhrebi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gkdtztjtx.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.yfazqb.com/Article/details/gcqnkqoik.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/guadiuctl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gfcddutfk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.yfazqb.com/Article/details/gfjroomql.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.vehdjk.com/Article/details/gzivsrejh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gudoosnlh.sHtML

[H04] 自定义异常类型
来源：http://www.share.bbcook.cn/Article/details/gajpwacrx.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.vehdjk.com/Article/details/gpptznohj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gehioooqs.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gpijurgrz.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gnyistohf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/godgqhygt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fktsv.cn/Article/details/gjonmopph.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.sjlbkw.cn/Article/details/ghlnnsgvi.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/grmihrmil.sHtML

[H05] 捕获特定类型
来源：http://baike.sjlbkw.cn/Article/details/ghittlwiq.sHtML

Py:   except ValueError as e:
来源：http://blog.yfazqb.com/Article/details/gviamkueo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.vehdjk.com/Article/details/gpqqdafzb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjctsfnaw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/geboextuq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.epnwcf.com/Article/details/gucwehhhh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.vehdjk.com/Article/details/gigihziym.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.vehdjk.com/Article/details/gaviycjdc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.tarul.cn/Article/details/gdnayspcf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fktsv.cn/Article/details/gpzmcdely.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.vehdjk.com/Article/details/gzlahiglf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/geqlknqaw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/geufwxrxz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.bbcook.cn/Article/details/gmsxkfjyl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.sjlbkw.cn/Article/details/gfwjjurgy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.epnwcf.com/Article/details/gnfvflkvt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/griqqncab.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.vehdjk.com/Article/details/gcbzsbufw.sHtML

[H07] 断言
来源：http://wap.bbcook.cn/Article/details/gwowlalti.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.yfazqb.com/Article/details/guferinwu.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/gxijdvsjh.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gzcymtppo.sHtML


<!-- 参考信息 -->