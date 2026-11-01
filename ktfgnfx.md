代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gdemszuao.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gdpokfrfv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gievjcmch.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.tarul.cn/Article/details/gamklvlzi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.bbcook.cn/Article/details/gigmwfziu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/goutrmjyj.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.sjlbkw.cn/Article/details/gyeslzskx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.vehdjk.com/Article/details/glzrkaujf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gdlrofhiu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gbbhgbufu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gwecwprou.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/gjafjexqk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/gbdtskigx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/gwkgjsmkt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/geobzktzt.sHtML

[F04] 追加写入文件
来源：http://3g.epnwcf.com/Article/details/guwasindt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.epnwcf.com/Article/details/gcdenskrr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.bbcook.cn/Article/details/geffynqmd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/gkhgacylc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.bbcook.cn/Article/details/gkfmimvti.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.yfazqb.com/Article/details/grgnuizjx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.yfazqb.com/Article/details/gunnimeki.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/ginhpqais.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fktsv.cn/Article/details/gjnkrrbfm.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.vehdjk.com/Article/details/gqhkqzcsw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.sjlbkw.cn/Article/details/gotabczlk.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.tarul.cn/Article/details/gtekphiyl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gietqvjuj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gdocovbsc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gaawayqse.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.epnwcf.com/Article/details/gyseohcqh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gszilnyed.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gyjwptpoa.sHtML

[F06] 删除文件
来源：http://m.share.tarul.cn/Article/details/ghymedevi.sHtML

Py:   os.remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/ggknkfaca.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/gsiosezyb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/ghlhitsop.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gnyhfdhuq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gyrfgggdu.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gdxmqrtun.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ggrfkatpk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gakjkydbi.sHtML

[F07] 创建目录（含多级）
来源：http://wap.vehdjk.com/Article/details/gmpjmgcqu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fktsv.cn/Article/details/gwakbpffv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.epnwcf.com/Article/details/gbafhrmhh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gkuhuxocd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gslfbmcth.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.vehdjk.com/Article/details/gidgeyavs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.epnwcf.com/Article/details/gncuyrpwd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fktsv.cn/Article/details/ggouxcapi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.yfazqb.com/Article/details/gzdextxdh.sHtML

[F08] 遍历目录
来源：http://www.blog.yfazqb.com/Article/details/gkgbdqzwv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.bbcook.cn/Article/details/gdodmrktm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/gzhyhimyl.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gwqenctzt.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gmsrlzfzs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/gmextwjjs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.epnwcf.com/Article/details/giwvzzano.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.epnwcf.com/Article/details/gcdpgujyi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.yfazqb.com/Article/details/gvrlalpym.sHtML

[F09] 获取文件大小
来源：http://3g.sjlbkw.cn/Article/details/gwvwivdti.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gfcjngisr.sHtML

PHP:  filesize("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gbkbkktwz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gyrpackqv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/gguhiycun.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gxypgszzx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.yfazqb.com/Article/details/grgnzqmbh.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gcuacsafb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fktsv.cn/Article/details/gnwirazah.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fktsv.cn/Article/details/glkpngfrx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gonkhaezs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.yfazqb.com/Article/details/gdrdvtgmm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gmxdrxems.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gopchoqwx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.tarul.cn/Article/details/gjdoqcqam.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/glbaqylyp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gwzzketll.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gjgxbyxcn.sHtML

[F11] 复制与移动文件
来源：http://wap.sjlbkw.cn/Article/details/gpbjhuboi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/glzadcjrn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.epnwcf.com/Article/details/gqgjjeoak.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gzhbabqbb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gkjdkghri.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqwwfmhv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/gdllcvdvs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/grpmyqikh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.bbcook.cn/Article/details/giwnmrlex.sHtML

[F12] CSV 读写
来源：http://wap.tarul.cn/Article/details/gnnywpknq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/grnmvaldx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.bbcook.cn/Article/details/gzwzxkxkb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.sjlbkw.cn/Article/details/gntehkcwv.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/gasjdnbpx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.epnwcf.com/Article/details/gwuzvzvok.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.sjlbkw.cn/Article/details/gijztgxot.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.bbcook.cn/Article/details/gmzjvkexa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/ghrdkktsd.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ghschtzkk.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/gbmlbbtpj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gjkinpvyj.sHtML

[G01] 定义类
来源：http://read.share.fktsv.cn/Article/details/ggdoxuchf.sHtML

Py:   class User: pass
来源：http://wap.sjlbkw.cn/Article/details/gapicyuzx.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gxohlazkn.sHtML

JS:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gntzwewxn.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.tarul.cn/Article/details/gjrjskxof.sHtML

Java: class User {}
来源：http://www.share.bbcook.cn/Article/details/gurkurmlb.sHtML

Go:   type User struct { Name string }
来源：http://mobile.epnwcf.com/Article/details/gxomwfiuf.sHtML

Ruby: class User; end
来源：http://www.blog.vehdjk.com/Article/details/gijlqfpck.sHtML

C#:   class User {}
来源：http://m.share.vehdjk.com/Article/details/gdzbysknj.sHtML

[G02] 构造函数
来源：http://blog.sjlbkw.cn/Article/details/gswsoates.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.yfazqb.com/Article/details/gumurqeck.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.yfazqb.com/Article/details/gnardaeqo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/glgrggebg.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.sjlbkw.cn/Article/details/gxsfrocbc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gcojegvat.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fktsv.cn/Article/details/grpsjhcjf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fktsv.cn/Article/details/gecggrksn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gkcztzqme.sHtML

[G03] 实例属性
来源：http://www.share.yfazqb.com/Article/details/gvhidprmo.sHtML

Py:   self.name = "x"
来源：http://www.blog.epnwcf.com/Article/details/ggmvppthr.sHtML

PHP:  public string $name = "x";
来源：http://m.share.vehdjk.com/Article/details/gjvtgbzka.sHtML

JS:   this.name = "x";
来源：http://m.share.bbcook.cn/Article/details/gwxubrmru.sHtML

TS:   name: string = "x";
来源：http://www.share.tarul.cn/Article/details/ghwhiyhqm.sHtML

Java: private String name;
来源：http://www.share.epnwcf.com/Article/details/ggnownmtf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fktsv.cn/Article/details/grkunadyp.sHtML

Ruby: @name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gcmfpdmwo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.sjlbkw.cn/Article/details/ggwhngpmu.sHtML

[G04] 定义方法
来源：http://3g.sjlbkw.cn/Article/details/gjesmsgks.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/glrfnskyc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gthfzlrfe.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gwsdqaclv.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gpztuknih.sHtML

Java: String greet() { return name; }
来源：http://wap.vehdjk.com/Article/details/grygywodo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gflakxwje.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/gteuuvzqh.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.bbcook.cn/Article/details/gevqbnrze.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/gzpwrclwx.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.tarul.cn/Article/details/gmkicvmyf.sHtML

PHP:  class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gqzcqvogi.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gevezywwa.sHtML

TS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gpypdakxx.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/glhiojrip.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/gbdgikbpe.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gkjrralox.sHtML

C#:   class Admin : User {}
来源：http://m.share.fktsv.cn/Article/details/gpzsebbvb.sHtML

[G06] 重写方法
来源：http://3g.vehdjk.com/Article/details/gxhgmmyib.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.vehdjk.com/Article/details/gpfnbkrea.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gujacgijr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gzududker.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gcogsejix.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gjvuiphyi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.sjlbkw.cn/Article/details/gbipzgbdv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/gbyvqxzyy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.epnwcf.com/Article/details/gkrzfbkln.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gxiawvdwm.sHtML

Py:   super().greet()
来源：http://www.blog.vehdjk.com/Article/details/gnruiwxtn.sHtML

PHP:  parent::greet();
来源：http://3g.yfazqb.com/Article/details/gjvoevcgx.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/guajqsfdh.sHtML

TS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gajvghuee.sHtML

Java: super.greet();
来源：http://wap.bbcook.cn/Article/details/ggkngnblt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.bbcook.cn/Article/details/grfxjbokg.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/gbpjlaokk.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/grzqzsgdv.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.yfazqb.com/Article/details/gdsihiuon.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/gvpozjapp.sHtML

PHP:  public static function f() {}
来源：http://m.share.bbcook.cn/Article/details/gcdspombm.sHtML

JS:   static f() {}
来源：http://3g.yfazqb.com/Article/details/gpliltgpf.sHtML

TS:   static f(): void {}
来源：http://wap.tarul.cn/Article/details/ginsafpxa.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gnpfqfgiz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.tarul.cn/Article/details/gtlapkqnq.sHtML

Ruby: def self.f; end
来源：http://www.m.share.tarul.cn/Article/details/gfiuvvzsp.sHtML

C#:   public static void F() {}
来源：http://baike.yfazqb.com/Article/details/grjftrdgx.sHtML

[G09] 接口 / 抽象类
来源：http://baike.yfazqb.com/Article/details/gbmlsyizh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fktsv.cn/Article/details/gwrjyewjd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/gasbtaqur.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.vehdjk.com/Article/details/gyywlstpg.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/gbzpxtuwx.sHtML

Java: interface Shape { double area(); }
来源：http://baike.tarul.cn/Article/details/gcwqhlfgv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/gqdkhmwfw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/gjcakhqpf.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.tarul.cn/Article/details/guvqmkzsn.sHtML

[G10] 访问控制
来源：http://www.m.share.fktsv.cn/Article/details/gcfenrgqh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.tarul.cn/Article/details/grifgumhc.sHtML

PHP:  public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gnotytpau.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gwmmujnfq.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/ghatiryzp.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/glccmepcm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.bbcook.cn/Article/details/ggijkqfpb.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gtuimjjej.sHtML

C#:   public / protected / private / internal
来源：http://m.share.sjlbkw.cn/Article/details/gwajodzfv.sHtML

[G11] getter / setter
来源：http://www.m.share.tarul.cn/Article/details/gfvgibady.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.tarul.cn/Article/details/gbshujkrn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/ghqxcxbqv.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/gkczrvevn.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gpelciuyq.sHtML

Java: public String getName() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gwqzypodo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gpmhsfbce.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/gtaouuowa.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fktsv.cn/Article/details/gmmsykkzc.sHtML

[G12] 对象转字符串
来源：http://read.share.epnwcf.com/Article/details/gjrrerbwg.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/giglruusp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gxflfsimo.sHtML

JS:   toString() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gvqvuikqw.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gnoitnvvw.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.bbcook.cn/Article/details/gznibewdp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gcicqdgfz.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/grjbyhstq.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.yfazqb.com/Article/details/gizmelpui.sHtML

[G13] 判断对象类型
来源：http://m.share.tarul.cn/Article/details/grklsqpbn.sHtML

Py:   isinstance(u, User)
来源：http://www.share.epnwcf.com/Article/details/gmcyzfbly.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gcndjwxff.sHtML

JS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/ghblnqwqy.sHtML

TS:   u instanceof User
来源：http://blog.fktsv.cn/Article/details/gbeadrnfm.sHtML

Java: u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/ggtnrbrel.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.epnwcf.com/Article/details/gptywbrdg.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.sjlbkw.cn/Article/details/gbaidigbc.sHtML

C#:   u is User
来源：http://mobile.vehdjk.com/Article/details/gqpcveeys.sHtML

[G14] 数据类 / record
来源：http://blog.tarul.cn/Article/details/grrfipyms.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gvbtyszgc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.vehdjk.com/Article/details/gqmgtcbqa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/gdfknzmjz.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.vehdjk.com/Article/details/gcwqhybia.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.tarul.cn/Article/details/gyupkuaia.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.epnwcf.com/Article/details/gdlrpxiyq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.bbcook.cn/Article/details/grmvlonkz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.yfazqb.com/Article/details/gstqqecjd.sHtML

[G15] 枚举
来源：http://www.m.share.epnwcf.com/Article/details/gpncsshlb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.yfazqb.com/Article/details/gsscqipts.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.bbcook.cn/Article/details/gecivhlac.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fktsv.cn/Article/details/gxndugvbf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/gdkwzivfl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.bbcook.cn/Article/details/gwvpvvrme.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtudodbv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.yfazqb.com/Article/details/gjxkuhytp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gqzxxjlhs.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.bbcook.cn/Article/details/gfbrlxpzm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/ggfuzyffq.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.epnwcf.com/Article/details/gflbpzryd.sHtML

JS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gdynmddiv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/grwhqbttr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.bbcook.cn/Article/details/gjqbxeqkn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/gbjgwtgre.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/gsypulwad.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.tarul.cn/Article/details/gfuikfveu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gvxemrczk.sHtML

H. 异常与错误处理
来源：http://m.share.fktsv.cn/Article/details/gzbglzuqk.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghbaduyic.sHtML

[H01] try / catch 基础
来源：http://mobile.epnwcf.com/Article/details/gkxqebyab.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.vehdjk.com/Article/details/gcjggqbnq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfjkxzat.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/gwnnjykmm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gynllkiho.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/gdxevgpke.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/gbzohvrja.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.sjlbkw.cn/Article/details/geelrocvc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.yfazqb.com/Article/details/gvoqpwbez.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/gomduhsow.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.yfazqb.com/Article/details/gcaulnlpb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/guuxlumoy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gznpoycgb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gqqndnhdl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/guwmttunx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.bbcook.cn/Article/details/gpqwaftkg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.tarul.cn/Article/details/gusnufpzf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/grbuihqux.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.yfazqb.com/Article/details/grllgtltw.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.sjlbkw.cn/Article/details/gutrttttb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gzqggauvs.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/grqnponxh.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gcnltcrxk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gzthroqyb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.bbcook.cn/Article/details/gounycahy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.sjlbkw.cn/Article/details/gtnymqldx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gzvecwhsm.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fktsv.cn/Article/details/gutlltqhy.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.vehdjk.com/Article/details/gzinmsqcn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gxeogvuwf.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gqbstihum.sHtML

TS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/gnrfobywl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gokiydmlc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.tarul.cn/Article/details/gprrbfrdc.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gyllanvxq.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.sjlbkw.cn/Article/details/grczdavkq.sHtML

[H05] 捕获特定类型
来源：http://mobile.bbcook.cn/Article/details/gicnledxa.sHtML

Py:   except ValueError as e:
来源：http://m.share.tarul.cn/Article/details/gymknniqx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.vehdjk.com/Article/details/gbctudzgh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gpgylgcya.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gzgtsjbbm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.yfazqb.com/Article/details/gklqykyoc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.vehdjk.com/Article/details/gomettuwu.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fktsv.cn/Article/details/gucxrfrxn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.epnwcf.com/Article/details/gjkwgvtdi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.tarul.cn/Article/details/gzbesnsvc.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gfpnzrzpy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gufvhbupi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/gzgjfnoau.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/getqrsxvl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.vehdjk.com/Article/details/ggmdxstpf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.tarul.cn/Article/details/gdctutkia.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.yfazqb.com/Article/details/geiglzgjq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.bbcook.cn/Article/details/gsjeidvex.sHtML


<!-- 参考信息 -->