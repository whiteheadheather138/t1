代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gfxzurbss.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gnbcdrojj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gvbwxiguq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.tarul.cn/Article/details/gnlvbabme.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fktsv.cn/Article/details/gfipzsfgg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/guujgubzm.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.tarul.cn/Article/details/gbutapipq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gwwvbkfop.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gfforyxco.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gfeavgqpy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gvkhfwbkq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.bbcook.cn/Article/details/gyaasiend.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.bbcook.cn/Article/details/gkeslayyw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.bbcook.cn/Article/details/gqpenqbsy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gixdbmcpy.sHtML

[F04] 追加写入文件
来源：http://blog.tarul.cn/Article/details/gnhptholl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.vehdjk.com/Article/details/gadlfjmnv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gvfksecwq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gpyqtbzrz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/gtyuznvuq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.yfazqb.com/Article/details/gklmcptcb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gcgcqhouf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.vehdjk.com/Article/details/gyypoysrq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/gjamljdag.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.yfazqb.com/Article/details/gyicsiwqi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.vehdjk.com/Article/details/gisbymmlc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gqzpcijwt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gdipixmvj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gvpfszlzy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gsmufmyfo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.vehdjk.com/Article/details/gbufwathn.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gvzubxmwv.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/gezkpghlt.sHtML

[F06] 删除文件
来源：http://baike.epnwcf.com/Article/details/gvsvsaqwu.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gnebxnfyi.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gcevktgll.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gfwddnern.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gieikcwkf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gxmkuurjl.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/grzffhhvq.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.vehdjk.com/Article/details/ggvtqzszh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.tarul.cn/Article/details/gtbysleyl.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.vehdjk.com/Article/details/glbamuven.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gvupqgaur.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.yfazqb.com/Article/details/ghcouvgml.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/ghfrchhni.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gopdtphbr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlrkgrtk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.yfazqb.com/Article/details/gbjkfsmhz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.sjlbkw.cn/Article/details/gekdslaqj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/gpbyrcxvh.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gtyxxqfwd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.sjlbkw.cn/Article/details/gpvehhxvr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/gvhsvqnzp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gsphejfvp.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gnjnbwxle.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/gbkxznykn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.vehdjk.com/Article/details/geerppgdk.sHtML

Ruby: Dir.children("dir")
来源：http://wap.vehdjk.com/Article/details/glfcrtknx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.sjlbkw.cn/Article/details/gnbmpnkpl.sHtML

[F09] 获取文件大小
来源：http://3g.tarul.cn/Article/details/gjpyqybot.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gwcagboly.sHtML

PHP:  filesize("a.txt");
来源：http://baike.bbcook.cn/Article/details/gkxyvznen.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/ggcgdpvqw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gugrksbqo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gdhebdnxr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.tarul.cn/Article/details/gvydgoooo.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/gqpnncsil.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.tarul.cn/Article/details/gjazgvoiv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.yfazqb.com/Article/details/gswohanou.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ghyudrhww.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fktsv.cn/Article/details/gmssrmgxz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gxeabofjy.sHtML

TS:   path.extname("a.txt")
来源：http://3g.tarul.cn/Article/details/googjobzp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.bbcook.cn/Article/details/gneiuiepg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gnfhgizuc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gztekqmhk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gmuculuri.sHtML

[F11] 复制与移动文件
来源：http://blog.vehdjk.com/Article/details/gkcpjugrm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjmbodln.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.tarul.cn/Article/details/gbnabpcke.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gihjtmdef.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gpdfjmefu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.yfazqb.com/Article/details/ghxtyzzep.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/gthlnppql.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gooxrcxqw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fktsv.cn/Article/details/gwgwombte.sHtML

[F12] CSV 读写
来源：http://mobile.fktsv.cn/Article/details/gfjdnpill.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.sjlbkw.cn/Article/details/gyxhgjlvw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.tarul.cn/Article/details/gvrinahpq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.bbcook.cn/Article/details/gqixradqs.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/ghdzxfpop.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fktsv.cn/Article/details/gwposcatr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.yfazqb.com/Article/details/gvpojprgk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.bbcook.cn/Article/details/gaqwsrrhv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyaluxol.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gekxeihev.sHtML

G. 面向对象
来源：http://read.share.vehdjk.com/Article/details/grioizaoi.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdyehiqjp.sHtML

[G01] 定义类
来源：http://mobile.tarul.cn/Article/details/gpesbauor.sHtML

Py:   class User: pass
来源：http://m.share.bbcook.cn/Article/details/gzkjdtkqv.sHtML

PHP:  class User {}
来源：http://read.share.fktsv.cn/Article/details/gaugmutdh.sHtML

JS:   class User {}
来源：http://m.share.bbcook.cn/Article/details/ghvahnfyd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/grchhxdic.sHtML

Java: class User {}
来源：http://read.share.yfazqb.com/Article/details/giyzryjfy.sHtML

Go:   type User struct { Name string }
来源：http://3g.bbcook.cn/Article/details/gpioesixm.sHtML

Ruby: class User; end
来源：http://www.m.share.bbcook.cn/Article/details/gqcppghxw.sHtML

C#:   class User {}
来源：http://m.share.vehdjk.com/Article/details/guxyqizjd.sHtML

[G02] 构造函数
来源：http://wap.sjlbkw.cn/Article/details/gstdhfrxu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/ggchwbkrg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fktsv.cn/Article/details/gdzwpexnb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/genezvwll.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.epnwcf.com/Article/details/ggfzzuqez.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/gokoaohnt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gwzsttkmk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fktsv.cn/Article/details/grbddajdd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/gqgxtvecv.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/ggwaujiqn.sHtML

Py:   self.name = "x"
来源：http://m.share.tarul.cn/Article/details/ggkplxhoa.sHtML

PHP:  public string $name = "x";
来源：http://www.share.bbcook.cn/Article/details/gymbektsj.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gapbyejvu.sHtML

TS:   name: string = "x";
来源：http://www.share.bbcook.cn/Article/details/gdxbrngft.sHtML

Java: private String name;
来源：http://read.share.sjlbkw.cn/Article/details/gvbwqdler.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/ghbwvgage.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/gbivhtwtm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.bbcook.cn/Article/details/gqqazepub.sHtML

[G04] 定义方法
来源：http://www.m.share.yfazqb.com/Article/details/gigbfgpdl.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.tarul.cn/Article/details/glookdmxf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpncgyuei.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gqdbniljy.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gowppbaii.sHtML

Java: String greet() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gmqdixecd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gotwqpxxv.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fktsv.cn/Article/details/gxdqhzsjz.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gjctmchiv.sHtML

[G05] 继承
来源：http://www.share.tarul.cn/Article/details/gfmsksnqd.sHtML

Py:   class Admin(User): pass
来源：http://www.share.epnwcf.com/Article/details/gsotebgcu.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gozcarywa.sHtML

JS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gbqnssthu.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gtusxtzdw.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gkjbfessa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.tarul.cn/Article/details/gkbeggbni.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gurvurneb.sHtML

C#:   class Admin : User {}
来源：http://wap.epnwcf.com/Article/details/gnmfiwglf.sHtML

[G06] 重写方法
来源：http://www.m.share.tarul.cn/Article/details/gfyyopipa.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/gcvyqnzxf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gvslqlfet.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gyrvbfzwx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gxcetnbpz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gxjvnhxjb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.yfazqb.com/Article/details/gbypyibxf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gfkuazxvd.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.vehdjk.com/Article/details/gapnwiovp.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/gamncnuzs.sHtML

Py:   super().greet()
来源：http://wap.fktsv.cn/Article/details/gcgjvoiev.sHtML

PHP:  parent::greet();
来源：http://read.share.vehdjk.com/Article/details/gzmjmoaep.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gemmmgcan.sHtML

TS:   super.greet();
来源：http://m.share.vehdjk.com/Article/details/gjzumzefn.sHtML

Java: super.greet();
来源：http://wap.bbcook.cn/Article/details/gcetuoooe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.yfazqb.com/Article/details/gfsdkdoft.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/gkqhobhvs.sHtML

C#:   base.Greet();
来源：http://blog.vehdjk.com/Article/details/gzazdgumb.sHtML

[G08] 静态方法与属性
来源：http://www.share.epnwcf.com/Article/details/gwclcnllh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/gjeeqiueq.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gqtawmtld.sHtML

JS:   static f() {}
来源：http://wap.fktsv.cn/Article/details/golfvfkuw.sHtML

TS:   static f(): void {}
来源：http://mobile.tarul.cn/Article/details/gbnlfdmai.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/gjebafwst.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.vehdjk.com/Article/details/gsqomudoj.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/gdvedzkve.sHtML

C#:   public static void F() {}
来源：http://read.share.fktsv.cn/Article/details/gttsextdr.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.tarul.cn/Article/details/gzvfiaxet.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.tarul.cn/Article/details/gzuvzkhef.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.epnwcf.com/Article/details/gcmnkdfdx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fktsv.cn/Article/details/gwujotklo.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.epnwcf.com/Article/details/gnazqyonw.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtpiamrxr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.vehdjk.com/Article/details/gnfsdhcia.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.bbcook.cn/Article/details/grunkgtwt.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fktsv.cn/Article/details/gjxwrpfpu.sHtML

[G10] 访问控制
来源：http://blog.yfazqb.com/Article/details/gerfxstzj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.tarul.cn/Article/details/gphmvenxb.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gezeunubr.sHtML

JS:   #private 字段；其余公开
来源：http://3g.bbcook.cn/Article/details/golvhzkzj.sHtML

TS:   public / protected / private
来源：http://baike.fktsv.cn/Article/details/gmjhvmhvu.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/gulzqeisc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.tarul.cn/Article/details/gbjbjvihz.sHtML

Ruby: public / protected / private
来源：http://blog.tarul.cn/Article/details/gbwtfrfij.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gdlabebfx.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/gjvczyfzi.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/gantodaem.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gkabxvxwh.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gaeoawsmf.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/greakomag.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gfbplkxjj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gcngqnziq.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/goihzvkmz.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gusamzoad.sHtML

[G12] 对象转字符串
来源：http://read.share.tarul.cn/Article/details/gvyjojklv.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gdabgobrz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gpnybngcd.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gbsmtbwet.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/givcyvzns.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fktsv.cn/Article/details/gqfosaxqh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gohhhgxdb.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gdzqeghep.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fktsv.cn/Article/details/gzymaevop.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/gjpkpwulw.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fktsv.cn/Article/details/glojkxfco.sHtML

PHP:  $u instanceof User
来源：http://blog.tarul.cn/Article/details/gyfaynxyg.sHtML

JS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/grhdolbzd.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/ghcsyexcs.sHtML

Java: u instanceof User
来源：http://wap.bbcook.cn/Article/details/gswdhxngl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.tarul.cn/Article/details/gkkkzlvai.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/grtpzxiyn.sHtML

C#:   u is User
来源：http://read.share.bbcook.cn/Article/details/gapmdjtcf.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/gqjuvcfiz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.bbcook.cn/Article/details/gqjyylecm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.epnwcf.com/Article/details/gemubrlne.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.epnwcf.com/Article/details/glotyvixh.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.bbcook.cn/Article/details/ghxvzjztf.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.sjlbkw.cn/Article/details/glyaddirp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gabhfesql.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gzbielrzm.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.yfazqb.com/Article/details/ghtzquuxh.sHtML

[G15] 枚举
来源：http://www.blog.fktsv.cn/Article/details/gcbxtudvn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.epnwcf.com/Article/details/gdmcovmzx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/gmsvjesxx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/gvztfrasb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.epnwcf.com/Article/details/grifhbpxr.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.sjlbkw.cn/Article/details/gvwkujrkx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fktsv.cn/Article/details/gnmybttvi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.vehdjk.com/Article/details/gtjhechqy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gdzdtlhla.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.bbcook.cn/Article/details/gbkzslfpn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.yfazqb.com/Article/details/gymlbnaxj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.sjlbkw.cn/Article/details/gehguisdt.sHtML

JS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/gxkarsenz.sHtML

TS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gmjriuuho.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.sjlbkw.cn/Article/details/gwkckhpem.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.bbcook.cn/Article/details/gzbddmyuf.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gzgthfamo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gfzwgsqhu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkuisgoie.sHtML

H. 异常与错误处理
来源：http://baike.epnwcf.com/Article/details/gvyzmbrkj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gakzxjjoo.sHtML

[H01] try / catch 基础
来源：http://m.share.epnwcf.com/Article/details/gipazwbkm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.epnwcf.com/Article/details/gmlnleebj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fktsv.cn/Article/details/gvoixiwgk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gnpgaiqhg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/guxhjecst.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.sjlbkw.cn/Article/details/gjkabjhhq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.yfazqb.com/Article/details/glmdvtrmh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.sjlbkw.cn/Article/details/gyonmksex.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.bbcook.cn/Article/details/gccdzyeah.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.bbcook.cn/Article/details/gpmjmdsae.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.vehdjk.com/Article/details/glhluiubl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gcddpxmuq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gqnfkwjnh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gfycbiryt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/grcmelvjo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.sjlbkw.cn/Article/details/gieobgutl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fktsv.cn/Article/details/ghewdumcj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gtqgqkwwh.sHtML

[H03] 主动抛出异常
来源：http://read.share.epnwcf.com/Article/details/ghzdsktpx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fktsv.cn/Article/details/godqmfbgi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gbsafpyqu.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/gprxqoeav.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gogafiurr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/goxkxphpx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.sjlbkw.cn/Article/details/gbcesweip.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.bbcook.cn/Article/details/gpwkmzqaf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gmljysnrf.sHtML

[H04] 自定义异常类型
来源：http://www.blog.epnwcf.com/Article/details/gdspabztp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.sjlbkw.cn/Article/details/gjgbszlnb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gxiyzwyrk.sHtML

JS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gpykrarjb.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/giyxuncho.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gkuarafmz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.tarul.cn/Article/details/gzvhnietw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyndzyzl.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fktsv.cn/Article/details/gbqfnmbyg.sHtML

[H05] 捕获特定类型
来源：http://m.share.epnwcf.com/Article/details/gxllutaky.sHtML

Py:   except ValueError as e:
来源：http://3g.epnwcf.com/Article/details/gynplppsp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fktsv.cn/Article/details/gczchphpe.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gxuqnceyf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gveyllwbw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.yfazqb.com/Article/details/gmquevody.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.epnwcf.com/Article/details/gmmwyxkfw.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/geudjllrg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.tarul.cn/Article/details/gnvifrfju.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.tarul.cn/Article/details/grzqsivre.sHtML

Py:   value = d.get("k") or default
来源：http://3g.tarul.cn/Article/details/gefxkqskj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.bbcook.cn/Article/details/ghujgixpx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gxivgkxgs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gvdcdlswk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.tarul.cn/Article/details/gcmdckgyd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.vehdjk.com/Article/details/glflvegip.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.sjlbkw.cn/Article/details/gkuolxqhn.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.epnwcf.com/Article/details/gbydvcsuf.sHtML


<!-- 参考信息 -->