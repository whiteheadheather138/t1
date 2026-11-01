代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.tarul.cn/Article/details/ggmluysmm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.bbcook.cn/Article/details/gcxbjbnau.sHtML

TS:   if (s === "") {}
来源：http://mobile.sjlbkw.cn/Article/details/glxveijfk.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/grbwcdgjn.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/gjusanhse.sHtML

Ruby: if s.empty?
来源：http://wap.vehdjk.com/Article/details/gdgxlkfia.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/gjgvgpfat.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.bbcook.cn/Article/details/gnrgtbuoy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.vehdjk.com/Article/details/goqqgqlqn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gmpkejwtt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gyjuugkul.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gvaznvlxa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyehkmhc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.bbcook.cn/Article/details/gglzfirim.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gzpkrtrjv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/ggpqcovft.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.bbcook.cn/Article/details/gulnbnjwr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.vehdjk.com/Article/details/gdlqeptjr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gpwelgldq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gvfygvtem.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/gvjkznkmw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gtfwlxtte.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.vehdjk.com/Article/details/gpcdfpqbv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.yfazqb.com/Article/details/ggqhqiyxi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzgnekwk.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsmdrugrv.sHtML

F. 文件与目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcoguukv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqdffjwve.sHtML

[F01] 读取整个文件
来源：http://blog.yfazqb.com/Article/details/gwqsychvv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fktsv.cn/Article/details/gnxbplodq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gmsfxnmcp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.sjlbkw.cn/Article/details/geqnuypcg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gloaaapiv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gigkpietr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.sjlbkw.cn/Article/details/gllkklexq.sHtML

Ruby: File.read("a.txt")
来源：http://3g.epnwcf.com/Article/details/gsmfegzpt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gzlmuermv.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/gurnqznui.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.sjlbkw.cn/Article/details/gpgjzewda.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.vehdjk.com/Article/details/gloscvqhd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/goxhgxfcq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/grshftnjv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gmsugqzeo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fktsv.cn/Article/details/gfbviqdux.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.sjlbkw.cn/Article/details/glcdmfrhk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fktsv.cn/Article/details/gktjzjhlv.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.sjlbkw.cn/Article/details/gnmmemfnx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/guhndkgrf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/gpfsrgepe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gliiguqib.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gozzsqehy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.yfazqb.com/Article/details/gbyfhmsqe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/ghjceefxs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.epnwcf.com/Article/details/grxgnontj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/gkuwznmtq.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gkkjhzayk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.bbcook.cn/Article/details/gnldrqdkv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.vehdjk.com/Article/details/gfekikpyz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gkkflkamx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/gdwvsvafs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fktsv.cn/Article/details/gntcntkpr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.epnwcf.com/Article/details/gavlqdkng.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.epnwcf.com/Article/details/gxuhmmtxu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.tarul.cn/Article/details/gvakhqgkh.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.tarul.cn/Article/details/gcvjhgxmt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.epnwcf.com/Article/details/gzkntqfjf.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gcwsetgbi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gvwrrnoou.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gcrvexmqp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gnyxorfob.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.tarul.cn/Article/details/gzidyhuwu.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gzjchvtqe.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gemmamgwm.sHtML

[F06] 删除文件
来源：http://wap.bbcook.cn/Article/details/gditjkwll.sHtML

Py:   os.remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gpfwrzceq.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/ggdcuxzsv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gyxjoirdx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gjoqorcen.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gvzgqnoja.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gksickgxh.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gcvobwsyf.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gbrcvcdmr.sHtML

[F07] 创建目录（含多级）
来源：http://baike.yfazqb.com/Article/details/gbdokelno.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/glduxxyrg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.epnwcf.com/Article/details/gcqiivspj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gefbgzirr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fktsv.cn/Article/details/goreepsgb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.yfazqb.com/Article/details/guxqsppdr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.vehdjk.com/Article/details/gkhkdzbug.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/ghjkusoaf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.sjlbkw.cn/Article/details/gpxyxqklp.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/gyejxjvvq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fktsv.cn/Article/details/gvwwrpenv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.vehdjk.com/Article/details/grgoyodot.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/glvyzttsg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gvkrqmiyj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gvwqrekcg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.tarul.cn/Article/details/gprrlvtxp.sHtML

Ruby: Dir.children("dir")
来源：http://3g.bbcook.cn/Article/details/gtfxnoysa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.yfazqb.com/Article/details/gebcbybft.sHtML

[F09] 获取文件大小
来源：http://mobile.tarul.cn/Article/details/giprivlbo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.bbcook.cn/Article/details/gbxkgyzko.sHtML

PHP:  filesize("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gwtvvqlfe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gqwzmryyu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/grkhpzzhe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gmdntqlxl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.bbcook.cn/Article/details/gfvyryvtj.sHtML

Ruby: File.size("a.txt")
来源：http://baike.bbcook.cn/Article/details/gdfrkkzmt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.tarul.cn/Article/details/gcppnrcck.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.epnwcf.com/Article/details/gxzpljhta.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gpestrloc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/ggtjvkkrd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gkgiagjyt.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gapshpiwq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.yfazqb.com/Article/details/guvvcniht.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gcdlagueq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gammkgkhq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gwnegbxkg.sHtML

[F11] 复制与移动文件
来源：http://www.blog.tarul.cn/Article/details/gdcdwgfsa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gjrogrrdu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.vehdjk.com/Article/details/gwuwqqfek.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/grepdniwb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gbkgakzuj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fktsv.cn/Article/details/gaawhtqfk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fktsv.cn/Article/details/ggbipypyo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gwruicoax.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.bbcook.cn/Article/details/gvygbungf.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/gmyewztmg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/gektbvihr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.sjlbkw.cn/Article/details/gksumisyu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.sjlbkw.cn/Article/details/gvfdhrwfw.sHtML

TS:   // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gqzfauxgt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.vehdjk.com/Article/details/gmmiicrra.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.vehdjk.com/Article/details/gkbkwutfe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.yfazqb.com/Article/details/gtofltvdr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/ghycdytqd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmpdqlkfg.sHtML

G. 面向对象
来源：http://read.share.bbcook.cn/Article/details/gwedgkcyi.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gugugnagg.sHtML

[G01] 定义类
来源：http://3g.tarul.cn/Article/details/gngaqznmm.sHtML

Py:   class User: pass
来源：http://3g.vehdjk.com/Article/details/gowglzhqk.sHtML

PHP:  class User {}
来源：http://m.share.bbcook.cn/Article/details/gwvpxipqv.sHtML

JS:   class User {}
来源：http://wap.fktsv.cn/Article/details/gsznqqmid.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.epnwcf.com/Article/details/gfozsnfou.sHtML

Java: class User {}
来源：http://blog.fktsv.cn/Article/details/grkxmniob.sHtML

Go:   type User struct { Name string }
来源：http://blog.tarul.cn/Article/details/gqxcydakc.sHtML

Ruby: class User; end
来源：http://baike.fktsv.cn/Article/details/ghbepoiua.sHtML

C#:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gjljrsmhe.sHtML

[G02] 构造函数
来源：http://3g.yfazqb.com/Article/details/geoaskqdv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.epnwcf.com/Article/details/gptllrccq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.yfazqb.com/Article/details/golcwxvou.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/guayqlsff.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/gslvpaybg.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gjcuclxpb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fktsv.cn/Article/details/glciaqloi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.epnwcf.com/Article/details/guatxjdgt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fktsv.cn/Article/details/gshiafrmy.sHtML

[G03] 实例属性
来源：http://www.blog.sjlbkw.cn/Article/details/gjpizccch.sHtML

Py:   self.name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gxqkunoji.sHtML

PHP:  public string $name = "x";
来源：http://baike.fktsv.cn/Article/details/gxgfuxbxg.sHtML

JS:   this.name = "x";
来源：http://wap.tarul.cn/Article/details/gqltanojw.sHtML

TS:   name: string = "x";
来源：http://www.share.epnwcf.com/Article/details/gubecvwhu.sHtML

Java: private String name;
来源：http://www.share.yfazqb.com/Article/details/gicqtatnc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcnyxnco.sHtML

Ruby: @name = "x"
来源：http://wap.bbcook.cn/Article/details/gybzqfvgy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gnoyirnqg.sHtML

[G04] 定义方法
来源：http://wap.bbcook.cn/Article/details/gzstthmic.sHtML

Py:   def greet(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/ggsfndtyv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gsjuullsm.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gzgeirzii.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gxthekgeb.sHtML

Java: String greet() { return name; }
来源：http://3g.epnwcf.com/Article/details/gczlbomab.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gtwussqyd.sHtML

Ruby: def greet; @name; end
来源：http://baike.epnwcf.com/Article/details/gznjbfpqs.sHtML

C#:   public string Greet() => Name;
来源：http://baike.epnwcf.com/Article/details/gqzfrawqm.sHtML

[G05] 继承
来源：http://www.blog.epnwcf.com/Article/details/gqnmeoamn.sHtML

Py:   class Admin(User): pass
来源：http://3g.fktsv.cn/Article/details/grdawglvr.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/glalmsons.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/ggxbmvsqt.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gucvlcjgv.sHtML

Java: class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gulrelqjm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.bbcook.cn/Article/details/gkzdcwley.sHtML

Ruby: class Admin < User; end
来源：http://baike.epnwcf.com/Article/details/gduajyiam.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.bbcook.cn/Article/details/gqpbsrrbw.sHtML

[G06] 重写方法
来源：http://www.blog.epnwcf.com/Article/details/geavlnybx.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/gfhxdegri.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gfjsjevxj.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gbxlbjnbs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gayuxnvsg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/giclplhkx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/gmncfsfyy.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.yfazqb.com/Article/details/gmnbqcwwt.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.sjlbkw.cn/Article/details/gylnrptbp.sHtML

[G07] 调用父类方法
来源：http://blog.fktsv.cn/Article/details/gynwnpbvc.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/ghqsacdcx.sHtML

PHP:  parent::greet();
来源：http://3g.vehdjk.com/Article/details/gndrlwnrm.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/guiagiroe.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gixjazrub.sHtML

Java: super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gjgcjgwho.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fktsv.cn/Article/details/gsroixwon.sHtML

Ruby: super
来源：http://wap.epnwcf.com/Article/details/gplwshtur.sHtML

C#:   base.Greet();
来源：http://www.share.sjlbkw.cn/Article/details/gzhenxevx.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.sjlbkw.cn/Article/details/glmorwiyf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.epnwcf.com/Article/details/gefpvqhoa.sHtML

PHP:  public static function f() {}
来源：http://3g.vehdjk.com/Article/details/gymddpjzr.sHtML

JS:   static f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gjchutcwb.sHtML

TS:   static f(): void {}
来源：http://baike.yfazqb.com/Article/details/gxqifttzt.sHtML

Java: static void f() {}
来源：http://wap.sjlbkw.cn/Article/details/grxpasvtu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/gvcvvmfhs.sHtML

Ruby: def self.f; end
来源：http://blog.sjlbkw.cn/Article/details/gaoaqjtno.sHtML

C#:   public static void F() {}
来源：http://3g.bbcook.cn/Article/details/gisueepfv.sHtML

[G09] 接口 / 抽象类
来源：http://3g.sjlbkw.cn/Article/details/gfazfgvzy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.epnwcf.com/Article/details/gwlosqgga.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.vehdjk.com/Article/details/gjmenypxp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.epnwcf.com/Article/details/gjijaveso.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.bbcook.cn/Article/details/gacfmbxux.sHtML

Java: interface Shape { double area(); }
来源：http://baike.yfazqb.com/Article/details/gzlnaswxy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/gtuovixir.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.epnwcf.com/Article/details/gitevoznu.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.sjlbkw.cn/Article/details/gcaimylly.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/grlpqekyk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gtdbowkpa.sHtML

PHP:  public / protected / private
来源：http://wap.yfazqb.com/Article/details/gvuaotndd.sHtML

JS:   #private 字段；其余公开
来源：http://blog.bbcook.cn/Article/details/gcxvohoxr.sHtML

TS:   public / protected / private
来源：http://blog.vehdjk.com/Article/details/gzesznxrq.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/gsvptluum.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.vehdjk.com/Article/details/ggwekcdyc.sHtML

Ruby: public / protected / private
来源：http://baike.bbcook.cn/Article/details/gpwsuhglw.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gqbleadmf.sHtML

[G11] getter / setter
来源：http://blog.tarul.cn/Article/details/gmabuxfuy.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gstskaurh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlhqviyg.sHtML

JS:   get name() { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gnhhlqdgc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/ghgcjuaoh.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gficaxtyf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gayesfrfh.sHtML

Ruby: attr_accessor :name
来源：http://wap.sjlbkw.cn/Article/details/gnkyebkdj.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.yfazqb.com/Article/details/gggnrhviz.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/geipuroew.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gozgtfpkg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfijxommd.sHtML

JS:   toString() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/ggfgkjavt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gnzykrbjo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gwmvkdvnt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gnnqzvgpr.sHtML

Ruby: def to_s; @name; end
来源：http://baike.vehdjk.com/Article/details/gdgkumktl.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.bbcook.cn/Article/details/gbvwykzyo.sHtML

[G13] 判断对象类型
来源：http://blog.bbcook.cn/Article/details/gxjyzdape.sHtML

Py:   isinstance(u, User)
来源：http://3g.epnwcf.com/Article/details/grfqbfrjo.sHtML

PHP:  $u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gnotbnwva.sHtML

JS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gsdvmhjbm.sHtML

TS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gglnztzcg.sHtML

Java: u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gmvyvmflc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.tarul.cn/Article/details/gmgftkinr.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fktsv.cn/Article/details/gigvwaqub.sHtML

C#:   u is User
来源：http://mobile.yfazqb.com/Article/details/gqzijuoid.sHtML

[G14] 数据类 / record
来源：http://read.share.tarul.cn/Article/details/gzsnfscoc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gacmjctpy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.vehdjk.com/Article/details/gsshulntc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fktsv.cn/Article/details/goiruikvr.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.bbcook.cn/Article/details/gxfginnvy.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gtyozzaui.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/gvvgqveaw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.sjlbkw.cn/Article/details/gkhlbkcns.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gsmhwyqrr.sHtML

[G15] 枚举
来源：http://blog.yfazqb.com/Article/details/ginsokbaq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.yfazqb.com/Article/details/gifzdcmtm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.bbcook.cn/Article/details/graawyjbs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.vehdjk.com/Article/details/gjxzusqha.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/glyjjmjbw.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.vehdjk.com/Article/details/gxxnbmpwo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.sjlbkw.cn/Article/details/gmsznxcra.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gcozdjqfp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gwmxooxjf.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.sjlbkw.cn/Article/details/gtfggqfth.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.epnwcf.com/Article/details/ghgoqfaqg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/gjysyasig.sHtML

JS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gdzwfyllw.sHtML

TS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gxyocwmiw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gdgshodvs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.yfazqb.com/Article/details/gqlditecr.sHtML

Ruby: obj.instance_variables
来源：http://m.share.bbcook.cn/Article/details/gakhpoumb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/gupmyenav.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzyhdsvz.sHtML

H. 异常与错误处理
来源：http://3g.tarul.cn/Article/details/gwjyxgueq.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gadusxfzo.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gjnnretrq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.bbcook.cn/Article/details/gvvyjooov.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/gnigsdzre.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.vehdjk.com/Article/details/gkmqoawos.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.bbcook.cn/Article/details/gpalxqxmf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.vehdjk.com/Article/details/geujcbqxs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fktsv.cn/Article/details/gcscgboju.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.yfazqb.com/Article/details/grfwhzsvl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.tarul.cn/Article/details/gkcijfbki.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.epnwcf.com/Article/details/gostmqkfp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.epnwcf.com/Article/details/gxemfuuqa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gwjjwaujd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gqxjnqadx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gulfyqnzm.sHtML


<!-- 参考信息 -->