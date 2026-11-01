代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fktsv.cn/Article/details/gklxqazwi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.epnwcf.com/Article/details/gfxiytcwu.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gleboahkm.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/grabietbv.sHtML

Go:   if s == "" {}
来源：http://wap.tarul.cn/Article/details/gxjiowkuy.sHtML

Ruby: if s.empty?
来源：http://3g.sjlbkw.cn/Article/details/gbgjszqgm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/ggclzwtps.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.bbcook.cn/Article/details/ghnwlscwf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.vehdjk.com/Article/details/gwlbfqwkq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gpyudkfdr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gqbwiwinz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gyaieibty.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/guzkmfubz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.bbcook.cn/Article/details/gvfumxdkv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gsavqpthz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gypmpzvig.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gyblvhggn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.yfazqb.com/Article/details/gwjtmspnb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/glwopvjli.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gtvbqyuva.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gjkhpxadz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gbtpqypuk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.yfazqb.com/Article/details/gftfbassr.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fktsv.cn/Article/details/gomnoccnl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.bbcook.cn/Article/details/gfbwijgjs.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gdoiqpobe.sHtML

F. 文件与目录
来源：http://m.share.vehdjk.com/Article/details/gluxhugxs.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gocnuzcpr.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/gxxvvtuao.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/gfzwdukpw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gnzwolovl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.epnwcf.com/Article/details/gfqonrvib.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/giuhdilqx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gsbvgcxsv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gtpuqakdy.sHtML

Ruby: File.read("a.txt")
来源：http://baike.epnwcf.com/Article/details/gyppevzmy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gzfhfgrpz.sHtML

[F02] 逐行读取文件
来源：http://m.share.sjlbkw.cn/Article/details/gueoyjlvi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/gvwvqsozq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.tarul.cn/Article/details/gdcrywdjl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gyylukwqo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gxiaojqjd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gdxsqhnkp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.vehdjk.com/Article/details/gkwkutatg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.epnwcf.com/Article/details/gszgwlgve.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/grlfjaxqo.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.yfazqb.com/Article/details/gjymjgphz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gbzvmgjfq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/guzbhgamf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/grynwzrqw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gcqwzpzxx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fktsv.cn/Article/details/ggdzaacvt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.yfazqb.com/Article/details/gfqhovsds.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gxjtcakty.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gkfcoxoqd.sHtML

[F04] 追加写入文件
来源：http://read.share.fktsv.cn/Article/details/gtgdgstcr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gmhdwjyyj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.vehdjk.com/Article/details/gevhunuou.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gurpyhwvl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gbsdxnzst.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/gkazhhsej.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gqzbqhyfx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.epnwcf.com/Article/details/gomwydpnb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.epnwcf.com/Article/details/gzcbwqosz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.tarul.cn/Article/details/gfegytiyl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.bbcook.cn/Article/details/gimymfvew.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gwybcyzfj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/godzikwmj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gzmyyvdpd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gyahacaks.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.vehdjk.com/Article/details/gkjvepemk.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.tarul.cn/Article/details/gewrmaulv.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gkaxagqel.sHtML

[F06] 删除文件
来源：http://blog.fktsv.cn/Article/details/gxqsjxzwa.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gjjzytokv.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gihsvkqwu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/givamboum.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gneppjugq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gpxwbqyor.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gqylkwjab.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.epnwcf.com/Article/details/gmihnvblj.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gambhdklm.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.bbcook.cn/Article/details/gbcjmpkaz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/gbysdbslk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fktsv.cn/Article/details/gjpyzsoje.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.epnwcf.com/Article/details/gnlrcoznx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gfdjoxstn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.sjlbkw.cn/Article/details/gboatagcm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.vehdjk.com/Article/details/gxrumllnl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.yfazqb.com/Article/details/gjbskgqau.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.epnwcf.com/Article/details/ghltdmrri.sHtML

[F08] 遍历目录
来源：http://www.blog.tarul.cn/Article/details/glfbsaajr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/gyqiakvkt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fktsv.cn/Article/details/gbdyqolfu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gtilfjrqn.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gffvluvpt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gcdudiosu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.bbcook.cn/Article/details/gtyrdhnyk.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gljmoldpp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gidlcaxxt.sHtML

[F09] 获取文件大小
来源：http://read.share.yfazqb.com/Article/details/gaatdufwo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/giejlqyju.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gnoumwpgp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gkyaeytvg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/ggzysvnmt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gfnhkcwra.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.tarul.cn/Article/details/gqbiikzxl.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gbqnqfxcb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.tarul.cn/Article/details/gxcxfvcln.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.tarul.cn/Article/details/gogskzqvl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gmlugdlje.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gxfwbxvpt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ghdlgzpyd.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/gggybrbbp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fktsv.cn/Article/details/gikhczpef.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/goldssbbm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/glwnrwhof.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gtyweexkw.sHtML

[F11] 复制与移动文件
来源：http://baike.fktsv.cn/Article/details/gixvhlwzq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gpeatpetu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.yfazqb.com/Article/details/gwvtbxgtx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/ghntbmbbd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gkuokbmhw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gzuyedgfj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.sjlbkw.cn/Article/details/gtjfnpvij.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gpevflfcs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.tarul.cn/Article/details/gyjsemjre.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/gcxnocses.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.sjlbkw.cn/Article/details/gvqvchpxv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.bbcook.cn/Article/details/ghgwrhvct.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/gtumjdhde.sHtML

TS:   // 同上
来源：http://blog.tarul.cn/Article/details/gxntogmjt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.epnwcf.com/Article/details/gnxgawkqh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.yfazqb.com/Article/details/ghhboekzq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fktsv.cn/Article/details/giwytckuw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjazwgns.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gznqxvyii.sHtML

G. 面向对象
来源：http://www.m.share.tarul.cn/Article/details/gtgaxuwnw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gtkivfbxg.sHtML

[G01] 定义类
来源：http://www.share.epnwcf.com/Article/details/gzjuugtuv.sHtML

Py:   class User: pass
来源：http://baike.vehdjk.com/Article/details/gzzjscnhg.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gjmtyfjpj.sHtML

JS:   class User {}
来源：http://3g.epnwcf.com/Article/details/ghtvaqwdl.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.epnwcf.com/Article/details/gjglttyys.sHtML

Java: class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gozhdcdjq.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/gfbkukzft.sHtML

Ruby: class User; end
来源：http://m.share.sjlbkw.cn/Article/details/gmjepvnkp.sHtML

C#:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gjnyiwrwo.sHtML

[G02] 构造函数
来源：http://m.share.vehdjk.com/Article/details/ghqzipwce.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.bbcook.cn/Article/details/gbazuwrpr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/gtcyovbcd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gjikrnfmi.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gmvizuanx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gvxgfnjph.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.sjlbkw.cn/Article/details/glxbnfipt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fktsv.cn/Article/details/gfozprdpx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fktsv.cn/Article/details/gybtgydvp.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/gnylygxcd.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/gzfhlnnjy.sHtML

PHP:  public string $name = "x";
来源：http://blog.epnwcf.com/Article/details/giwlvztgj.sHtML

JS:   this.name = "x";
来源：http://3g.yfazqb.com/Article/details/guarvhbxt.sHtML

TS:   name: string = "x";
来源：http://blog.sjlbkw.cn/Article/details/ggnxiampl.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/gurnxdevd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.yfazqb.com/Article/details/gabywxbvm.sHtML

Ruby: @name = "x"
来源：http://read.share.tarul.cn/Article/details/gebymqxgs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.epnwcf.com/Article/details/gvywhfwut.sHtML

[G04] 定义方法
来源：http://baike.tarul.cn/Article/details/gvavaufmi.sHtML

Py:   def greet(self): return self.name
来源：http://baike.tarul.cn/Article/details/gvuldwltq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gbfwidajl.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gejhwfnfp.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gthhjknwp.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/glonsnffm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gsggnntfm.sHtML

Ruby: def greet; @name; end
来源：http://read.share.bbcook.cn/Article/details/grnwcllka.sHtML

C#:   public string Greet() => Name;
来源：http://baike.tarul.cn/Article/details/gboahangm.sHtML

[G05] 继承
来源：http://baike.vehdjk.com/Article/details/gsfoummlh.sHtML

Py:   class Admin(User): pass
来源：http://blog.bbcook.cn/Article/details/gfhcrmypb.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/ghimgyukf.sHtML

JS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gohuyjzxr.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gqazijjcw.sHtML

Java: class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gcoihwtdu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fktsv.cn/Article/details/gcbgvqrgz.sHtML

Ruby: class Admin < User; end
来源：http://wap.epnwcf.com/Article/details/gjwqeirit.sHtML

C#:   class Admin : User {}
来源：http://m.share.yfazqb.com/Article/details/gutdmvfwi.sHtML

[G06] 重写方法
来源：http://baike.vehdjk.com/Article/details/gvowpwobs.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.yfazqb.com/Article/details/gazppcioh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gshymghzq.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gwcfnzttx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/girarxigp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gnorkswve.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.tarul.cn/Article/details/gqzosnugt.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.sjlbkw.cn/Article/details/gffghxovu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.epnwcf.com/Article/details/ggmojzqap.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/gmtkeiybm.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/gqapjnwvm.sHtML

PHP:  parent::greet();
来源：http://read.share.vehdjk.com/Article/details/gzvaechle.sHtML

JS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gmhsvjuii.sHtML

TS:   super.greet();
来源：http://wap.tarul.cn/Article/details/glimdvmyq.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gguumtxdb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.vehdjk.com/Article/details/gmhowgyol.sHtML

Ruby: super
来源：http://www.m.share.fktsv.cn/Article/details/gwmhwfwyx.sHtML

C#:   base.Greet();
来源：http://m.share.fktsv.cn/Article/details/gjylqislq.sHtML

[G08] 静态方法与属性
来源：http://www.blog.epnwcf.com/Article/details/gykacivfb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/gnfkcqtty.sHtML

PHP:  public static function f() {}
来源：http://blog.sjlbkw.cn/Article/details/gcgfxpzts.sHtML

JS:   static f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gqyiqjbxj.sHtML

TS:   static f(): void {}
来源：http://wap.bbcook.cn/Article/details/gztremnqx.sHtML

Java: static void f() {}
来源：http://www.share.epnwcf.com/Article/details/gigufybde.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.vehdjk.com/Article/details/gxtvunjjf.sHtML

Ruby: def self.f; end
来源：http://baike.sjlbkw.cn/Article/details/gzzugcyhr.sHtML

C#:   public static void F() {}
来源：http://read.share.yfazqb.com/Article/details/giojiaesh.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fktsv.cn/Article/details/gsmeahdes.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.sjlbkw.cn/Article/details/gcklvmhih.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gnsbbczlg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.tarul.cn/Article/details/ggaobnamq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.vehdjk.com/Article/details/gqfadknhj.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.tarul.cn/Article/details/gyzxazufk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.epnwcf.com/Article/details/gtrmsaoar.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/garfokusw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gacdmjqpu.sHtML

[G10] 访问控制
来源：http://m.share.yfazqb.com/Article/details/gabfgxzmx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/gbqotcevq.sHtML

PHP:  public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gxcetbxls.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.epnwcf.com/Article/details/gcoldylvb.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gsdaqnkrk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.sjlbkw.cn/Article/details/gulhypsic.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.yfazqb.com/Article/details/gccbrited.sHtML

Ruby: public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gulsqpwkf.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/gesskhvcx.sHtML

[G11] getter / setter
来源：http://blog.fktsv.cn/Article/details/gsukyzoxx.sHtML

Py:   @property 与 @x.setter
来源：http://3g.yfazqb.com/Article/details/gyqkavgrc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gemgikpca.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/geuslpirz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.tarul.cn/Article/details/gauecjrii.sHtML

Java: public String getName() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gyrrtgwxo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gzsqaykts.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/gyoitfkzn.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.bbcook.cn/Article/details/gjdkgzqeu.sHtML

[G12] 对象转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gynrrvhcv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gydpbnacu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gjzqkrlrc.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gelxpbzah.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gmclxbpzg.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.epnwcf.com/Article/details/ggpvmfgvm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gyhhcaqos.sHtML

Ruby: def to_s; @name; end
来源：http://blog.tarul.cn/Article/details/gwbddzhky.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.vehdjk.com/Article/details/gkqxanumu.sHtML

[G13] 判断对象类型
来源：http://wap.tarul.cn/Article/details/givpoelke.sHtML

Py:   isinstance(u, User)
来源：http://wap.tarul.cn/Article/details/gmcremuvo.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gxfwlfvtj.sHtML

JS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gadtclrrt.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gnmnjtong.sHtML

Java: u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gkiwijzlx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.sjlbkw.cn/Article/details/gdihankdn.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/ginjdpqmt.sHtML

C#:   u is User
来源：http://www.m.share.fktsv.cn/Article/details/gmtysqzrb.sHtML

[G14] 数据类 / record
来源：http://wap.vehdjk.com/Article/details/gatexatjg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.epnwcf.com/Article/details/gronkamyh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/glmnfiagq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/gdyalwyqk.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/ghxfeelyu.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.epnwcf.com/Article/details/gelqwoicd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.bbcook.cn/Article/details/gmubqvmyu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.yfazqb.com/Article/details/gwckpzoui.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gfyyrvtbk.sHtML

[G15] 枚举
来源：http://www.m.share.tarul.cn/Article/details/gupypceja.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.vehdjk.com/Article/details/guypveqxc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.tarul.cn/Article/details/gckbevoeb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.sjlbkw.cn/Article/details/gnaaiafud.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gzogkwygd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.vehdjk.com/Article/details/gworvvajh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.yfazqb.com/Article/details/gawhcrjhs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/gdisbzdjn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/giduyadom.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.tarul.cn/Article/details/gejgpugju.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/grakonfdm.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.tarul.cn/Article/details/gpojteujb.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gczlcqjbs.sHtML

TS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gscsynfbu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.bbcook.cn/Article/details/gizrvonrq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/gplzbwzhv.sHtML

Ruby: obj.instance_variables
来源：http://m.share.tarul.cn/Article/details/gfajzfqwv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/grwzappeb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsvyvezxg.sHtML

H. 异常与错误处理
来源：http://baike.fktsv.cn/Article/details/ghwuerjoy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gowfnenht.sHtML

[H01] try / catch 基础
来源：http://read.share.vehdjk.com/Article/details/gfzgjzsbr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.yfazqb.com/Article/details/gvbltmncp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fktsv.cn/Article/details/gutrqroyx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gjfylxsqm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gpbzeolqv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fktsv.cn/Article/details/grwalbomz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.yfazqb.com/Article/details/gzgjdmbdo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.bbcook.cn/Article/details/ghltrpfjl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.yfazqb.com/Article/details/gxzwjmdrh.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/gmzbcqoqd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.vehdjk.com/Article/details/grwuytbvr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gvnbbgaqv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gbjgpytkf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gfqbujwpx.sHtML


<!-- 参考信息 -->