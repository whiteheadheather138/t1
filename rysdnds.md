代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.vehdjk.com/Article/details/geazyxbbl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.epnwcf.com/Article/details/gxrphntoh.sHtML

TS:   if (s === "") {}
来源：http://www.blog.vehdjk.com/Article/details/gyvgbivov.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/goxuuiolv.sHtML

Go:   if s == "" {}
来源：http://blog.fktsv.cn/Article/details/gqgecevlq.sHtML

Ruby: if s.empty?
来源：http://wap.fktsv.cn/Article/details/gjpuresba.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.yfazqb.com/Article/details/gruyzhiyf.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.epnwcf.com/Article/details/gbiulcqrh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.tarul.cn/Article/details/gdlwhomif.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gctssuueu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gjghlffdj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gxfnwuhxn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gdcazwnan.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.yfazqb.com/Article/details/gcvkyqvdl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gjdviycce.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/ghywempma.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.tarul.cn/Article/details/gagvfbuhb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gjfgvecew.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/guctdguot.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gydmthrcz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gbxbzemyp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.tarul.cn/Article/details/gmruugokl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fktsv.cn/Article/details/gqhkllfzj.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.epnwcf.com/Article/details/guxkjmqyp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwdtunfh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/guaowxfag.sHtML

F. 文件与目录
来源：http://blog.sjlbkw.cn/Article/details/gsfnaqidl.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gkiabzzed.sHtML

[F01] 读取整个文件
来源：http://read.share.vehdjk.com/Article/details/grguhdgvp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/gqsfsrtol.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gutetfayy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.bbcook.cn/Article/details/gmuolkvnw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fktsv.cn/Article/details/gggolqavm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gizruwfmi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.vehdjk.com/Article/details/ggulvfqfc.sHtML

Ruby: File.read("a.txt")
来源：http://baike.vehdjk.com/Article/details/gvhfyuona.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.yfazqb.com/Article/details/glzicqzfl.sHtML

[F02] 逐行读取文件
来源：http://baike.yfazqb.com/Article/details/gweaqxfmt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.sjlbkw.cn/Article/details/gomxykynp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.bbcook.cn/Article/details/gqkavlfwr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gpdvvlbbl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gwedpyoyr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/ghhnjtaoc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/gunukvhlj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.yfazqb.com/Article/details/gwuwujvna.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.tarul.cn/Article/details/gcvpituap.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/giwcrdeug.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.sjlbkw.cn/Article/details/grpaibxwo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gwsguuhly.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gehntjibi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gicjqfoaz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.yfazqb.com/Article/details/gsfwikzno.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.yfazqb.com/Article/details/gjrxffqgv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/gefwdsslk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gjqnhqfta.sHtML

[F04] 追加写入文件
来源：http://blog.vehdjk.com/Article/details/gydedotst.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fktsv.cn/Article/details/gwikcjzsr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.vehdjk.com/Article/details/gcyglvvxx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gatdwqwxj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/gprrjhnuk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.vehdjk.com/Article/details/gxeawarhk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.bbcook.cn/Article/details/gesdulfum.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/gvbweywyv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gyxpexquc.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.vehdjk.com/Article/details/gsejfrqws.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.yfazqb.com/Article/details/gadusexca.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.vehdjk.com/Article/details/gkqpcevww.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/geekcguno.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gvnqmgvjn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gcmdwssap.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.yfazqb.com/Article/details/gokrqncfr.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gvvsbxzde.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gfibbdloe.sHtML

[F06] 删除文件
来源：http://3g.sjlbkw.cn/Article/details/gwdpkkdfz.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gadlxfupz.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gglfvsumn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ggzdnswel.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gbcmtjzhk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gbusysnyu.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gaqacrmmf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/glzzlfuqp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/geglvvswp.sHtML

[F07] 创建目录（含多级）
来源：http://baike.yfazqb.com/Article/details/gzfnyxkyb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/gwxrakgkp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fktsv.cn/Article/details/giyqmohbl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/glydcxwxa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gdczwmkyi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.yfazqb.com/Article/details/gbzprzytc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.tarul.cn/Article/details/gqlatvcmk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fktsv.cn/Article/details/ggynlmgfm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fktsv.cn/Article/details/gwnzrajtx.sHtML

[F08] 遍历目录
来源：http://www.blog.yfazqb.com/Article/details/ghblgytvn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/giziyrdkp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/ggnsrlrbs.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gapkevmdq.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gspmuvmrw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gkgwiacrx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.bbcook.cn/Article/details/ghwdieihq.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.tarul.cn/Article/details/gegmbotfs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fktsv.cn/Article/details/gxmevplgi.sHtML

[F09] 获取文件大小
来源：http://3g.fktsv.cn/Article/details/gekxqayfp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gikezrtuf.sHtML

PHP:  filesize("a.txt");
来源：http://wap.epnwcf.com/Article/details/gsbaxjbpu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/gbwxlsfql.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/giiuddkyi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gdflesuna.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/glfyphwmw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.tarul.cn/Article/details/gipvpdkey.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.tarul.cn/Article/details/ghuwicurk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.bbcook.cn/Article/details/gijwnbhvf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gggglzegj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.vehdjk.com/Article/details/guxqxnutc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gnuwwdqck.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fktsv.cn/Article/details/gvkxzppsh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.bbcook.cn/Article/details/guisofldh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gwpszfgaa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/ggxhshdif.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gaandnhwy.sHtML

[F11] 复制与移动文件
来源：http://blog.bbcook.cn/Article/details/gavviwpwc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gdxshncux.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.bbcook.cn/Article/details/gevtxsorh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gkaorgblb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/ggfjhhdyh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/geimljspt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.epnwcf.com/Article/details/gxpneuvtl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gsqzqfboa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.tarul.cn/Article/details/gvdwulgcb.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gxvwjqcht.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fktsv.cn/Article/details/gazpftuiq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.yfazqb.com/Article/details/gfpgpteao.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.epnwcf.com/Article/details/gpjatvccc.sHtML

TS:   // 同上
来源：http://3g.vehdjk.com/Article/details/gsmpfszlf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/gbhccxtiu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fktsv.cn/Article/details/gammwpxow.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.tarul.cn/Article/details/gcedrvmdc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/gcultyvzu.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwaudjioy.sHtML

G. 面向对象
来源：http://www.share.tarul.cn/Article/details/ggrlbgrgh.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grxdnbzdf.sHtML

[G01] 定义类
来源：http://3g.bbcook.cn/Article/details/gkftfiqtn.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gahglwesc.sHtML

PHP:  class User {}
来源：http://baike.sjlbkw.cn/Article/details/gmkowzmdr.sHtML

JS:   class User {}
来源：http://wap.bbcook.cn/Article/details/ghhnryefb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.vehdjk.com/Article/details/ghjllrczh.sHtML

Java: class User {}
来源：http://baike.fktsv.cn/Article/details/gthlebvvy.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/gibakyzpa.sHtML

Ruby: class User; end
来源：http://baike.yfazqb.com/Article/details/gusrrcrrg.sHtML

C#:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gelbalemr.sHtML

[G02] 构造函数
来源：http://blog.bbcook.cn/Article/details/gjvmphrvl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.yfazqb.com/Article/details/gsmynakgh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.bbcook.cn/Article/details/ghudiwwof.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gmvafkyzl.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.yfazqb.com/Article/details/glycciyta.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/goigschpy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.bbcook.cn/Article/details/guynodsef.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.tarul.cn/Article/details/gwcguvvkd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.tarul.cn/Article/details/gotkybxak.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gbkqvnnxg.sHtML

Py:   self.name = "x"
来源：http://read.share.vehdjk.com/Article/details/gjiyjjyxb.sHtML

PHP:  public string $name = "x";
来源：http://blog.sjlbkw.cn/Article/details/guwivdgau.sHtML

JS:   this.name = "x";
来源：http://www.blog.epnwcf.com/Article/details/gjbhevidr.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/gqwylvqrb.sHtML

Java: private String name;
来源：http://blog.tarul.cn/Article/details/gdetvcxmu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.sjlbkw.cn/Article/details/gkwrgxlex.sHtML

Ruby: @name = "x"
来源：http://wap.epnwcf.com/Article/details/givzsnmgf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.tarul.cn/Article/details/gaqkkbujk.sHtML

[G04] 定义方法
来源：http://m.share.fktsv.cn/Article/details/gupoamrgz.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.sjlbkw.cn/Article/details/gnahpvuhf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gqmwgxlzx.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gpwutylbr.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gczkdjkip.sHtML

Java: String greet() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gbwmtemnp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/ghufhzrkr.sHtML

Ruby: def greet; @name; end
来源：http://www.share.bbcook.cn/Article/details/gxvfdckud.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gpwbjwojt.sHtML

[G05] 继承
来源：http://baike.vehdjk.com/Article/details/gdiqaynxb.sHtML

Py:   class Admin(User): pass
来源：http://wap.tarul.cn/Article/details/gftfjcqeb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gsvbtmnec.sHtML

JS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gduchglfr.sHtML

TS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gieboxoqr.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gsbjmbzfr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.tarul.cn/Article/details/gxurhvxla.sHtML

Ruby: class Admin < User; end
来源：http://baike.epnwcf.com/Article/details/gukjlbtyw.sHtML

C#:   class Admin : User {}
来源：http://www.share.sjlbkw.cn/Article/details/gwhesntqo.sHtML

[G06] 重写方法
来源：http://3g.sjlbkw.cn/Article/details/gvvsqpttf.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/gmlfkorgm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/giluxifdk.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gocljbnqe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gnxcirvxd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gxxkvuime.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.epnwcf.com/Article/details/gvkhkbjlf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.vehdjk.com/Article/details/ghoxprjio.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.bbcook.cn/Article/details/gingcqvfv.sHtML

[G07] 调用父类方法
来源：http://baike.sjlbkw.cn/Article/details/gcrmsuijl.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gyrgjepqa.sHtML

PHP:  parent::greet();
来源：http://3g.bbcook.cn/Article/details/gigtgfepd.sHtML

JS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/glfppbrnx.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/ggmnzamvv.sHtML

Java: super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gcebfquec.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.tarul.cn/Article/details/gbooktlss.sHtML

Ruby: super
来源：http://wap.epnwcf.com/Article/details/gjwgogeha.sHtML

C#:   base.Greet();
来源：http://read.share.vehdjk.com/Article/details/gonhvplpa.sHtML

[G08] 静态方法与属性
来源：http://www.blog.vehdjk.com/Article/details/gzngkeijd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fktsv.cn/Article/details/gtthpgtdj.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/gpywhdeop.sHtML

JS:   static f() {}
来源：http://read.share.tarul.cn/Article/details/gjqefrscx.sHtML

TS:   static f(): void {}
来源：http://baike.sjlbkw.cn/Article/details/gjhktqzvb.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/grgfjyqet.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.sjlbkw.cn/Article/details/ggdqcbqnl.sHtML

Ruby: def self.f; end
来源：http://read.share.bbcook.cn/Article/details/gbenxreie.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/gepvkskpx.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/gchchviqs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.bbcook.cn/Article/details/gvzylhuic.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.epnwcf.com/Article/details/ggzsbkcmq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.tarul.cn/Article/details/ghifgbbym.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.vehdjk.com/Article/details/gqkyrfiej.sHtML

Java: interface Shape { double area(); }
来源：http://3g.epnwcf.com/Article/details/geavktkcs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.sjlbkw.cn/Article/details/gxmtyxbzh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/gzjjksmgg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fktsv.cn/Article/details/gtnbsvaxe.sHtML

[G10] 访问控制
来源：http://baike.vehdjk.com/Article/details/ghdeqcavh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.vehdjk.com/Article/details/gusnaulbf.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gcvsjccgu.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.epnwcf.com/Article/details/gslkftbvg.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/geozjhxnm.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/gpssmhbgd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.sjlbkw.cn/Article/details/glefypzhq.sHtML

Ruby: public / protected / private
来源：http://3g.bbcook.cn/Article/details/gqablmwwt.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gderaaawg.sHtML

[G11] getter / setter
来源：http://read.share.yfazqb.com/Article/details/gnaawokml.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.epnwcf.com/Article/details/gcrzsrehf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/guxikdftz.sHtML

JS:   get name() { return this._name; }
来源：http://3g.epnwcf.com/Article/details/gjnxcqbea.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gnnkyzcsw.sHtML

Java: public String getName() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gjoxwbvqq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gbuaprwnv.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.vehdjk.com/Article/details/glsxaaeon.sHtML

C#:   public string Name { get; set; }
来源：http://blog.epnwcf.com/Article/details/gnadubvmc.sHtML

[G12] 对象转字符串
来源：http://3g.bbcook.cn/Article/details/gevbfihvz.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gdshpmyrt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.tarul.cn/Article/details/gjavmoghn.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gldzlfrfu.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/gqxjnoqat.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gvpdqyzrc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/ghxdsyclq.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/gvakdqype.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.tarul.cn/Article/details/ggftoyaxz.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/gefjsntdc.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.tarul.cn/Article/details/gwylnitub.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gughdbhdd.sHtML

JS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gsfhqpgdl.sHtML

TS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gmzluklws.sHtML

Java: u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gjeirfsjx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.tarul.cn/Article/details/gbylmuzou.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.vehdjk.com/Article/details/gpzufwajh.sHtML

C#:   u is User
来源：http://mobile.fktsv.cn/Article/details/gyqrxnfyo.sHtML

[G14] 数据类 / record
来源：http://blog.fktsv.cn/Article/details/gfcwnlkuc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/gubmdfmdh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.yfazqb.com/Article/details/gyffmqjfk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.bbcook.cn/Article/details/gumuehsvl.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.sjlbkw.cn/Article/details/ggsxsncnu.sHtML

Java: record User(String name, int age) {}
来源：http://baike.yfazqb.com/Article/details/gupvhfeea.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.bbcook.cn/Article/details/gprllrkzf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/gxrfvctpj.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.vehdjk.com/Article/details/grxrpoxkp.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gupenfziz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.sjlbkw.cn/Article/details/glscjmwvr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.tarul.cn/Article/details/ginjzebnt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.yfazqb.com/Article/details/gwmkrdyak.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gsmgkfajr.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/gguxsxgqi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/ggsxkxdgs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.yfazqb.com/Article/details/gvntsrgsx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gkktiimly.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.vehdjk.com/Article/details/gfrboxjux.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.sjlbkw.cn/Article/details/ggtkvfadr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.yfazqb.com/Article/details/ghjrkfofm.sHtML

JS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/ghpmkapha.sHtML

TS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/gysezcsth.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.bbcook.cn/Article/details/gsuowexpa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqwoexpt.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fktsv.cn/Article/details/gqnqsuepv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.tarul.cn/Article/details/ghbeevbim.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/giqnyuvqi.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/gaawdmtol.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gomjheoeh.sHtML

[H01] try / catch 基础
来源：http://3g.tarul.cn/Article/details/gtuagtguy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/gsxlpldpu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.yfazqb.com/Article/details/gnhfeenzg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gyknkjuoc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gjbrfyzoh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.tarul.cn/Article/details/gdjgbobme.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.vehdjk.com/Article/details/gshphzuro.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.bbcook.cn/Article/details/gmefhydzt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/gknktklsu.sHtML

[H02] finally / ensure 收尾
来源：http://wap.yfazqb.com/Article/details/guqvnnjqc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.tarul.cn/Article/details/gfgezjmzz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/grisckchr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/gkrjylnvc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gapwkkpcc.sHtML


<!-- 参考信息 -->