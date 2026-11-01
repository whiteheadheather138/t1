代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.bbcook.cn/Article/details/ghvhvofbe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gbpeapoag.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.sjlbkw.cn/Article/details/gdralypde.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.tarul.cn/Article/details/gwzjsehtf.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.bbcook.cn/Article/details/gdsgwcrlw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.epnwcf.com/Article/details/ghoqjgmdb.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.vehdjk.com/Article/details/gczuhjlee.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gdixrpabi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gijeptgks.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/ghkswahcr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.yfazqb.com/Article/details/gmhsrklfi.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.epnwcf.com/Article/details/gclkpefut.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gpjcfsngg.sHtML

[F06] 删除文件
来源：http://mobile.tarul.cn/Article/details/ghmneutiv.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/geewxshdb.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gukbxjkkt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gkajsxngf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gnyndjezg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gcqftjqgn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gceafxwgt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gzqeukehy.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.yfazqb.com/Article/details/gswubuyrj.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.sjlbkw.cn/Article/details/gbahrnrwu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/gzjeodxga.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.epnwcf.com/Article/details/gmjplldrr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gsreidbev.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gyoenyavy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.vehdjk.com/Article/details/gnkonlxgf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.sjlbkw.cn/Article/details/gepiefnoh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.sjlbkw.cn/Article/details/ghszbzsnp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gpkzbobuf.sHtML

[F08] 遍历目录
来源：http://www.share.yfazqb.com/Article/details/gufuaousx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fktsv.cn/Article/details/gbxlnfbtj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/gtnnnkmbf.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gpvdjzxsk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gccxucegp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gejkkmqkg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.tarul.cn/Article/details/graxotzuf.sHtML

Ruby: Dir.children("dir")
来源：http://baike.epnwcf.com/Article/details/gzxiyxsbx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/gyccoochb.sHtML

[F09] 获取文件大小
来源：http://read.share.sjlbkw.cn/Article/details/gwhsekjpi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gtnfrrzqp.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/guangwmim.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gldfqzhhq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gmuadsvie.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gohbtgjbm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.bbcook.cn/Article/details/grrakowww.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gbigtejnr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.epnwcf.com/Article/details/gyvwfnfcp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.epnwcf.com/Article/details/gdkiuxcyv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gkyiedecb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/gfxuzqcmr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gwxfscqwp.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/ggqlqjibp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.vehdjk.com/Article/details/gilqmjzmw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gitpyucjq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gicrqhaip.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/giaaauknk.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/gedvyhrsz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ghyarkkzx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.tarul.cn/Article/details/gprwqqghv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gefyvdxzo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gakoyxeeb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.vehdjk.com/Article/details/gcvppnssk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gchfhyuox.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gjbtptqhm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.epnwcf.com/Article/details/ghregeqam.sHtML

[F12] CSV 读写
来源：http://baike.sjlbkw.cn/Article/details/gphbscsfr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fktsv.cn/Article/details/guaknczyq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.sjlbkw.cn/Article/details/gqotdjrwl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.yfazqb.com/Article/details/gfgczlpnj.sHtML

TS:   // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gyhjuktmu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.vehdjk.com/Article/details/ggbyrstgu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fktsv.cn/Article/details/ggjvfxbzk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.epnwcf.com/Article/details/gfeuyicha.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.epnwcf.com/Article/details/geqcwrimr.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfsddzbve.sHtML

G. 面向对象
来源：http://www.m.share.vehdjk.com/Article/details/grdquoaxr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmumjqgxu.sHtML

[G01] 定义类
来源：http://www.share.vehdjk.com/Article/details/geirgpzow.sHtML

Py:   class User: pass
来源：http://m.share.vehdjk.com/Article/details/gdqyfqumm.sHtML

PHP:  class User {}
来源：http://baike.yfazqb.com/Article/details/gtonbgxds.sHtML

JS:   class User {}
来源：http://www.blog.tarul.cn/Article/details/govnaqbjx.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.sjlbkw.cn/Article/details/gwghaxfvk.sHtML

Java: class User {}
来源：http://blog.bbcook.cn/Article/details/gqswckqkx.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/gjirepkik.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/guuhwdnxf.sHtML

C#:   class User {}
来源：http://blog.bbcook.cn/Article/details/gpcquppll.sHtML

[G02] 构造函数
来源：http://3g.sjlbkw.cn/Article/details/gbdwnicoa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.yfazqb.com/Article/details/gpqmnsuvn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gofvwrudu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/ggppvncbi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.yfazqb.com/Article/details/gndvvolio.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gihgoxtqk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.vehdjk.com/Article/details/ghorhuwjt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.bbcook.cn/Article/details/gjjhxvtrb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.bbcook.cn/Article/details/ghiybetcf.sHtML

[G03] 实例属性
来源：http://wap.yfazqb.com/Article/details/gfkldnhln.sHtML

Py:   self.name = "x"
来源：http://m.share.epnwcf.com/Article/details/ggqcvsesa.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gbheytbxp.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gaeqbumpe.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/grdlclpqq.sHtML

Java: private String name;
来源：http://www.m.share.yfazqb.com/Article/details/gwzbqycli.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.vehdjk.com/Article/details/gytnlaeoe.sHtML

Ruby: @name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/givgsdhmi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.epnwcf.com/Article/details/gxommkuya.sHtML

[G04] 定义方法
来源：http://mobile.yfazqb.com/Article/details/gbbojlrgk.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/gzifeduon.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gsncqsgui.sHtML

JS:   greet() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gievyyvkk.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gxzachwcg.sHtML

Java: String greet() { return name; }
来源：http://blog.bbcook.cn/Article/details/ggzeowvlk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gtpoipgxf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.vehdjk.com/Article/details/gcdbkoqhf.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/gjwdrwnfm.sHtML

[G05] 继承
来源：http://www.blog.vehdjk.com/Article/details/gkqtjnfop.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/gksrdknvd.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gagvhwsjq.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gzanpijkh.sHtML

TS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/geaklvfqb.sHtML

Java: class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gtaqecswi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.tarul.cn/Article/details/gnvfhekgh.sHtML

Ruby: class Admin < User; end
来源：http://blog.bbcook.cn/Article/details/geyfddnpi.sHtML

C#:   class Admin : User {}
来源：http://mobile.fktsv.cn/Article/details/gaiqbrokd.sHtML

[G06] 重写方法
来源：http://mobile.sjlbkw.cn/Article/details/gkvgugann.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.bbcook.cn/Article/details/gblezrknj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gngswmsrv.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/glgyhrewp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/glhcszhar.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gewzokyiu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.epnwcf.com/Article/details/gfgnvzibf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/gjkpdfmtr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.bbcook.cn/Article/details/gmerdljhe.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/glxsxvloi.sHtML

Py:   super().greet()
来源：http://www.blog.epnwcf.com/Article/details/gqmulrdrc.sHtML

PHP:  parent::greet();
来源：http://mobile.fktsv.cn/Article/details/guimszkvh.sHtML

JS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/gwcgcfjyd.sHtML

TS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gknxqlljs.sHtML

Java: super.greet();
来源：http://blog.tarul.cn/Article/details/guskzqtvw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.sjlbkw.cn/Article/details/geshetvwx.sHtML

Ruby: super
来源：http://mobile.tarul.cn/Article/details/gmbviolyr.sHtML

C#:   base.Greet();
来源：http://3g.yfazqb.com/Article/details/guvowpbsr.sHtML

[G08] 静态方法与属性
来源：http://www.share.tarul.cn/Article/details/gwxabaakh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fktsv.cn/Article/details/gxmqiehdg.sHtML

PHP:  public static function f() {}
来源：http://www.blog.vehdjk.com/Article/details/gxpujwrtu.sHtML

JS:   static f() {}
来源：http://baike.sjlbkw.cn/Article/details/gvconxbvd.sHtML

TS:   static f(): void {}
来源：http://www.blog.fktsv.cn/Article/details/guoclxrds.sHtML

Java: static void f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gugopwzbo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.vehdjk.com/Article/details/gqpbgiutr.sHtML

Ruby: def self.f; end
来源：http://m.share.epnwcf.com/Article/details/gkxxkxkvj.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/gtnigxasq.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gjsltdavw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/gcrekunuu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.epnwcf.com/Article/details/gnzxbhhrj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/ggdqvleaq.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.vehdjk.com/Article/details/guktuxkzf.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gogiroaky.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.tarul.cn/Article/details/gfzflwbkc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.bbcook.cn/Article/details/glmxhbqut.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/gvsdkevvh.sHtML

[G10] 访问控制
来源：http://wap.tarul.cn/Article/details/gjxggpehf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/gwvoozitn.sHtML

PHP:  public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gilgaurps.sHtML

JS:   #private 字段；其余公开
来源：http://3g.vehdjk.com/Article/details/glhzdnucs.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gyozbegnn.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.tarul.cn/Article/details/gtfkiglmq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/guqvkwszm.sHtML

Ruby: public / protected / private
来源：http://mobile.tarul.cn/Article/details/gzxvyhkdw.sHtML

C#:   public / protected / private / internal
来源：http://3g.bbcook.cn/Article/details/gjfcrspqw.sHtML

[G11] getter / setter
来源：http://www.share.fktsv.cn/Article/details/gnhfuhihn.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.vehdjk.com/Article/details/gkqcxunct.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gqvqdzchw.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/gjcuqbviy.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gxsnrocmk.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/guwbvoqvy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gijtveopb.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/gqikwimjy.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.yfazqb.com/Article/details/gujznudyc.sHtML

[G12] 对象转字符串
来源：http://blog.tarul.cn/Article/details/gwynwusbi.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gimucdmua.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gwmoxgxbn.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gmeldalhe.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gthhztgef.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gmaodidil.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gmtzfgukf.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.bbcook.cn/Article/details/gxyabnanc.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/gqfvjfuho.sHtML

[G13] 判断对象类型
来源：http://www.share.tarul.cn/Article/details/gjwtzzyop.sHtML

Py:   isinstance(u, User)
来源：http://read.share.yfazqb.com/Article/details/gxdprboax.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gpzcqptju.sHtML

JS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gcziqybkz.sHtML

TS:   u instanceof User
来源：http://wap.tarul.cn/Article/details/gaxaphcdx.sHtML

Java: u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gkhybgewf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.sjlbkw.cn/Article/details/gmmgigwou.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.vehdjk.com/Article/details/gbyobjaoq.sHtML

C#:   u is User
来源：http://www.share.yfazqb.com/Article/details/ghlylpgeb.sHtML

[G14] 数据类 / record
来源：http://blog.fktsv.cn/Article/details/gkgeoclta.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.bbcook.cn/Article/details/goguvqiap.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.sjlbkw.cn/Article/details/gysnmrvux.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.sjlbkw.cn/Article/details/gebmvclin.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.vehdjk.com/Article/details/gbysohjdo.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fktsv.cn/Article/details/grwfqdnxp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.bbcook.cn/Article/details/gyikmzkqf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fktsv.cn/Article/details/gnmzcgrib.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.bbcook.cn/Article/details/gxxejcntu.sHtML

[G15] 枚举
来源：http://www.share.epnwcf.com/Article/details/gmzpchmyc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.vehdjk.com/Article/details/gpoewwtrz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.vehdjk.com/Article/details/gkpflmjju.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gewowirae.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.epnwcf.com/Article/details/gfpgnuuom.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/gymzpiopa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.bbcook.cn/Article/details/gswktyqbx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fktsv.cn/Article/details/grvymxkdm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gkufybilx.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/gidanqsyi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.bbcook.cn/Article/details/gobdyafwy.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.sjlbkw.cn/Article/details/gdqgekvfy.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gvizbzaxl.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gciukajvq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.epnwcf.com/Article/details/ggvbfvvyc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.bbcook.cn/Article/details/ggcrmzgya.sHtML

Ruby: obj.instance_variables
来源：http://baike.vehdjk.com/Article/details/gudmfjwvv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/glgobqlif.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gmkueljup.sHtML

H. 异常与错误处理
来源：http://baike.yfazqb.com/Article/details/giuzxjipl.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvwfkfhcz.sHtML

[H01] try / catch 基础
来源：http://read.share.sjlbkw.cn/Article/details/gbcwcwfcz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.tarul.cn/Article/details/gmmacycvf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.vehdjk.com/Article/details/gnhjrnhrx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/ghhvtipio.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gkfawwrdk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.yfazqb.com/Article/details/ggfyfignd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.yfazqb.com/Article/details/gbqnjyvib.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.epnwcf.com/Article/details/gtubimhzp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.tarul.cn/Article/details/grevrpzzz.sHtML

[H02] finally / ensure 收尾
来源：http://3g.epnwcf.com/Article/details/gltkybxwt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.vehdjk.com/Article/details/grzufygmp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gbldjrqtd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gmxxcgafv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gnyblydrc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gxyfxegld.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.tarul.cn/Article/details/gzrhkaugt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.bbcook.cn/Article/details/gjkatobuh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gwgigftrw.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/ghfgcsfyb.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.bbcook.cn/Article/details/gydffmkrj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gcokiiepz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gmvfhigyc.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gpykcqmrc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gtatfhxpc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.vehdjk.com/Article/details/ggqxjbwfs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.epnwcf.com/Article/details/grciwfllj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gzquljqhg.sHtML

[H04] 自定义异常类型
来源：http://m.share.yfazqb.com/Article/details/gdjsfolqo.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.vehdjk.com/Article/details/grmtrkrln.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvolhslk.sHtML

JS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/gmtdhmqfk.sHtML

TS:   class MyError extends Error {}
来源：http://baike.epnwcf.com/Article/details/gykvzqpqx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/gzanpdwhl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.yfazqb.com/Article/details/gjzuyifpt.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gdqrjekle.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.yfazqb.com/Article/details/gxthhnkrc.sHtML

[H05] 捕获特定类型
来源：http://wap.epnwcf.com/Article/details/gxdvmmrcs.sHtML

Py:   except ValueError as e:
来源：http://blog.yfazqb.com/Article/details/gjpkqtgig.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/gpvklaqbf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gwoqibzpr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/golpoqjdz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.vehdjk.com/Article/details/grplfomrm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.bbcook.cn/Article/details/gwnnuutia.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.vehdjk.com/Article/details/gzqqcgoxw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.tarul.cn/Article/details/grgkhwlot.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/gwjailvhc.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.tarul.cn/Article/details/ggxtojoay.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.tarul.cn/Article/details/ghjhdmfvm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gypkqbfuj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gnlibkdfu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fktsv.cn/Article/details/gfozlaftf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.yfazqb.com/Article/details/glohpujvf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.epnwcf.com/Article/details/gbqypckua.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gltbzltjy.sHtML

[H07] 断言
来源：http://mobile.tarul.cn/Article/details/gydltzxmv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.sjlbkw.cn/Article/details/ghrrxixie.sHtML

PHP:  assert($x > 0);
来源：http://blog.yfazqb.com/Article/details/guxqsxxrw.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/grsnlyrcf.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gjevyefxd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.epnwcf.com/Article/details/gjilbxpay.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.bbcook.cn/Article/details/glkpypbqx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.tarul.cn/Article/details/gqwcyayoa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gqpbgsuhg.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.bbcook.cn/Article/details/gcrqjddwr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.epnwcf.com/Article/details/gehcmxhfp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fktsv.cn/Article/details/grnamybbo.sHtML

JS:   e.message;  e.stack
来源：http://baike.sjlbkw.cn/Article/details/grxhtxpkq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.epnwcf.com/Article/details/gjamvrwfi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.yfazqb.com/Article/details/gtgyjesie.sHtML

Go:   err.Error()
来源：http://read.share.epnwcf.com/Article/details/gdqtlqqtm.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.epnwcf.com/Article/details/goxiebijy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.bbcook.cn/Article/details/gmbkgqpbw.sHtML

[H09] 带错误码的异常
来源：http://3g.epnwcf.com/Article/details/gzzivguig.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.bbcook.cn/Article/details/ggboireqy.sHtML


<!-- 参考信息 -->