代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gidxjtlvg.sHtML

[F06] 删除文件
来源：http://www.m.share.epnwcf.com/Article/details/gmekfwtgd.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gpqtysrmd.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/garxqaqyl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gcejteols.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gmgygkjed.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gugdbhiyo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ghxzzegsl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/grxqadjvg.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gwoeuxrlz.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fktsv.cn/Article/details/gxcwobpvz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gztavzitc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.vehdjk.com/Article/details/gujomgiqw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/glikosviz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gwjxvqdfy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.bbcook.cn/Article/details/gtdtarcag.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/gevlezzfp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.vehdjk.com/Article/details/gyzkquyhp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/gofacpxwo.sHtML

[F08] 遍历目录
来源：http://www.blog.tarul.cn/Article/details/gevkdfeuv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjayxrxl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/grtfjculr.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/ghlbjrdja.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gcnswkcti.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gdelflfqk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fktsv.cn/Article/details/gxtqgkbmi.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/gchmboito.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gsjewamky.sHtML

[F09] 获取文件大小
来源：http://wap.tarul.cn/Article/details/gdohxmapu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gbmitpzpo.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gmdhoqydr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/gqshrzdxs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/ghymlspge.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/grbbktadt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.epnwcf.com/Article/details/galdttohf.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gsnijrdnl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.bbcook.cn/Article/details/gxomjmhxo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.bbcook.cn/Article/details/griqgltmn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gvyiifoly.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gbxjtwvji.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gilcxpgtb.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/gfhjcxsxr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.vehdjk.com/Article/details/gzntsxryz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gmuqlupbi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gjvkvkuqq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gtdthzzjb.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.epnwcf.com/Article/details/ghejqvwxc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gzhbctkex.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gmbuiwqmc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/ghkpdbdme.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gnfwoztnn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.tarul.cn/Article/details/gqjnluwjt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/gctmzuhrx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gnksciiku.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.vehdjk.com/Article/details/gkvqjdopm.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/gywnxcybi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/gupchflwt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.yfazqb.com/Article/details/gbpflrqyo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.bbcook.cn/Article/details/gsfhwqbcb.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gurjvbyfg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.tarul.cn/Article/details/guhmzvhgu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.vehdjk.com/Article/details/gzyuxhpgy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.vehdjk.com/Article/details/gtrodwnwy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.bbcook.cn/Article/details/gstrfavuj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmjfujtbj.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/gjyrrlfry.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/grdkxvrri.sHtML

[G01] 定义类
来源：http://m.share.epnwcf.com/Article/details/gvfugcojm.sHtML

Py:   class User: pass
来源：http://wap.tarul.cn/Article/details/gvimhmumj.sHtML

PHP:  class User {}
来源：http://www.share.yfazqb.com/Article/details/gbmfcvxxy.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gkmmljcpt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/gswzrvzox.sHtML

Java: class User {}
来源：http://read.share.fktsv.cn/Article/details/gryeotran.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/ggdbpvuzs.sHtML

Ruby: class User; end
来源：http://blog.tarul.cn/Article/details/gsinslljs.sHtML

C#:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gqzoztvfd.sHtML

[G02] 构造函数
来源：http://3g.vehdjk.com/Article/details/gstcxfhfx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.vehdjk.com/Article/details/gglevxapr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.bbcook.cn/Article/details/gazvoavvf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gstugwjjy.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.tarul.cn/Article/details/gonybgrbu.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gehufgzsz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fktsv.cn/Article/details/gvxodlnfy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/gdjufgsau.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gigivfmsz.sHtML

[G03] 实例属性
来源：http://mobile.fktsv.cn/Article/details/gcwoaujwd.sHtML

Py:   self.name = "x"
来源：http://mobile.bbcook.cn/Article/details/gtewonbux.sHtML

PHP:  public string $name = "x";
来源：http://3g.tarul.cn/Article/details/ghqjiiogn.sHtML

JS:   this.name = "x";
来源：http://blog.bbcook.cn/Article/details/gtypxqbdr.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/ghqyeymzo.sHtML

Java: private String name;
来源：http://m.share.sjlbkw.cn/Article/details/gnegvwzwd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.sjlbkw.cn/Article/details/gqcbdvjvh.sHtML

Ruby: @name = "x"
来源：http://baike.epnwcf.com/Article/details/glzhmkiyg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.bbcook.cn/Article/details/gjxgalhvo.sHtML

[G04] 定义方法
来源：http://www.share.bbcook.cn/Article/details/gtlhrtzyl.sHtML

Py:   def greet(self): return self.name
来源：http://blog.tarul.cn/Article/details/gvfuqzata.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gzhhceykq.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/glppozujs.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gqpgqxudr.sHtML

Java: String greet() { return name; }
来源：http://m.share.yfazqb.com/Article/details/giqlzchcj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/giewsiaxe.sHtML

Ruby: def greet; @name; end
来源：http://baike.epnwcf.com/Article/details/gedkmwour.sHtML

C#:   public string Greet() => Name;
来源：http://blog.bbcook.cn/Article/details/gjqvxemrb.sHtML

[G05] 继承
来源：http://m.share.yfazqb.com/Article/details/gksyipdue.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.tarul.cn/Article/details/gpfeclkof.sHtML

PHP:  class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/glauoipcm.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gjftjgudb.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/ggsfgawdk.sHtML

Java: class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gxgcpbdzv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.epnwcf.com/Article/details/gawcplgne.sHtML

Ruby: class Admin < User; end
来源：http://3g.tarul.cn/Article/details/gtqzdcyli.sHtML

C#:   class Admin : User {}
来源：http://read.share.tarul.cn/Article/details/gcyyxldof.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/gicqsthcv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/gabjrousp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gsbumhssy.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/ggyvzlvxv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.tarul.cn/Article/details/guytigqap.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwqnatbq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gksjoabov.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.epnwcf.com/Article/details/gcqfjpkxx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.sjlbkw.cn/Article/details/gaeyxoyrv.sHtML

[G07] 调用父类方法
来源：http://read.share.yfazqb.com/Article/details/gdyrckiqu.sHtML

Py:   super().greet()
来源：http://blog.fktsv.cn/Article/details/gtwbalhdt.sHtML

PHP:  parent::greet();
来源：http://mobile.vehdjk.com/Article/details/gwhwrtnia.sHtML

JS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gdyvqqzle.sHtML

TS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gurzzlnoh.sHtML

Java: super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gwvitbfgt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.epnwcf.com/Article/details/gstawmdpg.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/gujmeehcb.sHtML

C#:   base.Greet();
来源：http://www.m.share.epnwcf.com/Article/details/ghipdbwtb.sHtML

[G08] 静态方法与属性
来源：http://read.share.fktsv.cn/Article/details/gbyduulzl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/ghyscfnxw.sHtML

PHP:  public static function f() {}
来源：http://3g.sjlbkw.cn/Article/details/gqvteeaun.sHtML

JS:   static f() {}
来源：http://mobile.bbcook.cn/Article/details/gqwopykvs.sHtML

TS:   static f(): void {}
来源：http://m.share.vehdjk.com/Article/details/gkgcysbyg.sHtML

Java: static void f() {}
来源：http://www.share.tarul.cn/Article/details/gjppbwcsg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gxhihouhc.sHtML

Ruby: def self.f; end
来源：http://www.share.yfazqb.com/Article/details/gltcaveud.sHtML

C#:   public static void F() {}
来源：http://blog.vehdjk.com/Article/details/gvxeojbkx.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.yfazqb.com/Article/details/gaqovapfm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/gnljrfagc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.tarul.cn/Article/details/gfvivceuz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/geyxrsnxy.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.tarul.cn/Article/details/gndtvmgsy.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gtdtzkkan.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.vehdjk.com/Article/details/geicxekyr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.epnwcf.com/Article/details/gyldefdbc.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.yfazqb.com/Article/details/gefujivfb.sHtML

[G10] 访问控制
来源：http://baike.epnwcf.com/Article/details/gdzzpjymj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gtsdbxvdq.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gsznxluar.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fktsv.cn/Article/details/glkziklhq.sHtML

TS:   public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gzlshgsqy.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.vehdjk.com/Article/details/gfkvubswr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.tarul.cn/Article/details/gugtxuhex.sHtML

Ruby: public / protected / private
来源：http://baike.fktsv.cn/Article/details/gxwovddld.sHtML

C#:   public / protected / private / internal
来源：http://wap.yfazqb.com/Article/details/gpltzpxuj.sHtML

[G11] getter / setter
来源：http://read.share.yfazqb.com/Article/details/gqxnuhgjz.sHtML

Py:   @property 与 @x.setter
来源：http://wap.bbcook.cn/Article/details/gsvaswqgo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gsdfjtrhf.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gosenomcv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/galhcowfl.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gglfejkol.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gpbcyphbp.sHtML

Ruby: attr_accessor :name
来源：http://mobile.epnwcf.com/Article/details/gmtjmbvor.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fktsv.cn/Article/details/gnrvvlptd.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gphqpynmv.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.yfazqb.com/Article/details/gxealsrzu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gmxmxzoew.sHtML

JS:   toString() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gotihvsaj.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gyjlsjzar.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fktsv.cn/Article/details/gqtfdrzdj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gzeaxggdd.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gvgmnwxfh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gpbtrfhvg.sHtML

[G13] 判断对象类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkcaexhn.sHtML

Py:   isinstance(u, User)
来源：http://read.share.vehdjk.com/Article/details/gwoxooqph.sHtML

PHP:  $u instanceof User
来源：http://baike.fktsv.cn/Article/details/gggbyfbrf.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/ggbsnjppc.sHtML

TS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gkmarlakp.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gpntgpntz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.tarul.cn/Article/details/gjfxwizpn.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gngyoiltq.sHtML

C#:   u is User
来源：http://www.m.share.epnwcf.com/Article/details/gfziarppg.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/gevxqsvym.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.yfazqb.com/Article/details/gszdddkcc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.vehdjk.com/Article/details/gisxxdoda.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/gflljpdha.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gzwnsiejw.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.sjlbkw.cn/Article/details/gosxxkghz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.sjlbkw.cn/Article/details/gjogyypmv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.tarul.cn/Article/details/glmlbuzaj.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.sjlbkw.cn/Article/details/gxuionfus.sHtML

[G15] 枚举
来源：http://www.m.share.fktsv.cn/Article/details/gtquyqmae.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.vehdjk.com/Article/details/gubixmmyr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.sjlbkw.cn/Article/details/gfknxvnlu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.vehdjk.com/Article/details/gwntjcuqd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gndluiked.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gauupevtf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.yfazqb.com/Article/details/gjlpxnqjb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.sjlbkw.cn/Article/details/gcowfymfj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gxnibkafs.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.sjlbkw.cn/Article/details/gikvqncfk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.bbcook.cn/Article/details/gopbqozhw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/geqkbkpcb.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gtterwjta.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/ghdrxhszg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gkrtenlst.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fktsv.cn/Article/details/gazuxmhnh.sHtML

Ruby: obj.instance_variables
来源：http://3g.yfazqb.com/Article/details/gghtpebsw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/gllxtbmsm.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxdqjtnqo.sHtML

H. 异常与错误处理
来源：http://www.share.bbcook.cn/Article/details/gagdmghyf.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/giqxodgxu.sHtML

[H01] try / catch 基础
来源：http://mobile.yfazqb.com/Article/details/gteuvwgyr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.tarul.cn/Article/details/gfjyhpxlb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/gezayfkwp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/ghpowvmqz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/guhrtnayr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.vehdjk.com/Article/details/gqlllaonp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.vehdjk.com/Article/details/gvngbmgjh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/gifyzxnux.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.epnwcf.com/Article/details/gkqgwvchh.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/gsqlvkmda.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.vehdjk.com/Article/details/gwrixqsfc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gowcdjecw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gzrjooxsl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gcxhmenvy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gjbckyypn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fktsv.cn/Article/details/gkpgoqivt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwxhkrib.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gbqzupido.sHtML

[H03] 主动抛出异常
来源：http://mobile.yfazqb.com/Article/details/ggkzkyomz.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.bbcook.cn/Article/details/gxvmyrmjj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gkgljmyok.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gysdkfiun.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfympkef.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/grmkmqtvd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.tarul.cn/Article/details/gejnegwcw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.vehdjk.com/Article/details/gzvqethui.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gthjsoxat.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gpwaaydcs.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.sjlbkw.cn/Article/details/glratjhqq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gpsdneibw.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gqwndocny.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/gjiutxzoy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.epnwcf.com/Article/details/gzglpfetb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.vehdjk.com/Article/details/gxisigvwm.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.bbcook.cn/Article/details/gjmapacuf.sHtML

C#:   class MyException : Exception {}
来源：http://baike.vehdjk.com/Article/details/guicnwmnx.sHtML

[H05] 捕获特定类型
来源：http://baike.tarul.cn/Article/details/gfocfxquc.sHtML

Py:   except ValueError as e:
来源：http://blog.bbcook.cn/Article/details/gcbttfhxi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.bbcook.cn/Article/details/guwiuvtea.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/gelpujdat.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.yfazqb.com/Article/details/gqcvyntko.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.vehdjk.com/Article/details/gkomrprlv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fktsv.cn/Article/details/gwjrdgnqx.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.epnwcf.com/Article/details/geassaatw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/gsmtmveik.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvyrazvz.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.bbcook.cn/Article/details/gtvobfmtw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gxeihepsi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.yfazqb.com/Article/details/gbltmiofq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gmhnquggg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.epnwcf.com/Article/details/gxhljujio.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.tarul.cn/Article/details/glhusxgps.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.yfazqb.com/Article/details/gednaaqbr.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.epnwcf.com/Article/details/goydyehfi.sHtML

[H07] 断言
来源：http://mobile.fktsv.cn/Article/details/gfnbnsyyn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.vehdjk.com/Article/details/guwumeunr.sHtML

PHP:  assert($x > 0);
来源：http://3g.vehdjk.com/Article/details/gcesjefdi.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/gagkqjjwk.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gibtwkynb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.tarul.cn/Article/details/gablpfnbd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.yfazqb.com/Article/details/ghlebeahy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.vehdjk.com/Article/details/giyycrtxu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gxdxaoomt.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.tarul.cn/Article/details/giuwbzral.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.epnwcf.com/Article/details/gjdxrcxnc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.sjlbkw.cn/Article/details/gcotxhvve.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/gefbijuqw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.bbcook.cn/Article/details/guqxzwzwn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.tarul.cn/Article/details/ggjfeoisr.sHtML

Go:   err.Error()
来源：http://mobile.fktsv.cn/Article/details/gmmawwdlz.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.epnwcf.com/Article/details/griqpgrlo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.epnwcf.com/Article/details/gmtekiump.sHtML

[H09] 带错误码的异常
来源：http://3g.sjlbkw.cn/Article/details/gjteouudb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.vehdjk.com/Article/details/ghuqwqbwo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.tarul.cn/Article/details/gcpkuiszs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.vehdjk.com/Article/details/gbmdicros.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.sjlbkw.cn/Article/details/ghpsfzced.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmpenlhh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.epnwcf.com/Article/details/gicpqczje.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.tarul.cn/Article/details/gorodbkqc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.bbcook.cn/Article/details/gtqajcxme.sHtML

[H10] 资源自动释放
来源：http://m.share.epnwcf.com/Article/details/gyxbgfleu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/gbwuzgkbt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.vehdjk.com/Article/details/gukejpjii.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gubwwsjfa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.yfazqb.com/Article/details/gosjyqven.sHtML


<!-- 参考信息 -->