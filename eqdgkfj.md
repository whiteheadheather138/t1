代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gqrtwtjeo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gapyhlfqf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.tarul.cn/Article/details/gwhmtjtpy.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.vehdjk.com/Article/details/gauudyfqm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.tarul.cn/Article/details/gqowjjkza.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/geirgfizm.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/goxfleknq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gllaxqdsh.sHtML

[F01] 读取整个文件
来源：http://wap.yfazqb.com/Article/details/gzoeowcsb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gpasmvqgy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gwfwnyffy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.yfazqb.com/Article/details/gysymptqp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/grmjlfdtu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gjznupplv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.sjlbkw.cn/Article/details/gvrvhbvhm.sHtML

Ruby: File.read("a.txt")
来源：http://baike.epnwcf.com/Article/details/gareeefjb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/goxxieppv.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/gmbfidkuu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.yfazqb.com/Article/details/gljxwvxqu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.vehdjk.com/Article/details/gqfdjfsze.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gzfpdqlzv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gqhgeescb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrcmwolo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.epnwcf.com/Article/details/gpslorlgx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/gatfqooyx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.tarul.cn/Article/details/grmipappu.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fktsv.cn/Article/details/glstehzvq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.vehdjk.com/Article/details/gdwemdkyt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.bbcook.cn/Article/details/gqgqzevjg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gkkbrwkgo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbxgwgfl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gvlbepjlt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.vehdjk.com/Article/details/gemxitpih.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gkohyedwm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gdrwkpaqx.sHtML

[F04] 追加写入文件
来源：http://www.share.fktsv.cn/Article/details/gqsfcgwcg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.bbcook.cn/Article/details/gkmqeyutd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fktsv.cn/Article/details/gnwddupqo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/gokweeldb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gjivcucfr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fktsv.cn/Article/details/gzkwyhmsc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.vehdjk.com/Article/details/ggyfivati.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.yfazqb.com/Article/details/gdrnkxlbt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.tarul.cn/Article/details/gsthyquju.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.epnwcf.com/Article/details/geamxjzkd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.bbcook.cn/Article/details/gpwskuitm.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/geyksfwhw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/groouvctt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gcjisjnyx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gzvmjnwhz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/gpnhsqzsc.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fktsv.cn/Article/details/glkjtpvvx.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fktsv.cn/Article/details/gihafnvrt.sHtML

[F06] 删除文件
来源：http://blog.yfazqb.com/Article/details/gdqlchgac.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gsftztorv.sHtML

PHP:  unlink("a.txt");
来源：http://blog.vehdjk.com/Article/details/grahrefmy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gwldpujhy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gltzropwl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/guqgcpkxo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gtosoyijm.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fktsv.cn/Article/details/gfseuqvdv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fktsv.cn/Article/details/ggwsnqsvx.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/gpkdcctjx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gnpdlyxjr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.vehdjk.com/Article/details/ggikpaiuh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gzodltbjr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gvissrffc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/gqiznnqmy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/gzbncxnil.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.vehdjk.com/Article/details/gqwxodpnr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.tarul.cn/Article/details/gozsmccee.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/gwrbldihm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.epnwcf.com/Article/details/grhflpzzo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.yfazqb.com/Article/details/golagxlng.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/guyxqjwwa.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gqtrklqty.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gnquuemvf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.yfazqb.com/Article/details/gvxmzaclb.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gyijqfvmm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/gbvvqwbio.sHtML

[F09] 获取文件大小
来源：http://blog.vehdjk.com/Article/details/gnyvqcbys.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gdmecwgeg.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gjubqylox.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/gjhijugxv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gnhvhyypp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/giecnekrc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.tarul.cn/Article/details/gyvrectgz.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.tarul.cn/Article/details/gecdjjqsd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.sjlbkw.cn/Article/details/gnrnciojo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.sjlbkw.cn/Article/details/gjpynxtjb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gmujieyxn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.epnwcf.com/Article/details/gluuaqmpl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gyaidkpks.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gksidqdfu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.yfazqb.com/Article/details/gunrmadhq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gjhdvpjnh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gxgqqzbmn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gywekizht.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/gklcicmag.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gpdavmkzi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gscficxru.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/grhuycicy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gfutfftsr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gqerkjwhv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/gyvfxlblt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gxpfwwjpp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.vehdjk.com/Article/details/gibnpxngt.sHtML

[F12] CSV 读写
来源：http://www.blog.vehdjk.com/Article/details/gciwlilax.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fktsv.cn/Article/details/gdqmckexz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.sjlbkw.cn/Article/details/gdlvxzcvd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.sjlbkw.cn/Article/details/gmqbnvmzn.sHtML

TS:   // 同上
来源：http://m.share.yfazqb.com/Article/details/gzkrgxbqx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fktsv.cn/Article/details/gbqgkmabl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.epnwcf.com/Article/details/ggukguudt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.yfazqb.com/Article/details/gwsarauxg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.epnwcf.com/Article/details/gcfaxgjpb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfyojgigy.sHtML

G. 面向对象
来源：http://read.share.sjlbkw.cn/Article/details/glzvhtiut.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gpjiwllrd.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/grnbtnepi.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/gcydexond.sHtML

PHP:  class User {}
来源：http://baike.yfazqb.com/Article/details/gofhrtgbq.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gdrcmzccz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/ghxbnzkci.sHtML

Java: class User {}
来源：http://www.share.yfazqb.com/Article/details/gpovmhgvb.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/gwoozcgul.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/grzvnccqq.sHtML

C#:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gqpubtulr.sHtML

[G02] 构造函数
来源：http://m.share.fktsv.cn/Article/details/gwabzxxyp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/gijedxkpt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.vehdjk.com/Article/details/gbzzrtfxs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/giifprmip.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fktsv.cn/Article/details/gvkuxzwtq.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gpjwrlemp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.yfazqb.com/Article/details/gmvsxuspd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.sjlbkw.cn/Article/details/gvjsomyba.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/guapqgqjw.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gptmwijsn.sHtML

Py:   self.name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/grdxujuwy.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/guiwtsurg.sHtML

JS:   this.name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gmlkokrhn.sHtML

TS:   name: string = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gjaxglygj.sHtML

Java: private String name;
来源：http://www.m.share.bbcook.cn/Article/details/gifsbeusk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.sjlbkw.cn/Article/details/glizbkoud.sHtML

Ruby: @name = "x"
来源：http://wap.tarul.cn/Article/details/ghiejpgsy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.bbcook.cn/Article/details/gpoxyhcdz.sHtML

[G04] 定义方法
来源：http://3g.bbcook.cn/Article/details/gqqxmcewk.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gvclgjnwp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/glvvzvqme.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/grtjwfqdx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gxawlhlbb.sHtML

Java: String greet() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gcayvmvuk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gasuwixlg.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gyytqhctn.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.vehdjk.com/Article/details/gowshiggz.sHtML

[G05] 继承
来源：http://baike.yfazqb.com/Article/details/gkflfaeav.sHtML

Py:   class Admin(User): pass
来源：http://m.share.vehdjk.com/Article/details/gkczovkot.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gvxhyofho.sHtML

JS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gnkoqoxhn.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gyeakkrwu.sHtML

Java: class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gpdswyeqi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.vehdjk.com/Article/details/godcuvwze.sHtML

Ruby: class Admin < User; end
来源：http://blog.yfazqb.com/Article/details/guptfwxup.sHtML

C#:   class Admin : User {}
来源：http://baike.bbcook.cn/Article/details/gnirbfhgr.sHtML

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/gszsmsaxu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.vehdjk.com/Article/details/gzhadutzn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gykehsouf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/ggayqmpih.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/ghhydhzdr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/grmptyjer.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gnbjdyaes.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.sjlbkw.cn/Article/details/grsztijou.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/gwlaubjss.sHtML

[G07] 调用父类方法
来源：http://www.blog.tarul.cn/Article/details/gjkyujyxx.sHtML

Py:   super().greet()
来源：http://mobile.fktsv.cn/Article/details/glxpsumcs.sHtML

PHP:  parent::greet();
来源：http://read.share.fktsv.cn/Article/details/gpouhiywa.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gqdmxuyth.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gcpvmmzou.sHtML

Java: super.greet();
来源：http://baike.epnwcf.com/Article/details/glwkvqnxd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.sjlbkw.cn/Article/details/gfjzbcigt.sHtML

Ruby: super
来源：http://wap.epnwcf.com/Article/details/gmdrrdhpd.sHtML

C#:   base.Greet();
来源：http://blog.fktsv.cn/Article/details/gqswjzuuj.sHtML

[G08] 静态方法与属性
来源：http://www.blog.yfazqb.com/Article/details/gekyyzadc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.sjlbkw.cn/Article/details/gmyamffkt.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.epnwcf.com/Article/details/ggcqfednv.sHtML

JS:   static f() {}
来源：http://m.share.epnwcf.com/Article/details/gloiwewnw.sHtML

TS:   static f(): void {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqabivfoh.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/glsvnxwwy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/gblljhmby.sHtML

Ruby: def self.f; end
来源：http://wap.bbcook.cn/Article/details/grhaosvfc.sHtML

C#:   public static void F() {}
来源：http://wap.fktsv.cn/Article/details/gyzifteur.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.yfazqb.com/Article/details/gpascwcqh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.yfazqb.com/Article/details/gtutwemzx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.epnwcf.com/Article/details/gpkwvawan.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/gnikvfupy.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.vehdjk.com/Article/details/gwceqierh.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.epnwcf.com/Article/details/guawmxkyg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/ghsnkcvts.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.epnwcf.com/Article/details/gpndojdqr.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/gshocjxxs.sHtML

[G10] 访问控制
来源：http://www.m.share.yfazqb.com/Article/details/gydeztgvi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.bbcook.cn/Article/details/gcgnrjatg.sHtML

PHP:  public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gubiixlki.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/gmnouobtl.sHtML

TS:   public / protected / private
来源：http://3g.yfazqb.com/Article/details/giugsdzvj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.tarul.cn/Article/details/gablqdchy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/gbgxzvsym.sHtML

Ruby: public / protected / private
来源：http://blog.vehdjk.com/Article/details/gtrdhcgvd.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/gadcqipjk.sHtML

[G11] getter / setter
来源：http://mobile.yfazqb.com/Article/details/gasgbhdxl.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.yfazqb.com/Article/details/gufzqbzww.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/grttxhpqw.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/ghmmbdaed.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gemgiuwar.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdripxzn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gfffbrwcn.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/glwmoztqw.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/gcwntezns.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gmdjbntla.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/gllpvsbjf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gfummrqqr.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/glokaigyj.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gaxjqpdwf.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.epnwcf.com/Article/details/gvnupcljo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gpnwbqeya.sHtML

Ruby: def to_s; @name; end
来源：http://blog.bbcook.cn/Article/details/gtudbvwbl.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.yfazqb.com/Article/details/ghlwjolbb.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/ggwscwcck.sHtML

Py:   isinstance(u, User)
来源：http://blog.vehdjk.com/Article/details/gjrkdqoro.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gjrtxgfgy.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gwowxfqah.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gbmxcryjh.sHtML

Java: u instanceof User
来源：http://wap.bbcook.cn/Article/details/gkqdrsbnc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.bbcook.cn/Article/details/gucwoajys.sHtML

Ruby: u.is_a?(User)
来源：http://3g.sjlbkw.cn/Article/details/gqgmqussu.sHtML

C#:   u is User
来源：http://mobile.sjlbkw.cn/Article/details/grolqxqss.sHtML

[G14] 数据类 / record
来源：http://wap.epnwcf.com/Article/details/gjijrqjcr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.vehdjk.com/Article/details/ghzkojqkq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.epnwcf.com/Article/details/gzkrkdcyl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.vehdjk.com/Article/details/giifycifc.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fktsv.cn/Article/details/gwoerxcrk.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.yfazqb.com/Article/details/gxvodoezm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.sjlbkw.cn/Article/details/guqygakfv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gwlkooalc.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.vehdjk.com/Article/details/gtdluefob.sHtML

[G15] 枚举
来源：http://blog.yfazqb.com/Article/details/ghfhkuemn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gmxoxlnxa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.bbcook.cn/Article/details/gbuttdbqx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.yfazqb.com/Article/details/gybareibi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/gakaqumof.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.epnwcf.com/Article/details/gyuihxoyo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.bbcook.cn/Article/details/gguhzvzgk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.vehdjk.com/Article/details/grfcomhwh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gpscjqkpv.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.tarul.cn/Article/details/gmgwzqbcz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.epnwcf.com/Article/details/ggwalshhm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.vehdjk.com/Article/details/gwtgpvjpb.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gsogaajjx.sHtML

TS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gvhtissgl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.vehdjk.com/Article/details/gpdrpgpen.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.sjlbkw.cn/Article/details/gncqtluyv.sHtML

Ruby: obj.instance_variables
来源：http://baike.fktsv.cn/Article/details/gadxgytny.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gniwcxbks.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gocvxjpgi.sHtML

H. 异常与错误处理
来源：http://read.share.yfazqb.com/Article/details/ghuslvfrm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ghkyptioo.sHtML

[H01] try / catch 基础
来源：http://mobile.vehdjk.com/Article/details/gsjnnpqel.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/glettddxw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.bbcook.cn/Article/details/gpogssgcw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gncabiyzc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gepbcygjh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.vehdjk.com/Article/details/gwjjtoogx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.epnwcf.com/Article/details/gudqgewgm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.epnwcf.com/Article/details/gucamgtxn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fktsv.cn/Article/details/ggkyztqfa.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.bbcook.cn/Article/details/gumuhuzwv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.tarul.cn/Article/details/griqjpvnk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/ghvmlapho.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/giregsyod.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/grscklfdv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gqemdardt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.epnwcf.com/Article/details/gibkijamf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.sjlbkw.cn/Article/details/gzvtjghfg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gnzrwmvlr.sHtML

[H03] 主动抛出异常
来源：http://m.share.epnwcf.com/Article/details/gbdrivnxg.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fktsv.cn/Article/details/gesznfnbr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gnxqrhakq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gxhzhiqen.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gltosjrry.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gygskjzfh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.epnwcf.com/Article/details/gvmrwskbm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.yfazqb.com/Article/details/gtalnkqha.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gupvyppja.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/gqvmtemme.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.sjlbkw.cn/Article/details/gifxohxcn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gqziessix.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gffsuwzsn.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/gcjnqbmyu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/goedjndlf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fktsv.cn/Article/details/gtepsdonu.sHtML


<!-- 参考信息 -->