代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/gxaayfztb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.epnwcf.com/Article/details/gzuxyuieq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gvnwxyecu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gfkajofsf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fktsv.cn/Article/details/gtkxsuhkc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.epnwcf.com/Article/details/gbbeegxkp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.sjlbkw.cn/Article/details/gdjgvcoma.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.epnwcf.com/Article/details/grrrbiizx.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.yfazqb.com/Article/details/gjykxiprk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.bbcook.cn/Article/details/gwokstydr.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fktsv.cn/Article/details/gwiwhzwzz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gzdehbzoo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gvtubhyrz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gsgejvowr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.sjlbkw.cn/Article/details/gehruowej.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/ghzkeunvp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gsncfyilf.sHtML

[F06] 删除文件
来源：http://wap.fktsv.cn/Article/details/gpcmsfjli.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gosgwroqm.sHtML

PHP:  unlink("a.txt");
来源：http://blog.yfazqb.com/Article/details/ghpvbfyhs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/ghymnmfqm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gjxcdgrlg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gqakjxfdz.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gxcczlvss.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.tarul.cn/Article/details/gcpekzdbp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gphjkvrbp.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/gdjtqibtm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnmgqtsu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.vehdjk.com/Article/details/gvykhkywl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gyyhosqma.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gajquwtdm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/gitfuuiqr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.bbcook.cn/Article/details/gnkrtjqkj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.vehdjk.com/Article/details/gvjfzezvo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.sjlbkw.cn/Article/details/ghosfhctv.sHtML

[F08] 遍历目录
来源：http://3g.bbcook.cn/Article/details/gyjxsjuev.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gwcqxwopb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.epnwcf.com/Article/details/gmwiyugqk.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gdivnqbom.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gtayapcpm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/ggyvmptuy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fktsv.cn/Article/details/gbaibcijo.sHtML

Ruby: Dir.children("dir")
来源：http://blog.vehdjk.com/Article/details/gvonsjnig.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.sjlbkw.cn/Article/details/glfrbyjuo.sHtML

[F09] 获取文件大小
来源：http://wap.yfazqb.com/Article/details/gqwjzgxdb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gegiezyap.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gldcrpovo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/guunchlsb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gdydcoauv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gjfhuqenk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/gprgkpmrz.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gjlqsiltq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.bbcook.cn/Article/details/ggifqcjxv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fktsv.cn/Article/details/gvzspzwzi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/govvsszto.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.yfazqb.com/Article/details/gavszptzv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gjjehsjgl.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.tarul.cn/Article/details/gnqxziycm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/geytbrdsp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gsnoqeoqm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gxhtpjijy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gierbypio.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/grbixcdlq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gbuyjmjyi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.epnwcf.com/Article/details/grmjlqcsd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gbjgharun.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gytjbfqwe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzksjvzwl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.sjlbkw.cn/Article/details/gdwbgpiye.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gamgpoben.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.bbcook.cn/Article/details/gzxuhcmjn.sHtML

[F12] CSV 读写
来源：http://wap.bbcook.cn/Article/details/gkfzoquzk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/gzoatzdzj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.vehdjk.com/Article/details/gldekcmua.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.tarul.cn/Article/details/gdpznsxdf.sHtML

TS:   // 同上
来源：http://www.m.share.tarul.cn/Article/details/giamekqrc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gkjbcivhe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.bbcook.cn/Article/details/gsvfusesj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/gwmmvbnwv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.tarul.cn/Article/details/gtcdwhvpf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gndhflljl.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/gyneotwem.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkscrnzbl.sHtML

[G01] 定义类
来源：http://blog.yfazqb.com/Article/details/gjlzzpeah.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gysezuzov.sHtML

PHP:  class User {}
来源：http://wap.bbcook.cn/Article/details/gltkzhbhc.sHtML

JS:   class User {}
来源：http://mobile.tarul.cn/Article/details/gktylevcz.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.sjlbkw.cn/Article/details/guuxdpthh.sHtML

Java: class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gbhgdnmdd.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/guvaaupym.sHtML

Ruby: class User; end
来源：http://blog.vehdjk.com/Article/details/gemvlogvb.sHtML

C#:   class User {}
来源：http://3g.yfazqb.com/Article/details/gibdlvtis.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gfwmaudnz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.epnwcf.com/Article/details/ghyhcbywz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/ghsetmwdi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gflwqrhwt.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.sjlbkw.cn/Article/details/gnjjjhbmx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/goomiojlk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.bbcook.cn/Article/details/gaejpcvby.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fktsv.cn/Article/details/gujibpkfo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/gwxmzkftc.sHtML

[G03] 实例属性
来源：http://m.share.tarul.cn/Article/details/gdfynyxxt.sHtML

Py:   self.name = "x"
来源：http://3g.bbcook.cn/Article/details/gegsjkatz.sHtML

PHP:  public string $name = "x";
来源：http://3g.bbcook.cn/Article/details/gwslnnsim.sHtML

JS:   this.name = "x";
来源：http://wap.epnwcf.com/Article/details/gboazmnxv.sHtML

TS:   name: string = "x";
来源：http://wap.tarul.cn/Article/details/gzqkvrsfv.sHtML

Java: private String name;
来源：http://www.m.share.vehdjk.com/Article/details/gcpxoucaq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/gwwinfaxg.sHtML

Ruby: @name = "x"
来源：http://wap.bbcook.cn/Article/details/guvanhgoe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.bbcook.cn/Article/details/gqztwkgem.sHtML

[G04] 定义方法
来源：http://m.share.sjlbkw.cn/Article/details/gxdpevsri.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gbjvuffnj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gbgbseywg.sHtML

JS:   greet() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/ggxodxaum.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gbrjxqhse.sHtML

Java: String greet() { return name; }
来源：http://blog.yfazqb.com/Article/details/gpkwpxuzn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gcxgrrxha.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gexonewqj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gmafwdidl.sHtML

[G05] 继承
来源：http://wap.epnwcf.com/Article/details/gamwxfjcj.sHtML

Py:   class Admin(User): pass
来源：http://m.share.tarul.cn/Article/details/gjyvorehb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/glhosvwjw.sHtML

JS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gumlqybrk.sHtML

TS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gxbxhbszf.sHtML

Java: class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/graviqmhw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.sjlbkw.cn/Article/details/gfuakohpp.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/grfiphpth.sHtML

C#:   class Admin : User {}
来源：http://3g.vehdjk.com/Article/details/gnznfayfo.sHtML

[G06] 重写方法
来源：http://mobile.vehdjk.com/Article/details/gdqxaeibq.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/gycfvwnot.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gfmjaadbc.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/giktitbtp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/glutmuuht.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gbnnfrldw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.tarul.cn/Article/details/gysufybbw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/gezeonaon.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.epnwcf.com/Article/details/gxpnulrna.sHtML

[G07] 调用父类方法
来源：http://3g.fktsv.cn/Article/details/gghpsysog.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/gelhbiwac.sHtML

PHP:  parent::greet();
来源：http://read.share.fktsv.cn/Article/details/geszdkjrz.sHtML

JS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gfhhyaole.sHtML

TS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gtctwkeuy.sHtML

Java: super.greet();
来源：http://m.share.fktsv.cn/Article/details/gedslalmm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.yfazqb.com/Article/details/gsjhahzvh.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/goqjgswyn.sHtML

C#:   base.Greet();
来源：http://3g.vehdjk.com/Article/details/goiaaaswd.sHtML

[G08] 静态方法与属性
来源：http://www.share.fktsv.cn/Article/details/gfswnmizb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/gurjnrwvf.sHtML

PHP:  public static function f() {}
来源：http://baike.bbcook.cn/Article/details/gsxlcgblz.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/giodxnxfk.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/gbuzafyqg.sHtML

Java: static void f() {}
来源：http://m.share.fktsv.cn/Article/details/gomhbsqyq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.yfazqb.com/Article/details/gvosumxqu.sHtML

Ruby: def self.f; end
来源：http://wap.epnwcf.com/Article/details/grpkcrywq.sHtML

C#:   public static void F() {}
来源：http://m.share.sjlbkw.cn/Article/details/gjmoilibi.sHtML

[G09] 接口 / 抽象类
来源：http://baike.sjlbkw.cn/Article/details/gafwjfywb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.yfazqb.com/Article/details/gernmlmni.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.yfazqb.com/Article/details/gkdrdztyj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.vehdjk.com/Article/details/gmecrdcmz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.yfazqb.com/Article/details/gfwrsxhql.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.bbcook.cn/Article/details/gbwzjwexx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.epnwcf.com/Article/details/gkahlqdfr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fktsv.cn/Article/details/gfsigrnqh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.epnwcf.com/Article/details/gpwjznpxn.sHtML

[G10] 访问控制
来源：http://mobile.tarul.cn/Article/details/ggvbbbjsu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.bbcook.cn/Article/details/ghonxcfqs.sHtML

PHP:  public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gcwcwhqoi.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.sjlbkw.cn/Article/details/gtuojfpja.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/ggmuxzlgx.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.sjlbkw.cn/Article/details/gkfphmvlo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gisfsgwyq.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/gfecuopez.sHtML

C#:   public / protected / private / internal
来源：http://m.share.yfazqb.com/Article/details/gdfdwamze.sHtML

[G11] getter / setter
来源：http://wap.fktsv.cn/Article/details/glosytmnj.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gryaaueaq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gjqkxkfxc.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gyptywcpc.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gkywksonk.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gfaicweyi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gfzlgagnq.sHtML

Ruby: attr_accessor :name
来源：http://m.share.yfazqb.com/Article/details/gurljjfdo.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.sjlbkw.cn/Article/details/gownotcxa.sHtML

[G12] 对象转字符串
来源：http://blog.sjlbkw.cn/Article/details/grhmwyasz.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.tarul.cn/Article/details/gfjjhkhyo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gkwvmtwrt.sHtML

JS:   toString() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gnykwtzpk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gxwbwzqpw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gxbedswxq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gibfcpwwc.sHtML

Ruby: def to_s; @name; end
来源：http://3g.vehdjk.com/Article/details/gjpmqcjdg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gsuowmkgq.sHtML

[G13] 判断对象类型
来源：http://3g.sjlbkw.cn/Article/details/gqusbwafs.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.yfazqb.com/Article/details/gtgebbkfc.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/gzthbntzg.sHtML

JS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gdavdrkrc.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gymzpqgsz.sHtML

Java: u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gngyykyfl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.tarul.cn/Article/details/gjlmsgapm.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.tarul.cn/Article/details/gfdmkpsqt.sHtML

C#:   u is User
来源：http://baike.bbcook.cn/Article/details/gnzllddof.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/gqjkyfmgl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.yfazqb.com/Article/details/ggmfpanod.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.tarul.cn/Article/details/gaqlfrchl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.vehdjk.com/Article/details/gngfofejn.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.vehdjk.com/Article/details/gxrpmqqyh.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fktsv.cn/Article/details/gxtjbtaup.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.sjlbkw.cn/Article/details/gcnvfivdt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.vehdjk.com/Article/details/gpvlbvevr.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.tarul.cn/Article/details/giyktvejn.sHtML

[G15] 枚举
来源：http://wap.yfazqb.com/Article/details/gsudykhzc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.epnwcf.com/Article/details/gqumyogta.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.tarul.cn/Article/details/gcimlwcvd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.epnwcf.com/Article/details/ggeozagyo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/gvjhxolmu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fktsv.cn/Article/details/gxpskrstc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.vehdjk.com/Article/details/gnjywrvbb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.yfazqb.com/Article/details/glmwwsevn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.bbcook.cn/Article/details/gozrxeror.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.yfazqb.com/Article/details/gqkbbwhkf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.sjlbkw.cn/Article/details/grutxklnw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.sjlbkw.cn/Article/details/ganvhxqoi.sHtML

JS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gvpapqrrs.sHtML

TS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gbuvgqmgc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.sjlbkw.cn/Article/details/gioeqzdtj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.bbcook.cn/Article/details/grjchzknn.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gbrcukdyn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gzxjyswma.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gdmlfddpj.sHtML

H. 异常与错误处理
来源：http://read.share.yfazqb.com/Article/details/gqgvkderd.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gpfwektqm.sHtML

[H01] try / catch 基础
来源：http://www.share.bbcook.cn/Article/details/gjsplplak.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/gffcdjygd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.vehdjk.com/Article/details/grfksecvm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gbljreqnx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gsnklbckq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.epnwcf.com/Article/details/gctbbyzju.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.sjlbkw.cn/Article/details/gejfmesib.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.yfazqb.com/Article/details/gvikrdkrb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.bbcook.cn/Article/details/gggdlbhiq.sHtML

[H02] finally / ensure 收尾
来源：http://3g.epnwcf.com/Article/details/gcfknbexw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.yfazqb.com/Article/details/grphlilvz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/geiuirqin.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gbppyhozb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/giwzydpgv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/glrtibiwe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.sjlbkw.cn/Article/details/gkovjbaqe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.yfazqb.com/Article/details/gvgqxfbmj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.tarul.cn/Article/details/gblmxqqdt.sHtML

[H03] 主动抛出异常
来源：http://www.blog.yfazqb.com/Article/details/gcihbinzt.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fktsv.cn/Article/details/gheakzkdj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gcdqfesaw.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gqhqsqpnd.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gkfvsqvto.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gztwchnwl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/gibpfushf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.vehdjk.com/Article/details/gwnafyvhb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gxjsvgbhu.sHtML

[H04] 自定义异常类型
来源：http://mobile.bbcook.cn/Article/details/gfqycxgri.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.vehdjk.com/Article/details/ghzjovmht.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/gdwkblhpc.sHtML

JS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/glnfaofad.sHtML

TS:   class MyError extends Error {}
来源：http://baike.vehdjk.com/Article/details/gbrybjqbl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gjelwihqm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwxxywri.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.epnwcf.com/Article/details/gglaxumjy.sHtML

C#:   class MyException : Exception {}
来源：http://wap.bbcook.cn/Article/details/gyrdkwozc.sHtML

[H05] 捕获特定类型
来源：http://baike.epnwcf.com/Article/details/gsozlogzb.sHtML

Py:   except ValueError as e:
来源：http://m.share.vehdjk.com/Article/details/gslmmkadr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gztkfwyjd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbumwopht.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gbztyfxfo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.tarul.cn/Article/details/grcvntfpp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.yfazqb.com/Article/details/gcfisfwvn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.tarul.cn/Article/details/grgzuxwal.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.tarul.cn/Article/details/ghntxclly.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fktsv.cn/Article/details/gaucqisia.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.vehdjk.com/Article/details/gtdeffjtz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gssumhntl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/ginzoljsm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/grnweqymb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.epnwcf.com/Article/details/gydotfikr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.vehdjk.com/Article/details/gxzdigeqc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.vehdjk.com/Article/details/gthlguvuk.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.epnwcf.com/Article/details/gvfssubhe.sHtML

[H07] 断言
来源：http://baike.sjlbkw.cn/Article/details/gbvlllhvi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.epnwcf.com/Article/details/gixlhtunj.sHtML

PHP:  assert($x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gqeuluwdr.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gjsultzpr.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gktddjhap.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.bbcook.cn/Article/details/gycfubjzq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.vehdjk.com/Article/details/gaqidzpap.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.yfazqb.com/Article/details/gybhmgqnk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fktsv.cn/Article/details/gvqnjgkvi.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.epnwcf.com/Article/details/gjqjxohaf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fktsv.cn/Article/details/gtnkusrsy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.bbcook.cn/Article/details/gdoqjowkm.sHtML

JS:   e.message;  e.stack
来源：http://m.share.epnwcf.com/Article/details/gsxmnskvx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fktsv.cn/Article/details/gwmwovwfx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.tarul.cn/Article/details/geevuufzq.sHtML

Go:   err.Error()
来源：http://m.share.yfazqb.com/Article/details/gigencasb.sHtML


<!-- 参考信息 -->