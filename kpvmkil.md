代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/gybveevdk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gxjrhecww.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gubzhxcds.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.vehdjk.com/Article/details/gtjfbfutm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.vehdjk.com/Article/details/grbflbwwv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/grzkdwegj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.yfazqb.com/Article/details/gcodpobxm.sHtML

[F04] 追加写入文件
来源：http://blog.sjlbkw.cn/Article/details/gqrfzqyqm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.vehdjk.com/Article/details/guzcfdcrj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.bbcook.cn/Article/details/gtkmfnldg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gjnsznrgz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gdiiaagix.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/gjdqgnhgx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fktsv.cn/Article/details/gathspdlx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.vehdjk.com/Article/details/gezcujbqd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.tarul.cn/Article/details/gjsiahqkw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gqgbqxrsv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.vehdjk.com/Article/details/gwmchdicy.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gxtvukwkl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gllgbwcco.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/glzhegjab.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gsurxgkgh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/guvrbgwlz.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.bbcook.cn/Article/details/gansiflxv.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.tarul.cn/Article/details/gkqdkbipn.sHtML

[F06] 删除文件
来源：http://www.share.yfazqb.com/Article/details/ghmfihuoo.sHtML

Py:   os.remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gekkydcza.sHtML

PHP:  unlink("a.txt");
来源：http://wap.tarul.cn/Article/details/ggsoeahhn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gzbxdengs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gcknrrxra.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gfcmcugdc.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gqswwcfer.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/gssynwfib.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/grzbaalos.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.tarul.cn/Article/details/gvisoqejk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gkakfhvrn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.epnwcf.com/Article/details/gvduwmykq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/gzplkxcnl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gikfuurxs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.yfazqb.com/Article/details/gzhlcuuqo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.sjlbkw.cn/Article/details/ggitncbgy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gwkairbal.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/gspnoyxsf.sHtML

[F08] 遍历目录
来源：http://blog.yfazqb.com/Article/details/gwtcifyhw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fktsv.cn/Article/details/ggsfupkjf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gdlwulhfd.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gqlpaozqc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gzzizoewj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gzwdkymwj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gebyvkiiw.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.sjlbkw.cn/Article/details/ggicrsgpq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.vehdjk.com/Article/details/gfyvmumrz.sHtML

[F09] 获取文件大小
来源：http://baike.fktsv.cn/Article/details/gyiehquuf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/golotaebe.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/ghamjhqab.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gxfkwlfnk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gygoxerdz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gbsipeanf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gaquwqmpx.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/gongetpwb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.tarul.cn/Article/details/gvashuhum.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fktsv.cn/Article/details/gfhbixuor.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ggoiamhta.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gqoiblljs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gfxqhzano.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gqwwtcstu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.yfazqb.com/Article/details/gcrgrcosg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gsolpmwgj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaonjrblk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gcitpudis.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/gwufehkvv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gweukegvh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.tarul.cn/Article/details/gspaatbgu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gbzlkqihf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gtbeysvye.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/greznwamm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.vehdjk.com/Article/details/gjcwnjdrw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gosmglaxn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.epnwcf.com/Article/details/gwwumfnuc.sHtML

[F12] CSV 读写
来源：http://wap.sjlbkw.cn/Article/details/gjkfxuzde.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fktsv.cn/Article/details/gjyxhkeyb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fktsv.cn/Article/details/gmqubpjco.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.yfazqb.com/Article/details/gogdxzchc.sHtML

TS:   // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/gesqmckjr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gkdqjvkue.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/gbzbcxnjq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.tarul.cn/Article/details/grunvmdmv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fktsv.cn/Article/details/gfhzdcela.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gksjvzvbz.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/gsjurcdgw.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghytqtvmk.sHtML

[G01] 定义类
来源：http://baike.sjlbkw.cn/Article/details/gvueffdzd.sHtML

Py:   class User: pass
来源：http://baike.bbcook.cn/Article/details/gudpttoza.sHtML

PHP:  class User {}
来源：http://wap.fktsv.cn/Article/details/gleajwjpb.sHtML

JS:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/guohyijza.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.epnwcf.com/Article/details/gjehzwpep.sHtML

Java: class User {}
来源：http://www.share.epnwcf.com/Article/details/gsftnexdg.sHtML

Go:   type User struct { Name string }
来源：http://wap.sjlbkw.cn/Article/details/gszehtjiz.sHtML

Ruby: class User; end
来源：http://baike.tarul.cn/Article/details/grkjxfpbx.sHtML

C#:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gibcnlqmv.sHtML

[G02] 构造函数
来源：http://3g.bbcook.cn/Article/details/gjfjuecbq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.epnwcf.com/Article/details/gwgviljzo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.bbcook.cn/Article/details/gxdtwqyih.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/goffirjye.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fktsv.cn/Article/details/gemsjcpxc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gjmuunrhh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.epnwcf.com/Article/details/gzpcctimc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.epnwcf.com/Article/details/gdmkpuzok.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glpqcqavb.sHtML

[G03] 实例属性
来源：http://wap.fktsv.cn/Article/details/gghkcrxey.sHtML

Py:   self.name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gpqgkmaja.sHtML

PHP:  public string $name = "x";
来源：http://blog.tarul.cn/Article/details/gyuvaenqd.sHtML

JS:   this.name = "x";
来源：http://blog.tarul.cn/Article/details/ggoyxhgqj.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/gtudxuoxp.sHtML

Java: private String name;
来源：http://m.share.yfazqb.com/Article/details/gzqhmwxyr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.tarul.cn/Article/details/ggcqoaaec.sHtML

Ruby: @name = "x"
来源：http://read.share.vehdjk.com/Article/details/gmvlmglcp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fktsv.cn/Article/details/gekqeykob.sHtML

[G04] 定义方法
来源：http://wap.sjlbkw.cn/Article/details/gjdezmnju.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/gfeupemnp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/glyxkaoyt.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gbielnxrb.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gyulddpyz.sHtML

Java: String greet() { return name; }
来源：http://3g.vehdjk.com/Article/details/gbkndejsv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gdaegblef.sHtML

Ruby: def greet; @name; end
来源：http://3g.yfazqb.com/Article/details/ghpnhdyxi.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.tarul.cn/Article/details/glnwurown.sHtML

[G05] 继承
来源：http://3g.vehdjk.com/Article/details/gzcmguovk.sHtML

Py:   class Admin(User): pass
来源：http://blog.vehdjk.com/Article/details/gnnkwxvra.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/grejifckh.sHtML

JS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gpnnxmarw.sHtML

TS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gyjiftymo.sHtML

Java: class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gadfwfpoi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.bbcook.cn/Article/details/gymtswdpa.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fktsv.cn/Article/details/gzwjfbsab.sHtML

C#:   class Admin : User {}
来源：http://wap.sjlbkw.cn/Article/details/gcgdvgnyz.sHtML

[G06] 重写方法
来源：http://www.blog.epnwcf.com/Article/details/gyciutezg.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/gtvovcrwd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gjtuefwzh.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/genohizyr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gqimdyxen.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/giqsidsvr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.epnwcf.com/Article/details/gsngfsdpw.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/gxrkvzvdg.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/gedcxukvm.sHtML

[G07] 调用父类方法
来源：http://mobile.sjlbkw.cn/Article/details/gkulsynhg.sHtML

Py:   super().greet()
来源：http://www.m.share.bbcook.cn/Article/details/gyjyfnztk.sHtML

PHP:  parent::greet();
来源：http://blog.sjlbkw.cn/Article/details/ghdpfvyiu.sHtML

JS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gazxfffhq.sHtML

TS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/ghkqkcade.sHtML

Java: super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gubvxofku.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.sjlbkw.cn/Article/details/gfdhjyeqp.sHtML

Ruby: super
来源：http://mobile.fktsv.cn/Article/details/gmclvmiaf.sHtML

C#:   base.Greet();
来源：http://baike.epnwcf.com/Article/details/gghiftwlz.sHtML

[G08] 静态方法与属性
来源：http://3g.vehdjk.com/Article/details/gvxvsqhdf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fktsv.cn/Article/details/ggfwnibgn.sHtML

PHP:  public static function f() {}
来源：http://read.share.epnwcf.com/Article/details/gqytgsrop.sHtML

JS:   static f() {}
来源：http://www.blog.tarul.cn/Article/details/goszvzlyc.sHtML

TS:   static f(): void {}
来源：http://3g.bbcook.cn/Article/details/gbsqtjxdg.sHtML

Java: static void f() {}
来源：http://read.share.vehdjk.com/Article/details/gzwdhiyxa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.epnwcf.com/Article/details/gxwinuxqd.sHtML

Ruby: def self.f; end
来源：http://www.blog.bbcook.cn/Article/details/gxquoysnk.sHtML

C#:   public static void F() {}
来源：http://baike.sjlbkw.cn/Article/details/gssqurwbf.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.epnwcf.com/Article/details/gkwoupxkf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/gfuggdwzc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.bbcook.cn/Article/details/gjetynrpa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.yfazqb.com/Article/details/gbwnolttm.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fktsv.cn/Article/details/gfjqsdkdu.sHtML

Java: interface Shape { double area(); }
来源：http://baike.vehdjk.com/Article/details/gimnosgfw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/gotvwctdo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.tarul.cn/Article/details/guabjpewi.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.vehdjk.com/Article/details/guvzroyng.sHtML

[G10] 访问控制
来源：http://m.share.tarul.cn/Article/details/gwvgjakes.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gdzkciojj.sHtML

PHP:  public / protected / private
来源：http://wap.yfazqb.com/Article/details/gjwwtqomn.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.vehdjk.com/Article/details/gkgfhxxlw.sHtML

TS:   public / protected / private
来源：http://www.share.fktsv.cn/Article/details/grsliayqr.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.tarul.cn/Article/details/gvtyvubjf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.epnwcf.com/Article/details/gmghujnco.sHtML

Ruby: public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gjcabwpmu.sHtML

C#:   public / protected / private / internal
来源：http://mobile.epnwcf.com/Article/details/grcyjccbb.sHtML

[G11] getter / setter
来源：http://wap.sjlbkw.cn/Article/details/gflvtbyhc.sHtML

Py:   @property 与 @x.setter
来源：http://blog.tarul.cn/Article/details/gnofydqon.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gwcavwqkp.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/ggmurbcze.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/ggcvmcsyw.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gqetvzqsz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gxzlinajq.sHtML

Ruby: attr_accessor :name
来源：http://mobile.bbcook.cn/Article/details/gxhrdtlsl.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/ghqbcacka.sHtML

[G12] 对象转字符串
来源：http://www.blog.yfazqb.com/Article/details/gfiaklnch.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/ghvivruma.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gegagadje.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gzrfhfzuw.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gnacxzakd.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gljrmsxfj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gucfzmgaf.sHtML

Ruby: def to_s; @name; end
来源：http://3g.sjlbkw.cn/Article/details/glrytwvar.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/gufguxsox.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/gvgicuqdk.sHtML

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/gnbmtipah.sHtML

PHP:  $u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/genurtbvh.sHtML

JS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gkhqwddnt.sHtML

TS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gvvquhzbe.sHtML

Java: u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gbwdqpavf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.yfazqb.com/Article/details/gaqvvitfm.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.yfazqb.com/Article/details/gkcimhmoi.sHtML

C#:   u is User
来源：http://www.m.share.epnwcf.com/Article/details/gzvrqvsko.sHtML

[G14] 数据类 / record
来源：http://m.share.epnwcf.com/Article/details/guprznkyb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/gevmvfbep.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/gokrvdazh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.yfazqb.com/Article/details/gaxyxpfxk.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gkxgcztuv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/gikywkhsc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fktsv.cn/Article/details/glrfomaaz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.yfazqb.com/Article/details/gezgnshps.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.epnwcf.com/Article/details/gtycfvlee.sHtML

[G15] 枚举
来源：http://mobile.yfazqb.com/Article/details/gsyvnseqb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.yfazqb.com/Article/details/gvkjsfiso.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.epnwcf.com/Article/details/gkiatymrg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.yfazqb.com/Article/details/ghjxnkryx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/garhuqyju.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.tarul.cn/Article/details/gsfyxrnqz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.yfazqb.com/Article/details/grqdtbtau.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.bbcook.cn/Article/details/gyuqnebys.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/giqvkewzp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.sjlbkw.cn/Article/details/gnehfrydf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.tarul.cn/Article/details/gmisckggw.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.yfazqb.com/Article/details/gzhjwcypm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gzcovfgpc.sHtML

TS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gggcktddq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.bbcook.cn/Article/details/gupffdawr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gussvhjhp.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.tarul.cn/Article/details/gnarskovt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.tarul.cn/Article/details/gyogqzqam.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gklzvwusq.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/glawbqibx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmgbmvgfs.sHtML

[H01] try / catch 基础
来源：http://m.share.bbcook.cn/Article/details/gdnfuzakm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/gcwcopslf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.epnwcf.com/Article/details/guxjpqytd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gajfxgwgq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/glshrxvbl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.epnwcf.com/Article/details/gucxdrsoy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gfcqackiq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.yfazqb.com/Article/details/gbhtkusxo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.bbcook.cn/Article/details/gqzlhdtcx.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.epnwcf.com/Article/details/glrsgtcep.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.epnwcf.com/Article/details/gmsbjenph.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gdeogjrvr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gqaxlseeg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gcaokvqbt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gryidbjky.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.epnwcf.com/Article/details/gaaiotcan.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.tarul.cn/Article/details/gurjnhquu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gfbfoouxz.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gooxjwagj.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.yfazqb.com/Article/details/gzctbasfq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/guenyyfar.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gvclkuoyq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gcuogaogm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gnzumgnkn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhdfmbmm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.epnwcf.com/Article/details/gjulncfhp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gphnkinud.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/glvclatqt.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.sjlbkw.cn/Article/details/gycjacitw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/gnxrsqgxr.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gigrgocdv.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/gnipshbie.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gxowrhoxx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/gfacolior.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.yfazqb.com/Article/details/gihgzuedj.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.epnwcf.com/Article/details/gqunblaiz.sHtML

[H05] 捕获特定类型
来源：http://baike.sjlbkw.cn/Article/details/gqkayjyhj.sHtML

Py:   except ValueError as e:
来源：http://www.share.tarul.cn/Article/details/gtwxgfsye.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.sjlbkw.cn/Article/details/gcczcmxyw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gfgxcaqst.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.bbcook.cn/Article/details/guvslfbdq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpbeviqi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.yfazqb.com/Article/details/gbdxxvfiy.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.vehdjk.com/Article/details/gnsbxdjqc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/gomnfhfcl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.yfazqb.com/Article/details/gnopfljxh.sHtML

Py:   value = d.get("k") or default
来源：http://wap.vehdjk.com/Article/details/gbabigayg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.tarul.cn/Article/details/girwgdhlz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/ggxxwermm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/gmgwgtegy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.sjlbkw.cn/Article/details/gjuxdxngt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.bbcook.cn/Article/details/grqeqtdfj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.yfazqb.com/Article/details/gszcsdanq.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fktsv.cn/Article/details/gntanfvih.sHtML

[H07] 断言
来源：http://mobile.bbcook.cn/Article/details/gufamrgqd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/gnvemxcmb.sHtML

PHP:  assert($x > 0);
来源：http://m.share.epnwcf.com/Article/details/gtjldkcrk.sHtML

JS:   console.assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gmiwhetwh.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.tarul.cn/Article/details/gixcxqtlk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.epnwcf.com/Article/details/gmachotxv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.bbcook.cn/Article/details/gzghaczxh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.bbcook.cn/Article/details/gktiefhgp.sHtML


<!-- 参考信息 -->