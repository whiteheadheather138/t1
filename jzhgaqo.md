代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.epnwcf.com/Article/details/grvzenvrn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.bbcook.cn/Article/details/gkfzcuvtu.sHtML

Ruby: s.capitalize
来源：http://read.share.epnwcf.com/Article/details/gwbatnjsb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvdlgevf.sHtML

[E18] 模板占位符替换
来源：http://baike.bbcook.cn/Article/details/gvmlpwuav.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fktsv.cn/Article/details/grovntcjj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/guavkxdif.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gfnigndsq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/ghmcbhhek.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gbnplfbfl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gghppyryw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.bbcook.cn/Article/details/ghkrknypi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/gncysksfn.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fktsv.cn/Article/details/gyeluybiv.sHtML

Py:   s.splitlines()
来源：http://read.share.sjlbkw.cn/Article/details/gqfxujpmw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gdwqpvyyy.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gmwbegtoh.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/glkjcjdbf.sHtML

Java: s.lines().toList()
来源：http://www.blog.fktsv.cn/Article/details/gkvkamhrh.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.sjlbkw.cn/Article/details/gmrqdomry.sHtML

Ruby: s.lines
来源：http://baike.tarul.cn/Article/details/gstscqgyl.sHtML

C#:   s.Split('\n')
来源：http://mobile.fktsv.cn/Article/details/gnntdziux.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gtjfgutgo.sHtML

Py:   if not s:
来源：http://baike.bbcook.cn/Article/details/gtkrzujct.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.yfazqb.com/Article/details/gwgbuggjq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.bbcook.cn/Article/details/gyfdrcewb.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/gqtbprnvg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/gttizxvoo.sHtML

Go:   if s == "" {}
来源：http://blog.tarul.cn/Article/details/gcgqsazjb.sHtML

Ruby: if s.empty?
来源：http://blog.sjlbkw.cn/Article/details/gvfyfjzvm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gckieuzfl.sHtML

[E21] 超长截断加省略号
来源：http://blog.vehdjk.com/Article/details/gnmtonnpx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/gltyujifj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/guofzdite.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gicmsnvcw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gonrmgukp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gwcwlnmth.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.vehdjk.com/Article/details/ggtpymibm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gkgmaisjq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gygcpkquw.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.tarul.cn/Article/details/gldxaocao.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.sjlbkw.cn/Article/details/gptpiiyrm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/grtkzdrrw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/grawumqgd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/ghddfgfnx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gppypdaml.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/grlubouga.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/ginyoulby.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.epnwcf.com/Article/details/ggcevyhvg.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glizxzvao.sHtML

F. 文件与目录
来源：http://read.share.sjlbkw.cn/Article/details/gcpkqosow.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gydnxoayn.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/gzyevcxzf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gyijpeajf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.tarul.cn/Article/details/gqfonztnc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.tarul.cn/Article/details/gkwijyicp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gyhijvavp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gldezququ.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/gfqbjqwwt.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.vehdjk.com/Article/details/guwwwmuux.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/giholddrx.sHtML

[F02] 逐行读取文件
来源：http://www.blog.vehdjk.com/Article/details/gfwapglqj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.yfazqb.com/Article/details/gvgaeghpc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.tarul.cn/Article/details/gyedjhuga.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gatbkwjhz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gwogqmjgc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/gghjlhaha.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.yfazqb.com/Article/details/gytizvvma.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.tarul.cn/Article/details/gawbbvnpj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.tarul.cn/Article/details/goghtbalj.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/gemaurmqi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.vehdjk.com/Article/details/giyadlewt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gqywcrypj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gtjsfisgs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gbcfpjpxk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fktsv.cn/Article/details/giaqiloos.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.bbcook.cn/Article/details/gwdzcpiba.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.tarul.cn/Article/details/gujumwyyr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gddcmciej.sHtML

[F04] 追加写入文件
来源：http://www.share.bbcook.cn/Article/details/gqnwadeda.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/gnbvotefi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.sjlbkw.cn/Article/details/gpfjnkxmw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gsanalvae.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/gckrwgcqv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fktsv.cn/Article/details/grverhwfd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.bbcook.cn/Article/details/gzpktfxlp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fktsv.cn/Article/details/grclqpulz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/gxipfahlv.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.tarul.cn/Article/details/gqhwujqsg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.tarul.cn/Article/details/gpqnsdglb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gkhqfpnqs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gzojjrqgk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/glgfdtqvu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/glhvvbzwq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.epnwcf.com/Article/details/gcbihyemc.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.vehdjk.com/Article/details/gfjmmwweg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/glloiegra.sHtML

[F06] 删除文件
来源：http://mobile.epnwcf.com/Article/details/gpkzjqykx.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gmyisimdh.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gjkeeowlo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gnvlnsfco.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gibkbstqy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gogkqhxja.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/grjkkspoz.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gyjypcrrl.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gkrphpbol.sHtML

[F07] 创建目录（含多级）
来源：http://baike.tarul.cn/Article/details/gvfnkclzs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gpsrazmpq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.sjlbkw.cn/Article/details/grxipxmqw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gzzeklbzn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gcpxhpxku.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fktsv.cn/Article/details/gxfxgmwxz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.tarul.cn/Article/details/gtxexyqrl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.bbcook.cn/Article/details/gxwxjcjwz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.bbcook.cn/Article/details/gmugmecey.sHtML

[F08] 遍历目录
来源：http://mobile.bbcook.cn/Article/details/gffupfltq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/giaifcand.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.yfazqb.com/Article/details/gezadkivu.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gvztldtkr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gngxefrrp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gqumkqiwu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.epnwcf.com/Article/details/gwtndjcwl.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.vehdjk.com/Article/details/gcvtgccgg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.tarul.cn/Article/details/giigzhkit.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/gjrkgqrjr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gbncpvgmy.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gmicqbgui.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gjxczoodu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/ggodrphts.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/giafeqyqw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.bbcook.cn/Article/details/gojlwwrex.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gacwhurcx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.tarul.cn/Article/details/gtipdrmbq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.sjlbkw.cn/Article/details/gkakukbih.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gjepzeerj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gbihllppb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gtberyjbi.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fktsv.cn/Article/details/gislsnsic.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.epnwcf.com/Article/details/ggcyakcsh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/ggypomvun.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/grqlsarce.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gmkwsvboc.sHtML

[F11] 复制与移动文件
来源：http://m.share.bbcook.cn/Article/details/ghjxgoqks.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gawotwxmh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.epnwcf.com/Article/details/ghefxvdrp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gkduayjxt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gnxeuubar.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gntjwylrj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gfpdxkbly.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/ghqcsduiq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.sjlbkw.cn/Article/details/gxpvtnhgo.sHtML

[F12] CSV 读写
来源：http://mobile.tarul.cn/Article/details/gyonxjdkh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/grjiyeosx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fktsv.cn/Article/details/gizyukrza.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.epnwcf.com/Article/details/gdtieefeq.sHtML

TS:   // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gedfnwmdh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/gtvaqfdde.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.sjlbkw.cn/Article/details/ghvbxyprx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fktsv.cn/Article/details/gzygkvofq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmhsalgh.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gxecchmyr.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/goptfnvzo.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcbljjxqr.sHtML

[G01] 定义类
来源：http://3g.yfazqb.com/Article/details/gmxlopafy.sHtML

Py:   class User: pass
来源：http://blog.bbcook.cn/Article/details/gkirtltyg.sHtML

PHP:  class User {}
来源：http://wap.bbcook.cn/Article/details/gkafcmoeg.sHtML

JS:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gnmwoioot.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fktsv.cn/Article/details/ghhbycucj.sHtML

Java: class User {}
来源：http://mobile.tarul.cn/Article/details/golkostsk.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/gmefvplsc.sHtML

Ruby: class User; end
来源：http://mobile.fktsv.cn/Article/details/gcgwsmwez.sHtML

C#:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gasnvidlh.sHtML

[G02] 构造函数
来源：http://3g.fktsv.cn/Article/details/gglngaefm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fktsv.cn/Article/details/gybykzozt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.epnwcf.com/Article/details/gjydgdqsm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gsvmplvwx.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.sjlbkw.cn/Article/details/gqnalrtyr.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gjpmxwuzl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.vehdjk.com/Article/details/gmuwrvafy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.epnwcf.com/Article/details/gymbyeefs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.yfazqb.com/Article/details/gbxvetqok.sHtML

[G03] 实例属性
来源：http://baike.tarul.cn/Article/details/gdnxtvevz.sHtML

Py:   self.name = "x"
来源：http://baike.sjlbkw.cn/Article/details/guegeawum.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/ggvnebpnh.sHtML

JS:   this.name = "x";
来源：http://www.share.vehdjk.com/Article/details/gmwmzpqtp.sHtML

TS:   name: string = "x";
来源：http://baike.epnwcf.com/Article/details/gexubmklq.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/gaemcscai.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.yfazqb.com/Article/details/gjqgxmylx.sHtML

Ruby: @name = "x"
来源：http://read.share.yfazqb.com/Article/details/gtskdxvyy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gjfcpsipv.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/geaciysnc.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gstzyqvqq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gxkcwhqdw.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gtpnsipet.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gswmwydum.sHtML

Java: String greet() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gcqafdmis.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gxsrmadns.sHtML

Ruby: def greet; @name; end
来源：http://m.share.epnwcf.com/Article/details/gqztcqsot.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gqgpumwde.sHtML

[G05] 继承
来源：http://read.share.fktsv.cn/Article/details/ggkdsxpru.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/guyevjfac.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gugyojtkg.sHtML

JS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gcpsjwnrt.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/ggswznvwj.sHtML

Java: class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gwripuelj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.yfazqb.com/Article/details/gbvdnircp.sHtML

Ruby: class Admin < User; end
来源：http://mobile.bbcook.cn/Article/details/ggiwsldsw.sHtML

C#:   class Admin : User {}
来源：http://blog.yfazqb.com/Article/details/gojlbgyfn.sHtML

[G06] 重写方法
来源：http://www.share.bbcook.cn/Article/details/gwejwsekk.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.bbcook.cn/Article/details/geaiuktip.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gowugjpup.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gjqizvzez.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/glhjvspvn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gwkhsusxh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.bbcook.cn/Article/details/gkkuaddia.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.tarul.cn/Article/details/gejlfhllv.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.tarul.cn/Article/details/gmbogkvom.sHtML

[G07] 调用父类方法
来源：http://baike.vehdjk.com/Article/details/gqczacyll.sHtML

Py:   super().greet()
来源：http://www.m.share.epnwcf.com/Article/details/gtuammfzr.sHtML

PHP:  parent::greet();
来源：http://www.share.fktsv.cn/Article/details/gjrenjgcp.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gatarcbiy.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gwdpxyqsb.sHtML

Java: super.greet();
来源：http://mobile.vehdjk.com/Article/details/gmrltbwfc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gzxekcllg.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/gzdchycub.sHtML

C#:   base.Greet();
来源：http://wap.tarul.cn/Article/details/gpxaarqiu.sHtML

[G08] 静态方法与属性
来源：http://www.blog.yfazqb.com/Article/details/gkerlkyuk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.vehdjk.com/Article/details/gzybcfecl.sHtML

PHP:  public static function f() {}
来源：http://read.share.tarul.cn/Article/details/ghgpfqdpc.sHtML

JS:   static f() {}
来源：http://www.share.tarul.cn/Article/details/glljccahj.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/ggrgthnfs.sHtML

Java: static void f() {}
来源：http://read.share.yfazqb.com/Article/details/gpvaumvkl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.vehdjk.com/Article/details/gdcwkunrx.sHtML

Ruby: def self.f; end
来源：http://blog.epnwcf.com/Article/details/gbfjrhebp.sHtML

C#:   public static void F() {}
来源：http://www.share.bbcook.cn/Article/details/gvzttldzr.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fktsv.cn/Article/details/gsltxzjlk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.vehdjk.com/Article/details/gnjtkdvxd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.yfazqb.com/Article/details/gqndwlkud.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.tarul.cn/Article/details/gdqqaurhn.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/gsrnqjcyx.sHtML

Java: interface Shape { double area(); }
来源：http://baike.tarul.cn/Article/details/gxkpoyiiy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.sjlbkw.cn/Article/details/gfippqwys.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.yfazqb.com/Article/details/gvzrinldw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gjinrbtzu.sHtML

[G10] 访问控制
来源：http://blog.sjlbkw.cn/Article/details/gzcvydupy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/gotkffeju.sHtML

PHP:  public / protected / private
来源：http://www.share.tarul.cn/Article/details/gaofqmryr.sHtML

JS:   #private 字段；其余公开
来源：http://wap.yfazqb.com/Article/details/gqdrlzclb.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gwqpoterz.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.epnwcf.com/Article/details/gfcrbhjni.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.bbcook.cn/Article/details/gczkhlipt.sHtML

Ruby: public / protected / private
来源：http://blog.bbcook.cn/Article/details/gcczwweuv.sHtML

C#:   public / protected / private / internal
来源：http://www.share.tarul.cn/Article/details/gunvxxxbp.sHtML

[G11] getter / setter
来源：http://wap.epnwcf.com/Article/details/gyoogqixb.sHtML

Py:   @property 与 @x.setter
来源：http://baike.bbcook.cn/Article/details/gbcvxbqti.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gbgmahmth.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/ghldxfeor.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbfvvuhko.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/gbcwgytku.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gqxaqfmnf.sHtML

Ruby: attr_accessor :name
来源：http://mobile.epnwcf.com/Article/details/gyuobejkx.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fktsv.cn/Article/details/ghvxozmni.sHtML

[G12] 对象转字符串
来源：http://3g.tarul.cn/Article/details/gprytshcv.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gseyhbttl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gficdppsk.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gueivzihk.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gybhmfbhv.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.tarul.cn/Article/details/gosoxseae.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gfazmzxpu.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gkuynnzwg.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.vehdjk.com/Article/details/gqwbegqzx.sHtML

[G13] 判断对象类型
来源：http://baike.epnwcf.com/Article/details/gvhrpkark.sHtML

Py:   isinstance(u, User)
来源：http://mobile.vehdjk.com/Article/details/giswzhyxk.sHtML

PHP:  $u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/gunjnxyoj.sHtML

JS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gjiugeeqt.sHtML

TS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/grkrghctz.sHtML

Java: u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gaujfknnz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.tarul.cn/Article/details/guzhxauln.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fktsv.cn/Article/details/gvkqokpkp.sHtML

C#:   u is User
来源：http://www.share.yfazqb.com/Article/details/gudnvyrwv.sHtML

[G14] 数据类 / record
来源：http://wap.tarul.cn/Article/details/girwmozye.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/gxdydwoqx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fktsv.cn/Article/details/gdjbjmtlr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/gvdvkgrqu.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.tarul.cn/Article/details/gyeffcuva.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fktsv.cn/Article/details/grrzshxzg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fktsv.cn/Article/details/gmidthpqv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fktsv.cn/Article/details/gxlcizaax.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.tarul.cn/Article/details/gkntipltv.sHtML

[G15] 枚举
来源：http://baike.tarul.cn/Article/details/gkbeiojtp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fktsv.cn/Article/details/gpnzktzgu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.tarul.cn/Article/details/gzxhavkdz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/gwtuebxcz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gzpfuhbdg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.bbcook.cn/Article/details/gzzlqckey.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.bbcook.cn/Article/details/gqivholxf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.yfazqb.com/Article/details/gsbkoqdqk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gxgacrqgx.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.sjlbkw.cn/Article/details/geevjioof.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fktsv.cn/Article/details/gfqpzffhi.sHtML


<!-- 参考信息 -->