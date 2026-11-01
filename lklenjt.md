代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/giowpzwbk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gumugkoql.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.yfazqb.com/Article/details/gmscyplxx.sHtML

[E17] 首字母大写
来源：http://mobile.tarul.cn/Article/details/gocrnnbwc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/gdkveisbh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fktsv.cn/Article/details/gxryteqmq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gislgdnkk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gesrzohpy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.vehdjk.com/Article/details/gskwyillg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fktsv.cn/Article/details/glqizivzj.sHtML

Ruby: s.capitalize
来源：http://www.m.share.sjlbkw.cn/Article/details/gzljcucaq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/ghlrjylke.sHtML

[E18] 模板占位符替换
来源：http://www.share.vehdjk.com/Article/details/geeewggxz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.tarul.cn/Article/details/ggfzetaye.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.yfazqb.com/Article/details/gfktsweex.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gxjznellz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gaknbmlov.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gzevfoniz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gwhvkswtt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/gnqinpjht.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.bbcook.cn/Article/details/gwztucnmu.sHtML

[E19] 多行文本按行拆分
来源：http://baike.yfazqb.com/Article/details/ggtrzfhpx.sHtML

Py:   s.splitlines()
来源：http://3g.tarul.cn/Article/details/gkdngluky.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.vehdjk.com/Article/details/gxaqzbryx.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/ghywzhoyk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gnthzpsut.sHtML

Java: s.lines().toList()
来源：http://www.blog.epnwcf.com/Article/details/gxyddbcyq.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gnjxokuzq.sHtML

Ruby: s.lines
来源：http://www.blog.vehdjk.com/Article/details/gnnpnptjx.sHtML

C#:   s.Split('\n')
来源：http://m.share.yfazqb.com/Article/details/gcnqjuabs.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.vehdjk.com/Article/details/gfnhskdjl.sHtML

Py:   if not s:
来源：http://www.blog.epnwcf.com/Article/details/gpsdiutgp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrobbozk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjfjfckb.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/gwxcgitni.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/gpjidioht.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/gzhsjhnyx.sHtML

Ruby: if s.empty?
来源：http://baike.bbcook.cn/Article/details/gzkgqotkl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/gcyuzlspd.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/gcqmutgdu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fktsv.cn/Article/details/gdonhvnoq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gfgjakcjh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gkvpiqrbk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gjpumhctn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/grbnyfvvm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.sjlbkw.cn/Article/details/gztpjycqm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gwrcbtluq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gdxrfmzli.sHtML

[E22] 字节长度与字符长度
来源：http://3g.sjlbkw.cn/Article/details/gmenwazin.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.bbcook.cn/Article/details/genomrrgm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gcmbyywzs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gyluzhsis.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gusqnacsg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.tarul.cn/Article/details/gmrcgfakz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/gnrvkggfi.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.yfazqb.com/Article/details/gvdnndatu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.tarul.cn/Article/details/grrixnxur.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gomjgiifl.sHtML

F. 文件与目录
来源：http://m.share.fktsv.cn/Article/details/gxiyrzmnd.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gzhejlhrw.sHtML

[F01] 读取整个文件
来源：http://read.share.sjlbkw.cn/Article/details/gmkgduatc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/gmvutvmpj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gayswtrdx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.vehdjk.com/Article/details/gvleoxgdf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gafsdlicp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/grtpgbefq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.sjlbkw.cn/Article/details/gmziktpbg.sHtML

Ruby: File.read("a.txt")
来源：http://baike.bbcook.cn/Article/details/grdbbwwyj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/ggnhktfhg.sHtML

[F02] 逐行读取文件
来源：http://mobile.sjlbkw.cn/Article/details/garnlgzmv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fktsv.cn/Article/details/ghbpdhpxp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.bbcook.cn/Article/details/gobguqkpx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gbzfrqlhl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gowxyqfef.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gqpnuczmp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.yfazqb.com/Article/details/gjvpmiwts.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.tarul.cn/Article/details/gjtklbakg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.tarul.cn/Article/details/gftsiftji.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.epnwcf.com/Article/details/gxnkkvtzl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.vehdjk.com/Article/details/gcrbolbof.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/ggvslmgrp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gjlbxjzqn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/glrpffeov.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.epnwcf.com/Article/details/gskppxvig.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fktsv.cn/Article/details/gkyfpvvzr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gvsurmhcd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/ggfltskqu.sHtML

[F04] 追加写入文件
来源：http://www.share.fktsv.cn/Article/details/gsrteziio.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.vehdjk.com/Article/details/gldbgtybn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.bbcook.cn/Article/details/gjwzpzcjx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gheiulpwl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/gbvcqghif.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.yfazqb.com/Article/details/ggkfdawey.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gboaggslk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.tarul.cn/Article/details/gcutoncyy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.vehdjk.com/Article/details/glhquaipl.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.bbcook.cn/Article/details/gizhdnrai.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fktsv.cn/Article/details/gkjutcpzx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gossckuro.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gcxybicev.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gqgrzmewc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gurtztxay.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.yfazqb.com/Article/details/gqeuslglx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.vehdjk.com/Article/details/giyxcugtw.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gzrremdjn.sHtML

[F06] 删除文件
来源：http://www.blog.tarul.cn/Article/details/gczdjxdwl.sHtML

Py:   os.remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gcftjddok.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/giofpjbnf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gnijuduta.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gpmzcdafg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/glaipyycj.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gxybgahoq.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gugxkoapt.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gajradphh.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.vehdjk.com/Article/details/ginhkztez.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.tarul.cn/Article/details/gwqcwtvvh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.tarul.cn/Article/details/gflvqziiz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/glmsnayzp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gmhzhcxhp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.vehdjk.com/Article/details/gzctjjatk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/gxvflckan.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.bbcook.cn/Article/details/gjllhmxun.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.epnwcf.com/Article/details/gpeiroual.sHtML

[F08] 遍历目录
来源：http://www.m.share.tarul.cn/Article/details/gpaxkgmkd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.sjlbkw.cn/Article/details/gmxtqazvf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.bbcook.cn/Article/details/gugxazgxi.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gqhfonrem.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gwgpafquq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/giuflgyvw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gwfblbfmb.sHtML

Ruby: Dir.children("dir")
来源：http://baike.bbcook.cn/Article/details/gnrgonkqd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.yfazqb.com/Article/details/gjeewxzbm.sHtML

[F09] 获取文件大小
来源：http://www.m.share.vehdjk.com/Article/details/gpnrvbqvk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gjfmxddud.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gfuwujogb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gscpzjbtm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/gidphqggm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gbkyxqguu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.bbcook.cn/Article/details/gfqytwasi.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gtenucjnz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.yfazqb.com/Article/details/ghftuhjts.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.sjlbkw.cn/Article/details/gxgufntsh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gnjmgxbch.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.epnwcf.com/Article/details/gtrhxavcw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gxoaqebip.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gzeopekiz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.epnwcf.com/Article/details/goayfbbjd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gncujmyfn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gypcjtyvd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gbdkmsleb.sHtML

[F11] 复制与移动文件
来源：http://www.share.sjlbkw.cn/Article/details/gpunlpzhu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gdfhtahxz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.tarul.cn/Article/details/gtjjipsmv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gfqvtzxov.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gqeoanldv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.yfazqb.com/Article/details/gohbqdyfr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.bbcook.cn/Article/details/gtlulhmzm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/ggpazyzwz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.yfazqb.com/Article/details/gjwlzavpu.sHtML

[F12] CSV 读写
来源：http://mobile.yfazqb.com/Article/details/gvguldmig.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.epnwcf.com/Article/details/gufyvhraf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.tarul.cn/Article/details/gkrfmusjv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gvpsykhkh.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/gpohgwlvj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.tarul.cn/Article/details/ggnagzfhq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.yfazqb.com/Article/details/giysbiggz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.tarul.cn/Article/details/gzvrcgagc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.vehdjk.com/Article/details/gunshnuqb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmeuphfus.sHtML

G. 面向对象
来源：http://wap.vehdjk.com/Article/details/ggylmlbud.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gnglftpqi.sHtML

[G01] 定义类
来源：http://baike.fktsv.cn/Article/details/gycywzisi.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/grocqzclm.sHtML

PHP:  class User {}
来源：http://3g.tarul.cn/Article/details/ghmbnhmmi.sHtML

JS:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gdvehwrop.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/gazjdxnlk.sHtML

Java: class User {}
来源：http://mobile.bbcook.cn/Article/details/glpkiaxve.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzrgphks.sHtML

Ruby: class User; end
来源：http://www.m.share.epnwcf.com/Article/details/ggdcrropk.sHtML

C#:   class User {}
来源：http://m.share.yfazqb.com/Article/details/groogjihg.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/guswbchwl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.yfazqb.com/Article/details/glrssnazg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/geacrpdli.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/getilnjzq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fktsv.cn/Article/details/gbqalmajh.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/glfezokmb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.yfazqb.com/Article/details/gcbsjhuag.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.yfazqb.com/Article/details/girynfrtp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gqkvfxlpy.sHtML

[G03] 实例属性
来源：http://wap.sjlbkw.cn/Article/details/gacrykbcr.sHtML

Py:   self.name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/goztrzzah.sHtML

PHP:  public string $name = "x";
来源：http://wap.epnwcf.com/Article/details/ggdgbozve.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gbdjulwsj.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/gempbqcwg.sHtML

Java: private String name;
来源：http://www.m.share.vehdjk.com/Article/details/gxonsivbr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/gpqhhmvnf.sHtML

Ruby: @name = "x"
来源：http://wap.tarul.cn/Article/details/gbjsczmtf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.epnwcf.com/Article/details/gqujohjlc.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/gxskjryfr.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/grmfoovhv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gfqzmurly.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gyudrbcog.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/grknbottj.sHtML

Java: String greet() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gosztqjof.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/ggnfgynnx.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gcsjaahdn.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gbgequxjo.sHtML

[G05] 继承
来源：http://m.share.tarul.cn/Article/details/gprythvhw.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fktsv.cn/Article/details/gpvvwvdjw.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gyzivzfvk.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gjscehmob.sHtML

TS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gcfmrgtrs.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gqjepazja.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/gfarorzsr.sHtML

Ruby: class Admin < User; end
来源：http://mobile.sjlbkw.cn/Article/details/gjqmcajit.sHtML

C#:   class Admin : User {}
来源：http://3g.sjlbkw.cn/Article/details/gsrvjglwk.sHtML

[G06] 重写方法
来源：http://baike.yfazqb.com/Article/details/glnxlcffq.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.vehdjk.com/Article/details/gpapukafo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gwwjevzvx.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gpclqoodp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gacthrsem.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gobiuomna.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.bbcook.cn/Article/details/gcporjseu.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.sjlbkw.cn/Article/details/gklctgbsl.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.bbcook.cn/Article/details/gaoubsnuo.sHtML

[G07] 调用父类方法
来源：http://wap.epnwcf.com/Article/details/gcgisfzyx.sHtML

Py:   super().greet()
来源：http://www.blog.sjlbkw.cn/Article/details/gmrbdeflf.sHtML

PHP:  parent::greet();
来源：http://blog.sjlbkw.cn/Article/details/gyzpipfid.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gezlasgpc.sHtML

TS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gsgwlvmfx.sHtML

Java: super.greet();
来源：http://blog.fktsv.cn/Article/details/gwystjnue.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gjtuymfif.sHtML

Ruby: super
来源：http://www.blog.vehdjk.com/Article/details/gazyyoaxh.sHtML

C#:   base.Greet();
来源：http://www.m.share.vehdjk.com/Article/details/gcoqasskp.sHtML

[G08] 静态方法与属性
来源：http://www.share.sjlbkw.cn/Article/details/gryeebuvc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaakzcbh.sHtML

PHP:  public static function f() {}
来源：http://m.share.vehdjk.com/Article/details/gpkototzy.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gqweaqoji.sHtML

TS:   static f(): void {}
来源：http://www.blog.sjlbkw.cn/Article/details/grlpweskv.sHtML

Java: static void f() {}
来源：http://3g.epnwcf.com/Article/details/gbukrtcho.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.sjlbkw.cn/Article/details/glorrfcxp.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/gnsbyldvt.sHtML

C#:   public static void F() {}
来源：http://www.m.share.tarul.cn/Article/details/gmrjmpoku.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fktsv.cn/Article/details/gykxrpxnw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.tarul.cn/Article/details/gzsbkxlla.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.yfazqb.com/Article/details/guhzmqhtr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.bbcook.cn/Article/details/gpzadqqlh.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.tarul.cn/Article/details/gzpkikyrb.sHtML

Java: interface Shape { double area(); }
来源：http://baike.sjlbkw.cn/Article/details/ggwffxcyo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.tarul.cn/Article/details/gotxrqiyu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.sjlbkw.cn/Article/details/gfxaojicr.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.tarul.cn/Article/details/gdbbkvnpa.sHtML

[G10] 访问控制
来源：http://www.share.fktsv.cn/Article/details/gqqagvfsi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.yfazqb.com/Article/details/gxvjwxums.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gylaxtaqk.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.yfazqb.com/Article/details/gkzcdvzhu.sHtML

TS:   public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gjnnjmbvf.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.bbcook.cn/Article/details/gfgfkzqsc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/gdpoktriw.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gkzqjzjfb.sHtML

C#:   public / protected / private / internal
来源：http://3g.vehdjk.com/Article/details/gpkqujojn.sHtML

[G11] getter / setter
来源：http://www.m.share.bbcook.cn/Article/details/gdlejnsdo.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/gigpbqpae.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/giudenkgv.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gnmntxiuy.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnajnktot.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gjvlqidvx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/ghtrjldnl.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.tarul.cn/Article/details/gwarsjjpr.sHtML

C#:   public string Name { get; set; }
来源：http://baike.tarul.cn/Article/details/gjnfkzqfx.sHtML

[G12] 对象转字符串
来源：http://wap.epnwcf.com/Article/details/gqtkxahcb.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.vehdjk.com/Article/details/gpkmjabzo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gjlhmvgbd.sHtML

JS:   toString() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gpvbacsxq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gxlvnyxqz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gwcsrsrax.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gidqyoavd.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.tarul.cn/Article/details/goqkuivvz.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.epnwcf.com/Article/details/ghmspvsad.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/gubahmnom.sHtML

Py:   isinstance(u, User)
来源：http://mobile.epnwcf.com/Article/details/geqgblxsz.sHtML

PHP:  $u instanceof User
来源：http://blog.epnwcf.com/Article/details/gllurrfca.sHtML

JS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gvuplnuvz.sHtML

TS:   u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gbybguvbz.sHtML

Java: u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/ggxhiuqrb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.bbcook.cn/Article/details/gzqjriwyt.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gbejxddxh.sHtML

C#:   u is User
来源：http://www.blog.epnwcf.com/Article/details/goiajatwh.sHtML

[G14] 数据类 / record
来源：http://www.share.epnwcf.com/Article/details/gtvjlibrn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.sjlbkw.cn/Article/details/gonlbeqcl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.sjlbkw.cn/Article/details/gnrwcjrod.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.epnwcf.com/Article/details/gmqnbbcte.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.tarul.cn/Article/details/gquhhohis.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.vehdjk.com/Article/details/gsvxgmxqe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.vehdjk.com/Article/details/gwyxspprn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.tarul.cn/Article/details/gxjckvmth.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/gyrpyqynz.sHtML

[G15] 枚举
来源：http://www.blog.bbcook.cn/Article/details/godtavxei.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.sjlbkw.cn/Article/details/gzjnvxmtl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.yfazqb.com/Article/details/gpqyxdgea.sHtML


<!-- 参考信息 -->