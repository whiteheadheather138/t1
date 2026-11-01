代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.bbcook.cn/Article/details/gmttyvffx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gsgojzgsf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gewglwuvi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/griiedqcv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gpmthmfip.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.sjlbkw.cn/Article/details/gffxbazur.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gogdmlplu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gbqlawsjh.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/gfxvfhggl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.epnwcf.com/Article/details/gapjcqcgt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gnkgpsqvj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fktsv.cn/Article/details/ghqnnxzdj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/grpofcfrj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.vehdjk.com/Article/details/gxggpnikx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.yfazqb.com/Article/details/gczzztnxm.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fktsv.cn/Article/details/gigzzokki.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.bbcook.cn/Article/details/gpttpeuey.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ganufovar.sHtML

F. 文件与目录
来源：http://www.m.share.epnwcf.com/Article/details/gbicnfexj.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfxdbtjbd.sHtML

[F01] 读取整个文件
来源：http://read.share.vehdjk.com/Article/details/givfcofcy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.epnwcf.com/Article/details/ghssljvdf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.tarul.cn/Article/details/gxwlbtheu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.sjlbkw.cn/Article/details/grhpotmex.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.tarul.cn/Article/details/giosswoqg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gcaebhsuj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.sjlbkw.cn/Article/details/gumpxmpuq.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gprremnaf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gkkajiqou.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/gllaijlcp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/gnuxrlhav.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.epnwcf.com/Article/details/gyzezxyru.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/ghkybbyma.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/goxogkose.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/gorbliits.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.tarul.cn/Article/details/ghkgfrinp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.vehdjk.com/Article/details/gldnfjpek.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.yfazqb.com/Article/details/gtaldfjya.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.bbcook.cn/Article/details/gyaysaycx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/ggrwcjacr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/gqznjrxmy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gkseqauhw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gsztoofje.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.tarul.cn/Article/details/gckaoprag.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.tarul.cn/Article/details/gmqwobnrr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gxtcisoeh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gpsutqomi.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fktsv.cn/Article/details/gmjsajqbp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gnhrlnfoi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gzrxjckuw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/ggyieijzr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gqkvjwsvr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/gkyhlhnxi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.vehdjk.com/Article/details/gqcuuoywi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.tarul.cn/Article/details/gtircfbao.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.yfazqb.com/Article/details/gyjcsesdr.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gidrgdfua.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.yfazqb.com/Article/details/gzlgpkyym.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gzorbdzvo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gawcgmjae.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gvwtcfeuk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gsfdahwfn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/goenkkiwn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gonlvclbj.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gwtcfanms.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/glozsbotf.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gjgvpdxyb.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.yfazqb.com/Article/details/goazxgklg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/greqloquw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/glywbpghi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gvtyaxvgb.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/ggunqdycz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.tarul.cn/Article/details/gdptsrorq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.epnwcf.com/Article/details/guzopblgm.sHtML

[F07] 创建目录（含多级）
来源：http://blog.yfazqb.com/Article/details/gpihgfhip.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gjhvrgpve.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.bbcook.cn/Article/details/gfaiakqno.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/gcdccjhns.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gcltiylge.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fktsv.cn/Article/details/ghlybavge.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/gdgodhgtr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fktsv.cn/Article/details/gwaisakkg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.vehdjk.com/Article/details/gkzftenaa.sHtML

[F08] 遍历目录
来源：http://m.share.vehdjk.com/Article/details/ghyhxzjkj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.yfazqb.com/Article/details/grjocdoag.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.epnwcf.com/Article/details/grxtjvjff.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/guzqriahp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdwcqtup.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/ghdwdutou.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gmsiihkqk.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gtumtqlau.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.epnwcf.com/Article/details/gtybtnmcb.sHtML

[F09] 获取文件大小
来源：http://www.share.fktsv.cn/Article/details/gsibwugcu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/grvsmntrn.sHtML

PHP:  filesize("a.txt");
来源：http://baike.bbcook.cn/Article/details/gsjdnjtju.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gwsvjnhvq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gxvtabsjz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gnezqhqem.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.bbcook.cn/Article/details/gcdbqvnyg.sHtML

Ruby: File.size("a.txt")
来源：http://3g.epnwcf.com/Article/details/gppwhcpes.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fktsv.cn/Article/details/gobcdupat.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.bbcook.cn/Article/details/gvetltvvf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gbbtzreaj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/gfhlpellk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/ghlmtxfzp.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gsyohcvur.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fktsv.cn/Article/details/gxlmjgftc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gearchdwm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gdydxptdl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/ggmhsbgzw.sHtML

[F11] 复制与移动文件
来源：http://wap.epnwcf.com/Article/details/gaatprziu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gmfbhdfzh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.yfazqb.com/Article/details/gbuygbboo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gkuehossw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gzauvphxj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gtrhthbsr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.epnwcf.com/Article/details/gvvtfpboj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gmazzkmnc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/grjqbnxnt.sHtML

[F12] CSV 读写
来源：http://baike.vehdjk.com/Article/details/gpfhuwvgb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.bbcook.cn/Article/details/gurekoqfj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/gvjfpzwnl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gjuougixm.sHtML

TS:   // 同上
来源：http://baike.vehdjk.com/Article/details/gxjasnqrd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fktsv.cn/Article/details/glgemrttm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.vehdjk.com/Article/details/ghwymukdw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.yfazqb.com/Article/details/gcyqllwrc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.tarul.cn/Article/details/gguqgvatq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghqftocmw.sHtML

G. 面向对象
来源：http://mobile.yfazqb.com/Article/details/gekpbctoo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxhrhwwip.sHtML

[G01] 定义类
来源：http://wap.yfazqb.com/Article/details/gfblmzcwv.sHtML

Py:   class User: pass
来源：http://m.share.epnwcf.com/Article/details/gcbfmmfde.sHtML

PHP:  class User {}
来源：http://3g.yfazqb.com/Article/details/gppffbsaa.sHtML

JS:   class User {}
来源：http://baike.vehdjk.com/Article/details/gdtdbfjfw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fktsv.cn/Article/details/gbviifaln.sHtML

Java: class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gtzjzbsqj.sHtML

Go:   type User struct { Name string }
来源：http://blog.epnwcf.com/Article/details/gxnamyjjn.sHtML

Ruby: class User; end
来源：http://3g.yfazqb.com/Article/details/gafpjfjuk.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gwpptslij.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/ginyblhpk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/ghqnnfncg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.yfazqb.com/Article/details/guxvvfije.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/gknkivbmh.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.vehdjk.com/Article/details/gflqggkkm.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gpnffgoaa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/gbtqhzalr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/gwkytfrcd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fktsv.cn/Article/details/grlvxgssf.sHtML

[G03] 实例属性
来源：http://wap.vehdjk.com/Article/details/ganitkeug.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/gjdfywnzv.sHtML

PHP:  public string $name = "x";
来源：http://wap.fktsv.cn/Article/details/gbkovqiti.sHtML

JS:   this.name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxbpoemw.sHtML

TS:   name: string = "x";
来源：http://blog.bbcook.cn/Article/details/gpcbeygfi.sHtML

Java: private String name;
来源：http://read.share.yfazqb.com/Article/details/gqnjbtaeh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fktsv.cn/Article/details/gdkyfcmrc.sHtML

Ruby: @name = "x"
来源：http://blog.yfazqb.com/Article/details/gafowrpuz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.tarul.cn/Article/details/gevmbfvqg.sHtML

[G04] 定义方法
来源：http://www.m.share.tarul.cn/Article/details/gjbofdauo.sHtML

Py:   def greet(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gncyknfsk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gtdcfxyen.sHtML

JS:   greet() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gculrjbjm.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gwziufgeu.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/gwyklpssb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gjhgiajck.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/gigmeoqux.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gnhuzjsju.sHtML

[G05] 继承
来源：http://3g.sjlbkw.cn/Article/details/gxbprvuxd.sHtML

Py:   class Admin(User): pass
来源：http://mobile.epnwcf.com/Article/details/gdscljqru.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/ghyugxfrh.sHtML

JS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gfmzpycqm.sHtML

TS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gptpkrykr.sHtML

Java: class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/glpcqxtvq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gerhnncan.sHtML

Ruby: class Admin < User; end
来源：http://m.share.bbcook.cn/Article/details/gmilygyds.sHtML

C#:   class Admin : User {}
来源：http://mobile.tarul.cn/Article/details/gyvixtpug.sHtML

[G06] 重写方法
来源：http://www.blog.bbcook.cn/Article/details/gfdoaegfe.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/gussvklcr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gbveoiwdb.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/ghyuwwmwp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gbedxlrra.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/glhuwfmjg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fktsv.cn/Article/details/gpdzxvaum.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.vehdjk.com/Article/details/gsksifnmz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.epnwcf.com/Article/details/gibghjcgu.sHtML

[G07] 调用父类方法
来源：http://m.share.fktsv.cn/Article/details/gxgcyguvl.sHtML

Py:   super().greet()
来源：http://www.m.share.tarul.cn/Article/details/gfefvunjf.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/gpgggzkay.sHtML

JS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gdyozrxme.sHtML

TS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gnomtvwyb.sHtML

Java: super.greet();
来源：http://baike.fktsv.cn/Article/details/gvnrvpadj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.yfazqb.com/Article/details/giwdomhxj.sHtML

Ruby: super
来源：http://www.blog.yfazqb.com/Article/details/gwclavucf.sHtML

C#:   base.Greet();
来源：http://baike.bbcook.cn/Article/details/gzfnqwdyz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.vehdjk.com/Article/details/gfgzrbzqi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/gtckcesky.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/gvccgpwlx.sHtML

JS:   static f() {}
来源：http://mobile.bbcook.cn/Article/details/guzhrudin.sHtML

TS:   static f(): void {}
来源：http://mobile.bbcook.cn/Article/details/gllvfwlih.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/gtzxvsufy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gbamhhtdm.sHtML

Ruby: def self.f; end
来源：http://m.share.tarul.cn/Article/details/gpodoelwd.sHtML

C#:   public static void F() {}
来源：http://www.blog.tarul.cn/Article/details/gwdektwmo.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.yfazqb.com/Article/details/glydbnfhy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.bbcook.cn/Article/details/gcfgdmfue.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.bbcook.cn/Article/details/ghylyjdrh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.yfazqb.com/Article/details/gxchyykch.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.epnwcf.com/Article/details/gfqpsartj.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gafpnamzw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fktsv.cn/Article/details/gjnkbuslc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.sjlbkw.cn/Article/details/ghnhpercs.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.vehdjk.com/Article/details/gtsvtewou.sHtML

[G10] 访问控制
来源：http://www.blog.bbcook.cn/Article/details/grlzwitry.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.sjlbkw.cn/Article/details/gwrsfgaoe.sHtML

PHP:  public / protected / private
来源：http://3g.tarul.cn/Article/details/gnaztygrb.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.vehdjk.com/Article/details/ginwxiqqq.sHtML

TS:   public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/ghkldovhf.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.bbcook.cn/Article/details/gyhbiigru.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/gszwlbell.sHtML

Ruby: public / protected / private
来源：http://blog.fktsv.cn/Article/details/ggramuydn.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.yfazqb.com/Article/details/guuzocmjl.sHtML

[G11] getter / setter
来源：http://blog.bbcook.cn/Article/details/gaiqvxjes.sHtML

Py:   @property 与 @x.setter
来源：http://blog.vehdjk.com/Article/details/giekfzpih.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gwpmwferx.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gflmdajoe.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gtugbjzyk.sHtML

Java: public String getName() { return name; }
来源：http://read.share.tarul.cn/Article/details/gnnxpmrux.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/ggqnmhonu.sHtML

Ruby: attr_accessor :name
来源：http://www.share.epnwcf.com/Article/details/gieekwegv.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.tarul.cn/Article/details/gnjxjxegl.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/gefgctcgi.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/guoyisaur.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gjuvslxqv.sHtML

JS:   toString() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gvwkoginw.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gteplbwuc.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.yfazqb.com/Article/details/gkiynuubk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gqgtojjeu.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.vehdjk.com/Article/details/gzxpllrxa.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/giqnjetwz.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/gmxplgmjz.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.yfazqb.com/Article/details/gbjxqfzzu.sHtML

PHP:  $u instanceof User
来源：http://baike.epnwcf.com/Article/details/gfeptllez.sHtML

JS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gqugvslcv.sHtML

TS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gntntcnrg.sHtML

Java: u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gkgwhaios.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.bbcook.cn/Article/details/gfbrsaihs.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.sjlbkw.cn/Article/details/gmvhhtrkk.sHtML

C#:   u is User
来源：http://mobile.yfazqb.com/Article/details/grgywxdhd.sHtML

[G14] 数据类 / record
来源：http://www.m.share.yfazqb.com/Article/details/grmxiajxc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.sjlbkw.cn/Article/details/gduiemfbb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.epnwcf.com/Article/details/gphugxpkv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.sjlbkw.cn/Article/details/gxwcjtvwh.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.yfazqb.com/Article/details/gblrfhjhu.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.sjlbkw.cn/Article/details/gyxozcikq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.yfazqb.com/Article/details/gexjlfpan.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.yfazqb.com/Article/details/gduwvrbbu.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.sjlbkw.cn/Article/details/gnmjhdhki.sHtML

[G15] 枚举
来源：http://blog.epnwcf.com/Article/details/gdqxdwxiv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.vehdjk.com/Article/details/gsugdhanq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/ggkbtfsbm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.sjlbkw.cn/Article/details/gufiegxek.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/gwnocjtwo.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fktsv.cn/Article/details/gtxokjiwg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.sjlbkw.cn/Article/details/gjidvmjes.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.yfazqb.com/Article/details/gnwarlqzz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/gilmdbzeh.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.tarul.cn/Article/details/gqqgaahrg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/gqluhhjcb.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.epnwcf.com/Article/details/gyqzbkztp.sHtML

JS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/gppmeofbc.sHtML

TS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/guymryngr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.yfazqb.com/Article/details/gsehmkims.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fktsv.cn/Article/details/gwvzqzwca.sHtML

Ruby: obj.instance_variables
来源：http://baike.sjlbkw.cn/Article/details/gpchfjntf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gnlqycjso.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gouclqwtr.sHtML

H. 异常与错误处理
来源：http://3g.vehdjk.com/Article/details/gjgsqssmz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gcwfnclay.sHtML

[H01] try / catch 基础
来源：http://www.blog.sjlbkw.cn/Article/details/gllvctdvx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/gmlwtsxdy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fktsv.cn/Article/details/gjatilyuu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gryfovovq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.yfazqb.com/Article/details/gjglsucdn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.tarul.cn/Article/details/gkpodbzlh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.yfazqb.com/Article/details/gnvcqvgzk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gascgieth.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fktsv.cn/Article/details/gyurhrmjx.sHtML

[H02] finally / ensure 收尾
来源：http://3g.tarul.cn/Article/details/gopyelfmh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.sjlbkw.cn/Article/details/ghhalbllr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gbftiivos.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gryeyakar.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gluppnewa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gzyfhyiui.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.tarul.cn/Article/details/galdpntrd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.tarul.cn/Article/details/gwstanphu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gsowuvtrr.sHtML

[H03] 主动抛出异常
来源：http://m.share.bbcook.cn/Article/details/gdxgimcft.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.vehdjk.com/Article/details/gfuaoxifb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/glmryxqoa.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gonebdukf.sHtML


<!-- 参考信息 -->