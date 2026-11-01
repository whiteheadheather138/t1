代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fktsv.cn/Article/details/gegnqdagp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fktsv.cn/Article/details/grosmjwpu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.bbcook.cn/Article/details/gkisssleu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/gnjovimrp.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.sjlbkw.cn/Article/details/goznrfegf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.tarul.cn/Article/details/gcabjggva.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gyikgxqaq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gotaltthv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/goygqdvqf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gewjmnged.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/gmlxykucc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gzvvtntom.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gljjpvdva.sHtML

[F06] 删除文件
来源：http://mobile.epnwcf.com/Article/details/gshvnpugb.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gvytfiplr.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gruevhraj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gfxgstfin.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gfgyabvkf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/genvwjhee.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gimkiuvad.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gtmjmbcza.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.epnwcf.com/Article/details/guvhvfpuw.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fktsv.cn/Article/details/gkjrfasnl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.sjlbkw.cn/Article/details/ghbdntzbv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.bbcook.cn/Article/details/gtvncgbyl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gxllpgwqe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gxniezrdd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/grpgxuxap.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.epnwcf.com/Article/details/gwletenhy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.vehdjk.com/Article/details/gbfxwtyal.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.tarul.cn/Article/details/gojvwhoqc.sHtML

[F08] 遍历目录
来源：http://mobile.sjlbkw.cn/Article/details/gtgtcsnll.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.epnwcf.com/Article/details/gvynbuzsp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.tarul.cn/Article/details/grhuxpyyp.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gadzlnkrl.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gznurojrv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gaqjbrodv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fktsv.cn/Article/details/gkcuwuikf.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/ggkhvrqgn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.yfazqb.com/Article/details/gldgnxslh.sHtML

[F09] 获取文件大小
来源：http://wap.epnwcf.com/Article/details/gwfsjspvv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gowodgrvn.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gkzumrowk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gzkjfngsq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gweycezaz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gspljomir.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.yfazqb.com/Article/details/gvglcxbwg.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gphvsrfkg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.yfazqb.com/Article/details/gwskpbghb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.sjlbkw.cn/Article/details/gdgabffrh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/ghajdsmga.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/grnmpvnwf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gwzyhwgul.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gfmkfrmhp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.tarul.cn/Article/details/gfynbzekm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gttlsytau.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ghrqsfixx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gswrvyecf.sHtML

[F11] 复制与移动文件
来源：http://3g.yfazqb.com/Article/details/gcwayqukc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gpwgwixhm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.tarul.cn/Article/details/ggsbhnsdw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gilcuwfvd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gdiirohwx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.vehdjk.com/Article/details/gmfawigtq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/gzloxxahp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmecfwnvp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/gvkbfluvw.sHtML

[F12] CSV 读写
来源：http://www.blog.fktsv.cn/Article/details/ghzmbovvh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fktsv.cn/Article/details/gekomgwno.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.vehdjk.com/Article/details/gjmvvwnyn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.epnwcf.com/Article/details/gaogttgnp.sHtML

TS:   // 同上
来源：http://mobile.sjlbkw.cn/Article/details/gfshrrbob.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gslycjqbv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.vehdjk.com/Article/details/gvahkvaay.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.bbcook.cn/Article/details/gdlusenpf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.bbcook.cn/Article/details/gwsnsrrra.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/goamngvti.sHtML

G. 面向对象
来源：http://3g.yfazqb.com/Article/details/gjjivkyjo.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gcvidvryj.sHtML

[G01] 定义类
来源：http://wap.epnwcf.com/Article/details/gfkpliwvr.sHtML

Py:   class User: pass
来源：http://wap.vehdjk.com/Article/details/gdjzviipr.sHtML

PHP:  class User {}
来源：http://blog.sjlbkw.cn/Article/details/gmcxyzqiy.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gzvwtnpuv.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/ggtkzyxci.sHtML

Java: class User {}
来源：http://m.share.bbcook.cn/Article/details/gaeangdzw.sHtML

Go:   type User struct { Name string }
来源：http://www.share.bbcook.cn/Article/details/griwdndac.sHtML

Ruby: class User; end
来源：http://wap.bbcook.cn/Article/details/gvhwtwhvi.sHtML

C#:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/glvfgilgw.sHtML

[G02] 构造函数
来源：http://www.share.fktsv.cn/Article/details/gwnqfkhiv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.vehdjk.com/Article/details/guqgnoeap.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.vehdjk.com/Article/details/gpsptnpvk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gawniohfc.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.sjlbkw.cn/Article/details/gljakvodq.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gczolmigg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.epnwcf.com/Article/details/gzstyefor.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.bbcook.cn/Article/details/gaiuislcr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gudumimgb.sHtML

[G03] 实例属性
来源：http://blog.vehdjk.com/Article/details/gimewnwsd.sHtML

Py:   self.name = "x"
来源：http://blog.tarul.cn/Article/details/gfyaclpdp.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/gmkdzfhnb.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/gqkxoorye.sHtML

TS:   name: string = "x";
来源：http://baike.fktsv.cn/Article/details/gxsmrlsvm.sHtML

Java: private String name;
来源：http://m.share.vehdjk.com/Article/details/gjemqhuvy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gkgchcvbn.sHtML

Ruby: @name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gchzzfzdp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/glyrmtpke.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/gjyhzfncr.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gjuxrvtbw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gtbgwuoyy.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gyoaufwbw.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gfbojjqop.sHtML

Java: String greet() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gkzjtaune.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gudkxnmaq.sHtML

Ruby: def greet; @name; end
来源：http://m.share.vehdjk.com/Article/details/gmwgdjigd.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gbohoftfw.sHtML

[G05] 继承
来源：http://www.blog.vehdjk.com/Article/details/gjxddemsm.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fktsv.cn/Article/details/gcvfsdjxu.sHtML

PHP:  class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gibaudvrm.sHtML

JS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gtoxqcacn.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gbvyaseio.sHtML

Java: class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/ghodypxyj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.sjlbkw.cn/Article/details/gzbtfimqw.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.epnwcf.com/Article/details/gqqyasiuk.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/getomvbja.sHtML

[G06] 重写方法
来源：http://baike.vehdjk.com/Article/details/gpnhshaod.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/grdqcrbyk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gkcpdginr.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gklhvfrii.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gzoxmcdeh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/giluhtsyy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gkaspraml.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.sjlbkw.cn/Article/details/gjgffgovt.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.yfazqb.com/Article/details/gxkdcygsm.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gjepqjtgg.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/grtezprvp.sHtML

PHP:  parent::greet();
来源：http://www.share.fktsv.cn/Article/details/gcqngrfih.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gsvrjzcbu.sHtML

TS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gshhrmeol.sHtML

Java: super.greet();
来源：http://read.share.fktsv.cn/Article/details/gzamuqhwc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.vehdjk.com/Article/details/gdmfusbeg.sHtML

Ruby: super
来源：http://mobile.yfazqb.com/Article/details/gqmizkyuv.sHtML

C#:   base.Greet();
来源：http://read.share.epnwcf.com/Article/details/givwkebug.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/giktwatwm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.epnwcf.com/Article/details/gnqxcmybp.sHtML

PHP:  public static function f() {}
来源：http://blog.yfazqb.com/Article/details/gybuorgkl.sHtML

JS:   static f() {}
来源：http://baike.vehdjk.com/Article/details/glnbyzlxw.sHtML

TS:   static f(): void {}
来源：http://mobile.fktsv.cn/Article/details/ghketdren.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gowmbcwvx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.yfazqb.com/Article/details/gjeqmjwbj.sHtML

Ruby: def self.f; end
来源：http://read.share.yfazqb.com/Article/details/ggllncxus.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/ghxtaerdn.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/gswcfgxay.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/gpshwvhgz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.vehdjk.com/Article/details/gwwjbdxdg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.vehdjk.com/Article/details/gacpxppnc.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.sjlbkw.cn/Article/details/girrgoevp.sHtML

Java: interface Shape { double area(); }
来源：http://baike.sjlbkw.cn/Article/details/gwfsqsawr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.epnwcf.com/Article/details/gcbpypdhn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/gpcrktmxl.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/gvrpfvchf.sHtML

[G10] 访问控制
来源：http://read.share.epnwcf.com/Article/details/gxhuovkdn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/gfmyelqrp.sHtML

PHP:  public / protected / private
来源：http://baike.epnwcf.com/Article/details/gxnokkodv.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/gaupgzetv.sHtML

TS:   public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gzefdfxbx.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.sjlbkw.cn/Article/details/ghtdmstep.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fktsv.cn/Article/details/gpjgprqgh.sHtML

Ruby: public / protected / private
来源：http://wap.fktsv.cn/Article/details/gpupfokzz.sHtML

C#:   public / protected / private / internal
来源：http://blog.epnwcf.com/Article/details/gzifaodaa.sHtML

[G11] getter / setter
来源：http://www.blog.sjlbkw.cn/Article/details/gtlhpfpng.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/gsubvymke.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/ginmjpsxc.sHtML

JS:   get name() { return this._name; }
来源：http://3g.vehdjk.com/Article/details/grzlohtwp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gwpaabtgm.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gatwhfehk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gfdbsrfwh.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/gkrpoajnr.sHtML

C#:   public string Name { get; set; }
来源：http://3g.bbcook.cn/Article/details/gcusjkbvi.sHtML

[G12] 对象转字符串
来源：http://wap.fktsv.cn/Article/details/gaymzzkxv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/gnpycgcps.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gievlcmwb.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/geybjiqsk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gynpqjkqx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/geglayvzd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gwicrhnxn.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.bbcook.cn/Article/details/gjnovypgv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.vehdjk.com/Article/details/gewtdpige.sHtML

[G13] 判断对象类型
来源：http://blog.tarul.cn/Article/details/gjxgrlums.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.epnwcf.com/Article/details/grnqwbxma.sHtML

PHP:  $u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gsdzullnz.sHtML

JS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gqwwcunmp.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gyfvwplck.sHtML

Java: u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gcdgpvnbb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcxjzmko.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/gbuzhycrg.sHtML

C#:   u is User
来源：http://m.share.yfazqb.com/Article/details/gbanebala.sHtML

[G14] 数据类 / record
来源：http://mobile.vehdjk.com/Article/details/gkjvvfyun.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.vehdjk.com/Article/details/glxkodvcg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/gynlbdwwl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/gtglesiwu.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.yfazqb.com/Article/details/gitelwksy.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.sjlbkw.cn/Article/details/gmhpkztov.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.yfazqb.com/Article/details/gceafzdfd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.sjlbkw.cn/Article/details/gtuszywes.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.sjlbkw.cn/Article/details/gqttmqqjf.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/gqbzpkzzb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.vehdjk.com/Article/details/gtwdzwhkx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fktsv.cn/Article/details/gmopqxkul.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fktsv.cn/Article/details/glccgwwvk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/glltrwicl.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fktsv.cn/Article/details/gvzpslyuj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/gedgenokj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.vehdjk.com/Article/details/gmfehoqsn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gnqpbwqmv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.tarul.cn/Article/details/gilmcvhml.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.yfazqb.com/Article/details/gjbuxxodp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fktsv.cn/Article/details/gzswoqqzl.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/grcodbenm.sHtML

TS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gfofdvvve.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.bbcook.cn/Article/details/gkloxotsg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.bbcook.cn/Article/details/gzmjxjnkj.sHtML

Ruby: obj.instance_variables
来源：http://m.share.sjlbkw.cn/Article/details/gghndmgqk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gbnjrtctj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghqdvjyxi.sHtML

H. 异常与错误处理
来源：http://www.m.share.vehdjk.com/Article/details/guzdosbvi.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghwezfotx.sHtML

[H01] try / catch 基础
来源：http://blog.bbcook.cn/Article/details/gbfnqacdw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.epnwcf.com/Article/details/ggskeedcx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/gikahpxub.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gioyatpue.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gjuwnponq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.bbcook.cn/Article/details/ggpfwfzxv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.epnwcf.com/Article/details/gtchbuhbh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.epnwcf.com/Article/details/gdvekwbhm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.bbcook.cn/Article/details/goszgikun.sHtML

[H02] finally / ensure 收尾
来源：http://wap.yfazqb.com/Article/details/gipleabxr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.epnwcf.com/Article/details/gdgdkmlqm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/glyzsesls.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gvodpviva.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gynbpzuvh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gplyabbao.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.yfazqb.com/Article/details/gqnmjqpsx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fktsv.cn/Article/details/gybjdbwwa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gsgocggxn.sHtML

[H03] 主动抛出异常
来源：http://3g.vehdjk.com/Article/details/gpcixvxbc.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.epnwcf.com/Article/details/gbstzixqe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gowvujehp.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gzofxgace.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/guminczll.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gujruiist.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.sjlbkw.cn/Article/details/gttbeignm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.tarul.cn/Article/details/gcfkpfxhv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/glcaaebko.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gcdzqdyqc.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.epnwcf.com/Article/details/gyczncwln.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gpahmyvlq.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gqlsvymky.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gfvhfnvro.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/ggljqkudj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fktsv.cn/Article/details/gyeaogxet.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fktsv.cn/Article/details/gyxgqbtgy.sHtML

C#:   class MyException : Exception {}
来源：http://baike.epnwcf.com/Article/details/gazpazazf.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fktsv.cn/Article/details/gabqfsdqp.sHtML

Py:   except ValueError as e:
来源：http://www.share.tarul.cn/Article/details/gviwyenat.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.sjlbkw.cn/Article/details/gdshftqgq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.sjlbkw.cn/Article/details/goijfypls.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.vehdjk.com/Article/details/giijqrmng.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/gmgtrcrxg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.sjlbkw.cn/Article/details/gbeoerohj.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fktsv.cn/Article/details/gngdmafrf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.vehdjk.com/Article/details/gtfxllpti.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.tarul.cn/Article/details/gmtugffxw.sHtML

Py:   value = d.get("k") or default
来源：http://wap.sjlbkw.cn/Article/details/gkfvudbso.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/glmgkjaea.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.sjlbkw.cn/Article/details/gbnexlwfj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/gkfhpqyfp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.bbcook.cn/Article/details/gwubswble.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.yfazqb.com/Article/details/glfkojvfe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fktsv.cn/Article/details/gmiqsqtek.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.vehdjk.com/Article/details/ghpzfcrjx.sHtML

[H07] 断言
来源：http://read.share.bbcook.cn/Article/details/gpryzsqhf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.bbcook.cn/Article/details/gzxmweizr.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fktsv.cn/Article/details/ggeojrrew.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gymkxrsrw.sHtML

TS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/ggbwfcopf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.tarul.cn/Article/details/gozeffwye.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fktsv.cn/Article/details/gsjnllvug.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.bbcook.cn/Article/details/gsnfwrpbf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gmrzxyyrd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.yfazqb.com/Article/details/gyrxqqkcp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.bbcook.cn/Article/details/gynrjritr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.sjlbkw.cn/Article/details/gfncgfxbb.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fktsv.cn/Article/details/ggvgrskhi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gdaijwfss.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fktsv.cn/Article/details/gzaadbvzt.sHtML

Go:   err.Error()
来源：http://m.share.fktsv.cn/Article/details/gfchkfloq.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.bbcook.cn/Article/details/gginehxuz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.epnwcf.com/Article/details/gwwqmdypk.sHtML

[H09] 带错误码的异常
来源：http://baike.epnwcf.com/Article/details/gxjhnvkgm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.vehdjk.com/Article/details/gejtupxww.sHtML


<!-- 参考信息 -->