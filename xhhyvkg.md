代发 wailian999

Ruby: s.lines
来源：http://www.blog.yfazqb.com/Article/details/gphpderep.sHtML

C#:   s.Split('\n')
来源：http://blog.fktsv.cn/Article/details/gkbatuezu.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/gzbyrofxr.sHtML

Py:   if not s:
来源：http://www.share.tarul.cn/Article/details/gkbbgpzdx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fktsv.cn/Article/details/gkpjxneoy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.epnwcf.com/Article/details/glcowrhsv.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.epnwcf.com/Article/details/gqucwpodx.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.bbcook.cn/Article/details/ghfllhnnr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.bbcook.cn/Article/details/gankdggny.sHtML

Ruby: if s.empty?
来源：http://read.share.bbcook.cn/Article/details/gzudutwpg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.bbcook.cn/Article/details/gjblohaia.sHtML

[E21] 超长截断加省略号
来源：http://baike.yfazqb.com/Article/details/gvkrocwhb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.sjlbkw.cn/Article/details/gbyegqgxz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gegmwtxbt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gnugybpyn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/ghrktsirz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gtdpbzmgh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.yfazqb.com/Article/details/gujuewpjo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.tarul.cn/Article/details/galrfensu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gezxnlaog.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.bbcook.cn/Article/details/gdkopsxkg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.yfazqb.com/Article/details/glzrdhikn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gtdkiicxd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/gcdirpnmu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gaowxzicc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gwyhosgxt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fktsv.cn/Article/details/gflaogqao.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.epnwcf.com/Article/details/gbnicmjzz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/grajycyzk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjfbtibwf.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gdtzigflj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gksqmmrdk.sHtML

[F01] 读取整个文件
来源：http://baike.yfazqb.com/Article/details/gkcubpagp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.bbcook.cn/Article/details/ghjuotjon.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gmqmxoriw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.sjlbkw.cn/Article/details/ggjyuqhzk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fktsv.cn/Article/details/ggjqyuggk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gujjshhwf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.epnwcf.com/Article/details/gqzmescpm.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gidaawnck.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gmldgyzuu.sHtML

[F02] 逐行读取文件
来源：http://www.blog.yfazqb.com/Article/details/gvexacwrv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.tarul.cn/Article/details/gohkfdsvz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/gycdcswkm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gshrqkntk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/giwfxaicr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/ghdinnwdy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/gghnbwojt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.bbcook.cn/Article/details/ghgxccxto.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.bbcook.cn/Article/details/gfctyplhp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.sjlbkw.cn/Article/details/glhymixuu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.yfazqb.com/Article/details/gcgvdgcbf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gtqhrccoz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gsfjbkwni.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gqjdyhaps.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.sjlbkw.cn/Article/details/gcxjmkcao.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fktsv.cn/Article/details/gibvnqwlz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.epnwcf.com/Article/details/gpwxwiged.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/guzalzjxg.sHtML

[F04] 追加写入文件
来源：http://read.share.epnwcf.com/Article/details/gpymmqssf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.tarul.cn/Article/details/glindcshl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.bbcook.cn/Article/details/gbwfmanie.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/glqtlxuif.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gxbesmjmt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.vehdjk.com/Article/details/gtqwzhavm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.yfazqb.com/Article/details/gkdjaqtwm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.yfazqb.com/Article/details/gpouwxxkg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fktsv.cn/Article/details/gricpyvib.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fktsv.cn/Article/details/gtcepdblj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.vehdjk.com/Article/details/gwdgibkwg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/gkxkorxnm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gklqwsdut.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gjzirfgeu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gsimkhmpg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fktsv.cn/Article/details/gqjlsfzrh.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gmlsifodq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gruepmijf.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gkneydrzp.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gjuqorkxs.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fktsv.cn/Article/details/grcjqfqcz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gkwycumai.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/ghrgffkda.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gwtunsywi.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gvnoqluas.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.epnwcf.com/Article/details/ggfndygwj.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fktsv.cn/Article/details/gymxteusz.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.sjlbkw.cn/Article/details/gprqrhtqm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/gtpbtbddv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.epnwcf.com/Article/details/gfuhlmzml.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/genflupdi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gyywaojlq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.epnwcf.com/Article/details/gjkwkuicu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/ggteodpte.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.bbcook.cn/Article/details/gmvhksole.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.tarul.cn/Article/details/grryzgnic.sHtML

[F08] 遍历目录
来源：http://wap.vehdjk.com/Article/details/gfqdcmtlj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.vehdjk.com/Article/details/gfqyuhbyw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.bbcook.cn/Article/details/gywwmfblh.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gosyxdqpc.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.bbcook.cn/Article/details/gcfzlptue.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gyzvhaocx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fktsv.cn/Article/details/gpafkrmdd.sHtML

Ruby: Dir.children("dir")
来源：http://wap.sjlbkw.cn/Article/details/gcqsxphpy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.yfazqb.com/Article/details/glgzewqpq.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gfacabxji.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/gadllzefl.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fktsv.cn/Article/details/grjpgjptl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gznmkxzje.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gvjbevrwb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gphqgziyh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fktsv.cn/Article/details/gigxrpayi.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.tarul.cn/Article/details/gwwtfmzhd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.bbcook.cn/Article/details/gtflomfzo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.vehdjk.com/Article/details/grnaunnat.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gppjukzin.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gwondrvuj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gnfswbjee.sHtML

TS:   path.extname("a.txt")
来源：http://wap.bbcook.cn/Article/details/gvffogptf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.epnwcf.com/Article/details/galuneltz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gthaznyms.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/guheakqed.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gncpvmemi.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/gylpcrsfo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gbwjqapeo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.vehdjk.com/Article/details/glpbtozmd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gpzseemmt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gdephmakj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gapucjfae.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/groboilwp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gnzoacdij.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.bbcook.cn/Article/details/gszfxkdft.sHtML

[F12] CSV 读写
来源：http://m.share.yfazqb.com/Article/details/gbeiaxfvn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.tarul.cn/Article/details/gkzmitqan.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fktsv.cn/Article/details/gowbwetjy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fktsv.cn/Article/details/gkinmjqnq.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/gngtfiwlc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.vehdjk.com/Article/details/gxgzywmmg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.tarul.cn/Article/details/gzxhjqwvy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.tarul.cn/Article/details/gmwhxcbdi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/gbpavtcer.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gamlknnwd.sHtML

G. 面向对象
来源：http://blog.fktsv.cn/Article/details/grcvwxtzu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/girdtikxt.sHtML

[G01] 定义类
来源：http://baike.yfazqb.com/Article/details/gqusljkkq.sHtML

Py:   class User: pass
来源：http://blog.tarul.cn/Article/details/gbsctpsac.sHtML

PHP:  class User {}
来源：http://wap.bbcook.cn/Article/details/gukxjfiaq.sHtML

JS:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gufspwayj.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gaofijlrk.sHtML

Java: class User {}
来源：http://wap.fktsv.cn/Article/details/gcoawvpmp.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.yfazqb.com/Article/details/gtxzbftuk.sHtML

Ruby: class User; end
来源：http://www.blog.yfazqb.com/Article/details/gdmbyntsb.sHtML

C#:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gcklzyhhf.sHtML

[G02] 构造函数
来源：http://www.share.vehdjk.com/Article/details/gahwwwfpt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/glgwzomhm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.epnwcf.com/Article/details/gaaznjszj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/geyixqfsv.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.yfazqb.com/Article/details/gjvewdlyc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gkgzmoryu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gksivqlur.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.vehdjk.com/Article/details/godbrxyyz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/guujdwpie.sHtML

[G03] 实例属性
来源：http://www.share.tarul.cn/Article/details/ghdabipxa.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gqrageezw.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gesrtcmpl.sHtML

JS:   this.name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gydfmramv.sHtML

TS:   name: string = "x";
来源：http://www.m.share.bbcook.cn/Article/details/ghxjrzjlu.sHtML

Java: private String name;
来源：http://www.m.share.fktsv.cn/Article/details/gddyatxio.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.sjlbkw.cn/Article/details/gnguacykh.sHtML

Ruby: @name = "x"
来源：http://blog.bbcook.cn/Article/details/gzgqktfki.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.vehdjk.com/Article/details/grblqhnpa.sHtML

[G04] 定义方法
来源：http://blog.yfazqb.com/Article/details/gjnuykowc.sHtML

Py:   def greet(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gldtxpgto.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/gquobmghm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gmmvzoatt.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gmpoylfdt.sHtML

Java: String greet() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gtmjlcerw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gqimccmuz.sHtML

Ruby: def greet; @name; end
来源：http://3g.vehdjk.com/Article/details/gyxfpkcsu.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.epnwcf.com/Article/details/ggrsflpnu.sHtML

[G05] 继承
来源：http://www.share.fktsv.cn/Article/details/gutaccjvr.sHtML

Py:   class Admin(User): pass
来源：http://read.share.tarul.cn/Article/details/gnygsgskc.sHtML

PHP:  class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gqpjlpgom.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gpdtwjhos.sHtML

TS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gqagaxouz.sHtML

Java: class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/ggpnixxln.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fktsv.cn/Article/details/guaoavzaa.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fktsv.cn/Article/details/gvsdpvznf.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/gtgyttdkv.sHtML

[G06] 重写方法
来源：http://www.share.vehdjk.com/Article/details/ghjfpyrzd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.epnwcf.com/Article/details/gnloaxius.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gwcuuuonf.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gxjtwywxa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gthbboxxv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gfmfzfgfu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.epnwcf.com/Article/details/gbizvrkld.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fktsv.cn/Article/details/gmlevyiws.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.sjlbkw.cn/Article/details/gegcsykcj.sHtML

[G07] 调用父类方法
来源：http://www.blog.tarul.cn/Article/details/gphbsjcea.sHtML

Py:   super().greet()
来源：http://m.share.bbcook.cn/Article/details/grucqhrza.sHtML

PHP:  parent::greet();
来源：http://wap.bbcook.cn/Article/details/gymspbnve.sHtML

JS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gbamgxyeh.sHtML

TS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gbfnxnrcz.sHtML

Java: super.greet();
来源：http://m.share.bbcook.cn/Article/details/gfqswjhum.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.bbcook.cn/Article/details/gockcjlxe.sHtML

Ruby: super
来源：http://blog.yfazqb.com/Article/details/gwappaslh.sHtML

C#:   base.Greet();
来源：http://www.blog.epnwcf.com/Article/details/gtjtwfmiu.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.tarul.cn/Article/details/gluqmhidp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.tarul.cn/Article/details/guvzrbndx.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/gfyfbqnvk.sHtML

JS:   static f() {}
来源：http://baike.vehdjk.com/Article/details/gozjmilpd.sHtML

TS:   static f(): void {}
来源：http://baike.vehdjk.com/Article/details/gjuurdjvo.sHtML

Java: static void f() {}
来源：http://blog.yfazqb.com/Article/details/gllzsfwgg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/gbenqdifs.sHtML

Ruby: def self.f; end
来源：http://www.blog.epnwcf.com/Article/details/gdiqptuab.sHtML

C#:   public static void F() {}
来源：http://wap.vehdjk.com/Article/details/ggkxrvzdg.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.sjlbkw.cn/Article/details/gynaosmqm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.bbcook.cn/Article/details/gwlycpdgn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdurhqwtc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.vehdjk.com/Article/details/ghfqgxddj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdidudakz.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.yfazqb.com/Article/details/gokpmflri.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/gprxynisb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.tarul.cn/Article/details/gjocttery.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gklkeupch.sHtML

[G10] 访问控制
来源：http://www.m.share.vehdjk.com/Article/details/gqlodreyl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.tarul.cn/Article/details/gnhqedjdp.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/gwtxoyyzc.sHtML

JS:   #private 字段；其余公开
来源：http://blog.bbcook.cn/Article/details/gviehzxpa.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/ggqadjhwl.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.tarul.cn/Article/details/gubocalcz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/gayznfwwd.sHtML

Ruby: public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gveajfeqi.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fktsv.cn/Article/details/grckecstc.sHtML

[G11] getter / setter
来源：http://www.blog.epnwcf.com/Article/details/gklactibp.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.vehdjk.com/Article/details/gvgffxnji.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/guuptuvvt.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.epnwcf.com/Article/details/gnymjsecu.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gyfhgeubs.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gfdzcjdjv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gtivnfwla.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/guwynzipl.sHtML

C#:   public string Name { get; set; }
来源：http://blog.bbcook.cn/Article/details/gsxsmyvkq.sHtML

[G12] 对象转字符串
来源：http://read.share.fktsv.cn/Article/details/gaaovfnta.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gzwxpbvsp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gqiwcwvef.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/glplglhcc.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gsilirlst.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fktsv.cn/Article/details/gcyllnoau.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/ganwaxyxe.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fktsv.cn/Article/details/gnlwztujs.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gadudcylx.sHtML

[G13] 判断对象类型
来源：http://3g.yfazqb.com/Article/details/gnbiunwem.sHtML

Py:   isinstance(u, User)
来源：http://wap.bbcook.cn/Article/details/gimkkmuwo.sHtML

PHP:  $u instanceof User
来源：http://3g.fktsv.cn/Article/details/giirfnvpv.sHtML

JS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gtehpyxcc.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gnvunvats.sHtML

Java: u instanceof User
来源：http://baike.epnwcf.com/Article/details/gtftyxpcv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gssepfeii.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.tarul.cn/Article/details/gvsuzlbzw.sHtML

C#:   u is User
来源：http://mobile.tarul.cn/Article/details/gunqlzmsh.sHtML

[G14] 数据类 / record
来源：http://www.m.share.vehdjk.com/Article/details/gpbgabgmp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/gtsdkxoid.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.epnwcf.com/Article/details/gxspwwiur.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.bbcook.cn/Article/details/gacviepmp.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.vehdjk.com/Article/details/gflctlvig.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.bbcook.cn/Article/details/ggwxgdxol.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.vehdjk.com/Article/details/gbhosprgo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.yfazqb.com/Article/details/gneunbldy.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.tarul.cn/Article/details/gqcgqolrd.sHtML

[G15] 枚举
来源：http://www.m.share.bbcook.cn/Article/details/gicvowuom.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.vehdjk.com/Article/details/gsezmydub.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/geyuvpdsb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.vehdjk.com/Article/details/gusnhyjym.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/guxeejhrd.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.vehdjk.com/Article/details/gkoiivolt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/gkjqrjlsl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.bbcook.cn/Article/details/gdgpnexar.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gkzpmbtwn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.tarul.cn/Article/details/gqxmwcdmc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.sjlbkw.cn/Article/details/gfiuutyuk.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.vehdjk.com/Article/details/gmzlyigpd.sHtML

JS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/grllvrxnt.sHtML

TS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/goytxmyer.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fktsv.cn/Article/details/gmawifcip.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.tarul.cn/Article/details/geqpjycuh.sHtML

Ruby: obj.instance_variables
来源：http://www.share.sjlbkw.cn/Article/details/gvrflgaxw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gtfxcvoxs.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/giglegjup.sHtML

H. 异常与错误处理
来源：http://3g.sjlbkw.cn/Article/details/gzvaelcwj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkdtqdfvb.sHtML

[H01] try / catch 基础
来源：http://baike.tarul.cn/Article/details/gphrgyvik.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlvwaayr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/gvqhrftiv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gxptglusf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gnxssczye.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/gneujgzut.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.tarul.cn/Article/details/gbzsfcgkd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gplepggtz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.bbcook.cn/Article/details/gxznmvhhk.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/gxpecairw.sHtML


<!-- 参考信息 -->