代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.vehdjk.com/Article/details/gdphrhdci.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.tarul.cn/Article/details/grjyhvgqm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.vehdjk.com/Article/details/gadfhisoq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.vehdjk.com/Article/details/gcgmonixd.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/groajwery.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fktsv.cn/Article/details/gjfhlgbjr.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gzxjllquz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gxfjtzjsd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/ggispbpqc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gbqsitpfm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.sjlbkw.cn/Article/details/gvtxsuhll.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.tarul.cn/Article/details/gplolihae.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fktsv.cn/Article/details/goyefasbd.sHtML

[F06] 删除文件
来源：http://wap.vehdjk.com/Article/details/gjfntxjhq.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gaqztdsyy.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gmgwpwvjy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gekmiijjy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/ghnnzdtxu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gvcznlgbo.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gubizpoxr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.tarul.cn/Article/details/ggahpyvob.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gteydikvi.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.tarul.cn/Article/details/gqreneneu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/gynofwujq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.sjlbkw.cn/Article/details/gmmtrikqi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/gxuehsvac.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gysysfllp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.sjlbkw.cn/Article/details/gogfmnyae.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.yfazqb.com/Article/details/gozzicure.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.yfazqb.com/Article/details/gohewpzbv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.sjlbkw.cn/Article/details/gwxhtjvwp.sHtML

[F08] 遍历目录
来源：http://m.share.sjlbkw.cn/Article/details/gsooqnkrz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.yfazqb.com/Article/details/galftfqmd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fktsv.cn/Article/details/ghebkqkqf.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gqzeozxxo.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gjojvgpwo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/ghvpthzhy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.yfazqb.com/Article/details/gjncmvilg.sHtML

Ruby: Dir.children("dir")
来源：http://wap.vehdjk.com/Article/details/gqcztfjdi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gmletlsqa.sHtML

[F09] 获取文件大小
来源：http://blog.epnwcf.com/Article/details/gosjkaltn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.yfazqb.com/Article/details/gixnmpfrp.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fktsv.cn/Article/details/gmboxajll.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gisqqhkjr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/glukxitle.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gmcyagctb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.bbcook.cn/Article/details/gftysmytp.sHtML

Ruby: File.size("a.txt")
来源：http://wap.epnwcf.com/Article/details/gtsasmpmy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.yfazqb.com/Article/details/gveapighr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.epnwcf.com/Article/details/gckccqjvb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gcqfhhfma.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.bbcook.cn/Article/details/gmvknjuuk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gksbrnivl.sHtML

TS:   path.extname("a.txt")
来源：http://baike.tarul.cn/Article/details/gzajluzcw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.epnwcf.com/Article/details/gsvwlnrjs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gftovdreg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gmvgneueu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gxrvhxvbt.sHtML

[F11] 复制与移动文件
来源：http://m.share.bbcook.cn/Article/details/gddnqrzqb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gwrbnddgd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.epnwcf.com/Article/details/gxjrlrwat.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/ggujoeznq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gcotnbtkj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.tarul.cn/Article/details/gszfkovst.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.bbcook.cn/Article/details/gsmnlaxwz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gewptigmd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.tarul.cn/Article/details/goerqgams.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/gmejktygg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fktsv.cn/Article/details/gacughhtd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.vehdjk.com/Article/details/gumikobqd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/gbcvusyuu.sHtML

TS:   // 同上
来源：http://m.share.tarul.cn/Article/details/gtoqvmkmo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.epnwcf.com/Article/details/gjijrzdiv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.epnwcf.com/Article/details/geyglggis.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/gcqombhga.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/gngzgtbbw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gwiuivqfz.sHtML

G. 面向对象
来源：http://www.share.yfazqb.com/Article/details/gokndzayp.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gvxhdzeim.sHtML

[G01] 定义类
来源：http://blog.yfazqb.com/Article/details/gubwgrvdw.sHtML

Py:   class User: pass
来源：http://mobile.yfazqb.com/Article/details/gfrhwqeqd.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/ggemzmonf.sHtML

JS:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/geztapkbe.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/gohgzeoin.sHtML

Java: class User {}
来源：http://www.blog.yfazqb.com/Article/details/gzwkajmtk.sHtML

Go:   type User struct { Name string }
来源：http://m.share.tarul.cn/Article/details/gnfpacxie.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gstzjzgdc.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gdotufcuk.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gqtqecthr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fktsv.cn/Article/details/gplvffuxf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/gorsiewfg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gonuhvfaw.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/gzuzbxgig.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gzscclsbn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gmejxzmwg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.vehdjk.com/Article/details/glhlcbcxa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gypomgeqi.sHtML

[G03] 实例属性
来源：http://baike.bbcook.cn/Article/details/gqwvdvfin.sHtML

Py:   self.name = "x"
来源：http://baike.fktsv.cn/Article/details/guwrmwqoa.sHtML

PHP:  public string $name = "x";
来源：http://read.share.vehdjk.com/Article/details/gohqpksro.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gnfjnskmv.sHtML

TS:   name: string = "x";
来源：http://m.share.bbcook.cn/Article/details/gwghtpyyo.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/gzyryhrzk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.bbcook.cn/Article/details/ggwxojaaj.sHtML

Ruby: @name = "x"
来源：http://mobile.epnwcf.com/Article/details/gnrbxccrq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gvxjyjwaf.sHtML

[G04] 定义方法
来源：http://mobile.tarul.cn/Article/details/gtvlvaejr.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gblznfuyr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/glxjhbwmi.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/grgmhluzp.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/grfuzzqjp.sHtML

Java: String greet() { return name; }
来源：http://3g.bbcook.cn/Article/details/gnmlzgvji.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gdrhycyhx.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gcfipzliq.sHtML

C#:   public string Greet() => Name;
来源：http://blog.bbcook.cn/Article/details/gzxiecima.sHtML

[G05] 继承
来源：http://read.share.fktsv.cn/Article/details/godrafgec.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fktsv.cn/Article/details/gbgsniigc.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gmanlbtof.sHtML

JS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/ghvydafqw.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gqtqddven.sHtML

Java: class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gjwosmdco.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gvpserbgr.sHtML

Ruby: class Admin < User; end
来源：http://baike.bbcook.cn/Article/details/ginvtstjd.sHtML

C#:   class Admin : User {}
来源：http://read.share.fktsv.cn/Article/details/glqiqpgxz.sHtML

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/gfduoajic.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.yfazqb.com/Article/details/gjpwernlv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gvybsuwev.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/glrekzqqq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/grosadosa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gxrfkqrwg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/gjphkgyml.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/goclsycuw.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/gungxngtz.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/gyybledre.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gkmsuyaeq.sHtML

PHP:  parent::greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gllizblwj.sHtML

JS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/glqwogvfl.sHtML

TS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/ghqonkoyy.sHtML

Java: super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gcqmqtpqi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.yfazqb.com/Article/details/gjybjzdsp.sHtML

Ruby: super
来源：http://mobile.bbcook.cn/Article/details/gxjfrgnbg.sHtML

C#:   base.Greet();
来源：http://www.m.share.bbcook.cn/Article/details/gdkuprruh.sHtML

[G08] 静态方法与属性
来源：http://wap.epnwcf.com/Article/details/gravzkamm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.sjlbkw.cn/Article/details/gjnqfugaa.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/ghgafwemm.sHtML

JS:   static f() {}
来源：http://read.share.bbcook.cn/Article/details/gsypgpann.sHtML

TS:   static f(): void {}
来源：http://www.m.share.epnwcf.com/Article/details/gigfyzubg.sHtML

Java: static void f() {}
来源：http://wap.epnwcf.com/Article/details/gwqhbglxi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fktsv.cn/Article/details/gmvcpneeq.sHtML

Ruby: def self.f; end
来源：http://3g.yfazqb.com/Article/details/ghckqerfk.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/gmjazlojp.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.vehdjk.com/Article/details/gzvdjxonc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.sjlbkw.cn/Article/details/gpzpmotzk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.bbcook.cn/Article/details/gwozvbdsh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.vehdjk.com/Article/details/gszgohgcp.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.sjlbkw.cn/Article/details/glrbgtwse.sHtML

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/gpeqhiqux.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.sjlbkw.cn/Article/details/glzluioco.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.tarul.cn/Article/details/gmkvpwejt.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/ggaddsnig.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/gcregawmk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/gusysclrh.sHtML

PHP:  public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gprcabgap.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.tarul.cn/Article/details/glefextsx.sHtML

TS:   public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/glssxsvwf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.yfazqb.com/Article/details/gxlenurvs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.bbcook.cn/Article/details/gwvaumkzd.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gdsiqxhko.sHtML

C#:   public / protected / private / internal
来源：http://mobile.sjlbkw.cn/Article/details/gtmcrqbzg.sHtML

[G11] getter / setter
来源：http://blog.epnwcf.com/Article/details/gupdjidzw.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fktsv.cn/Article/details/gvubxvocy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/ggkxxougr.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/ganrpkmyy.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gpajmrmzq.sHtML

Java: public String getName() { return name; }
来源：http://3g.bbcook.cn/Article/details/gwpbzfdgm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gpobktpot.sHtML

Ruby: attr_accessor :name
来源：http://baike.yfazqb.com/Article/details/gkrzbingc.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.epnwcf.com/Article/details/gxlylymal.sHtML

[G12] 对象转字符串
来源：http://baike.yfazqb.com/Article/details/gjlplzfns.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gsyrfzhah.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gnuyyfwpo.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gotxfmmdr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gooxexqet.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gzerejvut.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gnrsnjutu.sHtML

Ruby: def to_s; @name; end
来源：http://blog.epnwcf.com/Article/details/goxhytqqu.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fktsv.cn/Article/details/gctkxzhem.sHtML

[G13] 判断对象类型
来源：http://baike.sjlbkw.cn/Article/details/gforahdas.sHtML

Py:   isinstance(u, User)
来源：http://m.share.sjlbkw.cn/Article/details/gkbqpvmjh.sHtML

PHP:  $u instanceof User
来源：http://blog.yfazqb.com/Article/details/gwyyfbtyq.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gdilmwjwq.sHtML

TS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gdqcqcdmv.sHtML

Java: u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gzykpgrcw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.sjlbkw.cn/Article/details/giwfjdaka.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.tarul.cn/Article/details/gwcczdllt.sHtML

C#:   u is User
来源：http://blog.vehdjk.com/Article/details/gyhmvbgkw.sHtML

[G14] 数据类 / record
来源：http://www.m.share.tarul.cn/Article/details/gxrnwysft.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.vehdjk.com/Article/details/gtqwvmcpx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.epnwcf.com/Article/details/gnduidclx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.epnwcf.com/Article/details/gxnrahhgn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.yfazqb.com/Article/details/gxkzslxor.sHtML

Java: record User(String name, int age) {}
来源：http://3g.bbcook.cn/Article/details/glmhhphcn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.bbcook.cn/Article/details/gfqzxmzuv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.sjlbkw.cn/Article/details/gaxgjzyys.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.sjlbkw.cn/Article/details/glcvplwno.sHtML

[G15] 枚举
来源：http://blog.yfazqb.com/Article/details/gpsdwtvmm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.bbcook.cn/Article/details/gztqniilt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.yfazqb.com/Article/details/gdcuulyci.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fktsv.cn/Article/details/gtrqotopd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/gwxmzzzax.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.sjlbkw.cn/Article/details/gszybeiqb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.sjlbkw.cn/Article/details/gwlxacvwi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.bbcook.cn/Article/details/gfpeaqenx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.bbcook.cn/Article/details/grgbizqzr.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.tarul.cn/Article/details/gbjpijeax.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.yfazqb.com/Article/details/gtffomgay.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.sjlbkw.cn/Article/details/gycdoeqzp.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gkespjhxj.sHtML

TS:   Object.entries(obj)
来源：http://3g.tarul.cn/Article/details/gfsevdbyu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/gdqowzcex.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/glaffcbok.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/gjmwcthsq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gorduutpp.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gypznuusj.sHtML

H. 异常与错误处理
来源：http://wap.vehdjk.com/Article/details/gfybqplss.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcsncrbeq.sHtML

[H01] try / catch 基础
来源：http://wap.epnwcf.com/Article/details/geypivcst.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.bbcook.cn/Article/details/gbzxgocck.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/grqcenemf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gibpilbfs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/glusiyvta.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.yfazqb.com/Article/details/gfupfuygz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.sjlbkw.cn/Article/details/gfiwxgvzt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.vehdjk.com/Article/details/geincgxhg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/geegtavym.sHtML

[H02] finally / ensure 收尾
来源：http://baike.tarul.cn/Article/details/gygforxpi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.yfazqb.com/Article/details/gqcoxwalo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gowngawqk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gxewyhvgh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gjlspggkz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/ggjrtqanv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.sjlbkw.cn/Article/details/ghkzkerkn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.epnwcf.com/Article/details/gyuktkbdz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.tarul.cn/Article/details/gcwditmuh.sHtML

[H03] 主动抛出异常
来源：http://m.share.epnwcf.com/Article/details/gcbpmbccs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fktsv.cn/Article/details/gklzzgslm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/gqiyrbufa.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/gwbbertvo.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gasnqxeto.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gxihaoklz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.epnwcf.com/Article/details/gqkmvxpec.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.epnwcf.com/Article/details/gsvmaiofr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gueihtwew.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/glclkredm.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.epnwcf.com/Article/details/gqdbvmdjh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/gmtytmpdk.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/gbywceafi.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/guwhqcddy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/grvijuxlg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.epnwcf.com/Article/details/gxbvovqfr.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.yfazqb.com/Article/details/gczzgckdr.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/gghbveddb.sHtML

[H05] 捕获特定类型
来源：http://www.share.bbcook.cn/Article/details/gazrbvkqc.sHtML

Py:   except ValueError as e:
来源：http://www.share.yfazqb.com/Article/details/gdgxjygta.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/gzbmcqujg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gozzvionw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/gicjhijvt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.sjlbkw.cn/Article/details/gzodvpzua.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.yfazqb.com/Article/details/gpoxodedt.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/gcvoymqhi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.tarul.cn/Article/details/gtwvioyrn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/geatwdple.sHtML

Py:   value = d.get("k") or default
来源：http://baike.tarul.cn/Article/details/gewgzocsg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gjhbnkcyq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/glrhtflak.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gorefrkqr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.tarul.cn/Article/details/gbxfzvwyf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.yfazqb.com/Article/details/gnkvumxoo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.tarul.cn/Article/details/gkpdbuist.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.yfazqb.com/Article/details/gxqakmzos.sHtML

[H07] 断言
来源：http://3g.vehdjk.com/Article/details/gjjttetnc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fktsv.cn/Article/details/gwtavcacq.sHtML

PHP:  assert($x > 0);
来源：http://mobile.bbcook.cn/Article/details/gabxoeitx.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.bbcook.cn/Article/details/ggafdpoij.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/gjvafrjly.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gjgtrwtvh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.sjlbkw.cn/Article/details/gvvxyclew.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.yfazqb.com/Article/details/gfbvtxgok.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.bbcook.cn/Article/details/gsppjysbh.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.vehdjk.com/Article/details/gjkwwgoat.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.sjlbkw.cn/Article/details/glvihptsn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.bbcook.cn/Article/details/gkmngison.sHtML

JS:   e.message;  e.stack
来源：http://wap.sjlbkw.cn/Article/details/gyxuapsgq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fktsv.cn/Article/details/gvwzzewcb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.bbcook.cn/Article/details/gkwppebym.sHtML

Go:   err.Error()
来源：http://3g.yfazqb.com/Article/details/gbolwgiim.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.tarul.cn/Article/details/gizoqgyug.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.vehdjk.com/Article/details/gojlpkljn.sHtML

[H09] 带错误码的异常
来源：http://wap.vehdjk.com/Article/details/grhcuvdtc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.epnwcf.com/Article/details/gxsfrtuwi.sHtML


<!-- 参考信息 -->