代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.tarul.cn/Article/details/gehlmzzjo.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.epnwcf.com/Article/details/gmidumuws.sHtML

Py:   s.splitlines()
来源：http://mobile.fktsv.cn/Article/details/gaabjurlb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gldiwvbhf.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/gdyeagail.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gjxryfuav.sHtML

Java: s.lines().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gtnyhengu.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.vehdjk.com/Article/details/gjaeiemor.sHtML

Ruby: s.lines
来源：http://www.blog.fktsv.cn/Article/details/gocpuqcvx.sHtML

C#:   s.Split('\n')
来源：http://www.blog.epnwcf.com/Article/details/gwukzpbdh.sHtML

[E20] 判断字符串是否为空
来源：http://3g.yfazqb.com/Article/details/gfufepqpp.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/gwcequjip.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gebpfohyq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.vehdjk.com/Article/details/gpoxbtlye.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/gvwguhtnx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gnayokqgb.sHtML

Go:   if s == "" {}
来源：http://www.blog.epnwcf.com/Article/details/gylaybloo.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/ggrogoxcq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fktsv.cn/Article/details/gvuwwufoc.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.epnwcf.com/Article/details/gzkalrfog.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.tarul.cn/Article/details/ghtvkmnmu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gdtuwfaoj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gmslxtzkc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gscqmcuas.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gsymrubaz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.bbcook.cn/Article/details/gdbbhweyx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gdormmivx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gacuzxbnp.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.bbcook.cn/Article/details/gnttdyjya.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.yfazqb.com/Article/details/gxkjqyjkm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/ghehysjnm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gcluwwhpk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gviqqtubp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.vehdjk.com/Article/details/gpstuwnnj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/gupqvexcc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.tarul.cn/Article/details/gtockkcap.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.vehdjk.com/Article/details/gijjpjvak.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gspvpgguh.sHtML

F. 文件与目录
来源：http://m.share.epnwcf.com/Article/details/gobyrfjld.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glapfbewm.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/gtthfvjzx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.bbcook.cn/Article/details/gspdhoqqr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/giccrjyop.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.bbcook.cn/Article/details/gfmyosqoy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.vehdjk.com/Article/details/gudbslmis.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gjwdcwsmg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/gspvtptaq.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gbigacfcs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/gqjzqpwle.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.bbcook.cn/Article/details/gpkyooqmh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.tarul.cn/Article/details/gyrvbsawk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.vehdjk.com/Article/details/grdrqksqk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/gaayapvyw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/ggnrzwuqr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gbfrfpqmr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/gpelwygxp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fktsv.cn/Article/details/ghmszetcr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.tarul.cn/Article/details/gzykmevfk.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.epnwcf.com/Article/details/gvtxlkjgn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.bbcook.cn/Article/details/gijkpylqt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gecbkrbym.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/gvuobgmri.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/gbwawtlzu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.bbcook.cn/Article/details/gwgxlihzv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fktsv.cn/Article/details/gwmtobiyf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.vehdjk.com/Article/details/gsdjpgxoy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/glhpaefdc.sHtML

[F04] 追加写入文件
来源：http://www.share.vehdjk.com/Article/details/gmletepgn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.vehdjk.com/Article/details/glciwvgjw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.epnwcf.com/Article/details/gwjdxewmi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fktsv.cn/Article/details/gskvogyfx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gofvasllb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/gtdvkajbh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gkbxdfjkz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fktsv.cn/Article/details/gexyjraht.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.yfazqb.com/Article/details/glmtkrjkq.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.yfazqb.com/Article/details/guvdbszrl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.bbcook.cn/Article/details/gfnygqcqr.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.tarul.cn/Article/details/gxdzmouef.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/guskwosis.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gytbsvufr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gwlbglovb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.tarul.cn/Article/details/gwgqoffvr.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.tarul.cn/Article/details/gzhbankkz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gethyxcxz.sHtML

[F06] 删除文件
来源：http://blog.bbcook.cn/Article/details/grwzdmsun.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gflobkmoc.sHtML

PHP:  unlink("a.txt");
来源：http://3g.tarul.cn/Article/details/gonxnxfmp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gifgachew.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gpkgailmm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gcbiopcxl.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/gptjajnst.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/gkdsplspe.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.epnwcf.com/Article/details/gplejlldr.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.yfazqb.com/Article/details/gzyeafqse.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/glhvhvkwz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fktsv.cn/Article/details/gfsigigou.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gzndjplps.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/grrgxinqs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/ggjtpnvsj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.epnwcf.com/Article/details/gmeztvdul.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.epnwcf.com/Article/details/gefzpbasc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/gnljjjoxn.sHtML

[F08] 遍历目录
来源：http://3g.sjlbkw.cn/Article/details/gnoskdlnm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.tarul.cn/Article/details/gsqepvqjr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/gbmwxwzmc.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gcvmoddsm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gbaizulqw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gmxzxncgo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.sjlbkw.cn/Article/details/gzcoilssi.sHtML

Ruby: Dir.children("dir")
来源：http://baike.yfazqb.com/Article/details/gnhhrgalq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/ggfohbpjm.sHtML

[F09] 获取文件大小
来源：http://3g.yfazqb.com/Article/details/gfzhybice.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.vehdjk.com/Article/details/gjrzfxjsh.sHtML

PHP:  filesize("a.txt");
来源：http://blog.yfazqb.com/Article/details/gqdxruxef.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gccnopdjh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gspddbyqf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gkuymdmnd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.epnwcf.com/Article/details/gjjmmmpjf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ghkhopwjk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.epnwcf.com/Article/details/gnlcddnut.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.vehdjk.com/Article/details/gtflwpllr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ghppyhyda.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.tarul.cn/Article/details/gsamsybld.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gzaxedxkz.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/graymrtpn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fktsv.cn/Article/details/gxlftxxjc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gykyzekae.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/ghlppevff.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gchxblypa.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/gkljojxeb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gnbvwysjp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gngcfyyox.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gomupjwqb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/guebjzuyv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.yfazqb.com/Article/details/gfqmogobo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/goskgqsnz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gfwcatdsh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.tarul.cn/Article/details/ggtkarjck.sHtML

[F12] CSV 读写
来源：http://3g.bbcook.cn/Article/details/gwnzmqqcb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.yfazqb.com/Article/details/ggsyviyxt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.tarul.cn/Article/details/gxnsgideq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.vehdjk.com/Article/details/gcuqmrgeh.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/gcpaoizsl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.vehdjk.com/Article/details/ghiefovec.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.bbcook.cn/Article/details/gdhswprsx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gtfxhipqy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.sjlbkw.cn/Article/details/gnpgrqalq.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gujbbwugo.sHtML

G. 面向对象
来源：http://www.m.share.bbcook.cn/Article/details/gjizmxsra.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/grnseftxv.sHtML

[G01] 定义类
来源：http://3g.yfazqb.com/Article/details/gnhlulmaw.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/gkqhifzua.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/gxfmdoioz.sHtML

JS:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gupazfbqe.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gbikjiqdc.sHtML

Java: class User {}
来源：http://wap.yfazqb.com/Article/details/gcwhwxexf.sHtML

Go:   type User struct { Name string }
来源：http://baike.vehdjk.com/Article/details/gjasiiisn.sHtML

Ruby: class User; end
来源：http://www.blog.tarul.cn/Article/details/gwmtesywl.sHtML

C#:   class User {}
来源：http://www.share.tarul.cn/Article/details/gogmscpuv.sHtML

[G02] 构造函数
来源：http://3g.fktsv.cn/Article/details/ghdkbcmlm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.yfazqb.com/Article/details/gjdxavtme.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/gxixdoyee.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/ghiyfsria.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.yfazqb.com/Article/details/gaidbmfzd.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gqpbymelz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fktsv.cn/Article/details/gzyzumvmr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.sjlbkw.cn/Article/details/gakfttmlp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.epnwcf.com/Article/details/ghditrvmr.sHtML

[G03] 实例属性
来源：http://mobile.bbcook.cn/Article/details/gixrlzbws.sHtML

Py:   self.name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gkstohmeo.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.tarul.cn/Article/details/gbvhqeuut.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gjmkiuslr.sHtML

TS:   name: string = "x";
来源：http://www.blog.yfazqb.com/Article/details/grrbqnoud.sHtML

Java: private String name;
来源：http://www.blog.vehdjk.com/Article/details/gqwmajtvw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.vehdjk.com/Article/details/gbrikycru.sHtML

Ruby: @name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gwveheibx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fktsv.cn/Article/details/gilgxsqpn.sHtML

[G04] 定义方法
来源：http://blog.vehdjk.com/Article/details/gbrojbyzo.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gloiffcya.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gaseesidj.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/ghrisnlvr.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gzitaxjzl.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gmclinvdu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gvtotzsuv.sHtML

Ruby: def greet; @name; end
来源：http://blog.fktsv.cn/Article/details/gksjcrwkn.sHtML

C#:   public string Greet() => Name;
来源：http://blog.epnwcf.com/Article/details/gdohmwswg.sHtML

[G05] 继承
来源：http://www.share.tarul.cn/Article/details/gppozxrbs.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.vehdjk.com/Article/details/gknevopad.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/guuvuwynj.sHtML

JS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gzhvjajrq.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gmlcgpwyw.sHtML

Java: class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gpeqoqxed.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.epnwcf.com/Article/details/gkkvazttc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gfrobmtrv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/gvzcynxlx.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gionfekgz.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.sjlbkw.cn/Article/details/grkhmyotu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gcmedmpjx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/ghqxgcdby.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gkjxjzndu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gxmfayxek.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/gbuizjtdk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.sjlbkw.cn/Article/details/gyuslyqhw.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gdpuohwzk.sHtML

[G07] 调用父类方法
来源：http://read.share.vehdjk.com/Article/details/gsdbfvotx.sHtML

Py:   super().greet()
来源：http://www.share.yfazqb.com/Article/details/gtnqjxozz.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gvfsllosx.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gqycgjntp.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gowmiipzr.sHtML

Java: super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gjcvydkoa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fktsv.cn/Article/details/gbzqxsomm.sHtML

Ruby: super
来源：http://blog.bbcook.cn/Article/details/gakbebkah.sHtML

C#:   base.Greet();
来源：http://3g.vehdjk.com/Article/details/gyhnqdspi.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/guviqfiuo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/gzmsyabfm.sHtML

PHP:  public static function f() {}
来源：http://www.share.bbcook.cn/Article/details/gwhxmfjww.sHtML

JS:   static f() {}
来源：http://3g.bbcook.cn/Article/details/gakolthkc.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/gsahgtikw.sHtML

Java: static void f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gsmyjxcou.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.vehdjk.com/Article/details/gsqktjnvi.sHtML

Ruby: def self.f; end
来源：http://wap.fktsv.cn/Article/details/giuedrbnh.sHtML

C#:   public static void F() {}
来源：http://m.share.tarul.cn/Article/details/gtgnicjnc.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fktsv.cn/Article/details/ghkriuabi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.tarul.cn/Article/details/gpdnhjnue.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.sjlbkw.cn/Article/details/gmsrmhpxo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.sjlbkw.cn/Article/details/guqhrqtnx.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.yfazqb.com/Article/details/gkjylpsxo.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gzsaohcrr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.yfazqb.com/Article/details/gfmzcumgu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.tarul.cn/Article/details/gjcdvwgxr.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.tarul.cn/Article/details/gpxiqpoeh.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/gxxslukge.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.bbcook.cn/Article/details/givrkobmp.sHtML

PHP:  public / protected / private
来源：http://m.share.yfazqb.com/Article/details/ghsylnyll.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/giqeastfk.sHtML

TS:   public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gsnbzettu.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.tarul.cn/Article/details/gbbddtvof.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.vehdjk.com/Article/details/gkaqcqqmx.sHtML

Ruby: public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gwupycnqa.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gtiodupab.sHtML

[G11] getter / setter
来源：http://read.share.tarul.cn/Article/details/giybpdzfc.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.yfazqb.com/Article/details/gmtkyfezj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gtmjmbqev.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/gtivnccgr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqogfkueo.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gtzqvvymq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gehujklpa.sHtML

Ruby: attr_accessor :name
来源：http://3g.bbcook.cn/Article/details/gkwpdnurl.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fktsv.cn/Article/details/ghjcnwnkm.sHtML

[G12] 对象转字符串
来源：http://m.share.fktsv.cn/Article/details/geqrqghoz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gphacfzdf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gtlafmvme.sHtML

JS:   toString() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gexifuhwh.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gbcsmgmel.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.epnwcf.com/Article/details/gellobyux.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gifxdfpqe.sHtML

Ruby: def to_s; @name; end
来源：http://3g.epnwcf.com/Article/details/glpztxhey.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fktsv.cn/Article/details/gzvdfuxnn.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/ggaskvpak.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fktsv.cn/Article/details/ghyxxirzb.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/gpvdtwwsi.sHtML

JS:   u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gmfdmrhog.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gawibuylo.sHtML

Java: u instanceof User
来源：http://3g.fktsv.cn/Article/details/gppkfwoks.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.vehdjk.com/Article/details/gmmtgukot.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.sjlbkw.cn/Article/details/grwabqsqe.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/gsrihlluw.sHtML

[G14] 数据类 / record
来源：http://mobile.epnwcf.com/Article/details/ggnzbcobn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/ggrufnfni.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fktsv.cn/Article/details/gzwihzbfw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.tarul.cn/Article/details/gfrvqbtfr.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/gusipfitn.sHtML

Java: record User(String name, int age) {}
来源：http://3g.yfazqb.com/Article/details/gjwpmoohd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.sjlbkw.cn/Article/details/gewgqlzns.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.yfazqb.com/Article/details/gvszxcgqp.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.epnwcf.com/Article/details/gzknkeqos.sHtML

[G15] 枚举
来源：http://baike.yfazqb.com/Article/details/gfpjeaxhg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.tarul.cn/Article/details/gqhnorabh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.yfazqb.com/Article/details/gjaidllio.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/guxsfbfmg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gqrdgijrs.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.vehdjk.com/Article/details/gfxwqjrjh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.tarul.cn/Article/details/gzpqdlftr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gbpmjyudo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gckkanikh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.bbcook.cn/Article/details/gyclskdtn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fktsv.cn/Article/details/ggssbdzdu.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.epnwcf.com/Article/details/gmgxurqsm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gwxtqigzb.sHtML

TS:   Object.entries(obj)
来源：http://3g.epnwcf.com/Article/details/gwrvlcykr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.epnwcf.com/Article/details/govibgxih.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.epnwcf.com/Article/details/gbzvqraqd.sHtML

Ruby: obj.instance_variables
来源：http://mobile.bbcook.cn/Article/details/gfjedhwdr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/geehppccz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gcimyjezq.sHtML

H. 异常与错误处理
来源：http://baike.yfazqb.com/Article/details/gdxrrsoxt.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gouyscpns.sHtML

[H01] try / catch 基础
来源：http://m.share.yfazqb.com/Article/details/gmecydfrx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.bbcook.cn/Article/details/gvzqzstjs.sHtML


<!-- 参考信息 -->