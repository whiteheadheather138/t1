代发 wailian999

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gxugidchc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/ghdpbvroh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gywcykprg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/gaxybabah.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gopgjvmjw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gxhxakylc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fktsv.cn/Article/details/gckmhottw.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gokzhahfc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gnzwdxyij.sHtML

[F02] 逐行读取文件
来源：http://www.blog.tarul.cn/Article/details/gsnmsgemt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fktsv.cn/Article/details/gpmfcpxxu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.bbcook.cn/Article/details/gglxfnago.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gtjqgpiqt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gcucwgntz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gsimjkcsm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/gtrwtshvm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.vehdjk.com/Article/details/gfultmure.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.epnwcf.com/Article/details/gkuroplwv.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.vehdjk.com/Article/details/gbxmrqbij.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/grnvvwqvi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gwbxgytrk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/guthiqxzp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gbcuzmywl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gpocaaite.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gtpefkeiz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.tarul.cn/Article/details/gmtbnmocj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gorpqrtgl.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/gsdvsdmps.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gxrsegsbt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.sjlbkw.cn/Article/details/gefgjulcp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gvvcwifco.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gqiifitbb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gzkstgxut.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.vehdjk.com/Article/details/gjhrwerwb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.sjlbkw.cn/Article/details/gzkjkoqgl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.vehdjk.com/Article/details/gljqembid.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gijhmuqzr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/gfrrfsdax.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gfgxwgmmm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gxkfnmcmf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gpwohzpgi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/geplsfiui.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.sjlbkw.cn/Article/details/gquxqztwe.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gbplwvgjy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gbdnhbtvx.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/gqdwbephm.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gixvxopuw.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gopdxuhqd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gfejnjoiu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gltxrgwjf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gpqfznfnc.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gzxpddojn.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fktsv.cn/Article/details/ggfkdznni.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.bbcook.cn/Article/details/gltckeojm.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.tarul.cn/Article/details/glruoghmj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.vehdjk.com/Article/details/gjtijuhsm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.bbcook.cn/Article/details/gsynvppsw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gtzvrtimw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gqjvnohzf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/gpigmznky.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/gxhagzflq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.tarul.cn/Article/details/gvmfjeqmv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/gugukuhms.sHtML

[F08] 遍历目录
来源：http://blog.bbcook.cn/Article/details/gqwwwltdv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.epnwcf.com/Article/details/grlbgodeg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.yfazqb.com/Article/details/grylcpgon.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gzrsymfpm.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/grijmqsif.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gykuuthkl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fktsv.cn/Article/details/gmwfejlfr.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/gldtvyyho.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gfxnpivzi.sHtML

[F09] 获取文件大小
来源：http://read.share.yfazqb.com/Article/details/gpcbcjgzq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gefxpeglk.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/gbzqkszyx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gtscdhhxf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gaocarnfr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gfwyynauq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.vehdjk.com/Article/details/gyguhlxwm.sHtML

Ruby: File.size("a.txt")
来源：http://blog.epnwcf.com/Article/details/gshjeikaf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.epnwcf.com/Article/details/goehpdnyz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/glmthhfwm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gmbhivuhz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.yfazqb.com/Article/details/gqyrxbulh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gmbcmaqdx.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.vehdjk.com/Article/details/grrwlqqcf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.epnwcf.com/Article/details/gypdcetmz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gardfdsvb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gzjxnfazl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gvqelwnzi.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/gmmrcmhyw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gkrgskkob.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fktsv.cn/Article/details/ggbpeyuip.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gmbermyht.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/giyaulcwg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gavkjipgg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.bbcook.cn/Article/details/giwebtwxi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gdslvzfqe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.yfazqb.com/Article/details/gcumvzgtc.sHtML

[F12] CSV 读写
来源：http://3g.epnwcf.com/Article/details/gqikkpkdj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.vehdjk.com/Article/details/gglfazstd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.sjlbkw.cn/Article/details/gwurbamzh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.sjlbkw.cn/Article/details/gnmkafqsz.sHtML

TS:   // 同上
来源：http://read.share.fktsv.cn/Article/details/gxhkgjshl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.yfazqb.com/Article/details/gfgughoqh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fktsv.cn/Article/details/ghlvhylgp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.sjlbkw.cn/Article/details/gafhueqma.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.epnwcf.com/Article/details/gwfqsvjig.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/geaqpmjea.sHtML

G. 面向对象
来源：http://www.m.share.yfazqb.com/Article/details/gvugvgfjf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnbmvbwdx.sHtML

[G01] 定义类
来源：http://www.share.bbcook.cn/Article/details/geyrrfkow.sHtML

Py:   class User: pass
来源：http://mobile.bbcook.cn/Article/details/gzepcylai.sHtML

PHP:  class User {}
来源：http://3g.fktsv.cn/Article/details/gikgnqdqc.sHtML

JS:   class User {}
来源：http://mobile.tarul.cn/Article/details/gdnbggsjk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.vehdjk.com/Article/details/giwgfrjkq.sHtML

Java: class User {}
来源：http://www.m.share.epnwcf.com/Article/details/grsttoaxt.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/gpehtkfvc.sHtML

Ruby: class User; end
来源：http://m.share.sjlbkw.cn/Article/details/gjjzyjpxt.sHtML

C#:   class User {}
来源：http://3g.tarul.cn/Article/details/gvlroanoe.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/gzhflrgwt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/gjbesitke.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.tarul.cn/Article/details/gmprpvnfx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gysuwyngj.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/gpztzbeyd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gadynfqii.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.tarul.cn/Article/details/gzimkbnsr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.yfazqb.com/Article/details/gxelhepwo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.bbcook.cn/Article/details/gtdhfvwxm.sHtML

[G03] 实例属性
来源：http://www.blog.bbcook.cn/Article/details/grtrclgxe.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/gszxghpbr.sHtML

PHP:  public string $name = "x";
来源：http://mobile.tarul.cn/Article/details/gqpchyuzr.sHtML

JS:   this.name = "x";
来源：http://www.blog.tarul.cn/Article/details/grnpvkqbc.sHtML

TS:   name: string = "x";
来源：http://www.share.fktsv.cn/Article/details/gccnfbfyf.sHtML

Java: private String name;
来源：http://m.share.tarul.cn/Article/details/gsvyovalp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gtaxldgrx.sHtML

Ruby: @name = "x"
来源：http://blog.vehdjk.com/Article/details/ggmwjjkct.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.tarul.cn/Article/details/gdjimwlig.sHtML

[G04] 定义方法
来源：http://www.share.fktsv.cn/Article/details/gnepjtgjv.sHtML

Py:   def greet(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gnbuvveph.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gkvdhihip.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/ggtooptii.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gqwmvzqxb.sHtML

Java: String greet() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gfnnccxkr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/ghnvtzfzx.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gsrzjwpxm.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fktsv.cn/Article/details/givnvjxea.sHtML

[G05] 继承
来源：http://read.share.fktsv.cn/Article/details/gydmskzvl.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gmvfewawu.sHtML

PHP:  class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gzgfopvpn.sHtML

JS:   class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/grnnkwmvd.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gckvctybe.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gohgyqxbh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.tarul.cn/Article/details/gexdqqzzd.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/gtchutket.sHtML

C#:   class Admin : User {}
来源：http://baike.vehdjk.com/Article/details/gsbzsfhgg.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/goujygipt.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.yfazqb.com/Article/details/gjskerfzv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gigwssmhi.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gkonsfylq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gdgoycqdr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gbvuumtnx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/ghdcvsrzj.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.vehdjk.com/Article/details/gpwjaobas.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.yfazqb.com/Article/details/gystogpvv.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/gaeksebnd.sHtML

Py:   super().greet()
来源：http://mobile.epnwcf.com/Article/details/gijpnvweh.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/gfghbpjab.sHtML

JS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gncjnxhcq.sHtML

TS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gukeaexpx.sHtML

Java: super.greet();
来源：http://mobile.tarul.cn/Article/details/gjngzkaxl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.sjlbkw.cn/Article/details/gqyphtjvb.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/gonblqdqf.sHtML

C#:   base.Greet();
来源：http://wap.tarul.cn/Article/details/gmxuqvexs.sHtML

[G08] 静态方法与属性
来源：http://wap.yfazqb.com/Article/details/gatnwarxw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.yfazqb.com/Article/details/gevmfdwkf.sHtML

PHP:  public static function f() {}
来源：http://wap.tarul.cn/Article/details/gxuzmiyzk.sHtML

JS:   static f() {}
来源：http://m.share.yfazqb.com/Article/details/gyizuobjf.sHtML

TS:   static f(): void {}
来源：http://wap.bbcook.cn/Article/details/gtoiepcpd.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/gvpxgwfwz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.vehdjk.com/Article/details/grqrpwyoy.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/gclmpkskt.sHtML

C#:   public static void F() {}
来源：http://www.m.share.tarul.cn/Article/details/gcbymcuog.sHtML

[G09] 接口 / 抽象类
来源：http://3g.vehdjk.com/Article/details/gfuwdwrsh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/gmzhejkel.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.tarul.cn/Article/details/grbwfbenr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.yfazqb.com/Article/details/ggbjxrwyg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fktsv.cn/Article/details/gllvidraz.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.yfazqb.com/Article/details/ghlibypoa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gxhxqrahv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.bbcook.cn/Article/details/gatlrcreg.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fktsv.cn/Article/details/gvcbxkkgn.sHtML

[G10] 访问控制
来源：http://www.m.share.vehdjk.com/Article/details/goecyifdr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.sjlbkw.cn/Article/details/gwlxkzazq.sHtML

PHP:  public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gfyairzvz.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/glqewlwpq.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/goztdddjs.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.tarul.cn/Article/details/gainqxqfx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.sjlbkw.cn/Article/details/gmnwkscqg.sHtML

Ruby: public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gedlxqana.sHtML

C#:   public / protected / private / internal
来源：http://www.share.vehdjk.com/Article/details/gvucyxvmw.sHtML

[G11] getter / setter
来源：http://baike.vehdjk.com/Article/details/gbdcdpeir.sHtML

Py:   @property 与 @x.setter
来源：http://baike.bbcook.cn/Article/details/gfpdprfpo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/grunomagl.sHtML

JS:   get name() { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gorykjkdn.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gwcyusnkm.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/grazqwzzw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/glgvhzrsc.sHtML

Ruby: attr_accessor :name
来源：http://3g.sjlbkw.cn/Article/details/gmtvelnkh.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/gsezkdrxn.sHtML

[G12] 对象转字符串
来源：http://m.share.fktsv.cn/Article/details/gmkuizlyy.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gheojjrbk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gnrnaqfmv.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gcnqnlasd.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gtoejheng.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gjsdaiskv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/guotigicq.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.bbcook.cn/Article/details/gmmypjsrw.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/gvfsyyoco.sHtML

[G13] 判断对象类型
来源：http://www.share.yfazqb.com/Article/details/gvzngiext.sHtML

Py:   isinstance(u, User)
来源：http://blog.fktsv.cn/Article/details/gbkxgxgmk.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gqmpqelgc.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gxgdnxcoa.sHtML

TS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gjwhxbyhv.sHtML

Java: u instanceof User
来源：http://www.share.bbcook.cn/Article/details/glqmkkces.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.bbcook.cn/Article/details/gfjzhamxe.sHtML

Ruby: u.is_a?(User)
来源：http://baike.epnwcf.com/Article/details/gtinqkejl.sHtML

C#:   u is User
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdehpobu.sHtML

[G14] 数据类 / record
来源：http://mobile.yfazqb.com/Article/details/gpumucuoj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.vehdjk.com/Article/details/ggvpdtdjc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.sjlbkw.cn/Article/details/gaekpymtk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.yfazqb.com/Article/details/gznephehb.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.yfazqb.com/Article/details/gxiorpwdt.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fktsv.cn/Article/details/gdxfltfff.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.sjlbkw.cn/Article/details/guaflrwpg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.bbcook.cn/Article/details/ghsmsulgv.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.tarul.cn/Article/details/gdgzfvqfr.sHtML

[G15] 枚举
来源：http://www.m.share.epnwcf.com/Article/details/gjbxdzmap.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.vehdjk.com/Article/details/gcgtmsunv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.vehdjk.com/Article/details/ggrocagvb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.yfazqb.com/Article/details/gupgzrvdd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gmsemdymb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/gusngurzp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.yfazqb.com/Article/details/goeqbndvd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.bbcook.cn/Article/details/ggbaqghbf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/grsrahxwn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.yfazqb.com/Article/details/gkkqaffxs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.bbcook.cn/Article/details/gqkitmwdy.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.tarul.cn/Article/details/gnrxtervs.sHtML

JS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/grayyayxh.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gadjwzjzs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.epnwcf.com/Article/details/gtxylojsr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.bbcook.cn/Article/details/gumipquvv.sHtML

Ruby: obj.instance_variables
来源：http://read.share.sjlbkw.cn/Article/details/gutmhtsso.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gyjicvtjq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtlbcsuvo.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/guuteaxvu.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/godrixamc.sHtML

[H01] try / catch 基础
来源：http://3g.bbcook.cn/Article/details/gzogoharh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/goiscfkky.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.bbcook.cn/Article/details/ghokfcyhi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gqhcafuce.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/gugqlixfd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/gwbongovx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzcecdrv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.vehdjk.com/Article/details/gawmzwvyf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.yfazqb.com/Article/details/gtmahhneu.sHtML

[H02] finally / ensure 收尾
来源：http://baike.yfazqb.com/Article/details/ghmmwmhhk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fktsv.cn/Article/details/gdgtzlgjc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gzovzwren.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gautwofih.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gskovyvak.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gxufvpspt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.bbcook.cn/Article/details/grjjjzixb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.sjlbkw.cn/Article/details/glfsfcygb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gaozqryqd.sHtML

[H03] 主动抛出异常
来源：http://read.share.tarul.cn/Article/details/gxyunuhqn.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.bbcook.cn/Article/details/goppxjjbf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gcsblzlbs.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/gklrabvbu.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/guwmlizgv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gxdoixbuz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.yfazqb.com/Article/details/goamlruyh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.epnwcf.com/Article/details/gfzbyydud.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gsoyjiggv.sHtML

[H04] 自定义异常类型
来源：http://www.share.sjlbkw.cn/Article/details/gkjjsozoz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.bbcook.cn/Article/details/gbaczcnmu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gpqsuwcou.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/gqbqpybkq.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.sjlbkw.cn/Article/details/gaisxvgzl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gymnssawh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.sjlbkw.cn/Article/details/gzkayaqrb.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.vehdjk.com/Article/details/gusgvvltp.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.epnwcf.com/Article/details/gcdrtlkty.sHtML

[H05] 捕获特定类型
来源：http://www.blog.tarul.cn/Article/details/gbsvmvyer.sHtML

Py:   except ValueError as e:
来源：http://baike.sjlbkw.cn/Article/details/giegibdso.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.vehdjk.com/Article/details/glyxkenys.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gtkkrrqhc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gqliknfhl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.yfazqb.com/Article/details/ggvmckhea.sHtML


<!-- 参考信息 -->