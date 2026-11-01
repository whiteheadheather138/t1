代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gnvvdlabl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gqxndxyrm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.tarul.cn/Article/details/gmdbqgchc.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/gyqdvraqc.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fktsv.cn/Article/details/gjsdkzkzp.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/ggdcloyrw.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/glaieounr.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gcimumgis.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gquafvtku.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gcjvnkimc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gxonnntmn.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gmfwhatew.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gdxjjycde.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.vehdjk.com/Article/details/grimawoyk.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.epnwcf.com/Article/details/gpyfgwogr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gqzptlfvz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.bbcook.cn/Article/details/gcpzxkfdy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gkkwqurnj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gzxapdxxv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.vehdjk.com/Article/details/geekzutes.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.tarul.cn/Article/details/gzajntmnk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.bbcook.cn/Article/details/gqqdqvkwi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.sjlbkw.cn/Article/details/glwjspaur.sHtML

[F08] 遍历目录
来源：http://baike.epnwcf.com/Article/details/gjndgnype.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.yfazqb.com/Article/details/gfhmtdsds.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.yfazqb.com/Article/details/gwitdboue.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gqplbqwse.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gopyfzbag.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.tarul.cn/Article/details/gsslebggc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gzvswhosa.sHtML

Ruby: Dir.children("dir")
来源：http://wap.vehdjk.com/Article/details/ggvelnncb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/glidpqckk.sHtML

[F09] 获取文件大小
来源：http://blog.tarul.cn/Article/details/grrbsvpqs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fktsv.cn/Article/details/ghmgsbpam.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gjsslkkku.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gpxnondrv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gfxxhcoru.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gapecwofi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fktsv.cn/Article/details/ggykicgzx.sHtML

Ruby: File.size("a.txt")
来源：http://blog.bbcook.cn/Article/details/gugbrrfnw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gwlmaygap.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.vehdjk.com/Article/details/gqhlcdmcy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gabcuqane.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnxhaght.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gsrxxrdhy.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.tarul.cn/Article/details/gxmhcrghw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.epnwcf.com/Article/details/ghwcnrxaw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/ghnnqiiyp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gvdrecbgb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/guqcqnscr.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gxworbynj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gypytsdxw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fktsv.cn/Article/details/gjseqkiyz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gjiplusyu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/geyzjujct.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.sjlbkw.cn/Article/details/ggjmwvodf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.vehdjk.com/Article/details/gnbxpryjy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gddneogxk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/gmuwurfsz.sHtML

[F12] CSV 读写
来源：http://www.share.epnwcf.com/Article/details/gtegxzffc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/gsxefrkxe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.sjlbkw.cn/Article/details/gypmnrbnp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.vehdjk.com/Article/details/guyaklokj.sHtML

TS:   // 同上
来源：http://3g.fktsv.cn/Article/details/gfedianrn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/gehcdghlc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.epnwcf.com/Article/details/guybideyh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.tarul.cn/Article/details/gozfokvll.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fktsv.cn/Article/details/gtzegkaeh.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/guijhzfcd.sHtML

G. 面向对象
来源：http://www.share.epnwcf.com/Article/details/gfzmkpcxe.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkeyxgcqr.sHtML

[G01] 定义类
来源：http://www.share.epnwcf.com/Article/details/gaicrgnpc.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/gyrqdxezy.sHtML

PHP:  class User {}
来源：http://baike.yfazqb.com/Article/details/geqjvmqwh.sHtML

JS:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzwrwomhy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.bbcook.cn/Article/details/gimgfwgec.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/gbebyzlft.sHtML

Go:   type User struct { Name string }
来源：http://wap.sjlbkw.cn/Article/details/govpdfhld.sHtML

Ruby: class User; end
来源：http://www.m.share.fktsv.cn/Article/details/gnrwclrmj.sHtML

C#:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/grubxdysp.sHtML

[G02] 构造函数
来源：http://www.share.fktsv.cn/Article/details/gckufitgd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.vehdjk.com/Article/details/gpakxlmyj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gmfyzdwwa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gnqnocvnu.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.epnwcf.com/Article/details/gpcmamsyv.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gnqwsydno.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.vehdjk.com/Article/details/gdgpbxwbr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gihlgqfvj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/glhldsmxx.sHtML

[G03] 实例属性
来源：http://m.share.epnwcf.com/Article/details/gzwqzjqpk.sHtML

Py:   self.name = "x"
来源：http://read.share.yfazqb.com/Article/details/gtzhfcpkb.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/gxqdgefbs.sHtML

JS:   this.name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gykcjpvpc.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gjtfsmkvm.sHtML

Java: private String name;
来源：http://wap.tarul.cn/Article/details/gphbozadf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.bbcook.cn/Article/details/gphvsqmcy.sHtML

Ruby: @name = "x"
来源：http://m.share.vehdjk.com/Article/details/gxyyjqcvw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.bbcook.cn/Article/details/gtukpgapj.sHtML

[G04] 定义方法
来源：http://read.share.vehdjk.com/Article/details/gfwkmvfkk.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gvkppkewf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gbyaubtne.sHtML

JS:   greet() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gtliiuwrb.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/grdwaqoci.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gfzcxovuz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gdtuzegqs.sHtML

Ruby: def greet; @name; end
来源：http://read.share.bbcook.cn/Article/details/gcmiyxfws.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/gpxmwmmrz.sHtML

[G05] 继承
来源：http://wap.fktsv.cn/Article/details/gtrgufoww.sHtML

Py:   class Admin(User): pass
来源：http://read.share.epnwcf.com/Article/details/gxoxaxlbm.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gloehywvk.sHtML

JS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gwahvifsx.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gdmgbvznw.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gtbsbukyo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gywulplkv.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/gjuuxxnef.sHtML

C#:   class Admin : User {}
来源：http://mobile.epnwcf.com/Article/details/gcfhxqxen.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/gqvxmdbjv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.yfazqb.com/Article/details/gzdnmeftc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/guvmurnzp.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gbmbdugtr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/grpimglnk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gjorhtaca.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.tarul.cn/Article/details/gfsfjtxun.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gsaccdkez.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.epnwcf.com/Article/details/gwrhgajko.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/gplzuzlfz.sHtML

Py:   super().greet()
来源：http://m.share.tarul.cn/Article/details/gclmvbhoe.sHtML

PHP:  parent::greet();
来源：http://baike.fktsv.cn/Article/details/gpudcupxe.sHtML

JS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/guqqzjxai.sHtML

TS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gowxvulmz.sHtML

Java: super.greet();
来源：http://3g.yfazqb.com/Article/details/gnltlckad.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gatevbeps.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/gvokkqeqt.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/gxfayuura.sHtML

[G08] 静态方法与属性
来源：http://3g.tarul.cn/Article/details/gdpqxivgu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.vehdjk.com/Article/details/gkkyhlwrt.sHtML

PHP:  public static function f() {}
来源：http://www.blog.bbcook.cn/Article/details/grvfjtqey.sHtML

JS:   static f() {}
来源：http://www.share.vehdjk.com/Article/details/goamjsynd.sHtML

TS:   static f(): void {}
来源：http://www.m.share.vehdjk.com/Article/details/gbfijnxsp.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/gzhelrkxm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.epnwcf.com/Article/details/gvrfrwrop.sHtML

Ruby: def self.f; end
来源：http://mobile.epnwcf.com/Article/details/gtlxmystu.sHtML

C#:   public static void F() {}
来源：http://www.share.yfazqb.com/Article/details/gmklhzzxc.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.epnwcf.com/Article/details/gkfdemogd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.epnwcf.com/Article/details/gmypgxaiv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/gupxvfqga.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/ggumpnpdt.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.bbcook.cn/Article/details/ghiqnfjan.sHtML

Java: interface Shape { double area(); }
来源：http://blog.vehdjk.com/Article/details/gcoaincjh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/gjuheshxd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.epnwcf.com/Article/details/ggmoirsft.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gldxxtvwz.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/ggwdqnwfq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.bbcook.cn/Article/details/gmrjdnzar.sHtML

PHP:  public / protected / private
来源：http://baike.bbcook.cn/Article/details/gkxeyivuy.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.vehdjk.com/Article/details/glecdxpwu.sHtML

TS:   public / protected / private
来源：http://wap.fktsv.cn/Article/details/glldycmhw.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.epnwcf.com/Article/details/ghlzaezag.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.yfazqb.com/Article/details/gcmpwneko.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gzryyvyxr.sHtML

C#:   public / protected / private / internal
来源：http://3g.epnwcf.com/Article/details/gnsxniimg.sHtML

[G11] getter / setter
来源：http://wap.tarul.cn/Article/details/gdnyuymlv.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.bbcook.cn/Article/details/gdzxnnigs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gzsfvygoy.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/guhonjunp.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gnjvyyyii.sHtML

Java: public String getName() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gjloashuv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gjhcqpini.sHtML

Ruby: attr_accessor :name
来源：http://wap.vehdjk.com/Article/details/gzjxulsqw.sHtML

C#:   public string Name { get; set; }
来源：http://blog.yfazqb.com/Article/details/gksmwpeja.sHtML

[G12] 对象转字符串
来源：http://blog.fktsv.cn/Article/details/gfswhrzbw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/ghkmlgvrb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gjfqnrznu.sHtML

JS:   toString() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gzoijinvm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gnidlwwtd.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fktsv.cn/Article/details/glxbwojbs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.yfazqb.com/Article/details/guvvucgdp.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gvknqvfll.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.epnwcf.com/Article/details/gxtzzhysd.sHtML

[G13] 判断对象类型
来源：http://baike.bbcook.cn/Article/details/gkrfdwofr.sHtML

Py:   isinstance(u, User)
来源：http://m.share.vehdjk.com/Article/details/gdpyjxhhu.sHtML

PHP:  $u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gbrphbbba.sHtML

JS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gyvygmkty.sHtML

TS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gdtsgxqpx.sHtML

Java: u instanceof User
来源：http://wap.vehdjk.com/Article/details/gngutkomf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.yfazqb.com/Article/details/gajybqfje.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.tarul.cn/Article/details/gknkzcxmq.sHtML

C#:   u is User
来源：http://3g.bbcook.cn/Article/details/gsrjaoyvz.sHtML

[G14] 数据类 / record
来源：http://3g.tarul.cn/Article/details/gzmectlbj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.yfazqb.com/Article/details/ggsgkizwd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/gupnustqz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.bbcook.cn/Article/details/gnkvqcbtp.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.sjlbkw.cn/Article/details/gsqdcuyhr.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/gjmlpkirh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.sjlbkw.cn/Article/details/guiihirqz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/gciieqjwx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.yfazqb.com/Article/details/gzjbwmcce.sHtML

[G15] 枚举
来源：http://mobile.vehdjk.com/Article/details/ghfmgcvtz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.yfazqb.com/Article/details/gjkoldrub.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.bbcook.cn/Article/details/gaefzublh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.sjlbkw.cn/Article/details/gwxflxlep.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gqhamkcja.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.epnwcf.com/Article/details/ghtsvkzaz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.epnwcf.com/Article/details/ghcrclozw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/glkslhaqr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gzgaafkcd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.epnwcf.com/Article/details/gbqcgkrvp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.bbcook.cn/Article/details/gzamtzwmj.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.bbcook.cn/Article/details/gtfrtquse.sHtML

JS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gtfzxtvjz.sHtML

TS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gmtztyfcz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.vehdjk.com/Article/details/gsqpyuxqt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.bbcook.cn/Article/details/gyhnesszg.sHtML

Ruby: obj.instance_variables
来源：http://blog.tarul.cn/Article/details/glmitkxov.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/gleoervlz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gulpmofjz.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gpsyguszq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gyjaemgqw.sHtML

[H01] try / catch 基础
来源：http://m.share.bbcook.cn/Article/details/gnauaisnx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.epnwcf.com/Article/details/gybngtsos.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.sjlbkw.cn/Article/details/gnxbbiuza.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gmsmvwyoz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gkdohguii.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.yfazqb.com/Article/details/ggpbdsihs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.vehdjk.com/Article/details/gwuqmfnvo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.epnwcf.com/Article/details/gxbicwpty.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fktsv.cn/Article/details/gbqrykomj.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.sjlbkw.cn/Article/details/gsvidoetb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fktsv.cn/Article/details/gwjwjjpeh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gtngpvriy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gerhiqivw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/ghqbvqesy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/grfsjnomb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.sjlbkw.cn/Article/details/gbycyboay.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.yfazqb.com/Article/details/gmzvxrjkm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gcodwjmuj.sHtML

[H03] 主动抛出异常
来源：http://3g.epnwcf.com/Article/details/gflnmjtxs.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/gyldnjiqs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gzqamdehy.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gveltfbzu.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/gqrisbyzc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gjgmneeil.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fktsv.cn/Article/details/giwrcbugw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.sjlbkw.cn/Article/details/gwmoepzqc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gbmlpbiaj.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnmjfnzn.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.vehdjk.com/Article/details/gzmypezni.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.vehdjk.com/Article/details/gebnlhhkw.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gcnuprfxk.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gknlgpogx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fktsv.cn/Article/details/ghjiirmlq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.sjlbkw.cn/Article/details/ghoxdjtce.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.yfazqb.com/Article/details/gfqesrqqm.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.yfazqb.com/Article/details/gchfelwzs.sHtML

[H05] 捕获特定类型
来源：http://blog.sjlbkw.cn/Article/details/grdtjijqh.sHtML

Py:   except ValueError as e:
来源：http://baike.fktsv.cn/Article/details/gkahbgzbc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.sjlbkw.cn/Article/details/gtgblikrb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gsajmhamk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gasuejtcf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.tarul.cn/Article/details/gmawecgbi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.epnwcf.com/Article/details/gonsdswkd.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.bbcook.cn/Article/details/glbpwhhma.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.yfazqb.com/Article/details/gitjrgbmr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.bbcook.cn/Article/details/gpkeuhuli.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/gviuanfde.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gkyaeeqvi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/grgdbtxpq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/grmetbfgq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fktsv.cn/Article/details/gwaumisfz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.yfazqb.com/Article/details/gzmmtcptz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.epnwcf.com/Article/details/ggyzjlpdk.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.epnwcf.com/Article/details/gcirbdvyt.sHtML

[H07] 断言
来源：http://www.share.fktsv.cn/Article/details/gzkzlvqte.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.epnwcf.com/Article/details/gzfoujhei.sHtML

PHP:  assert($x > 0);
来源：http://3g.epnwcf.com/Article/details/gtufcsnse.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fktsv.cn/Article/details/gbqimjizi.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gvgqahrre.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.bbcook.cn/Article/details/glmokjefw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.sjlbkw.cn/Article/details/goluhqvfs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.sjlbkw.cn/Article/details/gmjhtmgji.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gmiefmgle.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.yfazqb.com/Article/details/gfyqsgumw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fktsv.cn/Article/details/gejqnafgu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fktsv.cn/Article/details/ggpkojbdt.sHtML

JS:   e.message;  e.stack
来源：http://mobile.vehdjk.com/Article/details/gncofqbvj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.yfazqb.com/Article/details/gqghwnmxi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.bbcook.cn/Article/details/grtwaqobi.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/gumcgrrte.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fktsv.cn/Article/details/gqxxdvcaf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.tarul.cn/Article/details/gllpwmwlt.sHtML

[H09] 带错误码的异常
来源：http://m.share.yfazqb.com/Article/details/ghkidhwof.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gbfjyqlkt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fktsv.cn/Article/details/gcnwgdjvp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.vehdjk.com/Article/details/gjnrcrkdj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.sjlbkw.cn/Article/details/gujntcxpr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.epnwcf.com/Article/details/ggcqjrmgg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gotfobxpi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fktsv.cn/Article/details/gtscsltta.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.vehdjk.com/Article/details/gtptbsxga.sHtML

[H10] 资源自动释放
来源：http://baike.vehdjk.com/Article/details/gtuotebqv.sHtML


<!-- 参考信息 -->