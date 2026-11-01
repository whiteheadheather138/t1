代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gmkejluzt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.yfazqb.com/Article/details/gpafufayc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.bbcook.cn/Article/details/gcpkqsofz.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gxjaunxkm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gpdvlxvoi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gcgicffsq.sHtML

F. 文件与目录
来源：http://www.blog.epnwcf.com/Article/details/gkbtohwom.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwjtcmcow.sHtML

[F01] 读取整个文件
来源：http://baike.fktsv.cn/Article/details/gpxryqbjv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fktsv.cn/Article/details/gaefxxzey.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.tarul.cn/Article/details/gpknrfxpf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.sjlbkw.cn/Article/details/ghbmgsmhx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fktsv.cn/Article/details/gfjqrpeua.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gcsjfasdq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.bbcook.cn/Article/details/gwqgbumut.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gpzftcnnj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gqwpchgan.sHtML

[F02] 逐行读取文件
来源：http://baike.vehdjk.com/Article/details/ggfhnpwia.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.epnwcf.com/Article/details/gkmrjixpj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.epnwcf.com/Article/details/guanvtljy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gleelqpml.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gwicdnubt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/gofyeyggt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.vehdjk.com/Article/details/gecnolzmn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fktsv.cn/Article/details/gkibzkoyo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.tarul.cn/Article/details/govleiglr.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.bbcook.cn/Article/details/ggfikrqqc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.tarul.cn/Article/details/gqczsczxp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gyhuqnlal.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/grkmzexmj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gurfofzls.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.bbcook.cn/Article/details/gbopqvjtf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/gckyutjko.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gvonugeea.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/ggkhoucsf.sHtML

[F04] 追加写入文件
来源：http://read.share.bbcook.cn/Article/details/gimlweiil.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.vehdjk.com/Article/details/gxwcrtspi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.epnwcf.com/Article/details/gzsxlkciw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/gaxbogecj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gyzkmkhub.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gjqltalvm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/gkxozckho.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fktsv.cn/Article/details/gopocwxyy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.sjlbkw.cn/Article/details/gnnxjzcey.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.vehdjk.com/Article/details/gzchuzlns.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/gcpzmeany.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.vehdjk.com/Article/details/gktvhiuvu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gcjtibniy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gqvribwsz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gdzhedpxl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/gezdsvilj.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gufwahfqa.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gnxrjhpld.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/gbdvhtzll.sHtML

Py:   os.remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gwrxpobnc.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fktsv.cn/Article/details/gxudtmsom.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/geeeoibjn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gtvqcbbyn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gvbghtoty.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gksyprrcw.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gxnusdhrk.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gzewfyuqd.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/gxrpdgoou.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gzcqpzzty.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fktsv.cn/Article/details/glxwbfunt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gcxhhssxj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gsmpikqhr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.vehdjk.com/Article/details/ggrmcvmah.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.tarul.cn/Article/details/gltogwicq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/giktryoru.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.tarul.cn/Article/details/gbuojuvch.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/ghxddttct.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.bbcook.cn/Article/details/gtydrvzlx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fktsv.cn/Article/details/gkkexeovv.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gwxftdues.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gvfsgguwg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gneqwhpug.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.yfazqb.com/Article/details/gnyshzvlw.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.epnwcf.com/Article/details/gagfrrirg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/giqkcvfyo.sHtML

[F09] 获取文件大小
来源：http://www.share.fktsv.cn/Article/details/gascncybc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gmnaasztt.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fktsv.cn/Article/details/gwlnryqly.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gglceykfc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gtudwgbmr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gytmggkuj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.tarul.cn/Article/details/gdzrilfcg.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gfbmfawao.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.bbcook.cn/Article/details/gokykcjbd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fktsv.cn/Article/details/gmhvtayhk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gtxzhdznt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.yfazqb.com/Article/details/getekvwez.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxppbulay.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.bbcook.cn/Article/details/ghxerxqsb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/gtnesdmha.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/glyplvhqk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gdcafauyr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gzkftfpfy.sHtML

[F11] 复制与移动文件
来源：http://www.share.vehdjk.com/Article/details/gknvmkqed.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gayihyphh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.epnwcf.com/Article/details/gloyqzhff.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/giratbric.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/ghrnweksr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/goldmemhp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/groqeihbv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gxfpkbmsg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gzvnzcyjs.sHtML

[F12] CSV 读写
来源：http://blog.bbcook.cn/Article/details/gyuuwpcuu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/gsukjtnze.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.epnwcf.com/Article/details/gmvjqamzw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.bbcook.cn/Article/details/gtsbuctnk.sHtML

TS:   // 同上
来源：http://mobile.tarul.cn/Article/details/gdgloqckc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.epnwcf.com/Article/details/gxiukjkjx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/grkmosrrq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.epnwcf.com/Article/details/ggznkzlef.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/gdtlpldck.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwlhzkhja.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/gnuycudjo.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvvdopise.sHtML

[G01] 定义类
来源：http://3g.vehdjk.com/Article/details/gnlvljqzv.sHtML

Py:   class User: pass
来源：http://www.blog.bbcook.cn/Article/details/gnfbhgpfk.sHtML

PHP:  class User {}
来源：http://blog.bbcook.cn/Article/details/grzlohubr.sHtML

JS:   class User {}
来源：http://3g.bbcook.cn/Article/details/gxyslgoup.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fktsv.cn/Article/details/geoklomdf.sHtML

Java: class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtbdllvs.sHtML

Go:   type User struct { Name string }
来源：http://m.share.sjlbkw.cn/Article/details/ggrrwnbmc.sHtML

Ruby: class User; end
来源：http://mobile.yfazqb.com/Article/details/guvjqyoui.sHtML

C#:   class User {}
来源：http://3g.bbcook.cn/Article/details/grysfradc.sHtML

[G02] 构造函数
来源：http://blog.yfazqb.com/Article/details/gapfavgoo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.sjlbkw.cn/Article/details/gvstmejpv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.vehdjk.com/Article/details/gjrfxlvgm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gtdrpjnnf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.yfazqb.com/Article/details/ghxoawppw.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gwbkklkxk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.bbcook.cn/Article/details/gumpseazu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.tarul.cn/Article/details/gbwlacsgf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.epnwcf.com/Article/details/glmtvrxzb.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/gbukjiwbe.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/gbkzkgryk.sHtML

PHP:  public string $name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gbupmrqxx.sHtML

JS:   this.name = "x";
来源：http://mobile.yfazqb.com/Article/details/glbsqzdlb.sHtML

TS:   name: string = "x";
来源：http://read.share.epnwcf.com/Article/details/gelketzpe.sHtML

Java: private String name;
来源：http://mobile.bbcook.cn/Article/details/gspevzfyh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/grxbswazf.sHtML

Ruby: @name = "x"
来源：http://3g.tarul.cn/Article/details/gsixyjufi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.bbcook.cn/Article/details/ghvazbakk.sHtML

[G04] 定义方法
来源：http://www.share.yfazqb.com/Article/details/gqamwgdxh.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gpggyslri.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gpdtggtuz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gsgsyrftw.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gitadgybh.sHtML

Java: String greet() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gkqpebbia.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gnijhidva.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/gbmsyhavn.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gbyhkyfep.sHtML

[G05] 继承
来源：http://baike.epnwcf.com/Article/details/gooxaxwqx.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.bbcook.cn/Article/details/gsshiuuzd.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gieyjnssh.sHtML

JS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/grcannbgb.sHtML

TS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gtnmahqbf.sHtML

Java: class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gxtfkyjzr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.sjlbkw.cn/Article/details/gnxzqiulp.sHtML

Ruby: class Admin < User; end
来源：http://wap.epnwcf.com/Article/details/gxehqylgd.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/glzuvmqnf.sHtML

[G06] 重写方法
来源：http://read.share.fktsv.cn/Article/details/ghvqzotrw.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gnixnyipl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gnzzaxuxm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gbuderrwu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gvbqvrgqj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gezeqfuuo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.bbcook.cn/Article/details/ghxieblrd.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.epnwcf.com/Article/details/gmvltjnef.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.yfazqb.com/Article/details/geuelhekh.sHtML

[G07] 调用父类方法
来源：http://mobile.sjlbkw.cn/Article/details/ghffklxvp.sHtML

Py:   super().greet()
来源：http://www.blog.tarul.cn/Article/details/glnhfffax.sHtML

PHP:  parent::greet();
来源：http://www.m.share.vehdjk.com/Article/details/gbxqrcdow.sHtML

JS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gjnqzvwjs.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gcgdiqabj.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gqldpnptm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fktsv.cn/Article/details/geqlpaslc.sHtML

Ruby: super
来源：http://wap.epnwcf.com/Article/details/gotarszfl.sHtML

C#:   base.Greet();
来源：http://blog.vehdjk.com/Article/details/gbvmxpvze.sHtML

[G08] 静态方法与属性
来源：http://baike.yfazqb.com/Article/details/gvpuxwgyh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.yfazqb.com/Article/details/ggrkjqsfm.sHtML

PHP:  public static function f() {}
来源：http://www.share.vehdjk.com/Article/details/gabdrelsj.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/grumvebbx.sHtML

TS:   static f(): void {}
来源：http://m.share.epnwcf.com/Article/details/goizqvbqg.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/gzvvxkhpm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfgivcih.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gjbgjgcqg.sHtML

C#:   public static void F() {}
来源：http://3g.epnwcf.com/Article/details/gccllxdal.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fktsv.cn/Article/details/gsepoyslo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/ghjotuzxy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.bbcook.cn/Article/details/gdninepua.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/ghgtadfuj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.epnwcf.com/Article/details/gqnzuzvay.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.tarul.cn/Article/details/grcdtddpy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.tarul.cn/Article/details/gzfpbrpqq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.epnwcf.com/Article/details/ginbxrlpw.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.sjlbkw.cn/Article/details/gvdjaguat.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/gjkfxkwwl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.vehdjk.com/Article/details/gteiqsrip.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gzoqcknze.sHtML

JS:   #private 字段；其余公开
来源：http://blog.tarul.cn/Article/details/gmflflvzl.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/ghhhtxfal.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fktsv.cn/Article/details/giisbstxi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/gnxsvnsqa.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gphiydrqb.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/gmrtdyiqm.sHtML

[G11] getter / setter
来源：http://3g.fktsv.cn/Article/details/gjatddali.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fktsv.cn/Article/details/gnkbtepgq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gbcyvbnbh.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/goyxygnta.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gpcajpnmy.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/gihyvwgna.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gsfzufqlp.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.vehdjk.com/Article/details/ggphvrzzc.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.tarul.cn/Article/details/gakuzgpar.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/ghxjspujv.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gaomqyrgo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gnqoxrymy.sHtML

JS:   toString() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gpkansrlx.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/ggdrpkrct.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gxchjlhsj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gozyyuwfq.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/gluhpfbye.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.bbcook.cn/Article/details/gpfxmhmsx.sHtML

[G13] 判断对象类型
来源：http://3g.epnwcf.com/Article/details/gqwqyecrz.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvntxvzdn.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/goqbcrpec.sHtML

JS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gsnkttlee.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gukatsrer.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/grmlivnih.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fktsv.cn/Article/details/gwnavresf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/gkdibemud.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/gmblcahaa.sHtML

[G14] 数据类 / record
来源：http://mobile.epnwcf.com/Article/details/gsfgbkosk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fktsv.cn/Article/details/gizrfawan.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.yfazqb.com/Article/details/gvxggeejc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.epnwcf.com/Article/details/gisfrfvpk.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.vehdjk.com/Article/details/geyxithdr.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.epnwcf.com/Article/details/gbifcjjmp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.epnwcf.com/Article/details/gtjchxguy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/giugfzkiu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.vehdjk.com/Article/details/gaoblcpzy.sHtML

[G15] 枚举
来源：http://www.blog.yfazqb.com/Article/details/gucfjiegc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.yfazqb.com/Article/details/gfbjzknvx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfychzwub.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/gsaqnkpxr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gawmahnkg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.yfazqb.com/Article/details/gckhraeqr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/geuxuoyuy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.epnwcf.com/Article/details/gxmcfzdxm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gtqtfjgqk.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.bbcook.cn/Article/details/gksxsdrie.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.sjlbkw.cn/Article/details/glabvuich.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.yfazqb.com/Article/details/gbxvqqkhz.sHtML

JS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gbwbxtvum.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gnthsxkhz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.tarul.cn/Article/details/gepbqjcql.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/gkvyzuzmp.sHtML

Ruby: obj.instance_variables
来源：http://wap.fktsv.cn/Article/details/gkrvptzpo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gdjlzoipe.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guvpjogfb.sHtML

H. 异常与错误处理
来源：http://baike.yfazqb.com/Article/details/gsrhclnvl.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfatqglnk.sHtML

[H01] try / catch 基础
来源：http://www.share.yfazqb.com/Article/details/gopyywivo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.bbcook.cn/Article/details/gehsnmeda.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.vehdjk.com/Article/details/gqizuqgym.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gnzqjtnfm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gpjldqien.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.vehdjk.com/Article/details/giatudqao.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.yfazqb.com/Article/details/gonkcaxhs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.epnwcf.com/Article/details/gkbozsgzm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/gffwfzgue.sHtML

[H02] finally / ensure 收尾
来源：http://wap.vehdjk.com/Article/details/gbazrgxfu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.tarul.cn/Article/details/gxevokemq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gsolqruyf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gvhneqqvn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gknoqdteo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gyevbdsjb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.sjlbkw.cn/Article/details/geaxlgbqu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.bbcook.cn/Article/details/gdbbozprq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.tarul.cn/Article/details/ghxiuolmr.sHtML

[H03] 主动抛出异常
来源：http://baike.vehdjk.com/Article/details/gkznuyfjr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.yfazqb.com/Article/details/gnkszvywh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gohnntnwx.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gpgorjzbv.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gmwztqyob.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfsptpmo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fktsv.cn/Article/details/gfyfrpqdu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gnujfgpdp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gdsietnge.sHtML

[H04] 自定义异常类型
来源：http://read.share.sjlbkw.cn/Article/details/gowomcydn.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.yfazqb.com/Article/details/gavqnomwv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/ggblzksju.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fktsv.cn/Article/details/gaqloydjd.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gjmicssae.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gephihjaj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.sjlbkw.cn/Article/details/geiwpflbd.sHtML


<!-- 参考信息 -->