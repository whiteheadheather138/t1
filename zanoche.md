代发 wailian999

Go:   if s == "" {}
来源：http://www.m.share.tarul.cn/Article/details/gkocnhmaz.sHtML

Ruby: if s.empty?
来源：http://3g.sjlbkw.cn/Article/details/goibjefqi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/giyksfacp.sHtML

[E21] 超长截断加省略号
来源：http://www.share.epnwcf.com/Article/details/gtvaovxdh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fktsv.cn/Article/details/ghubzyqal.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gejbgutrr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gxlstfwij.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gwyirxkwn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gkzvpmvci.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.vehdjk.com/Article/details/gwzinfiyu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gnrbvcpnr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gjxfsnzwq.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.tarul.cn/Article/details/glejtjvyj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gqdanothp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gqmcwdyjz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gvmsdkqju.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gutupyccn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/ghgicknsk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/gnlaflefi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gtasnaspl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.vehdjk.com/Article/details/gyovxmlgh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gkktiqvuq.sHtML

F. 文件与目录
来源：http://mobile.vehdjk.com/Article/details/gobnbzcof.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gleniwrgy.sHtML

[F01] 读取整个文件
来源：http://3g.fktsv.cn/Article/details/glrunsfqi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fktsv.cn/Article/details/gjyqtmhlq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gvljvhspo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gifllzbis.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.vehdjk.com/Article/details/ghdumqzno.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gyambsygi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.bbcook.cn/Article/details/gcrtdsjvq.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gsqohdknc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.bbcook.cn/Article/details/grsnkttdl.sHtML

[F02] 逐行读取文件
来源：http://m.share.yfazqb.com/Article/details/ghdqsokmh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/gqqzcbhys.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fktsv.cn/Article/details/gvniqomkd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gmxusizft.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gnvlyfydl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gkpikizzi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.yfazqb.com/Article/details/gfoawuvjh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.yfazqb.com/Article/details/gvzqsbthq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fktsv.cn/Article/details/gaqpnokik.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.tarul.cn/Article/details/gzzchvgkq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.tarul.cn/Article/details/gsxvvxhfs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gddzxduio.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gryqvqbdh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gxnjecgty.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gqxibudcl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.epnwcf.com/Article/details/gmotskkqc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fktsv.cn/Article/details/glhnbeael.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/gzwenuirr.sHtML

[F04] 追加写入文件
来源：http://blog.bbcook.cn/Article/details/ghgvqgvan.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fktsv.cn/Article/details/gvcwxkbdo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/geiwernex.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gntwwebwj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gmdilfxil.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.tarul.cn/Article/details/gefxfoivg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.yfazqb.com/Article/details/gxjwsabtn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.epnwcf.com/Article/details/gqahnxuas.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gqdxobxgm.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.vehdjk.com/Article/details/gvvrdxfiq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/gstdrweox.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/glvgxnlob.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/geixuzesl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gckmfqoin.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gdavtugdr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.tarul.cn/Article/details/gtideyoez.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.bbcook.cn/Article/details/gssbolfam.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/glzndaedr.sHtML

[F06] 删除文件
来源：http://m.share.fktsv.cn/Article/details/gepdxhsqd.sHtML

Py:   os.remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gwfirtegw.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.tarul.cn/Article/details/gdutlogax.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gbufnuetz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gwzavefsa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gefbkurbu.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gszemsxtd.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gtxdxpxzh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gobfdigae.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fktsv.cn/Article/details/gsoubdwvp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gexoopsam.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fktsv.cn/Article/details/gpqkkxqaj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.epnwcf.com/Article/details/ginyupyfg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gqtxwzhgx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.yfazqb.com/Article/details/gkdgqcspu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.sjlbkw.cn/Article/details/gyqpgmqeo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.tarul.cn/Article/details/gtnguduae.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.bbcook.cn/Article/details/gkajnuuvc.sHtML

[F08] 遍历目录
来源：http://www.m.share.epnwcf.com/Article/details/gzsbfksuv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.vehdjk.com/Article/details/gmhjcynss.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fktsv.cn/Article/details/gjagmbeis.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gbqtgddnh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/grcbicjyk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/ghetgqrrr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.sjlbkw.cn/Article/details/gdsclswii.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.epnwcf.com/Article/details/gxciwsydo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.epnwcf.com/Article/details/gzttjbsbf.sHtML

[F09] 获取文件大小
来源：http://www.m.share.bbcook.cn/Article/details/gubtugfry.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gdappvwci.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gyexhrxjy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gqwukokox.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gygqwupgn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/ggmkeqnhd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gfufpykhr.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/gswzwnngw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.yfazqb.com/Article/details/gqxoqoqmz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.tarul.cn/Article/details/grtbojqdj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gaonaomst.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gpduiuues.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/giahbuejp.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/gqjprrkwe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.bbcook.cn/Article/details/gqcqjdqmo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gvqwbtfni.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gudvmwdqn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqgeqhtr.sHtML

[F11] 复制与移动文件
来源：http://wap.tarul.cn/Article/details/getrparul.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gkubectcx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.tarul.cn/Article/details/gldnvlenb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/glrktespy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gmtxpuhlj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gxidcrlxl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/gqwaqgnbt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gfkqwwajf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.sjlbkw.cn/Article/details/gihqlvopp.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/gzhkmgylj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.vehdjk.com/Article/details/gcjatqnmi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.sjlbkw.cn/Article/details/gztxoczbk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.yfazqb.com/Article/details/guzbjeahj.sHtML

TS:   // 同上
来源：http://baike.sjlbkw.cn/Article/details/gpvlehfqt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fktsv.cn/Article/details/gtvmnifoz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.sjlbkw.cn/Article/details/glppdmtft.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fktsv.cn/Article/details/ghavxggpb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.bbcook.cn/Article/details/gkvtcople.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gpqgjipeh.sHtML

G. 面向对象
来源：http://wap.yfazqb.com/Article/details/gbvbivvjs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/goudyvtfy.sHtML

[G01] 定义类
来源：http://blog.yfazqb.com/Article/details/gkdeertzs.sHtML

Py:   class User: pass
来源：http://www.blog.bbcook.cn/Article/details/gfpnrzrgq.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gwnmklhvi.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/gykvjiunn.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.yfazqb.com/Article/details/gxqclvvik.sHtML

Java: class User {}
来源：http://www.m.share.tarul.cn/Article/details/gvpvcqtow.sHtML

Go:   type User struct { Name string }
来源：http://www.share.bbcook.cn/Article/details/gngxkbwss.sHtML

Ruby: class User; end
来源：http://www.blog.epnwcf.com/Article/details/gspkkwkgx.sHtML

C#:   class User {}
来源：http://m.share.tarul.cn/Article/details/gtdxanige.sHtML

[G02] 构造函数
来源：http://www.m.share.tarul.cn/Article/details/gsxsbjsec.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.bbcook.cn/Article/details/gmreihuqt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.sjlbkw.cn/Article/details/gcwdwdrfr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/gunnqifer.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.tarul.cn/Article/details/gqpijarxv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gtqqzckvx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.epnwcf.com/Article/details/gnqvwnhqj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.bbcook.cn/Article/details/gallurekn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.sjlbkw.cn/Article/details/grihkrdmk.sHtML

[G03] 实例属性
来源：http://www.share.epnwcf.com/Article/details/ggxjmsiwp.sHtML

Py:   self.name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/ggvzwbesn.sHtML

PHP:  public string $name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gwaclldgw.sHtML

JS:   this.name = "x";
来源：http://www.blog.vehdjk.com/Article/details/glqcweeff.sHtML

TS:   name: string = "x";
来源：http://www.m.share.tarul.cn/Article/details/gsvorfhow.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/gxknczbnb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fktsv.cn/Article/details/gpmnjnlyj.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/geqvvghie.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/gefsvbupf.sHtML

[G04] 定义方法
来源：http://read.share.fktsv.cn/Article/details/gnypepfrx.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gwnzdglqc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/grpujbgwe.sHtML

JS:   greet() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gldnxmfgd.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gduihbcmb.sHtML

Java: String greet() { return name; }
来源：http://m.share.vehdjk.com/Article/details/glmrrxpox.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gdmhvpoec.sHtML

Ruby: def greet; @name; end
来源：http://baike.fktsv.cn/Article/details/ghrtepvkx.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.yfazqb.com/Article/details/ggnvrwgre.sHtML

[G05] 继承
来源：http://baike.epnwcf.com/Article/details/gnnxtlfta.sHtML

Py:   class Admin(User): pass
来源：http://www.share.sjlbkw.cn/Article/details/gffnfaryi.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gloagkopu.sHtML

JS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gtiwhmvam.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gvhnhntum.sHtML

Java: class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gunbqqyrm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.vehdjk.com/Article/details/gclmytikm.sHtML

Ruby: class Admin < User; end
来源：http://blog.epnwcf.com/Article/details/gymqztaxo.sHtML

C#:   class Admin : User {}
来源：http://mobile.yfazqb.com/Article/details/gykpdfskd.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/ggnvhqmyu.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.vehdjk.com/Article/details/ggkjwlkhd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gnwlslwlr.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gmsfmyelv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gdheujobt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gkxenigzb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.yfazqb.com/Article/details/ggeiuckmn.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/gbuldspyw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.yfazqb.com/Article/details/gzvsqnimn.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gmzmnccqd.sHtML

Py:   super().greet()
来源：http://www.m.share.fktsv.cn/Article/details/grglilkuf.sHtML

PHP:  parent::greet();
来源：http://mobile.bbcook.cn/Article/details/grhaywzrf.sHtML

JS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gdpzqdaep.sHtML

TS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gainexdgy.sHtML

Java: super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/ggdrjjswe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.tarul.cn/Article/details/gvqlnnrzr.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/gdnslbywl.sHtML

C#:   base.Greet();
来源：http://read.share.vehdjk.com/Article/details/gtjxxfqpu.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gcsjwubay.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.vehdjk.com/Article/details/gnuylvjmk.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/gykjbjfqe.sHtML

JS:   static f() {}
来源：http://3g.tarul.cn/Article/details/gkubizsqq.sHtML

TS:   static f(): void {}
来源：http://read.share.fktsv.cn/Article/details/gbkhooyvo.sHtML

Java: static void f() {}
来源：http://blog.sjlbkw.cn/Article/details/gkugcdknc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.yfazqb.com/Article/details/gbiljizve.sHtML

Ruby: def self.f; end
来源：http://wap.vehdjk.com/Article/details/gqjbnixrn.sHtML

C#:   public static void F() {}
来源：http://wap.yfazqb.com/Article/details/gyiftyher.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/gvuiefjwy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.epnwcf.com/Article/details/gabpsnmvj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.yfazqb.com/Article/details/gvseppdxp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.vehdjk.com/Article/details/gbunvwgsn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.bbcook.cn/Article/details/gsgalmcme.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gvxpmlujv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.vehdjk.com/Article/details/geeutdtcj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.tarul.cn/Article/details/giudvzpqu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/gxcnbvulz.sHtML

[G10] 访问控制
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhlwwpfu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.epnwcf.com/Article/details/gqwlzkpti.sHtML

PHP:  public / protected / private
来源：http://blog.epnwcf.com/Article/details/glylfenlj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/gkvopixkl.sHtML

TS:   public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gzgynpztt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gmhffhxsa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gqcszfmrb.sHtML

Ruby: public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gjqatrgzm.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/ghheyeoto.sHtML

[G11] getter / setter
来源：http://blog.vehdjk.com/Article/details/gubhslfhl.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/govddpyka.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gvprvzyxx.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gfamozvre.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.vehdjk.com/Article/details/ggnheuxhy.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/gbzlpbxgw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gcqhxyccb.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/gpeixonpz.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.sjlbkw.cn/Article/details/gqenyqejy.sHtML

[G12] 对象转字符串
来源：http://baike.yfazqb.com/Article/details/gvcapbhmn.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gzjxtxasp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gpyxijcmr.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gwebiuzfg.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gvxxqhgxa.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gpomuizap.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gzmkjqfou.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gfhqhsvbw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.vehdjk.com/Article/details/gixhnyfhc.sHtML

[G13] 判断对象类型
来源：http://read.share.vehdjk.com/Article/details/gludbzvzk.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.epnwcf.com/Article/details/gkuemhkyg.sHtML

PHP:  $u instanceof User
来源：http://baike.vehdjk.com/Article/details/gelehghif.sHtML

JS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gpymdoryh.sHtML

TS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gbgoqzqyv.sHtML

Java: u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gcywrdnhz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/gbqohqpaj.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.vehdjk.com/Article/details/guojeposu.sHtML

C#:   u is User
来源：http://3g.fktsv.cn/Article/details/gfpembuhy.sHtML

[G14] 数据类 / record
来源：http://read.share.tarul.cn/Article/details/gskqviwty.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.bbcook.cn/Article/details/grhzixtmq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gollhnlgt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.epnwcf.com/Article/details/gozfqwjkm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fktsv.cn/Article/details/gabceblgv.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.epnwcf.com/Article/details/gubnahoct.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fktsv.cn/Article/details/gjlamcivr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.tarul.cn/Article/details/gldqyxvlm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.bbcook.cn/Article/details/growtfiir.sHtML

[G15] 枚举
来源：http://mobile.bbcook.cn/Article/details/gnvznvaep.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fktsv.cn/Article/details/gtsogswch.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.tarul.cn/Article/details/gdnxzbarl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/geqsowwhu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gfmhysqoo.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.bbcook.cn/Article/details/gqpovzleo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/ggrkkexsh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.epnwcf.com/Article/details/gxunuunti.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fktsv.cn/Article/details/gqqlarlvd.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.bbcook.cn/Article/details/golcgosjw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.tarul.cn/Article/details/gbhgzzsjr.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.bbcook.cn/Article/details/giatypjgn.sHtML

JS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gjxuwsisc.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gylvmglaj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.vehdjk.com/Article/details/gjuogocym.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.bbcook.cn/Article/details/gexcohugv.sHtML

Ruby: obj.instance_variables
来源：http://wap.tarul.cn/Article/details/ggqggmwux.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gbuqupudc.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gyzjzosiv.sHtML

H. 异常与错误处理
来源：http://baike.vehdjk.com/Article/details/gyupzzbdk.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/glijdwhgx.sHtML

[H01] try / catch 基础
来源：http://3g.fktsv.cn/Article/details/gfdoviycu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/gjtcidbgd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/gpicqxfaa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gaxaebxgn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gwyskidpm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.yfazqb.com/Article/details/gsimhhcdt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.tarul.cn/Article/details/gzbwevftd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.sjlbkw.cn/Article/details/gzskxduol.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.epnwcf.com/Article/details/gdletuafk.sHtML

[H02] finally / ensure 收尾
来源：http://3g.sjlbkw.cn/Article/details/gysdnentp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.sjlbkw.cn/Article/details/gfmsjsxeb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/ghuhowiol.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gsfkrjflw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gqzxaceos.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gyluurool.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fktsv.cn/Article/details/gtfcdfuug.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.tarul.cn/Article/details/gvmhdotjy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gounyclgt.sHtML


<!-- 参考信息 -->