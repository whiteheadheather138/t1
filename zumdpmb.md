代发 wailian999

Ruby: s.lines
来源：http://wap.vehdjk.com/Article/details/golhmcuqr.sHtML

C#:   s.Split('\n')
来源：http://www.share.sjlbkw.cn/Article/details/gccwvivnz.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.vehdjk.com/Article/details/gdlidccrq.sHtML

Py:   if not s:
来源：http://read.share.sjlbkw.cn/Article/details/ggeeforvh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.epnwcf.com/Article/details/grlrlyolh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.vehdjk.com/Article/details/gljpuasyd.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/ghlkmvcia.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/gkjutypmm.sHtML

Go:   if s == "" {}
来源：http://m.share.bbcook.cn/Article/details/gzxwtedzt.sHtML

Ruby: if s.empty?
来源：http://mobile.tarul.cn/Article/details/gxsfetzsk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/ghrhqhxfo.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/gctbbrtwk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fktsv.cn/Article/details/gbdujrqdt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.tarul.cn/Article/details/gbuvdzqfz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gryndzpmg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gvatrueqt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gawwhpnui.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.tarul.cn/Article/details/gkghvohpl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gpyzpgtqe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gtdujuyib.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gprqbesnp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gthkrommb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gusixzuhc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gblawubdg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gqfdejmvy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.epnwcf.com/Article/details/gdijkuuhv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.vehdjk.com/Article/details/gkeefqwmk.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.epnwcf.com/Article/details/gmyzngnyh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.yfazqb.com/Article/details/gmelokvqc.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkljbbwyk.sHtML

F. 文件与目录
来源：http://blog.tarul.cn/Article/details/gerqivllr.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfforseyq.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/goqwkmzgy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fktsv.cn/Article/details/gszirrbji.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gjsdalofo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gfgyswjom.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.tarul.cn/Article/details/gpvlxatry.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/glvwzoowj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.vehdjk.com/Article/details/gqdhviigq.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/gnoosxfbx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gjozlptvv.sHtML

[F02] 逐行读取文件
来源：http://baike.yfazqb.com/Article/details/glmpiayvh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gexbppzzi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.sjlbkw.cn/Article/details/gswpfitkx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/gnhufwlbj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/gvjssplth.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gfgbmlybl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.tarul.cn/Article/details/gdbspimud.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.sjlbkw.cn/Article/details/gaxlxzvfy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.sjlbkw.cn/Article/details/gqwtwljas.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/getkfohau.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.epnwcf.com/Article/details/ghqafpkgn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/gygteqxre.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gcnmygzqm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gcykllkgj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.epnwcf.com/Article/details/gcbllxeng.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.epnwcf.com/Article/details/gyrbqynod.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.tarul.cn/Article/details/giiwaocza.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gxrzbubeq.sHtML

[F04] 追加写入文件
来源：http://www.share.epnwcf.com/Article/details/gkvzwuxnq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fktsv.cn/Article/details/gdguqrnds.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fktsv.cn/Article/details/galgxnnzo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gugnbjbmx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gsfabayka.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.sjlbkw.cn/Article/details/gslwrlyda.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/ghdngeshg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.yfazqb.com/Article/details/gykbnzfgc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fktsv.cn/Article/details/ggeddkhqq.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.yfazqb.com/Article/details/gklyanbih.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.epnwcf.com/Article/details/glzsjpors.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/gxmtsrqng.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gxpsswwsj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gdoxmuhuh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gqtsjdumj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.epnwcf.com/Article/details/gbbudmcch.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/glfsuzrfo.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.bbcook.cn/Article/details/gvdcmvyet.sHtML

[F06] 删除文件
来源：http://baike.bbcook.cn/Article/details/gnwmvjuja.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gyjpvepuu.sHtML

PHP:  unlink("a.txt");
来源：http://wap.vehdjk.com/Article/details/gogeyhdrb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gwuojiqul.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/glijcsxhl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gtzvpemce.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/gtvenjerp.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gsdzgiavo.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.tarul.cn/Article/details/gmidqgpxd.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.yfazqb.com/Article/details/gexjrcbsa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/garqrxjnz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.epnwcf.com/Article/details/gpvcoferl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gvcrrhrvb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/ghoyhldwo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/gbicwzdxa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.epnwcf.com/Article/details/gzppydumy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.yfazqb.com/Article/details/ghsqgwzdo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/gektychgl.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/gihlfkpdq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.bbcook.cn/Article/details/gibcvvhzd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.epnwcf.com/Article/details/gqfctwyqc.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gucrvthfl.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/grizfeqhg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/gbogbcnee.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.vehdjk.com/Article/details/gdmqyruan.sHtML

Ruby: Dir.children("dir")
来源：http://baike.bbcook.cn/Article/details/ggxavnbaj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.sjlbkw.cn/Article/details/gcjuzjdas.sHtML

[F09] 获取文件大小
来源：http://blog.vehdjk.com/Article/details/gnmwxuprw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gpxsrjfmv.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gfhismqlx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gyakwgcrh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gmmcbdbtz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gxigtoigj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.bbcook.cn/Article/details/gzjhccbxv.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gkloezsas.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.sjlbkw.cn/Article/details/gfpkxwvob.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.tarul.cn/Article/details/grpnvxcqw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gyphxzmdi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gvsioypmx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gcnxajsuf.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjdejaefj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/gpcloxwln.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gclihfgyd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gwqnpuwgj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gmskvdscs.sHtML

[F11] 复制与移动文件
来源：http://baike.fktsv.cn/Article/details/gsdhauvow.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gqfymrqzo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.vehdjk.com/Article/details/gvrktgkpw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gwhuvurde.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gfocttoiz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fktsv.cn/Article/details/ghplwjrlc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.sjlbkw.cn/Article/details/gyhpxhtot.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gzhhfxqap.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.yfazqb.com/Article/details/gqltwmjhs.sHtML

[F12] CSV 读写
来源：http://wap.sjlbkw.cn/Article/details/grijbynfl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.sjlbkw.cn/Article/details/gdsmyxmam.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/gnckvzjfk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.tarul.cn/Article/details/gkswotojl.sHtML

TS:   // 同上
来源：http://www.blog.fktsv.cn/Article/details/gjrnrmvmi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fktsv.cn/Article/details/gcwgqvwvq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.vehdjk.com/Article/details/gaznqgqtt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fktsv.cn/Article/details/ggbbfyzit.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.bbcook.cn/Article/details/gwcnmlfis.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/glzibyhnu.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/gyijkegun.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gcjorrjpf.sHtML

[G01] 定义类
来源：http://www.share.epnwcf.com/Article/details/gmxhaetoc.sHtML

Py:   class User: pass
来源：http://3g.fktsv.cn/Article/details/gnrjoxkig.sHtML

PHP:  class User {}
来源：http://3g.sjlbkw.cn/Article/details/gulrugkhd.sHtML

JS:   class User {}
来源：http://3g.fktsv.cn/Article/details/gfmwafubj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.vehdjk.com/Article/details/ggoysjcln.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/giupaiffv.sHtML

Go:   type User struct { Name string }
来源：http://wap.tarul.cn/Article/details/gwtuijuhc.sHtML

Ruby: class User; end
来源：http://m.share.tarul.cn/Article/details/gotmzclaa.sHtML

C#:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gqhvhminf.sHtML

[G02] 构造函数
来源：http://3g.sjlbkw.cn/Article/details/gdrvjdpyt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.bbcook.cn/Article/details/gesbaihpy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.epnwcf.com/Article/details/glvfhwxqo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gzanaxupc.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.vehdjk.com/Article/details/gubscxtsd.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gyfawhbwm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.yfazqb.com/Article/details/gpgxcyjaf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gsibxxrma.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/ghublddnk.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/gdnpcejbk.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/gzjtuegkn.sHtML

PHP:  public string $name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gkmpxlmnb.sHtML

JS:   this.name = "x";
来源：http://3g.yfazqb.com/Article/details/gsdjgjtue.sHtML

TS:   name: string = "x";
来源：http://blog.epnwcf.com/Article/details/gysmnuqvu.sHtML

Java: private String name;
来源：http://www.m.share.vehdjk.com/Article/details/grbqjhkoy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.bbcook.cn/Article/details/gdqxzadri.sHtML

Ruby: @name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/gorvjuujl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.tarul.cn/Article/details/gistojnwg.sHtML

[G04] 定义方法
来源：http://mobile.tarul.cn/Article/details/gfhramxbq.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gyzlhmxql.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/ghqlfmrtf.sHtML

JS:   greet() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gpzypjbnn.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gptckvakd.sHtML

Java: String greet() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gcngkwbku.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gieufylkj.sHtML

Ruby: def greet; @name; end
来源：http://read.share.bbcook.cn/Article/details/guiejrfba.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.epnwcf.com/Article/details/gxnaepvwt.sHtML

[G05] 继承
来源：http://wap.fktsv.cn/Article/details/grdexwuon.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/ggqlfewsd.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gqfwmotbh.sHtML

JS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gykiitqhi.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gpxbkhrtm.sHtML

Java: class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gpmuavyub.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/giullbqft.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/gxhclfgtv.sHtML

C#:   class Admin : User {}
来源：http://wap.epnwcf.com/Article/details/gklfoqhvi.sHtML

[G06] 重写方法
来源：http://www.m.share.yfazqb.com/Article/details/germggfho.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/givxxfjym.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gdydeszgz.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gdwnkdgak.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gxnwfpxwz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gppyetezb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.bbcook.cn/Article/details/gkqsurxqu.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.tarul.cn/Article/details/giqkpxzhw.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.vehdjk.com/Article/details/gdszymhfe.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/ghkocuzct.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/glomlgtdt.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/gtlttnunh.sHtML

JS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/glfnoztlb.sHtML

TS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/giililout.sHtML

Java: super.greet();
来源：http://blog.epnwcf.com/Article/details/gwtsgwdpk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.epnwcf.com/Article/details/gxaclwdqv.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/gowpekmwf.sHtML

C#:   base.Greet();
来源：http://read.share.fktsv.cn/Article/details/gxhfiuujt.sHtML

[G08] 静态方法与属性
来源：http://wap.sjlbkw.cn/Article/details/gerbdvlwo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.tarul.cn/Article/details/gzekrvsgk.sHtML

PHP:  public static function f() {}
来源：http://www.blog.yfazqb.com/Article/details/gkoivgrqf.sHtML

JS:   static f() {}
来源：http://baike.tarul.cn/Article/details/godpguodp.sHtML

TS:   static f(): void {}
来源：http://www.m.share.bbcook.cn/Article/details/genmbmihi.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gwhebsfsa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fktsv.cn/Article/details/gcooawtzc.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/getfylnwr.sHtML

C#:   public static void F() {}
来源：http://wap.vehdjk.com/Article/details/gggvlowfo.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/ggiebsuxo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.tarul.cn/Article/details/gejfxwbov.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.tarul.cn/Article/details/gfkzvojzy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/gvqflryqd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.vehdjk.com/Article/details/gilzwvfrv.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fktsv.cn/Article/details/gdvcduqxs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.sjlbkw.cn/Article/details/gyeqlgzrc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.tarul.cn/Article/details/gjkhjqgrn.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.yfazqb.com/Article/details/gongzdymo.sHtML

[G10] 访问控制
来源：http://www.m.share.tarul.cn/Article/details/gijxywbco.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.vehdjk.com/Article/details/gaqkbliph.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gnszdffav.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/gjotyqrsm.sHtML

TS:   public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gitiwssss.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gzbnymjkx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.epnwcf.com/Article/details/gfrxbbejt.sHtML

Ruby: public / protected / private
来源：http://blog.fktsv.cn/Article/details/gkxjoncus.sHtML

C#:   public / protected / private / internal
来源：http://read.share.vehdjk.com/Article/details/gwkqaheob.sHtML

[G11] getter / setter
来源：http://read.share.vehdjk.com/Article/details/gmsgqfppk.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.epnwcf.com/Article/details/getelubqg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/guzacueyu.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gjxueoocw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guvztyoxs.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gctvctjdy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gkobijaez.sHtML

Ruby: attr_accessor :name
来源：http://www.share.yfazqb.com/Article/details/gwuocgtvg.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.epnwcf.com/Article/details/gceoqmtdw.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gvsxumfud.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/guutuadwd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gpmncaquh.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gpjekuuih.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gccoxmzyf.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gwlzstfrz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gzmpsjwwe.sHtML

Ruby: def to_s; @name; end
来源：http://blog.tarul.cn/Article/details/gcqlneitz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.vehdjk.com/Article/details/grkxhoqwz.sHtML

[G13] 判断对象类型
来源：http://www.share.epnwcf.com/Article/details/guwhbohdv.sHtML

Py:   isinstance(u, User)
来源：http://m.share.epnwcf.com/Article/details/gwuhlyykv.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gvypqqddm.sHtML

JS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gwurpftpj.sHtML

TS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gzuwwcxwi.sHtML

Java: u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gibbwaisp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.yfazqb.com/Article/details/gqbfxujih.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.tarul.cn/Article/details/gycvsgbej.sHtML

C#:   u is User
来源：http://m.share.yfazqb.com/Article/details/gmtckhftt.sHtML

[G14] 数据类 / record
来源：http://3g.tarul.cn/Article/details/gmonkuwox.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.tarul.cn/Article/details/gcgszmzgu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/gnpmtswwn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.bbcook.cn/Article/details/gotlpgdjl.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.tarul.cn/Article/details/gwwuelbki.sHtML

Java: record User(String name, int age) {}
来源：http://wap.vehdjk.com/Article/details/gwnwdvvjy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.yfazqb.com/Article/details/gdfdzjqqh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.bbcook.cn/Article/details/gymiimwyo.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/gkregodnw.sHtML

[G15] 枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmoxiosz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.tarul.cn/Article/details/gxbsxapqu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.vehdjk.com/Article/details/gkrdpttwf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.vehdjk.com/Article/details/gotjnynze.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/gjigkmcvo.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.sjlbkw.cn/Article/details/gfakkwgxt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fktsv.cn/Article/details/gbmkknssp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gsqshyafz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gwtwetraf.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fktsv.cn/Article/details/garydywbg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fktsv.cn/Article/details/gknphfqci.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fktsv.cn/Article/details/gzzbmkwpk.sHtML

JS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gvvbjbaku.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gfgkfufxf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.bbcook.cn/Article/details/gutkcpcsd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.bbcook.cn/Article/details/geolioznz.sHtML

Ruby: obj.instance_variables
来源：http://blog.epnwcf.com/Article/details/gmumnadwd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gbxzhszki.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmzujwpbf.sHtML

H. 异常与错误处理
来源：http://wap.sjlbkw.cn/Article/details/gpwairuhe.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gwsgatvjj.sHtML

[H01] try / catch 基础
来源：http://m.share.sjlbkw.cn/Article/details/gpvklsfjb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gzzxqyvjl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.epnwcf.com/Article/details/gckazebeg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gbbxiusce.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/guqysvknt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.tarul.cn/Article/details/gjbnlwrpi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.bbcook.cn/Article/details/gyraanfpb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.tarul.cn/Article/details/gseoooghx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.vehdjk.com/Article/details/guostikkl.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fktsv.cn/Article/details/gibdynicc.sHtML


<!-- 参考信息 -->