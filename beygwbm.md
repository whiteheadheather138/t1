代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gtacgrlmh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/ggbnegohu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.tarul.cn/Article/details/glinrsuvf.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.vehdjk.com/Article/details/gwmwshgme.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.yfazqb.com/Article/details/gwtgzzszg.sHtML

[F06] 删除文件
来源：http://blog.bbcook.cn/Article/details/gzapyvhlp.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gvemkxvcr.sHtML

PHP:  unlink("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gggjfgnvo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gvlrcehht.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gmlztbpzd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gssaefbcc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gmisgdups.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.vehdjk.com/Article/details/grllxfokw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.tarul.cn/Article/details/ghyryhihg.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/gxisvbuxu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gooatwrzs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.yfazqb.com/Article/details/gxmbkrvrr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/glpolzhsn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gmipxrmfk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/gzamiscoq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fktsv.cn/Article/details/grzajzsnb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.sjlbkw.cn/Article/details/gnlivfoaz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gwauhmfxr.sHtML

[F08] 遍历目录
来源：http://baike.yfazqb.com/Article/details/gaurytntm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.bbcook.cn/Article/details/gduloyyeu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gkvuonqgr.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gqvhruwra.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gwofmsnjc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gvwzjolpd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.tarul.cn/Article/details/gfgydryod.sHtML

Ruby: Dir.children("dir")
来源：http://3g.epnwcf.com/Article/details/gugxrbmse.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.tarul.cn/Article/details/ggjnqxkqt.sHtML

[F09] 获取文件大小
来源：http://baike.epnwcf.com/Article/details/ggbwyimmk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/gwmjcbblw.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gpjjlsjkr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gsxgjilov.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gyxmvlllg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gbykuktdx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fktsv.cn/Article/details/gkidcgxxd.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gpfpzggad.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.sjlbkw.cn/Article/details/gdzuoluht.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.epnwcf.com/Article/details/gqgdigfus.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gzqjozyhs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.tarul.cn/Article/details/gqrgdtalc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/grqjodnbc.sHtML

TS:   path.extname("a.txt")
来源：http://wap.vehdjk.com/Article/details/gtlfjlmtv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.yfazqb.com/Article/details/gbaqmxeqy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/grflwirsz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gyetflyxe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gywbudupd.sHtML

[F11] 复制与移动文件
来源：http://baike.vehdjk.com/Article/details/gglhegcta.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gtvchyojb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.bbcook.cn/Article/details/guvcgeltq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gsqojzvfa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gxgxcuurp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gzfvjrzpp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.epnwcf.com/Article/details/gihladwro.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gracllgbi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.vehdjk.com/Article/details/giueiaazd.sHtML

[F12] CSV 读写
来源：http://mobile.sjlbkw.cn/Article/details/gwlvccppi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gkbprzbal.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/gzpxadaqn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.sjlbkw.cn/Article/details/giwmlmhfm.sHtML

TS:   // 同上
来源：http://www.m.share.vehdjk.com/Article/details/geanoyxwc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/gahphsyyi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gkdhtpcxd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/giiaawcwu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fktsv.cn/Article/details/geeuywsos.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gwillinqq.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/gwndsvsjm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxnabnmkz.sHtML

[G01] 定义类
来源：http://www.blog.tarul.cn/Article/details/gxqoefiga.sHtML

Py:   class User: pass
来源：http://mobile.vehdjk.com/Article/details/gredjvzzl.sHtML

PHP:  class User {}
来源：http://wap.epnwcf.com/Article/details/goochymxu.sHtML

JS:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gomqpwjty.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/gqwihputp.sHtML

Java: class User {}
来源：http://blog.yfazqb.com/Article/details/gqptwptub.sHtML

Go:   type User struct { Name string }
来源：http://read.share.tarul.cn/Article/details/gnhfbmidv.sHtML

Ruby: class User; end
来源：http://read.share.fktsv.cn/Article/details/gimczgzeb.sHtML

C#:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gnazqtnvk.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gkccqpcik.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.bbcook.cn/Article/details/gscwxdnmy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.vehdjk.com/Article/details/gaiqsdduy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gkwfwyrnx.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.vehdjk.com/Article/details/gvnnbyhcx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gzmoycrjr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fktsv.cn/Article/details/gffcrklkx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.sjlbkw.cn/Article/details/gaifkajpe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.yfazqb.com/Article/details/gbsutrlgc.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gevkhyaez.sHtML

Py:   self.name = "x"
来源：http://blog.epnwcf.com/Article/details/gzwqbqeap.sHtML

PHP:  public string $name = "x";
来源：http://mobile.yfazqb.com/Article/details/gybvjgpvf.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gdymwjovm.sHtML

TS:   name: string = "x";
来源：http://3g.vehdjk.com/Article/details/gvaussnyn.sHtML

Java: private String name;
来源：http://baike.vehdjk.com/Article/details/gyrgkemkx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.bbcook.cn/Article/details/godmfngtl.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/gcyhhrmgp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/gweitnuya.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/gvxlvtzww.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/ghgpftqrw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gzeyllsds.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gdzdfwbnk.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/ggstidreu.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gvvlskaqr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gnwzpiouz.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/grkzexgvh.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.vehdjk.com/Article/details/gwhzzhglm.sHtML

[G05] 继承
来源：http://www.share.fktsv.cn/Article/details/gsdbdbufl.sHtML

Py:   class Admin(User): pass
来源：http://wap.epnwcf.com/Article/details/gfmzcextg.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/ghrercmgn.sHtML

JS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/goaxbsrgp.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/giyptydef.sHtML

Java: class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gcytfogfz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/grrpkytyz.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fktsv.cn/Article/details/gpdomnklc.sHtML

C#:   class Admin : User {}
来源：http://baike.vehdjk.com/Article/details/gvathivug.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/gjbflidaq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.tarul.cn/Article/details/gavozubrn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gkmaxeapv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gfdxmpyir.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gmgjucivl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gufqeawiq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.vehdjk.com/Article/details/gxabofolr.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.epnwcf.com/Article/details/gmtmfcyav.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gpyamfibu.sHtML

[G07] 调用父类方法
来源：http://read.share.vehdjk.com/Article/details/grmuliude.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/gkpfcioob.sHtML

PHP:  parent::greet();
来源：http://www.blog.bbcook.cn/Article/details/gpzhqdwgo.sHtML

JS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/giwknpyeh.sHtML

TS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/glkmccewn.sHtML

Java: super.greet();
来源：http://read.share.tarul.cn/Article/details/ghevdmrsf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.tarul.cn/Article/details/gvbctgkyj.sHtML

Ruby: super
来源：http://www.share.bbcook.cn/Article/details/gfytzpalw.sHtML

C#:   base.Greet();
来源：http://www.m.share.yfazqb.com/Article/details/gwjebzdnu.sHtML

[G08] 静态方法与属性
来源：http://3g.vehdjk.com/Article/details/gwkkpfamk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.vehdjk.com/Article/details/grewgybyc.sHtML

PHP:  public static function f() {}
来源：http://blog.sjlbkw.cn/Article/details/gyepzhlef.sHtML

JS:   static f() {}
来源：http://baike.tarul.cn/Article/details/gkedntmoh.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fktsv.cn/Article/details/gjzcexzgb.sHtML

Java: static void f() {}
来源：http://baike.yfazqb.com/Article/details/ggelgeusk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fktsv.cn/Article/details/gppwmlqek.sHtML

Ruby: def self.f; end
来源：http://wap.epnwcf.com/Article/details/gbnnfpirv.sHtML

C#:   public static void F() {}
来源：http://m.share.vehdjk.com/Article/details/gzkghwfvx.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.epnwcf.com/Article/details/gboktihda.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.vehdjk.com/Article/details/goolfqlya.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.yfazqb.com/Article/details/gdxwrmqkh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.tarul.cn/Article/details/gnjxwjqho.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.epnwcf.com/Article/details/gmdafucmi.sHtML

Java: interface Shape { double area(); }
来源：http://blog.bbcook.cn/Article/details/gdlsfudnv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gnzklrjmh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.bbcook.cn/Article/details/gsqrfafyx.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.epnwcf.com/Article/details/gsrxcqydd.sHtML

[G10] 访问控制
来源：http://www.blog.epnwcf.com/Article/details/gnwudbduo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.sjlbkw.cn/Article/details/gxvyfonhi.sHtML

PHP:  public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gtnwdbxqt.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fktsv.cn/Article/details/guqeqmjfa.sHtML

TS:   public / protected / private
来源：http://3g.vehdjk.com/Article/details/geahfvjpe.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/gwtbfuths.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.epnwcf.com/Article/details/gliwirjjn.sHtML

Ruby: public / protected / private
来源：http://wap.epnwcf.com/Article/details/gsxbjemor.sHtML

C#:   public / protected / private / internal
来源：http://www.share.tarul.cn/Article/details/gryidoaak.sHtML

[G11] getter / setter
来源：http://www.blog.yfazqb.com/Article/details/gnanejglg.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/gnudcayea.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gwodcxbas.sHtML

JS:   get name() { return this._name; }
来源：http://baike.yfazqb.com/Article/details/golybqurh.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gmzozvgcj.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gmajhkdek.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gynxfwtvi.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/gxipearjs.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/gjhzagejl.sHtML

[G12] 对象转字符串
来源：http://baike.bbcook.cn/Article/details/ghhiypnhe.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gaimpiiem.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gqnimbbtp.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/ghvrnzhpq.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gtqqyjvtz.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.yfazqb.com/Article/details/gsbvpenij.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gkomcdyoa.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fktsv.cn/Article/details/gpakipzhc.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gwbfzntxm.sHtML

[G13] 判断对象类型
来源：http://baike.vehdjk.com/Article/details/gficnfgek.sHtML

Py:   isinstance(u, User)
来源：http://read.share.tarul.cn/Article/details/guetcoawa.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/gmciqjgoc.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/golbzrtvd.sHtML

TS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/ghermittl.sHtML

Java: u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gmttquikf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fktsv.cn/Article/details/ghyzdtijj.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gabehknik.sHtML

C#:   u is User
来源：http://read.share.bbcook.cn/Article/details/gusaffhzt.sHtML

[G14] 数据类 / record
来源：http://www.share.bbcook.cn/Article/details/gnomznydn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/gbdjltkie.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.vehdjk.com/Article/details/gclygibof.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.tarul.cn/Article/details/gbnkjlmac.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/gmwckntmz.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.tarul.cn/Article/details/gclijdcem.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.epnwcf.com/Article/details/gegaaschw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.vehdjk.com/Article/details/goianivlh.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/gnckhorct.sHtML

[G15] 枚举
来源：http://www.blog.tarul.cn/Article/details/grgoakbpn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fktsv.cn/Article/details/gvhdpcgdt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.epnwcf.com/Article/details/gmbzbfolz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fktsv.cn/Article/details/gkqexgmxt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/ghltwzgcw.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fktsv.cn/Article/details/gibczabni.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.sjlbkw.cn/Article/details/gjxaegiaq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.tarul.cn/Article/details/gixtvgjom.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/guhrtnjsd.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.tarul.cn/Article/details/gjelujbor.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.yfazqb.com/Article/details/gqfcvbuwu.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.vehdjk.com/Article/details/gfrqvhiiv.sHtML

JS:   Object.entries(obj)
来源：http://baike.yfazqb.com/Article/details/gwseymlmo.sHtML

TS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gdkzzwemq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gttsjvbyk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.bbcook.cn/Article/details/gbrhgzzaq.sHtML

Ruby: obj.instance_variables
来源：http://3g.fktsv.cn/Article/details/gemqvxxcn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gjmecddit.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfpvffcos.sHtML

H. 异常与错误处理
来源：http://wap.fktsv.cn/Article/details/gldlutxld.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gadsjdygr.sHtML

[H01] try / catch 基础
来源：http://read.share.fktsv.cn/Article/details/gihxognqe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/gyyaxvsgk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fktsv.cn/Article/details/gepltydex.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqivqjess.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/guipnpbvo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.yfazqb.com/Article/details/gdmpnkhia.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.tarul.cn/Article/details/grxpeamgp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.tarul.cn/Article/details/gyokptviw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.vehdjk.com/Article/details/goevqdhhe.sHtML

[H02] finally / ensure 收尾
来源：http://wap.tarul.cn/Article/details/gydamdqop.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.tarul.cn/Article/details/gexddfjgj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gepvoruhf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gnzrcexms.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gztozivwm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gmiqzalpk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.vehdjk.com/Article/details/gwqpdpbdf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.epnwcf.com/Article/details/gqkgrvxrn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/ghxqzctyf.sHtML

[H03] 主动抛出异常
来源：http://3g.vehdjk.com/Article/details/gnxqommbt.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fktsv.cn/Article/details/ggtfduexo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gtvuaepav.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gfzmhpsdh.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/glewdpwik.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gvpbglyag.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.tarul.cn/Article/details/gttouspnb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.bbcook.cn/Article/details/grqsvuotd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gzycjxmgp.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/glsmzwaoy.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.vehdjk.com/Article/details/gxucqjcon.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/gcgbnlpwu.sHtML

JS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/genwumsvw.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gvhlndbsm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/grbxlpedd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/gjkxkatvc.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/gweevejea.sHtML

C#:   class MyException : Exception {}
来源：http://baike.vehdjk.com/Article/details/gzojfvriw.sHtML

[H05] 捕获特定类型
来源：http://read.share.yfazqb.com/Article/details/gqvusevut.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/gytsygfxw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.tarul.cn/Article/details/gsbkvzmuz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fktsv.cn/Article/details/grdmnxcmn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.bbcook.cn/Article/details/gssqjdcom.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.bbcook.cn/Article/details/gghoznxmy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.bbcook.cn/Article/details/gauaesdnk.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/gngumvnht.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.vehdjk.com/Article/details/gyvzezbez.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.vehdjk.com/Article/details/ggqkggdzu.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.tarul.cn/Article/details/gzcsttitg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gecenxrxb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.bbcook.cn/Article/details/gikebobus.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gimhiplnm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.tarul.cn/Article/details/gjbiutgus.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.bbcook.cn/Article/details/gtgqscopl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.tarul.cn/Article/details/gerblbujg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqmxckct.sHtML

[H07] 断言
来源：http://mobile.epnwcf.com/Article/details/gyujkdpqi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.bbcook.cn/Article/details/gtfsbbbyn.sHtML

PHP:  assert($x > 0);
来源：http://wap.vehdjk.com/Article/details/ginjkggty.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gsuishvun.sHtML

TS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gohuylihl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fktsv.cn/Article/details/gzvqldjzy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.bbcook.cn/Article/details/ggyufhnrv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fktsv.cn/Article/details/gcqesgmxg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gxqyswpao.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.vehdjk.com/Article/details/gofimyubu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.bbcook.cn/Article/details/gkqtpfleg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.epnwcf.com/Article/details/geqxcmxbc.sHtML

JS:   e.message;  e.stack
来源：http://blog.bbcook.cn/Article/details/guddbgepm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.epnwcf.com/Article/details/gfixdbzvg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fktsv.cn/Article/details/ghfqvgflz.sHtML

Go:   err.Error()
来源：http://blog.epnwcf.com/Article/details/gvzthfzur.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.tarul.cn/Article/details/gwxvqydep.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.vehdjk.com/Article/details/gqsbcyiae.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/grutfapyl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.tarul.cn/Article/details/gbvoynnfg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.yfazqb.com/Article/details/gcfheidvz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.bbcook.cn/Article/details/gyhqmqons.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.bbcook.cn/Article/details/gggcteute.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.yfazqb.com/Article/details/gepfccddk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.tarul.cn/Article/details/gfimelcgj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fktsv.cn/Article/details/giozdtovl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.tarul.cn/Article/details/gdolxoqmj.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gxjozivnb.sHtML


<!-- 参考信息 -->