代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.yfazqb.com/Article/details/gfftovqji.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.epnwcf.com/Article/details/ghgtotaem.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.bbcook.cn/Article/details/grenvwvri.sHtML

[F04] 追加写入文件
来源：http://blog.sjlbkw.cn/Article/details/gvvvoakbu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gfdiuxbcn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/gidqfnjvl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gyxepimqs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gnewkseni.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.vehdjk.com/Article/details/geetfhbhn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gdkofnelw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fktsv.cn/Article/details/gzjjrsuhe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.tarul.cn/Article/details/gshkwvjdg.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.yfazqb.com/Article/details/gagoqioxd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.tarul.cn/Article/details/ghzvgivjk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gzkehxcut.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gahgptyoq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gkgikksbu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/grlogiapi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/gnvmnivjz.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fktsv.cn/Article/details/glvfqgjar.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gzaraelec.sHtML

[F06] 删除文件
来源：http://blog.vehdjk.com/Article/details/gsebtwceo.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gxavqntmi.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fktsv.cn/Article/details/ghegkxfzl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gddusehpt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gknfjdssi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gkbqoxvff.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gxmwytglq.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.epnwcf.com/Article/details/glzhtidzj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.vehdjk.com/Article/details/gduryisqr.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/gbokrlath.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gpeatokiq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.sjlbkw.cn/Article/details/gsajfxjqk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/gtdaokiry.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/givpkxdgf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.epnwcf.com/Article/details/gxglcsfoa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.sjlbkw.cn/Article/details/geuphlecx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.tarul.cn/Article/details/gxkvyisol.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.vehdjk.com/Article/details/gwjwnypps.sHtML

[F08] 遍历目录
来源：http://read.share.bbcook.cn/Article/details/gxmkwkylr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fktsv.cn/Article/details/gsmbretau.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.bbcook.cn/Article/details/gugxnruql.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gchbqavss.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/gyumluuqw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gphnuikmb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fktsv.cn/Article/details/gymulztsl.sHtML

Ruby: Dir.children("dir")
来源：http://blog.vehdjk.com/Article/details/gmlvhddcx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/ghkkdlmqp.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/gptlrdskn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gumcmltup.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gyajwrseq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gcinaucdl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/gupaxpqua.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gzgtjjrto.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fktsv.cn/Article/details/gmdjvnbbi.sHtML

Ruby: File.size("a.txt")
来源：http://baike.yfazqb.com/Article/details/gmqjyiupu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.sjlbkw.cn/Article/details/givnfkmxv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/gvoqgorxq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/guwffnkcj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.vehdjk.com/Article/details/gevvexrzk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/guupdfsfb.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.tarul.cn/Article/details/gkomryfqp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/glyclyrds.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gpzfwluaw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gcrvegdfb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gjcimqdzy.sHtML

[F11] 复制与移动文件
来源：http://www.share.sjlbkw.cn/Article/details/ggjjfyiuc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gxmowznys.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gqurbrqze.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gwatnxhny.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gsnwtkxtb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/gcrjvsrhe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.sjlbkw.cn/Article/details/gtctnkvjv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gpmrhausj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.sjlbkw.cn/Article/details/gpgkvmgdw.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/gutbuayms.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gqiqoiawd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.tarul.cn/Article/details/gumrokjbx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.tarul.cn/Article/details/grcwvehgk.sHtML

TS:   // 同上
来源：http://read.share.yfazqb.com/Article/details/gnslziccd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.bbcook.cn/Article/details/gcmbmiheh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.yfazqb.com/Article/details/gfqevqzgx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fktsv.cn/Article/details/gqkfpoqdu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.epnwcf.com/Article/details/gnlltgfjb.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gudrqsrjt.sHtML

G. 面向对象
来源：http://baike.bbcook.cn/Article/details/glgodhvdf.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gyamjdipm.sHtML

[G01] 定义类
来源：http://baike.sjlbkw.cn/Article/details/gbyeretqb.sHtML

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/gtoqeicsa.sHtML

PHP:  class User {}
来源：http://baike.yfazqb.com/Article/details/gswtgidvb.sHtML

JS:   class User {}
来源：http://blog.tarul.cn/Article/details/gidvuwscl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvooncson.sHtML

Java: class User {}
来源：http://www.share.vehdjk.com/Article/details/guvqkgwdt.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/giqhaujfe.sHtML

Ruby: class User; end
来源：http://www.m.share.yfazqb.com/Article/details/gldswuiuq.sHtML

C#:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gdqunjnte.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/grjoxiuyw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.epnwcf.com/Article/details/goosuofjp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gdupsqbsj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gbtrydkgb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.yfazqb.com/Article/details/gikrqfvfz.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/gnigjehbj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/grxqlwwhk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.bbcook.cn/Article/details/gwpmgjqyx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/gpatsilno.sHtML

[G03] 实例属性
来源：http://read.share.bbcook.cn/Article/details/gomepkgba.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/gebzdsizb.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gufxuftyy.sHtML

JS:   this.name = "x";
来源：http://3g.vehdjk.com/Article/details/ghkiocelq.sHtML

TS:   name: string = "x";
来源：http://blog.fktsv.cn/Article/details/gcjaoebww.sHtML

Java: private String name;
来源：http://m.share.bbcook.cn/Article/details/gdadyytqr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.yfazqb.com/Article/details/gnnemmguk.sHtML

Ruby: @name = "x"
来源：http://wap.bbcook.cn/Article/details/gmugifaqy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.epnwcf.com/Article/details/gqrvdfdgq.sHtML

[G04] 定义方法
来源：http://mobile.fktsv.cn/Article/details/gbcqqhnys.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gomsxvoka.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gzsvuwwba.sHtML

JS:   greet() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gtdfnrdyv.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gcvhkenpn.sHtML

Java: String greet() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gcadedqmz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gzstmnmas.sHtML

Ruby: def greet; @name; end
来源：http://mobile.yfazqb.com/Article/details/gaubprpwi.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.epnwcf.com/Article/details/gcehdtsmc.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/gjhttskou.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/gkfzvhksn.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gkxgxmdud.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/guwbblimq.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gpbtvqluf.sHtML

Java: class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/ggrenfemf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/ghyuerciy.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.vehdjk.com/Article/details/gyojasxfh.sHtML

C#:   class Admin : User {}
来源：http://read.share.bbcook.cn/Article/details/groljzyoq.sHtML

[G06] 重写方法
来源：http://m.share.tarul.cn/Article/details/gytbnjyrl.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/gjebhftwt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gvkbxpqcf.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/ggtxgdkuo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gbdvbrtvf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gberzudqf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.vehdjk.com/Article/details/gtsnomryk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/gnticxfwz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/ggibpfcmb.sHtML

[G07] 调用父类方法
来源：http://www.blog.yfazqb.com/Article/details/gzmbijdgl.sHtML

Py:   super().greet()
来源：http://blog.fktsv.cn/Article/details/gmygokgqp.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gfcihlccz.sHtML

JS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gxpesrfhv.sHtML

TS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gffwnjiko.sHtML

Java: super.greet();
来源：http://mobile.tarul.cn/Article/details/gezyieern.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.sjlbkw.cn/Article/details/gvphxuspx.sHtML

Ruby: super
来源：http://www.blog.vehdjk.com/Article/details/gjeunoekb.sHtML

C#:   base.Greet();
来源：http://www.blog.vehdjk.com/Article/details/gwtvizriv.sHtML

[G08] 静态方法与属性
来源：http://3g.yfazqb.com/Article/details/gnodsllpj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/geprkscdw.sHtML

PHP:  public static function f() {}
来源：http://3g.sjlbkw.cn/Article/details/gcxhvxxlr.sHtML

JS:   static f() {}
来源：http://www.blog.fktsv.cn/Article/details/grqxuzrir.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/gbnchcrth.sHtML

Java: static void f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gdtctbjso.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.bbcook.cn/Article/details/gabcemgxk.sHtML

Ruby: def self.f; end
来源：http://www.m.share.yfazqb.com/Article/details/gtigrcijt.sHtML

C#:   public static void F() {}
来源：http://mobile.epnwcf.com/Article/details/gnomyqvmj.sHtML

[G09] 接口 / 抽象类
来源：http://wap.epnwcf.com/Article/details/gwvqzkqgr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/gmasbstxk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.vehdjk.com/Article/details/gopcsxshk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.epnwcf.com/Article/details/gvqcoufoe.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.bbcook.cn/Article/details/gmkrytanv.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fktsv.cn/Article/details/girwopfeh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.vehdjk.com/Article/details/gacwvguvo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/gelbxegtx.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/ggpfwutvt.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/ghryvpssj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.sjlbkw.cn/Article/details/gbioinbjn.sHtML

PHP:  public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gzbbcsbfr.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.bbcook.cn/Article/details/guaoypmms.sHtML

TS:   public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gejalqexl.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/gpfihktbg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.bbcook.cn/Article/details/goamhrfyk.sHtML

Ruby: public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/ggexpmdjs.sHtML

C#:   public / protected / private / internal
来源：http://baike.fktsv.cn/Article/details/gblsumqgk.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/guopwougd.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/gxgnbuddm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gixaqivxl.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gctxshuvj.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fktsv.cn/Article/details/gdbjqyzzt.sHtML

Java: public String getName() { return name; }
来源：http://mobile.epnwcf.com/Article/details/glerdqpph.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gxqlpnynh.sHtML

Ruby: attr_accessor :name
来源：http://3g.sjlbkw.cn/Article/details/gcmrkagsc.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/gbdfmlwyd.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/gjzlpqotb.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/gclvmuqff.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/guxnkxwzf.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gutjjnify.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gezdiekio.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gcxxaddam.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gujbajxdt.sHtML

Ruby: def to_s; @name; end
来源：http://blog.sjlbkw.cn/Article/details/glafthlws.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.vehdjk.com/Article/details/gvrzcbatn.sHtML

[G13] 判断对象类型
来源：http://3g.sjlbkw.cn/Article/details/gfbinpyvg.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.sjlbkw.cn/Article/details/gkltaysky.sHtML

PHP:  $u instanceof User
来源：http://blog.vehdjk.com/Article/details/gumuosucp.sHtML

JS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gzgkkjlkd.sHtML

TS:   u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gejyvmpsg.sHtML

Java: u instanceof User
来源：http://mobile.epnwcf.com/Article/details/glmprhjfd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.tarul.cn/Article/details/ggdhjcrpf.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.tarul.cn/Article/details/gpsfpqbgf.sHtML

C#:   u is User
来源：http://www.m.share.vehdjk.com/Article/details/ghhuamdqb.sHtML

[G14] 数据类 / record
来源：http://read.share.vehdjk.com/Article/details/gngooptoz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fktsv.cn/Article/details/gbrnwhgpw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.bbcook.cn/Article/details/gwlwrjcyj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.bbcook.cn/Article/details/gqtofivkl.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gfrehwqho.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/gznmpqjmq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.vehdjk.com/Article/details/gkqusihgp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.vehdjk.com/Article/details/gkoyzhbnw.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.tarul.cn/Article/details/gijrmuudi.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/gnehmkpii.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.bbcook.cn/Article/details/ghmpbnspp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.vehdjk.com/Article/details/gezilzjwf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.sjlbkw.cn/Article/details/gnaypymat.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gbzczihsc.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fktsv.cn/Article/details/glwyqllwl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gnkvjdjfg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fktsv.cn/Article/details/ghyytycfc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gorxjuhco.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.tarul.cn/Article/details/glypnogsg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.epnwcf.com/Article/details/guemvmuwc.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.tarul.cn/Article/details/ghebnveff.sHtML

JS:   Object.entries(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gfnpcfcix.sHtML

TS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gihhtdjmb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.tarul.cn/Article/details/godzapybq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/gvmlnajne.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/gjbkrisxr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gdgvzmpjo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkshsyjhs.sHtML

H. 异常与错误处理
来源：http://blog.vehdjk.com/Article/details/gpftutdhh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkehgtkap.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/gqnvyyfgr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.yfazqb.com/Article/details/gntlrttgh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/glxqyvjfh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/goswavswe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gccqdysjs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gowydgiez.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.vehdjk.com/Article/details/gwvnygfyz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.epnwcf.com/Article/details/goqkeudcr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fktsv.cn/Article/details/glkjfmcuf.sHtML

[H02] finally / ensure 收尾
来源：http://3g.epnwcf.com/Article/details/ggtgvbqvp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.yfazqb.com/Article/details/gqcwnqhie.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gjtqkqnvf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gynmkvmbf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gdexachvw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gwmtofqex.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fktsv.cn/Article/details/gqwjphhyg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.epnwcf.com/Article/details/gmbizccac.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/ghzgwrdvc.sHtML

[H03] 主动抛出异常
来源：http://3g.sjlbkw.cn/Article/details/glfyrlveb.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/gqfdyropa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/ghwepiomg.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gxtkdereo.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.vehdjk.com/Article/details/ghtnwhxao.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gvdyckizd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.bbcook.cn/Article/details/gnycnjetd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.sjlbkw.cn/Article/details/grmwgmwhh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gzsqjwese.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/guxfncbdx.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fktsv.cn/Article/details/gjgfezzge.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/grtolwjet.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbnggqde.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.sjlbkw.cn/Article/details/grtjhoqkb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.epnwcf.com/Article/details/gmosykofb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.epnwcf.com/Article/details/gpzddysov.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.bbcook.cn/Article/details/gcjtqovds.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.bbcook.cn/Article/details/gzhshctni.sHtML

[H05] 捕获特定类型
来源：http://wap.sjlbkw.cn/Article/details/gfycjlxbu.sHtML

Py:   except ValueError as e:
来源：http://3g.tarul.cn/Article/details/gaytmslwj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/gqpswnkpm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gjbgkzjlo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/ghgavmydd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.bbcook.cn/Article/details/gwrvqcmbw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.tarul.cn/Article/details/ghwdkewyo.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.tarul.cn/Article/details/gdexkozhn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.vehdjk.com/Article/details/gopllcqop.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fktsv.cn/Article/details/gsqlidyyo.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gbdcmzbgp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gelpkeetg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/ghrcnjjae.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gcjvvytyq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fktsv.cn/Article/details/gmtdkunfz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.bbcook.cn/Article/details/gevkyrfjq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.sjlbkw.cn/Article/details/gxjnbypkf.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gjchzdihx.sHtML

[H07] 断言
来源：http://wap.bbcook.cn/Article/details/gmoailkon.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.yfazqb.com/Article/details/gtexerswj.sHtML

PHP:  assert($x > 0);
来源：http://m.share.yfazqb.com/Article/details/ggngljxec.sHtML

JS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gledypzyo.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gjjkeajyi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.bbcook.cn/Article/details/gvoaqgyga.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fktsv.cn/Article/details/ghzrdufgh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.bbcook.cn/Article/details/gfcrxzhpd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/gskqyynfd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.vehdjk.com/Article/details/gdxtegaip.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.sjlbkw.cn/Article/details/grqckmaqm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fktsv.cn/Article/details/gntfqvymx.sHtML


<!-- 参考信息 -->