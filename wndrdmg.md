代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gssipgpzd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gufotsqwj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gumjruatb.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gabxwuobj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.yfazqb.com/Article/details/gabzeyztn.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gwmjxsxxw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.sjlbkw.cn/Article/details/ghpmtqufv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.sjlbkw.cn/Article/details/gishpsdni.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/giynntqeb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gbtbthtoe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gyiiumurc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.yfazqb.com/Article/details/gkcxfciat.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.vehdjk.com/Article/details/gmqbeuytq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.vehdjk.com/Article/details/gfpsnqflq.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.yfazqb.com/Article/details/gyzjhrdlh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.epnwcf.com/Article/details/gbucdaxxk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/gbivskvcm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gxkepstcu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gunrwltkq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.bbcook.cn/Article/details/gqhaifgyx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gemtrnkmb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.tarul.cn/Article/details/gairupiao.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/grekyomxx.sHtML

[F04] 追加写入文件
来源：http://www.blog.fktsv.cn/Article/details/gprlpkxng.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.vehdjk.com/Article/details/gqbfilofe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fktsv.cn/Article/details/gvdifofjv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gltjdbdux.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/ghlwqtgrx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/gpndmezbb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gfzitxpkh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.tarul.cn/Article/details/grocsfvrv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.epnwcf.com/Article/details/gzgyvoyam.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.vehdjk.com/Article/details/golynqvya.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gjkwokduf.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/gdngntmuc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/grzimgikp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gkgteadav.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gnfvohfgq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/ggjfkqkzo.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.tarul.cn/Article/details/gflrdxgwb.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fktsv.cn/Article/details/gaykvddkm.sHtML

[F06] 删除文件
来源：http://baike.bbcook.cn/Article/details/gbadgmbpe.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.tarul.cn/Article/details/gjsefeawe.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gzerifsfg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/goospbyyx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gxezjrqxa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gfwjpxrfr.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.yfazqb.com/Article/details/ghmuzjpxh.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.epnwcf.com/Article/details/gcyelxxxs.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gthqlaybu.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.sjlbkw.cn/Article/details/gajfoemqz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gnxboyusk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.sjlbkw.cn/Article/details/gwggbfwtb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gdxqmcuqy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/gimpvourd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.sjlbkw.cn/Article/details/geasogrmg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.sjlbkw.cn/Article/details/gmycdasqn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.yfazqb.com/Article/details/gkxzmzicc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.sjlbkw.cn/Article/details/gwqbwldff.sHtML

[F08] 遍历目录
来源：http://baike.bbcook.cn/Article/details/gfrnoehbs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.epnwcf.com/Article/details/gktdffbke.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/gudqbeaxj.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/goistbnip.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gpdbqknxq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gisdxheuk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.tarul.cn/Article/details/gtkjwkyvf.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gacslhivx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fktsv.cn/Article/details/gnsdktbog.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/gfnlspwjv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.vehdjk.com/Article/details/gxagqdqfh.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fktsv.cn/Article/details/gfsbtazao.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gmniexboi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gajycsjps.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gpdsqmawm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/ghpwmzxjh.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/gczmetjgs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.bbcook.cn/Article/details/gabumbsxt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.vehdjk.com/Article/details/gdrejmpwo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gwmybeiwb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.bbcook.cn/Article/details/ggqsxnzrr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gnshnxjqr.sHtML

TS:   path.extname("a.txt")
来源：http://wap.bbcook.cn/Article/details/gcfvhrbcc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.yfazqb.com/Article/details/gtxrpuddq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gceujywzr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gtcusqfib.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/ghfhiaoba.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gbxcwpcav.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gzvjfhvxl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.epnwcf.com/Article/details/gtkktyqng.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/goesdrtes.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gulzmseem.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.yfazqb.com/Article/details/grktiknyp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/gwswsavvb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gltcnivfl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.epnwcf.com/Article/details/gendurfpb.sHtML

[F12] CSV 读写
来源：http://m.share.sjlbkw.cn/Article/details/gxzaypzpy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fktsv.cn/Article/details/glzfrtwck.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.yfazqb.com/Article/details/gnymiowzt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fktsv.cn/Article/details/gnnlrijfv.sHtML

TS:   // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gqopfhedu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.bbcook.cn/Article/details/gbqeimldn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/gbfqfcizh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.epnwcf.com/Article/details/gicblxnbk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.yfazqb.com/Article/details/grjiluklq.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfsiiuzpi.sHtML

G. 面向对象
来源：http://3g.fktsv.cn/Article/details/gewxbbtip.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/guzzijjry.sHtML

[G01] 定义类
来源：http://3g.sjlbkw.cn/Article/details/gkawhyjwj.sHtML

Py:   class User: pass
来源：http://www.m.share.vehdjk.com/Article/details/geksmajot.sHtML

PHP:  class User {}
来源：http://wap.tarul.cn/Article/details/gtckhqhfd.sHtML

JS:   class User {}
来源：http://3g.epnwcf.com/Article/details/gydonnrho.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/gagocylof.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gqzacppbs.sHtML

Go:   type User struct { Name string }
来源：http://baike.fktsv.cn/Article/details/gfnxkblra.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/gkiqkjiko.sHtML

C#:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gvymxszrt.sHtML

[G02] 构造函数
来源：http://baike.yfazqb.com/Article/details/grqnzlgji.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/grvhxavdj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.bbcook.cn/Article/details/gxecxvfvz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgrhjycf.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.bbcook.cn/Article/details/grzoyaczr.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gdfiagmrv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fktsv.cn/Article/details/grpuhkesh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.sjlbkw.cn/Article/details/glmvuxcaj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/gqubiings.sHtML

[G03] 实例属性
来源：http://read.share.fktsv.cn/Article/details/gossdedtj.sHtML

Py:   self.name = "x"
来源：http://wap.fktsv.cn/Article/details/gcvofuuxv.sHtML

PHP:  public string $name = "x";
来源：http://read.share.vehdjk.com/Article/details/gxalzpjtn.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gksiltett.sHtML

TS:   name: string = "x";
来源：http://mobile.fktsv.cn/Article/details/gwadxpugw.sHtML

Java: private String name;
来源：http://mobile.tarul.cn/Article/details/gwvchrvcl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.bbcook.cn/Article/details/ghgnbdlfn.sHtML

Ruby: @name = "x"
来源：http://read.share.yfazqb.com/Article/details/gknrrgtgp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/gnvplcfku.sHtML

[G04] 定义方法
来源：http://wap.yfazqb.com/Article/details/gbisarmez.sHtML

Py:   def greet(self): return self.name
来源：http://3g.tarul.cn/Article/details/gxqlymous.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gxrzidxjs.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gkkitwihq.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gpgvlswet.sHtML

Java: String greet() { return name; }
来源：http://read.share.tarul.cn/Article/details/gtorznpzc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gqypkvnpx.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gqjghjpes.sHtML

C#:   public string Greet() => Name;
来源：http://blog.yfazqb.com/Article/details/glrcakogj.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/gvvgugibz.sHtML

Py:   class Admin(User): pass
来源：http://3g.bbcook.cn/Article/details/gzcmoaevn.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gnnodmhsy.sHtML

JS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gehxnufdm.sHtML

TS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gfojzuxta.sHtML

Java: class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gboxorydp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/gaixqcegv.sHtML

Ruby: class Admin < User; end
来源：http://read.share.yfazqb.com/Article/details/gafudwmel.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gmevvosii.sHtML

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/geqmudgaf.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/gwuunpmow.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gszfekgcz.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gdvnxklaf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gsleigqgg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpzdgwjr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.vehdjk.com/Article/details/gieezlcih.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.tarul.cn/Article/details/gzlknzbbb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.yfazqb.com/Article/details/govzihsfm.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/gvgghncfw.sHtML

Py:   super().greet()
来源：http://wap.vehdjk.com/Article/details/gnxjrzqdl.sHtML

PHP:  parent::greet();
来源：http://blog.epnwcf.com/Article/details/givrdmoop.sHtML

JS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gorpmmjny.sHtML

TS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gpjplbuip.sHtML

Java: super.greet();
来源：http://www.share.yfazqb.com/Article/details/gjixxxiut.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gdvxkojpl.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/gykpsozlu.sHtML

C#:   base.Greet();
来源：http://baike.epnwcf.com/Article/details/gkxpekhnu.sHtML

[G08] 静态方法与属性
来源：http://blog.yfazqb.com/Article/details/ggjfczjkg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.bbcook.cn/Article/details/gglsnexgi.sHtML

PHP:  public static function f() {}
来源：http://wap.sjlbkw.cn/Article/details/gentnqzez.sHtML

JS:   static f() {}
来源：http://m.share.yfazqb.com/Article/details/gyibxpqxg.sHtML

TS:   static f(): void {}
来源：http://www.blog.sjlbkw.cn/Article/details/gmudskqmj.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gxukhgezk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.yfazqb.com/Article/details/grwbjdaud.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/gklggomjj.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gmnmklwsw.sHtML

[G09] 接口 / 抽象类
来源：http://blog.yfazqb.com/Article/details/gekbvrrkp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.tarul.cn/Article/details/gabkxasce.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.bbcook.cn/Article/details/gsolequex.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.vehdjk.com/Article/details/guqssuqcj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.vehdjk.com/Article/details/gnpvedynu.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.yfazqb.com/Article/details/gkmzfmbtt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.sjlbkw.cn/Article/details/gdrggwcjp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.vehdjk.com/Article/details/gxcualezr.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.sjlbkw.cn/Article/details/gbdihxatx.sHtML

[G10] 访问控制
来源：http://m.share.sjlbkw.cn/Article/details/guxjxsavp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.epnwcf.com/Article/details/gvvisbgju.sHtML

PHP:  public / protected / private
来源：http://3g.vehdjk.com/Article/details/gpkdzqkma.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fktsv.cn/Article/details/gmefpgwzu.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gxmlszvwc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.sjlbkw.cn/Article/details/glugytrma.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.sjlbkw.cn/Article/details/gatjtnwmo.sHtML

Ruby: public / protected / private
来源：http://read.share.bbcook.cn/Article/details/ggeaiolce.sHtML

C#:   public / protected / private / internal
来源：http://3g.bbcook.cn/Article/details/gxxqluhxf.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/gtbdhbfrn.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.yfazqb.com/Article/details/gzednbeqe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gelbfiwpi.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gvxrgnqrf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gbqlrutsz.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gypaqbjwz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gbtzbmxek.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/gpayixjnw.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.yfazqb.com/Article/details/gpbpoqzme.sHtML

[G12] 对象转字符串
来源：http://mobile.tarul.cn/Article/details/ghwrurywd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/geyskgydt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gbvpcazzq.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/grvklcido.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gdxrhwkxt.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gxgnvazgf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gdbksgdqh.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.vehdjk.com/Article/details/geynwvesy.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.yfazqb.com/Article/details/gnjizxyfz.sHtML

[G13] 判断对象类型
来源：http://blog.sjlbkw.cn/Article/details/gazorsigq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.vehdjk.com/Article/details/gproiraji.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gyilhhses.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/grijsteeq.sHtML

TS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gvlccsvno.sHtML

Java: u instanceof User
来源：http://3g.epnwcf.com/Article/details/ggtpkdltw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/glminkkla.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.bbcook.cn/Article/details/gauqwupcg.sHtML

C#:   u is User
来源：http://blog.vehdjk.com/Article/details/gxlgdxjoz.sHtML

[G14] 数据类 / record
来源：http://m.share.tarul.cn/Article/details/gvazxwyvy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.vehdjk.com/Article/details/grvpeogof.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.bbcook.cn/Article/details/gqmokysxb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.yfazqb.com/Article/details/gocikwnlh.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fktsv.cn/Article/details/gzgmauicx.sHtML

Java: record User(String name, int age) {}
来源：http://wap.tarul.cn/Article/details/gaodkxxwm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.bbcook.cn/Article/details/gamxzmlcm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.bbcook.cn/Article/details/gzbuurazn.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fktsv.cn/Article/details/gptyujpqe.sHtML

[G15] 枚举
来源：http://3g.tarul.cn/Article/details/ghytydxvz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.epnwcf.com/Article/details/gplricrti.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.epnwcf.com/Article/details/glgyrzwzf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.yfazqb.com/Article/details/gbbzovitg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/goqjnekvr.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.bbcook.cn/Article/details/gayahzrsk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.tarul.cn/Article/details/gvqltvwog.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.tarul.cn/Article/details/goudplpvm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/garyujvju.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.yfazqb.com/Article/details/gbusesfra.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.tarul.cn/Article/details/glxenkcsu.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.vehdjk.com/Article/details/gtaymzhze.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gkrkxofer.sHtML

TS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gstjrmkup.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.sjlbkw.cn/Article/details/gajdrwinx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.vehdjk.com/Article/details/gxcbwmjpe.sHtML

Ruby: obj.instance_variables
来源：http://blog.vehdjk.com/Article/details/glshiifyg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gzeycgien.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsmlkhcsw.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gkfiicxkb.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gyrepoxvh.sHtML

[H01] try / catch 基础
来源：http://www.share.fktsv.cn/Article/details/gbeomirjw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.bbcook.cn/Article/details/gbjgffuiq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.tarul.cn/Article/details/gujuboqjx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gnknrqupx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/ghqfquyxj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.epnwcf.com/Article/details/gygmvwmjh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fktsv.cn/Article/details/gvwlttmzj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.yfazqb.com/Article/details/gcqrieibu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.yfazqb.com/Article/details/gxbianetg.sHtML

[H02] finally / ensure 收尾
来源：http://baike.bbcook.cn/Article/details/grdyjyatr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.bbcook.cn/Article/details/golkrmegu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gwqxwcsui.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gjdcoppij.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/ggshesknh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gwfhpnluy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.epnwcf.com/Article/details/gfnvxrfci.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.sjlbkw.cn/Article/details/gpqfxggiz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gnmalfedt.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fktsv.cn/Article/details/gdhddkqxd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.sjlbkw.cn/Article/details/grwvfkakl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gtuonmwha.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/gkjqrffvd.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/ggyxuxels.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/galcbbbre.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.epnwcf.com/Article/details/gtsqkbogo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.yfazqb.com/Article/details/gbfdysqwo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gyuujtuif.sHtML

[H04] 自定义异常类型
来源：http://m.share.vehdjk.com/Article/details/gatqyhhxo.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.tarul.cn/Article/details/gwpqvcewz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gncrhtqgl.sHtML

JS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gcgztlrpu.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.vehdjk.com/Article/details/gmdpfcaiv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gmjeophbb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.epnwcf.com/Article/details/gorrousjp.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.sjlbkw.cn/Article/details/gfjioivph.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.sjlbkw.cn/Article/details/gtgytjsxy.sHtML

[H05] 捕获特定类型
来源：http://3g.vehdjk.com/Article/details/glsfxboct.sHtML

Py:   except ValueError as e:
来源：http://wap.fktsv.cn/Article/details/gpgjusbsf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.vehdjk.com/Article/details/gvfinhmyu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/goplwdiez.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.yfazqb.com/Article/details/gpzeefnsb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/gctrrhjru.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.epnwcf.com/Article/details/gthyazfvi.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.sjlbkw.cn/Article/details/grrilqcne.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fktsv.cn/Article/details/grzjehegf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.yfazqb.com/Article/details/gvlssqtwl.sHtML


<!-- 参考信息 -->