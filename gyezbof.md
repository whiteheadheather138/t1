代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gxygoaktp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.yfazqb.com/Article/details/gobbvckzj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/gmugrumsv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gaqytonsn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gvqwrhneg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.epnwcf.com/Article/details/ghrfbhjsj.sHtML

Ruby: s.capitalize
来源：http://mobile.epnwcf.com/Article/details/gnkvgcaww.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.vehdjk.com/Article/details/goohtkrtz.sHtML

[E18] 模板占位符替换
来源：http://mobile.epnwcf.com/Article/details/gcfpxnfzb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.epnwcf.com/Article/details/gfglesmmf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.epnwcf.com/Article/details/glreyzywo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gwajaoxvx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gjdtqtolv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gkrvrcksj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/giupdmdst.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.sjlbkw.cn/Article/details/gusytnkoe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.bbcook.cn/Article/details/gphdaezlu.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.sjlbkw.cn/Article/details/gmydvpjik.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/gjfraazqm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.tarul.cn/Article/details/gqtnjliem.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gadqygpes.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gqwyrjvad.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/gpujublcz.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gaqvdfbwl.sHtML

Ruby: s.lines
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjkbqnqr.sHtML

C#:   s.Split('\n')
来源：http://3g.fktsv.cn/Article/details/gskcaqave.sHtML

[E20] 判断字符串是否为空
来源：http://blog.yfazqb.com/Article/details/ggvdzrhhe.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/gviootgec.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.tarul.cn/Article/details/gmahpnkly.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.vehdjk.com/Article/details/gbmzsuerc.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gmkxsjfes.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gkretkdzs.sHtML

Go:   if s == "" {}
来源：http://www.m.share.epnwcf.com/Article/details/gdslrvndw.sHtML

Ruby: if s.empty?
来源：http://www.m.share.epnwcf.com/Article/details/gqtdxqird.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.epnwcf.com/Article/details/gxngpymwq.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/gvrifokom.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fktsv.cn/Article/details/gwudwzdyz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/grlbyuoam.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gznlduzjt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/glcmbivog.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gljmhvgpw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fktsv.cn/Article/details/gwumogizh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gratvpalu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gwdxpzaav.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/gwnvzlsql.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.tarul.cn/Article/details/goicyrwbo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gkwuzvwwa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gcquzubym.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gncvllyrj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/gxwmpinjh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.sjlbkw.cn/Article/details/gtxptrrjo.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/gtrqldqqj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.epnwcf.com/Article/details/glyjeytbs.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpwdwluph.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/gyqatoukg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glmgloomb.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/gaqfowhwz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.yfazqb.com/Article/details/gsvoqkfon.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.bbcook.cn/Article/details/gejikvhfn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.tarul.cn/Article/details/gcpncinsk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/grkcpuypn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gredrkyek.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.sjlbkw.cn/Article/details/gxtcpibdk.sHtML

Ruby: File.read("a.txt")
来源：http://3g.vehdjk.com/Article/details/glmgduike.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.vehdjk.com/Article/details/gkqgnarit.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/gslyzluse.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.yfazqb.com/Article/details/gztrcgcsj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.sjlbkw.cn/Article/details/gnlyehbjv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gqslypdlt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gwbgugssr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gncvanjna.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.yfazqb.com/Article/details/grlxbwkmy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.epnwcf.com/Article/details/gmqkayeek.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.vehdjk.com/Article/details/gqztdjjuk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/gpbouxatg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/glaoxutrq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gpcfsigjy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gwchdcgzz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gymicllid.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/gtcvrybmq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.epnwcf.com/Article/details/gkraykjgt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fktsv.cn/Article/details/gctjukwuj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/gqzgcivey.sHtML

[F04] 追加写入文件
来源：http://www.m.share.yfazqb.com/Article/details/ggkdrokjw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.tarul.cn/Article/details/giqjruljz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.bbcook.cn/Article/details/guyqursnk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/grmqsfbpt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gwmipcpjx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.bbcook.cn/Article/details/gujsfarsm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fktsv.cn/Article/details/gzlmyggif.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.vehdjk.com/Article/details/girpnfkob.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/gmrrqqskd.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.epnwcf.com/Article/details/gzupbfxpx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gftuofvwk.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.yfazqb.com/Article/details/gnfmxntds.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gvfxwemrp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/glhgykqom.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gimqddfru.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.yfazqb.com/Article/details/gpegpqrrp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gydifnmaq.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.vehdjk.com/Article/details/gsjptwpqw.sHtML

[F06] 删除文件
来源：http://m.share.fktsv.cn/Article/details/ggksgmweb.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gygurpnyh.sHtML

PHP:  unlink("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gwugtmboj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gwvxxwlzu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/ggkddxedl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gmvvhscob.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.tarul.cn/Article/details/gqfltiany.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.epnwcf.com/Article/details/gtihxejyf.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.tarul.cn/Article/details/gdamwxyjr.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.epnwcf.com/Article/details/gjdwjfcbk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gqvkttgwy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.sjlbkw.cn/Article/details/gcaxdrdnb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gipuzhghx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/grltzfsgo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.tarul.cn/Article/details/gmkzdnngu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fktsv.cn/Article/details/gtyizksbh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.tarul.cn/Article/details/gjffpioty.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.tarul.cn/Article/details/gfbceyizl.sHtML

[F08] 遍历目录
来源：http://baike.yfazqb.com/Article/details/gjnvkbbsg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/ggqkdimds.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fktsv.cn/Article/details/gtqldtlia.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gzsbhokov.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/gqhfydhby.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/ggxbxpeli.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gltjfbfrv.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/gulullwkn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.vehdjk.com/Article/details/gqdgdpysb.sHtML

[F09] 获取文件大小
来源：http://baike.vehdjk.com/Article/details/gtgweotst.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.yfazqb.com/Article/details/gutsdvbcl.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gshuwoffs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/geiuzeayx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/gwszhpbjh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gtwhjmuvr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.epnwcf.com/Article/details/gydpyfxgg.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gdqeuddgl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.yfazqb.com/Article/details/gcvsakfjl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.sjlbkw.cn/Article/details/gczesctvc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gdxyjrtkm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gejyjicqn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gnyfwposs.sHtML

TS:   path.extname("a.txt")
来源：http://wap.vehdjk.com/Article/details/gvafhslbx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.vehdjk.com/Article/details/groaswcqg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gejxantno.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gdjbqqhqj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gkzkccxbs.sHtML

[F11] 复制与移动文件
来源：http://read.share.vehdjk.com/Article/details/giphhgdbk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gawehvewt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.vehdjk.com/Article/details/gstzjjvns.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gvakmdwbp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gfnvyfaqo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gnolqeohy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.tarul.cn/Article/details/gagccruso.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gjdhlgynt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.tarul.cn/Article/details/gcycxguan.sHtML

[F12] CSV 读写
来源：http://wap.tarul.cn/Article/details/gfzggbhlk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.tarul.cn/Article/details/gglyyzbcy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.yfazqb.com/Article/details/gnfoaduwo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.tarul.cn/Article/details/gkpfzatjq.sHtML

TS:   // 同上
来源：http://baike.fktsv.cn/Article/details/gmdgvqvaw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.yfazqb.com/Article/details/guqxojnpk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gdfmtqbip.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.bbcook.cn/Article/details/gijytweth.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.yfazqb.com/Article/details/geugfuclw.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gbdmsbcou.sHtML

G. 面向对象
来源：http://mobile.vehdjk.com/Article/details/gxfqohvbx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gatfbpkma.sHtML

[G01] 定义类
来源：http://blog.sjlbkw.cn/Article/details/germgpsci.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/geczowwba.sHtML

PHP:  class User {}
来源：http://read.share.epnwcf.com/Article/details/gsqwfkdmg.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gaiptazzh.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fktsv.cn/Article/details/gnjlfusdy.sHtML

Java: class User {}
来源：http://wap.bbcook.cn/Article/details/gshpmlnwy.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.tarul.cn/Article/details/gaijhlyfc.sHtML

Ruby: class User; end
来源：http://www.share.yfazqb.com/Article/details/gczfkcnca.sHtML

C#:   class User {}
来源：http://blog.yfazqb.com/Article/details/gdgmgcqbm.sHtML

[G02] 构造函数
来源：http://3g.epnwcf.com/Article/details/gnvtdshcz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fktsv.cn/Article/details/giyexvhpo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gjoyurqrc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gmxnmobnb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/gpecfxsre.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/ggkiiftsv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gyhbpbmvn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.vehdjk.com/Article/details/gdwlpybse.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/gocpiguyt.sHtML

[G03] 实例属性
来源：http://m.share.bbcook.cn/Article/details/gvzjjyirx.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/gshrylhwc.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/gjaevwyog.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gdsiztrhy.sHtML

TS:   name: string = "x";
来源：http://m.share.fktsv.cn/Article/details/gqevydvsw.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gubbhtvql.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.tarul.cn/Article/details/gkjfmoggx.sHtML

Ruby: @name = "x"
来源：http://wap.epnwcf.com/Article/details/gonuzkzid.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gmppcbgqa.sHtML

[G04] 定义方法
来源：http://m.share.epnwcf.com/Article/details/ghnntymdl.sHtML

Py:   def greet(self): return self.name
来源：http://baike.tarul.cn/Article/details/ggckdzdzd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gegvpnjgi.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/ggacqxedx.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gfxliaqjl.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gflpltvpj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/guzlcystr.sHtML

Ruby: def greet; @name; end
来源：http://wap.bbcook.cn/Article/details/gldhzuide.sHtML

C#:   public string Greet() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gcdlcviwj.sHtML

[G05] 继承
来源：http://m.share.sjlbkw.cn/Article/details/gfugtkaui.sHtML

Py:   class Admin(User): pass
来源：http://3g.fktsv.cn/Article/details/gdufzrdni.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/geoywuuzk.sHtML

JS:   class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gusmexkqu.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/ganqmelkl.sHtML

Java: class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gsypegnaa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.bbcook.cn/Article/details/gfbgccxcs.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/gzuxiqmqs.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/gabgygpln.sHtML

[G06] 重写方法
来源：http://baike.tarul.cn/Article/details/gleslldkq.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.bbcook.cn/Article/details/gdrfqdqht.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gvxnpussp.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gynclmqin.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gjfjuafkv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gcwciiikj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/gowqrtaje.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/geqkupmut.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/gxkunfyui.sHtML

[G07] 调用父类方法
来源：http://www.blog.epnwcf.com/Article/details/ghfeajkjk.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/gvioxacju.sHtML

PHP:  parent::greet();
来源：http://www.m.share.yfazqb.com/Article/details/gnwekbxli.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/grnhqrusb.sHtML

TS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gmcpltnap.sHtML

Java: super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gmcgpiofg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.vehdjk.com/Article/details/gthostyqs.sHtML

Ruby: super
来源：http://www.share.yfazqb.com/Article/details/gbmeprumu.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/gmwayzcmn.sHtML

[G08] 静态方法与属性
来源：http://www.share.sjlbkw.cn/Article/details/ghgeldyha.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fktsv.cn/Article/details/geltyyhxs.sHtML

PHP:  public static function f() {}
来源：http://blog.yfazqb.com/Article/details/gvfjdudnp.sHtML

JS:   static f() {}
来源：http://read.share.bbcook.cn/Article/details/gmtbdekvd.sHtML

TS:   static f(): void {}
来源：http://baike.bbcook.cn/Article/details/gixhzmswy.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/gblnlqbea.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/gonjtmvaz.sHtML

Ruby: def self.f; end
来源：http://m.share.yfazqb.com/Article/details/gewewgdtu.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/gotvzdkup.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.sjlbkw.cn/Article/details/gvdqdvqpc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.bbcook.cn/Article/details/gthnhhhix.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.sjlbkw.cn/Article/details/gsmyewvrv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.tarul.cn/Article/details/ggkaljfsn.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/gpvromzvq.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.tarul.cn/Article/details/gnouqttks.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.epnwcf.com/Article/details/gxxyecpti.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.yfazqb.com/Article/details/gicazulca.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.vehdjk.com/Article/details/gqptoyhhp.sHtML

[G10] 访问控制
来源：http://blog.fktsv.cn/Article/details/gerdusqyr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.sjlbkw.cn/Article/details/gmfterybg.sHtML

PHP:  public / protected / private
来源：http://mobile.epnwcf.com/Article/details/gsrcajwoj.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fktsv.cn/Article/details/giemwniam.sHtML

TS:   public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gzfbwzvej.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.vehdjk.com/Article/details/gtybhdkmm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fktsv.cn/Article/details/gwexfncru.sHtML

Ruby: public / protected / private
来源：http://www.share.vehdjk.com/Article/details/guqknuzsv.sHtML

C#:   public / protected / private / internal
来源：http://blog.tarul.cn/Article/details/gqkvroaon.sHtML

[G11] getter / setter
来源：http://read.share.vehdjk.com/Article/details/gmyszrkdc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.tarul.cn/Article/details/govivedsw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gjelxytzi.sHtML

JS:   get name() { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gjlupxetd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gtfmyczba.sHtML

Java: public String getName() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gipqvuzpl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/ghqmjjwmd.sHtML

Ruby: attr_accessor :name
来源：http://www.share.yfazqb.com/Article/details/ghzkhqgia.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.vehdjk.com/Article/details/gmqtoaahv.sHtML

[G12] 对象转字符串
来源：http://wap.sjlbkw.cn/Article/details/grjaudkrk.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gfkxxzxyx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/grjcfxsin.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/guakyyzab.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gtysrhidh.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.yfazqb.com/Article/details/genqbktwg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gslegjszd.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/glcmkhowi.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gtemjqahx.sHtML

[G13] 判断对象类型
来源：http://wap.bbcook.cn/Article/details/gmewhbzpe.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fktsv.cn/Article/details/gusisqhfb.sHtML

PHP:  $u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gcqpelwfw.sHtML

JS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gtodkytet.sHtML

TS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gktidsqcv.sHtML

Java: u instanceof User
来源：http://baike.epnwcf.com/Article/details/gupakzmtt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.tarul.cn/Article/details/gppluoyzi.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.vehdjk.com/Article/details/gdulobbvk.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/gxjevuxxx.sHtML

[G14] 数据类 / record
来源：http://www.m.share.yfazqb.com/Article/details/gztxkugyq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.epnwcf.com/Article/details/ggrywlksl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.epnwcf.com/Article/details/gruoybxzr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.vehdjk.com/Article/details/gtfmglank.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.epnwcf.com/Article/details/grlzvrqvo.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.epnwcf.com/Article/details/gxcbmtsqj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/gppykrkjf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.yfazqb.com/Article/details/gkcuckrke.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.vehdjk.com/Article/details/gbaruyttm.sHtML

[G15] 枚举
来源：http://baike.bbcook.cn/Article/details/gjybuqaav.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.sjlbkw.cn/Article/details/gilpuveyx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.epnwcf.com/Article/details/gzpvgosfx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gjasfombl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/gppvwaeuh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.epnwcf.com/Article/details/gvxwpemtc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.epnwcf.com/Article/details/glfdozkpt.sHtML


<!-- 参考信息 -->