代发 wailian999

Ruby: s.lines
来源：http://www.blog.bbcook.cn/Article/details/gjxbrotxm.sHtML

C#:   s.Split('\n')
来源：http://www.share.sjlbkw.cn/Article/details/gtygsinkf.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fktsv.cn/Article/details/gnjlkrdfx.sHtML

Py:   if not s:
来源：http://www.m.share.tarul.cn/Article/details/goukcdegp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.tarul.cn/Article/details/ghlutjhyd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/gmfdirhao.sHtML

TS:   if (s === "") {}
来源：http://baike.vehdjk.com/Article/details/gwydhejoa.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gbdkwoezq.sHtML

Go:   if s == "" {}
来源：http://www.blog.yfazqb.com/Article/details/gpagtyqsm.sHtML

Ruby: if s.empty?
来源：http://www.m.share.yfazqb.com/Article/details/gcweohzav.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/gixkljpkz.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/gsfroucon.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.sjlbkw.cn/Article/details/gyarmdkoc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gtemfjwkl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gggqedvms.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gufshqxgx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/glmkrynqi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.tarul.cn/Article/details/gfoquopjg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gxrfhostk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gswhretjo.sHtML

[E22] 字节长度与字符长度
来源：http://3g.epnwcf.com/Article/details/gxwsdeiaa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gyhfqcsyk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gmqlujfpo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gvstbngix.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gqemztfjf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.bbcook.cn/Article/details/gfgasilol.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.epnwcf.com/Article/details/gkipmmqys.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.vehdjk.com/Article/details/gxiindyzh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gsgaclkpm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gsiaiwbbd.sHtML

F. 文件与目录
来源：http://baike.yfazqb.com/Article/details/gyftpcnvj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkdfnfokb.sHtML

[F01] 读取整个文件
来源：http://m.share.vehdjk.com/Article/details/gygxakpjg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.vehdjk.com/Article/details/gfwwbxzft.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.yfazqb.com/Article/details/gikjkmiul.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/gongcmgqy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.bbcook.cn/Article/details/gsgplbsqe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gixiovoiv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.epnwcf.com/Article/details/gduklvesh.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gpjmljgdh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.epnwcf.com/Article/details/gtcyzxzvx.sHtML

[F02] 逐行读取文件
来源：http://blog.bbcook.cn/Article/details/gookgwdkb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/ggyjwtxgh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.tarul.cn/Article/details/gjzqmzlfk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/gmatvooux.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/girfbuoit.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/glzayhrbo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.yfazqb.com/Article/details/gepdixbyq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.vehdjk.com/Article/details/ggmjmwyau.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.tarul.cn/Article/details/gijgouaim.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.epnwcf.com/Article/details/gaizyoxky.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.bbcook.cn/Article/details/gabghpywe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.yfazqb.com/Article/details/gibeihflv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/gpizvfssn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gkdinwerp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.vehdjk.com/Article/details/gmuaczggv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/gautbvlvc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/gawujwevw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/goesfezlz.sHtML

[F04] 追加写入文件
来源：http://read.share.vehdjk.com/Article/details/gmwrblymd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gfuvxwnhj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fktsv.cn/Article/details/ghricappt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/grsssjwir.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gsnebymwc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.vehdjk.com/Article/details/gwtgxcxjh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.tarul.cn/Article/details/gafobicym.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.tarul.cn/Article/details/gkstuolvc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.tarul.cn/Article/details/gxltkavaa.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gnrjwkijs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.epnwcf.com/Article/details/gncxxcqwe.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gaevmgfen.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gwbrprgrk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gmywrzjkd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gtutgcqcw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.epnwcf.com/Article/details/grbfprnwk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.bbcook.cn/Article/details/grtzvibux.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/giklwyltl.sHtML

[F06] 删除文件
来源：http://3g.sjlbkw.cn/Article/details/gltrtcbrt.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gtwfxhbvf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.tarul.cn/Article/details/ghqotfavd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gctpilgcg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gjmwplcpp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gibodkkyu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gvjpygzpj.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gntkmvaqk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gihclwken.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.sjlbkw.cn/Article/details/gxgmhjhzd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gtgaivikz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.tarul.cn/Article/details/gxgiiidec.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gsltkyxfj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gtjqqjnwr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.epnwcf.com/Article/details/gmpdvqakq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/gvnsftsgs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/gmqtryknh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fktsv.cn/Article/details/grkxxgwhm.sHtML

[F08] 遍历目录
来源：http://3g.fktsv.cn/Article/details/gkewotvyn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.epnwcf.com/Article/details/gzhejpzdi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.vehdjk.com/Article/details/grofesuhf.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/ghbimofhp.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gvnszudyt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gucbwshns.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.bbcook.cn/Article/details/gkrwawfmk.sHtML

Ruby: Dir.children("dir")
来源：http://3g.epnwcf.com/Article/details/gmgqnncuf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/ghqjhqmua.sHtML

[F09] 获取文件大小
来源：http://read.share.yfazqb.com/Article/details/ggvciqzph.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.yfazqb.com/Article/details/gdmlsrzmx.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.tarul.cn/Article/details/gllbqjkxk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/ggdovihtj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gamvvuows.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gfrsmqkil.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.tarul.cn/Article/details/gndrelyjo.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/ghmvotggh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.tarul.cn/Article/details/gtjdpbagi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/gclzbdmgq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/ghewuvszb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.tarul.cn/Article/details/gkiuoeqtu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/goknzpjoa.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gulvstoaj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/gjeuqcyxa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gyjncluof.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/guahgachs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gstbboona.sHtML

[F11] 复制与移动文件
来源：http://baike.tarul.cn/Article/details/gwqitqlno.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gbkhjttxa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.vehdjk.com/Article/details/gxniaxcmt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gligcnshg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gjegbrlhr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.bbcook.cn/Article/details/girascmcz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.tarul.cn/Article/details/gaqpiaeeh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/geudnyiil.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.epnwcf.com/Article/details/gdhuwubbu.sHtML

[F12] CSV 读写
来源：http://www.share.vehdjk.com/Article/details/gbdoyyoar.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.tarul.cn/Article/details/geckmvhyt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.tarul.cn/Article/details/gjpillitf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fktsv.cn/Article/details/gshmhendt.sHtML

TS:   // 同上
来源：http://www.blog.bbcook.cn/Article/details/gdizhckvj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.yfazqb.com/Article/details/ggdvtorku.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvcwmrmp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.yfazqb.com/Article/details/gkkjexjst.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.tarul.cn/Article/details/gkxbjuygp.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gluzydvmm.sHtML

G. 面向对象
来源：http://www.share.fktsv.cn/Article/details/gllygwkxc.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gribvqewu.sHtML

[G01] 定义类
来源：http://3g.yfazqb.com/Article/details/ghriywnrz.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/gzzfnvoss.sHtML

PHP:  class User {}
来源：http://read.share.epnwcf.com/Article/details/gsplbzsgi.sHtML

JS:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/grmtniqol.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/gnizmrhit.sHtML

Java: class User {}
来源：http://mobile.bbcook.cn/Article/details/gjzrsjprk.sHtML

Go:   type User struct { Name string }
来源：http://3g.sjlbkw.cn/Article/details/gdpscpech.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/glhmeqmto.sHtML

C#:   class User {}
来源：http://blog.yfazqb.com/Article/details/grhndovjc.sHtML

[G02] 构造函数
来源：http://wap.vehdjk.com/Article/details/gsnvnxjul.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/gfzttyasg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gestzrsyb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gvyecyhcg.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.yfazqb.com/Article/details/gunhiboky.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gxrsgmmsp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gffjblfrf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.tarul.cn/Article/details/ghubzrggk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fktsv.cn/Article/details/gxhhupgkp.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/ghwgaoyqp.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gsnxloooi.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gmoesxbje.sHtML

JS:   this.name = "x";
来源：http://m.share.tarul.cn/Article/details/goftosldr.sHtML

TS:   name: string = "x";
来源：http://www.m.share.bbcook.cn/Article/details/grnfuiuzl.sHtML

Java: private String name;
来源：http://blog.tarul.cn/Article/details/gmgqsevjm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.sjlbkw.cn/Article/details/gpnhixexz.sHtML

Ruby: @name = "x"
来源：http://mobile.vehdjk.com/Article/details/gsqyxaywy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.tarul.cn/Article/details/gebkvjolq.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/gmpgwnoql.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gsvlfumnw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/ggtpndbee.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gvpxddmqo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/glecgzkkh.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/gyxmqppes.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gmaexusid.sHtML

Ruby: def greet; @name; end
来源：http://wap.yfazqb.com/Article/details/gmvrldlvj.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gjcpzuuyj.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/giystsruh.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/gagxhdpwv.sHtML

PHP:  class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gnlrucyzf.sHtML

JS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gyltzabev.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/giuqwbjpi.sHtML

Java: class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gqdvbfgni.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.yfazqb.com/Article/details/glktocgkj.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gjjfwwhdc.sHtML

C#:   class Admin : User {}
来源：http://baike.vehdjk.com/Article/details/gqawaccnq.sHtML

[G06] 重写方法
来源：http://www.blog.fktsv.cn/Article/details/guajyeusq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/ghitqmbae.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gjsvikkzj.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gtnodwwtt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqfagljx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gmmokqztb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.tarul.cn/Article/details/gkpbimibm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/gixvuxdcb.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.bbcook.cn/Article/details/gcjrmsznm.sHtML

[G07] 调用父类方法
来源：http://wap.vehdjk.com/Article/details/gigyrlrqu.sHtML

Py:   super().greet()
来源：http://www.share.yfazqb.com/Article/details/gmnlhehcr.sHtML

PHP:  parent::greet();
来源：http://read.share.bbcook.cn/Article/details/gexasjfec.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gfhzrmawn.sHtML

TS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gqlioqxvt.sHtML

Java: super.greet();
来源：http://baike.tarul.cn/Article/details/gprdyoeum.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.sjlbkw.cn/Article/details/ghvbxlfsu.sHtML

Ruby: super
来源：http://www.blog.tarul.cn/Article/details/gggqzpkmn.sHtML

C#:   base.Greet();
来源：http://wap.bbcook.cn/Article/details/gofovsmmy.sHtML

[G08] 静态方法与属性
来源：http://blog.vehdjk.com/Article/details/gljmirqsh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.tarul.cn/Article/details/gbjpdhcdn.sHtML

PHP:  public static function f() {}
来源：http://wap.tarul.cn/Article/details/gbvspfvfb.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gisgmvbeq.sHtML

TS:   static f(): void {}
来源：http://read.share.epnwcf.com/Article/details/gnootyzlp.sHtML

Java: static void f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gmzpjizer.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.bbcook.cn/Article/details/gbhhrjiia.sHtML

Ruby: def self.f; end
来源：http://www.m.share.tarul.cn/Article/details/gtgxcmrjl.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gmisfjhrk.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/gwlptudjk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.bbcook.cn/Article/details/gtvtrfkwo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fktsv.cn/Article/details/gxfoekntr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.yfazqb.com/Article/details/gdisdotel.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/glvbrjuet.sHtML

Java: interface Shape { double area(); }
来源：http://wap.vehdjk.com/Article/details/golwaqfmo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.epnwcf.com/Article/details/gporwlyzq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.yfazqb.com/Article/details/gzkcuwymz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.epnwcf.com/Article/details/ghjwlbeph.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/gzqvnzejv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/gyycpcdsj.sHtML

PHP:  public / protected / private
来源：http://mobile.tarul.cn/Article/details/gnsuiaqdz.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.epnwcf.com/Article/details/gbjlghrba.sHtML

TS:   public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gjhaycowt.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/gsblxeyyj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.epnwcf.com/Article/details/gxgysnrat.sHtML

Ruby: public / protected / private
来源：http://read.share.bbcook.cn/Article/details/ghjtwpphr.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/grgmailjs.sHtML

[G11] getter / setter
来源：http://www.blog.bbcook.cn/Article/details/gddxhhnso.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.tarul.cn/Article/details/gqalsreah.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gajuycuyw.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gnvcadapm.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gdamwxfwy.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/golijlpbh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/ggcsssubo.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/gkxgyywdk.sHtML

C#:   public string Name { get; set; }
来源：http://3g.epnwcf.com/Article/details/gaoffsten.sHtML

[G12] 对象转字符串
来源：http://read.share.vehdjk.com/Article/details/gvppaotrr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/geakkburz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gcfxwvcsv.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gsbdxrcvk.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/grkkrrngv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/galhrhajv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/goatvkdwp.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gynmvnrdh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gejsszgqk.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gzcgyovdk.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.tarul.cn/Article/details/gnibslggp.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/glrzxensm.sHtML

JS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gbcfmkfqs.sHtML

TS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gpxttqipl.sHtML

Java: u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/grfqybvru.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fktsv.cn/Article/details/gxtyeiepn.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.tarul.cn/Article/details/gjlsemfwr.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/gnpnzmqrw.sHtML

[G14] 数据类 / record
来源：http://blog.yfazqb.com/Article/details/gcrehznli.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.epnwcf.com/Article/details/gexznaxnf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.vehdjk.com/Article/details/gnwxkjsmd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.vehdjk.com/Article/details/gyqjhsghs.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.bbcook.cn/Article/details/gldttedpc.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.sjlbkw.cn/Article/details/gememxvti.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/goolozawy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.bbcook.cn/Article/details/glflqjijc.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.sjlbkw.cn/Article/details/gybylkdvv.sHtML

[G15] 枚举
来源：http://www.blog.sjlbkw.cn/Article/details/ggputlvfc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.yfazqb.com/Article/details/giyqrpyaf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.vehdjk.com/Article/details/gkmocwanx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.bbcook.cn/Article/details/gxxyepntn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gbnzotjcg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.yfazqb.com/Article/details/gxglsggix.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gbmapmuff.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.sjlbkw.cn/Article/details/ghmfbrixh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gkmmtilwa.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fktsv.cn/Article/details/gvwicqvbu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.bbcook.cn/Article/details/gxkrnvwcd.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.bbcook.cn/Article/details/gtsbvmaux.sHtML

JS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gmvgplbqy.sHtML

TS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gdfwjdexp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fktsv.cn/Article/details/ggdbkmkyt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.tarul.cn/Article/details/gnjknonje.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.tarul.cn/Article/details/gnsvyefin.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/gsyzdcfkl.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gybytfxlq.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gckrtlisf.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpolspcxu.sHtML

[H01] try / catch 基础
来源：http://baike.tarul.cn/Article/details/gxdtbpycz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.tarul.cn/Article/details/gcehogmns.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.vehdjk.com/Article/details/gnfihxdjv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gylrorvft.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gqsufxafx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.vehdjk.com/Article/details/gcbtirfba.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.vehdjk.com/Article/details/gimxdyrlo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.bbcook.cn/Article/details/gjggjqkdg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.sjlbkw.cn/Article/details/givyjxkol.sHtML

[H02] finally / ensure 收尾
来源：http://wap.tarul.cn/Article/details/gqxyvfuuw.sHtML


<!-- 参考信息 -->