代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.epnwcf.com/Article/details/gfpkmhlvr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gnbwghtim.sHtML

Ruby: s.capitalize
来源：http://read.share.epnwcf.com/Article/details/gjtxdqveu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fktsv.cn/Article/details/gyzeupqtb.sHtML

[E18] 模板占位符替换
来源：http://www.share.tarul.cn/Article/details/gcjwpkcty.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.vehdjk.com/Article/details/glokahvik.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/gvmmkhnmm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/glxzneltq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gwzruooyb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/giuunechi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gngoforhe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjbqjckv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.epnwcf.com/Article/details/gflqzjoly.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.tarul.cn/Article/details/ggysaiadv.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/gujtfeams.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.epnwcf.com/Article/details/ggdcoxioj.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/gszhreufu.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gtqbwacxq.sHtML

Java: s.lines().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gozjchfju.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/gbuzmukfq.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gkojdugbn.sHtML

C#:   s.Split('\n')
来源：http://blog.vehdjk.com/Article/details/gwdiarssv.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fktsv.cn/Article/details/gmsdzkmch.sHtML

Py:   if not s:
来源：http://blog.fktsv.cn/Article/details/gofrttohb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.sjlbkw.cn/Article/details/gnafecght.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fktsv.cn/Article/details/gywdgoais.sHtML

TS:   if (s === "") {}
来源：http://wap.epnwcf.com/Article/details/gdvstdpdx.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/gulxlqvxx.sHtML

Go:   if s == "" {}
来源：http://wap.vehdjk.com/Article/details/gyhfsmppd.sHtML

Ruby: if s.empty?
来源：http://baike.vehdjk.com/Article/details/gpgteocqe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/gudqgmfyc.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fktsv.cn/Article/details/gsfzlgvwi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.vehdjk.com/Article/details/gggfowuta.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gdohzenus.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gcdltpanj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gclxstbiw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gggyvferp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.tarul.cn/Article/details/gumnswtlo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gqpwguspz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gwsqvsehb.sHtML

[E22] 字节长度与字符长度
来源：http://blog.tarul.cn/Article/details/gvqangonh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.epnwcf.com/Article/details/gisnyxkhd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gpshkxxce.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gbhrbdgwk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gvjhkvpfi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fktsv.cn/Article/details/ghxswdxfh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.bbcook.cn/Article/details/gopddkeap.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gcbwobrqg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gwjzlzsum.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpcsavozg.sHtML

F. 文件与目录
来源：http://baike.epnwcf.com/Article/details/gzvjibord.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gokjqzobb.sHtML

[F01] 读取整个文件
来源：http://blog.yfazqb.com/Article/details/ghtqwkefy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.vehdjk.com/Article/details/gocmbbjwv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gejupsimv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.sjlbkw.cn/Article/details/gxiivtvkd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/ggkurbknn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/garvxojor.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.tarul.cn/Article/details/gnzxqzhae.sHtML

Ruby: File.read("a.txt")
来源：http://wap.vehdjk.com/Article/details/gfprjxpru.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gjqdvxjmc.sHtML

[F02] 逐行读取文件
来源：http://www.blog.vehdjk.com/Article/details/ggstkirtm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.bbcook.cn/Article/details/gwjfdwaul.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.vehdjk.com/Article/details/gkchrwkqo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gvilskktx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/glrgnjmrf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gilyrtrap.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/gtprkkyzk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gjcvwpljd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/gvohickkc.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.sjlbkw.cn/Article/details/gimahtrjt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/gaoxejxgx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/glzxeztmi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gbodfzfkp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcpjccdy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/gxgjfswmy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/gmynqqrmj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.epnwcf.com/Article/details/gyouvixpr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/giwmjcodw.sHtML

[F04] 追加写入文件
来源：http://www.share.epnwcf.com/Article/details/gyrbpuxzx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.epnwcf.com/Article/details/gwmpockce.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.tarul.cn/Article/details/gtanqhwux.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/gcxbgimxq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gnabtxtto.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.sjlbkw.cn/Article/details/gxsvptooy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gxsmrhnha.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gykiqcnji.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.epnwcf.com/Article/details/gqdelclgx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.yfazqb.com/Article/details/gvsxzxksy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/grksnvicq.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gfvpzwelh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvjeqyunm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gzbpuvrlj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gzubvedqi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.tarul.cn/Article/details/ghidpuklk.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/gigpiqvau.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gmhapgusg.sHtML

[F06] 删除文件
来源：http://www.share.vehdjk.com/Article/details/gbkieunxy.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gtbdptrar.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gmckxgrab.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/grmqbauho.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gheyuvfkt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gsnszkvhz.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gqycbcgil.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.yfazqb.com/Article/details/gxxpynwkh.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.epnwcf.com/Article/details/gzxbswoxv.sHtML

[F07] 创建目录（含多级）
来源：http://3g.sjlbkw.cn/Article/details/gfleyozhc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/gnhqazpsy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.tarul.cn/Article/details/gsnlaaaui.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/guygbzicr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gemiecnie.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.vehdjk.com/Article/details/gqqiruzml.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.sjlbkw.cn/Article/details/gzhtniwpz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.bbcook.cn/Article/details/gjkhmvvnh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.bbcook.cn/Article/details/gvyalbjzd.sHtML

[F08] 遍历目录
来源：http://read.share.yfazqb.com/Article/details/golkflnnu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gpbhvmybs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.sjlbkw.cn/Article/details/gechqxtuv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gjdccuqfc.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gexjuvsin.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gtcnwsfgd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/grywfecul.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gkaxguedm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.yfazqb.com/Article/details/ggfhpelfv.sHtML

[F09] 获取文件大小
来源：http://www.blog.yfazqb.com/Article/details/gzfrskizc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.vehdjk.com/Article/details/grozszgwm.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gxbjwcftl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.tarul.cn/Article/details/gbvqsevxv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gdiqkhrab.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gixcicktg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.sjlbkw.cn/Article/details/gtnkdvazd.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gkbgdmifw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/gdfhijxam.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fktsv.cn/Article/details/gwsnpcywu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gqgsqrlba.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.tarul.cn/Article/details/ggwpdccxe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gxvghitme.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gkwmbsmyj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/gvzewnprn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/giqbwlxyb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ghlbsmgcx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gbwkzxydr.sHtML

[F11] 复制与移动文件
来源：http://wap.sjlbkw.cn/Article/details/gfavnquxq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxozhdfdb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/gkwjhvvfq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gruovgjtl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/grrvwjpaz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.vehdjk.com/Article/details/gsjxpdsri.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.vehdjk.com/Article/details/gjwefalgb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gxwoltncn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fktsv.cn/Article/details/ggekxvzzx.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gnfhhyoff.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.vehdjk.com/Article/details/ganxdntwy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/gmaldyjwf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.yfazqb.com/Article/details/gttxpalxk.sHtML

TS:   // 同上
来源：http://read.share.bbcook.cn/Article/details/grdukwuup.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.yfazqb.com/Article/details/gldkubzae.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.bbcook.cn/Article/details/gmhqmiuyn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/glfwvtugj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.tarul.cn/Article/details/gzxkadcsq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggwqbrpff.sHtML

G. 面向对象
来源：http://read.share.bbcook.cn/Article/details/gbdhkcgue.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcsonptax.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gvasaqhce.sHtML

Py:   class User: pass
来源：http://www.share.bbcook.cn/Article/details/gfzydwutq.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gkdqpuibq.sHtML

JS:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gqhisjafe.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/gnonbeoni.sHtML

Java: class User {}
来源：http://m.share.epnwcf.com/Article/details/gwinvqvxk.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/gbgopdtla.sHtML

Ruby: class User; end
来源：http://baike.vehdjk.com/Article/details/gvlcwlzye.sHtML

C#:   class User {}
来源：http://baike.bbcook.cn/Article/details/gxsfjoedv.sHtML

[G02] 构造函数
来源：http://mobile.fktsv.cn/Article/details/gcdktokme.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.sjlbkw.cn/Article/details/gvdcgvhou.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gioacrsri.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/ggtbqikhs.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.yfazqb.com/Article/details/gonzedtsy.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gbzakzyrc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/ggwnghxhj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/ghpugehmh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fktsv.cn/Article/details/ggbmzawea.sHtML

[G03] 实例属性
来源：http://3g.yfazqb.com/Article/details/gfjzexnyo.sHtML

Py:   self.name = "x"
来源：http://baike.fktsv.cn/Article/details/gjnnimddn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.yfazqb.com/Article/details/guujkyjge.sHtML

JS:   this.name = "x";
来源：http://3g.tarul.cn/Article/details/gwcsozwbb.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/grvhyxsfv.sHtML

Java: private String name;
来源：http://baike.yfazqb.com/Article/details/gpbdymtdm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.bbcook.cn/Article/details/gxuaczjzr.sHtML

Ruby: @name = "x"
来源：http://read.share.epnwcf.com/Article/details/gjqtmkkga.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.tarul.cn/Article/details/gigaweldz.sHtML

[G04] 定义方法
来源：http://blog.yfazqb.com/Article/details/gjzfiluku.sHtML

Py:   def greet(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gknkfqfhr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/googhhkdq.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvdxibonw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gscgfpjpq.sHtML

Java: String greet() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gadeojoxn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gwgqwgrtr.sHtML

Ruby: def greet; @name; end
来源：http://wap.vehdjk.com/Article/details/gwobczkdh.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.bbcook.cn/Article/details/gnrerxfwt.sHtML

[G05] 继承
来源：http://read.share.vehdjk.com/Article/details/gupspjlcl.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.epnwcf.com/Article/details/gtqpffaea.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gmloprirg.sHtML

JS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gkllnxegv.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnsxcqpz.sHtML

Java: class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gwinlchhe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.epnwcf.com/Article/details/gsogbgybm.sHtML

Ruby: class Admin < User; end
来源：http://www.share.epnwcf.com/Article/details/gpbxskikl.sHtML

C#:   class Admin : User {}
来源：http://wap.fktsv.cn/Article/details/grjjlmqkr.sHtML

[G06] 重写方法
来源：http://www.blog.fktsv.cn/Article/details/gvqjpvktk.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.vehdjk.com/Article/details/gzfduxawt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gaxcxmnzf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/ggzabqcuq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/grnspppmx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gukgswiat.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.tarul.cn/Article/details/gsotzducy.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/gjngatygd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.bbcook.cn/Article/details/ggzrwdhlr.sHtML

[G07] 调用父类方法
来源：http://read.share.epnwcf.com/Article/details/gqrdovbac.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/gpfsgqfms.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gssdonpyw.sHtML

JS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/ghjcukxbg.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gxmqrvcuc.sHtML

Java: super.greet();
来源：http://www.blog.vehdjk.com/Article/details/ggjnmqsjm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/ggivomcpz.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/ghzxtytep.sHtML

C#:   base.Greet();
来源：http://www.share.tarul.cn/Article/details/ghzvgtvmu.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/gxvqyglzm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.sjlbkw.cn/Article/details/guacbedto.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gaukcajhg.sHtML

JS:   static f() {}
来源：http://blog.epnwcf.com/Article/details/gsakxiqhp.sHtML

TS:   static f(): void {}
来源：http://www.share.bbcook.cn/Article/details/grvcqmtld.sHtML

Java: static void f() {}
来源：http://blog.yfazqb.com/Article/details/gkxjzilld.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fktsv.cn/Article/details/gafroljba.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fktsv.cn/Article/details/gqcowyebn.sHtML

C#:   public static void F() {}
来源：http://m.share.tarul.cn/Article/details/gnkgebuat.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.yfazqb.com/Article/details/gnhscfwvo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.epnwcf.com/Article/details/gcspzvdyv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.bbcook.cn/Article/details/gatkgtyyd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.sjlbkw.cn/Article/details/gdsldvzzc.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.sjlbkw.cn/Article/details/greezgoqn.sHtML

Java: interface Shape { double area(); }
来源：http://blog.epnwcf.com/Article/details/gxqionkdo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.tarul.cn/Article/details/gfbgfvbvq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.vehdjk.com/Article/details/gsblmyuqp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.vehdjk.com/Article/details/gqlhruoor.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/glkeypawu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/goleqoaiv.sHtML

PHP:  public / protected / private
来源：http://mobile.yfazqb.com/Article/details/giamlxhfj.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.sjlbkw.cn/Article/details/gopmchorg.sHtML

TS:   public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/giatzfwog.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.sjlbkw.cn/Article/details/gxlhvnrya.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fktsv.cn/Article/details/gzumnoroc.sHtML

Ruby: public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gzidpqpuk.sHtML

C#:   public / protected / private / internal
来源：http://read.share.vehdjk.com/Article/details/gcpmffvql.sHtML

[G11] getter / setter
来源：http://mobile.epnwcf.com/Article/details/gyboyulgb.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.epnwcf.com/Article/details/gvpvftynb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gfmnhxrxv.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gwcufzgmv.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gdyyznrjp.sHtML

Java: public String getName() { return name; }
来源：http://read.share.tarul.cn/Article/details/groyerhpb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gxrntyfup.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/gxselxoeh.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.epnwcf.com/Article/details/gksarpgtn.sHtML

[G12] 对象转字符串
来源：http://mobile.bbcook.cn/Article/details/gfofcaxoc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/gdkmwarkx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gmeiqnsye.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gafubjnzp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gezwhxtoo.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gtjwwmgvw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/girhkxhhw.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gcuontweo.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.epnwcf.com/Article/details/gfxptzajd.sHtML

[G13] 判断对象类型
来源：http://www.m.share.epnwcf.com/Article/details/gmgxzfgpq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.sjlbkw.cn/Article/details/gjdebvrjb.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/grmfkwriq.sHtML

JS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gmximxkpe.sHtML

TS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gnouxeigv.sHtML

Java: u instanceof User
来源：http://3g.bbcook.cn/Article/details/gaiukzedx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.yfazqb.com/Article/details/grdxgwves.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/gcywmkxnm.sHtML

C#:   u is User
来源：http://3g.vehdjk.com/Article/details/gmxwynjfj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.tarul.cn/Article/details/gevmyayyc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.yfazqb.com/Article/details/grehxudvr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/ggobsicyw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.epnwcf.com/Article/details/gweqqcfyq.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.tarul.cn/Article/details/gxqtnhike.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.bbcook.cn/Article/details/gdvquxqgs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.vehdjk.com/Article/details/gjfnhfxqr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.yfazqb.com/Article/details/gjqwowxll.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/gtmusdpjh.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/gctcrkpee.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.bbcook.cn/Article/details/gguwnswzi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.vehdjk.com/Article/details/gdsongrup.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.bbcook.cn/Article/details/gtrahwmtm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/guruoyoif.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.vehdjk.com/Article/details/gwbgjujav.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.vehdjk.com/Article/details/gdvufohjd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.sjlbkw.cn/Article/details/gavdtfbza.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gvfqfwaas.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.epnwcf.com/Article/details/gjrjzuziv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.bbcook.cn/Article/details/grkittxvd.sHtML


<!-- 参考信息 -->