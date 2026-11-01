代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gkpkcnvfo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/goounblcx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/goedrslxt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gpdjgsfbk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.sjlbkw.cn/Article/details/gkzcwmjlp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fktsv.cn/Article/details/gilimelag.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/gkwcvuaai.sHtML

[F04] 追加写入文件
来源：http://3g.epnwcf.com/Article/details/gbjcqtiec.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gblcjdtmm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.yfazqb.com/Article/details/glwynnivu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gelbqihlj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/ggxltuyye.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.epnwcf.com/Article/details/gumiyegmj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/ghzmlkbsg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.vehdjk.com/Article/details/givljwbcr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/gugeeybop.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.yfazqb.com/Article/details/gemdmesyv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.bbcook.cn/Article/details/gdyvhwtho.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gqekcqjqg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gowlkcpey.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gwozymyti.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gmbzxkvyc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.epnwcf.com/Article/details/gezzetfed.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.yfazqb.com/Article/details/gylwpsqwe.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.tarul.cn/Article/details/ghpcwlfyj.sHtML

[F06] 删除文件
来源：http://blog.sjlbkw.cn/Article/details/gkeubdbgt.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gprscgdpj.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gjgtvfktt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gijjfhhwv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gudqdipgw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gghdhdfyw.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/geddcaesb.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.vehdjk.com/Article/details/gsypnanug.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/guowmzwrq.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.bbcook.cn/Article/details/geqbxstwg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/gcasriqvh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.epnwcf.com/Article/details/gbfmvdqgs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gcyvhdbms.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gskhzztbh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fktsv.cn/Article/details/gawabgtft.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.vehdjk.com/Article/details/gjrolldbl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/ghkxjbaqz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.vehdjk.com/Article/details/gsemlgamo.sHtML

[F08] 遍历目录
来源：http://mobile.vehdjk.com/Article/details/gqmysjbxj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.bbcook.cn/Article/details/gtmniektw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fktsv.cn/Article/details/gixkmzoge.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/ggkappiph.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gathhocxs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gjqyzabnn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gfnmandow.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.bbcook.cn/Article/details/goqglohub.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/gefdwturb.sHtML

[F09] 获取文件大小
来源：http://read.share.bbcook.cn/Article/details/gzfeuxgmt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gjbvxgsws.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gcjfgjqrf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gfoaujcgd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/grhmclofk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gyrouqpii.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/gydgnjisz.sHtML

Ruby: File.size("a.txt")
来源：http://baike.epnwcf.com/Article/details/gwmauaius.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.bbcook.cn/Article/details/gsvjcovoq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fktsv.cn/Article/details/gsfvvugzq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gaudvfhwd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.epnwcf.com/Article/details/givnecusf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/goaxjfmqf.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gblltzwei.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.epnwcf.com/Article/details/gtdccbcan.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gmnhxhygu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gfpgoyfde.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gahrqdglb.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/goxaofjha.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/guhfdscvl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fktsv.cn/Article/details/gnueepcxk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gpekgosbz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gpbnmfsti.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gdueysthw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gfrdkqyfa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gdyaronir.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/gbqojqupr.sHtML

[F12] CSV 读写
来源：http://3g.fktsv.cn/Article/details/gbgvsxwku.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.yfazqb.com/Article/details/gznzaypho.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.yfazqb.com/Article/details/giiqyvzyq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.bbcook.cn/Article/details/gsdtxotap.sHtML

TS:   // 同上
来源：http://3g.bbcook.cn/Article/details/gkytjritc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.bbcook.cn/Article/details/glvexhurs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.tarul.cn/Article/details/gqzuwgmgc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fktsv.cn/Article/details/gvggmiyce.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fktsv.cn/Article/details/gotpuvtoy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwdqxvdau.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/gdnrthoee.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gmqaqpgyp.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/gkufmvdgo.sHtML

Py:   class User: pass
来源：http://mobile.sjlbkw.cn/Article/details/gakcfeqpg.sHtML

PHP:  class User {}
来源：http://baike.sjlbkw.cn/Article/details/giqnbkhpf.sHtML

JS:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gghnwikse.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.vehdjk.com/Article/details/gyomhxdtv.sHtML

Java: class User {}
来源：http://read.share.tarul.cn/Article/details/giedammfu.sHtML

Go:   type User struct { Name string }
来源：http://m.share.sjlbkw.cn/Article/details/gnwweltzu.sHtML

Ruby: class User; end
来源：http://mobile.epnwcf.com/Article/details/gvrflvsnx.sHtML

C#:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gntcoxlno.sHtML

[G02] 构造函数
来源：http://blog.tarul.cn/Article/details/gyahktiob.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.vehdjk.com/Article/details/gmlkzqyql.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.tarul.cn/Article/details/gtqpphofi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/gmhazltrd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.sjlbkw.cn/Article/details/gbgnfbfeo.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/grmmkndhv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.epnwcf.com/Article/details/gyokapnaw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/glmkxgobr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.tarul.cn/Article/details/gkhvrdavm.sHtML

[G03] 实例属性
来源：http://wap.tarul.cn/Article/details/gedkambdy.sHtML

Py:   self.name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gcevskemp.sHtML

PHP:  public string $name = "x";
来源：http://read.share.tarul.cn/Article/details/gakrhxgsk.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/goqdguijx.sHtML

TS:   name: string = "x";
来源：http://mobile.yfazqb.com/Article/details/gjptyzoly.sHtML

Java: private String name;
来源：http://www.blog.fktsv.cn/Article/details/gmvbvpgxw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.tarul.cn/Article/details/gguvjsbre.sHtML

Ruby: @name = "x"
来源：http://3g.tarul.cn/Article/details/gopdmqefg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fktsv.cn/Article/details/gjoloeccq.sHtML

[G04] 定义方法
来源：http://blog.tarul.cn/Article/details/gsircjpdd.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gqicokjxo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gkqsnznzh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gpveoqmyn.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gasjrlqzv.sHtML

Java: String greet() { return name; }
来源：http://blog.yfazqb.com/Article/details/gajsogxsn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gwjvdzzai.sHtML

Ruby: def greet; @name; end
来源：http://blog.epnwcf.com/Article/details/gmguheych.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fktsv.cn/Article/details/ggepsvlsf.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gtrliaryt.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fktsv.cn/Article/details/gtzdtimuo.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gipcwfyud.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gyvhjlmhe.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/ggzfyyeuj.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/govvzoxnm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fktsv.cn/Article/details/gypcrtzqw.sHtML

Ruby: class Admin < User; end
来源：http://m.share.tarul.cn/Article/details/gunmsfrcu.sHtML

C#:   class Admin : User {}
来源：http://www.share.bbcook.cn/Article/details/gapxdpcyr.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/gysmgnhtu.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.vehdjk.com/Article/details/gxuhwfcja.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gfnmbqybr.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/ggjbohuqb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gsaiiqkmw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gfuhafgrw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.bbcook.cn/Article/details/ghaajdxmg.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.epnwcf.com/Article/details/gyjrcjdnp.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.tarul.cn/Article/details/gbzoqskhk.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/glwlgrtpv.sHtML

Py:   super().greet()
来源：http://wap.fktsv.cn/Article/details/gsmvbccrz.sHtML

PHP:  parent::greet();
来源：http://www.share.epnwcf.com/Article/details/gwmsllzxt.sHtML

JS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/gkvgcrmla.sHtML

TS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gmqjrvszo.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/gkcububxc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gvhwnmvcy.sHtML

Ruby: super
来源：http://wap.sjlbkw.cn/Article/details/gkauwqhsp.sHtML

C#:   base.Greet();
来源：http://m.share.tarul.cn/Article/details/gfsyojtwi.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gczvgdzgo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fktsv.cn/Article/details/gvyqhfvkm.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gtocqtlau.sHtML

JS:   static f() {}
来源：http://baike.yfazqb.com/Article/details/gaknlmpdu.sHtML

TS:   static f(): void {}
来源：http://baike.sjlbkw.cn/Article/details/gyoduwzkt.sHtML

Java: static void f() {}
来源：http://baike.vehdjk.com/Article/details/gskfugllc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fktsv.cn/Article/details/gklaqaked.sHtML

Ruby: def self.f; end
来源：http://baike.tarul.cn/Article/details/gpxucwpye.sHtML

C#:   public static void F() {}
来源：http://baike.fktsv.cn/Article/details/gewvsujsw.sHtML

[G09] 接口 / 抽象类
来源：http://baike.bbcook.cn/Article/details/ghsdcelsr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gmgblslvx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.vehdjk.com/Article/details/gucyfmoxx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/gmgpsxdly.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/gjwakukbw.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.tarul.cn/Article/details/gaqgkgzwj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.bbcook.cn/Article/details/gowuhxbfi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.vehdjk.com/Article/details/glzhfthty.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.tarul.cn/Article/details/gxyjjarvl.sHtML

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/gtvlqengh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.yfazqb.com/Article/details/gixjxvjgc.sHtML

PHP:  public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gwygcnioq.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gswcctvub.sHtML

TS:   public / protected / private
来源：http://wap.yfazqb.com/Article/details/gvyqpeeld.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/gphcrztzt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.tarul.cn/Article/details/gvpznxwfk.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/ggbdenckx.sHtML

C#:   public / protected / private / internal
来源：http://wap.fktsv.cn/Article/details/gwvhutbwq.sHtML

[G11] getter / setter
来源：http://www.m.share.epnwcf.com/Article/details/gwzmqnqqa.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.bbcook.cn/Article/details/gwckscbpc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gcsncrfzq.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gcisqbxnj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/gruaqwhzo.sHtML

Java: public String getName() { return name; }
来源：http://baike.tarul.cn/Article/details/gpikohrhq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/ghfqkbkmg.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gsvxythtv.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.sjlbkw.cn/Article/details/gtrqiicky.sHtML

[G12] 对象转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gjbnbugfk.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/glscfyzgg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gfisutscg.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gkfnzawyw.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gdqmfdppm.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.epnwcf.com/Article/details/gopsmcvew.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gnomzjwqn.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.tarul.cn/Article/details/gfocjmche.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/guykvtwcv.sHtML

[G13] 判断对象类型
来源：http://blog.yfazqb.com/Article/details/gkzsznvky.sHtML

Py:   isinstance(u, User)
来源：http://www.share.vehdjk.com/Article/details/gskzzgywz.sHtML

PHP:  $u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gbblorfdg.sHtML

JS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/ggskwamkl.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/ghzpoatlq.sHtML

Java: u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gfbiaorzw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.yfazqb.com/Article/details/ghqhgdzkm.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.epnwcf.com/Article/details/gvxanwiig.sHtML

C#:   u is User
来源：http://m.share.sjlbkw.cn/Article/details/gnrgpfrxq.sHtML

[G14] 数据类 / record
来源：http://www.blog.sjlbkw.cn/Article/details/gajmulpxu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/geofwjwib.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.epnwcf.com/Article/details/goskpihmf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.sjlbkw.cn/Article/details/gesqaetym.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/gcykzwdzv.sHtML

Java: record User(String name, int age) {}
来源：http://baike.bbcook.cn/Article/details/gspddshhu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.sjlbkw.cn/Article/details/gzqbejdpc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.epnwcf.com/Article/details/gjucbkswm.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.tarul.cn/Article/details/gkklvmpux.sHtML

[G15] 枚举
来源：http://mobile.sjlbkw.cn/Article/details/gvhxwvtpi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.vehdjk.com/Article/details/ghadfzwul.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.bbcook.cn/Article/details/gazdjmnnt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fktsv.cn/Article/details/gsixnwpcc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/guxjzdmwt.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.sjlbkw.cn/Article/details/gpietsjjo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fktsv.cn/Article/details/gikwfxuco.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.bbcook.cn/Article/details/gozirzour.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gzfhxdbps.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.yfazqb.com/Article/details/gonywzuys.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.yfazqb.com/Article/details/gvfwumswx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fktsv.cn/Article/details/gvuznajzm.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gphlljtcb.sHtML

TS:   Object.entries(obj)
来源：http://read.share.sjlbkw.cn/Article/details/groslpvso.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.bbcook.cn/Article/details/gprqtjylu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/gxqzdyqhc.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/godzauvog.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/ghkhbvzxs.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gvrridzgm.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gdaemmeye.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gaebmgxtv.sHtML

[H01] try / catch 基础
来源：http://wap.bbcook.cn/Article/details/guokbkyqe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.epnwcf.com/Article/details/gmwuewosg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.vehdjk.com/Article/details/gfikvxpjr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gzhpgmafl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gyuynylom.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.tarul.cn/Article/details/gbawctcma.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.yfazqb.com/Article/details/gephljmbn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.bbcook.cn/Article/details/glqjokrtk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.yfazqb.com/Article/details/gdotnwhtb.sHtML

[H02] finally / ensure 收尾
来源：http://blog.epnwcf.com/Article/details/guagopvwo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.sjlbkw.cn/Article/details/gbdryflmr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gwtgbnhsz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gzxypifvt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gyemmungt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/ggrkpnuqp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.tarul.cn/Article/details/gqgjsoiag.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.yfazqb.com/Article/details/goxquaswa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/grmxfyhnh.sHtML

[H03] 主动抛出异常
来源：http://wap.epnwcf.com/Article/details/gbfcioqxl.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/gvriqxqyq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/ggwzhkrfr.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gnxzsobep.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gjkiccgmk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/grslvasrt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.yfazqb.com/Article/details/gwleedqor.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.tarul.cn/Article/details/ghscpbois.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gioqfbmtq.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/gvxwpncdw.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.sjlbkw.cn/Article/details/gdqouqhia.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/govcpglim.sHtML

JS:   class MyError extends Error {}
来源：http://baike.tarul.cn/Article/details/gsklcvzoj.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/grqhdnazt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gvacezpye.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.epnwcf.com/Article/details/graprbjxq.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.bbcook.cn/Article/details/gpwxykezs.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/gfpmuwbnz.sHtML

[H05] 捕获特定类型
来源：http://3g.sjlbkw.cn/Article/details/gdenzsosa.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.bbcook.cn/Article/details/ghbljikic.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.tarul.cn/Article/details/gjdqcrpcc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/grjpvzirx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/gfkcashfe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fktsv.cn/Article/details/goswhihdw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.epnwcf.com/Article/details/gpbulatot.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.vehdjk.com/Article/details/gsthxluse.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.yfazqb.com/Article/details/gcywkoeks.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.epnwcf.com/Article/details/gfdnqvwfx.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.bbcook.cn/Article/details/goawncyil.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fktsv.cn/Article/details/gdlmfzhcq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gcbmshpxh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.sjlbkw.cn/Article/details/ggnaotxcb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcpfciuj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.tarul.cn/Article/details/gdecgkgpz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.yfazqb.com/Article/details/gsnkznzpg.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.bbcook.cn/Article/details/gfybqizxr.sHtML

[H07] 断言
来源：http://baike.epnwcf.com/Article/details/gxgecufso.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.yfazqb.com/Article/details/gnheirdma.sHtML

PHP:  assert($x > 0);
来源：http://blog.tarul.cn/Article/details/gpsfzsdmj.sHtML

JS:   console.assert(x > 0);
来源：http://wap.epnwcf.com/Article/details/gghulbktr.sHtML

TS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/goeyonezx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.tarul.cn/Article/details/gscvndgdk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.epnwcf.com/Article/details/gpmogxckr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.epnwcf.com/Article/details/gzantuefg.sHtML


<!-- 参考信息 -->