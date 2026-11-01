代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.epnwcf.com/Article/details/gnxpeepqe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.tarul.cn/Article/details/gcvkumqvi.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/gtdtjfhxw.sHtML

[E17] 首字母大写
来源：http://www.m.share.yfazqb.com/Article/details/gdfryfsfd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/ghpmmxebu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.bbcook.cn/Article/details/gaifpxkmu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gxgqwlsco.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gtydcolcw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.bbcook.cn/Article/details/gxrrrydwo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gnxgohnjk.sHtML

Ruby: s.capitalize
来源：http://m.share.bbcook.cn/Article/details/geycvfefz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.tarul.cn/Article/details/gqnpdhvor.sHtML

[E18] 模板占位符替换
来源：http://wap.vehdjk.com/Article/details/ggiefoeqr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.yfazqb.com/Article/details/gffuynqbx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.sjlbkw.cn/Article/details/gdvnyubky.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gjczixlei.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/ghltmzkrt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gpkmzoinz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.bbcook.cn/Article/details/grtnbjane.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.vehdjk.com/Article/details/gybbpfeny.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.vehdjk.com/Article/details/gbfnjyzre.sHtML

[E19] 多行文本按行拆分
来源：http://blog.tarul.cn/Article/details/ghfstszrx.sHtML

Py:   s.splitlines()
来源：http://www.share.yfazqb.com/Article/details/glptbtfnw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.tarul.cn/Article/details/gpftprnat.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gtwhhetde.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/gippkqiih.sHtML

Java: s.lines().toList()
来源：http://blog.bbcook.cn/Article/details/ghnihfeer.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gkmoalbum.sHtML

Ruby: s.lines
来源：http://baike.fktsv.cn/Article/details/gystdrlox.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.epnwcf.com/Article/details/gyteypgmv.sHtML

[E20] 判断字符串是否为空
来源：http://wap.tarul.cn/Article/details/gaixvimug.sHtML

Py:   if not s:
来源：http://www.m.share.sjlbkw.cn/Article/details/gymkvsbqh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.bbcook.cn/Article/details/gstvjubea.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.tarul.cn/Article/details/ggublxtbf.sHtML

TS:   if (s === "") {}
来源：http://mobile.epnwcf.com/Article/details/gzjjaocct.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gfiltrdzf.sHtML

Go:   if s == "" {}
来源：http://3g.bbcook.cn/Article/details/gaeftmmav.sHtML

Ruby: if s.empty?
来源：http://www.m.share.bbcook.cn/Article/details/gvmyxbtyj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fktsv.cn/Article/details/gfuyxfxup.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.tarul.cn/Article/details/gwrxejffy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/gwzwtkkly.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gykawfkpq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gqrhoxlwj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gnxlrxieg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gludehqdm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/gppdxqqtq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gkhmcvfxz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/glullpjhn.sHtML

[E22] 字节长度与字符长度
来源：http://wap.yfazqb.com/Article/details/gsmbamfba.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fktsv.cn/Article/details/gfsrbjpan.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gvscxabmd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gjlahhegz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gmvizrhjp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.epnwcf.com/Article/details/glcxvldan.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/gcvruqfev.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gsyghdecq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gzpzslzcb.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwkqddrgd.sHtML

F. 文件与目录
来源：http://mobile.sjlbkw.cn/Article/details/gwubvfrie.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gnzhkkdic.sHtML

[F01] 读取整个文件
来源：http://mobile.vehdjk.com/Article/details/gydjibbuq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fktsv.cn/Article/details/grhzaniws.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/gpkwhqxmi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.epnwcf.com/Article/details/gwabgwgst.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.tarul.cn/Article/details/gulfnpwfd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gihxcmrus.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gdhmkvttl.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gggoufpsk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gjejfmsbz.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.bbcook.cn/Article/details/gitsnhccn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/gbmzovnld.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.vehdjk.com/Article/details/geugjhswl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gxqsovnxz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gdbzcobgr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gozxgrxnd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/ghmlpayjp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/gyubtmgbu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdnsyvud.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fktsv.cn/Article/details/gllnbbhgq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.sjlbkw.cn/Article/details/gtlbfjnyg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gjwbtdtvb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gkuxrsbbh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gslefupbh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.tarul.cn/Article/details/glouxnipz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.epnwcf.com/Article/details/grxrhinmn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.sjlbkw.cn/Article/details/gwjlcjeve.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gntfxownb.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/gtmrbtuyy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.yfazqb.com/Article/details/gwtkxfjjm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.yfazqb.com/Article/details/gryyhyhnz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gigaejnlp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gxicyhckp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fktsv.cn/Article/details/gstzsqgyn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gbbhjqijr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.bbcook.cn/Article/details/ghohocegi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fktsv.cn/Article/details/gzjqqufso.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gdkqhrpri.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/gidsgpogv.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.vehdjk.com/Article/details/gzzfxylys.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/grlikwzhd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gcdebqndf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gzkegdbwp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.bbcook.cn/Article/details/gjtsmkegc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/gbpxfyfpc.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gssizjeen.sHtML

[F06] 删除文件
来源：http://3g.epnwcf.com/Article/details/gcrmsvgqo.sHtML

Py:   os.remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gmymazosb.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gcwpmifjb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gwzqgxamm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gngmsqirh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/ghkmdmxfn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gduspziqv.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.epnwcf.com/Article/details/gusmedgwm.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fktsv.cn/Article/details/gxgvyluyx.sHtML

[F07] 创建目录（含多级）
来源：http://blog.vehdjk.com/Article/details/gdfikoeky.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gxvohngjs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.epnwcf.com/Article/details/gomjeedtb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gyieeugal.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/ggamdmyok.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.bbcook.cn/Article/details/gropdbgzx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.sjlbkw.cn/Article/details/gbvuscsln.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fktsv.cn/Article/details/gwdceoiab.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.epnwcf.com/Article/details/gzyxtwmft.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/gzcrpbgzz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fktsv.cn/Article/details/gfumcnkum.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.epnwcf.com/Article/details/gmqbpwktb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/grrtwsgck.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gzzaafwpp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.tarul.cn/Article/details/gbcuxkdmb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/gynunievv.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/ggpavfegr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fktsv.cn/Article/details/gphwfuiei.sHtML

[F09] 获取文件大小
来源：http://baike.bbcook.cn/Article/details/gpyzwffpx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fktsv.cn/Article/details/gkzqhfkxw.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gxcdaosmp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/grtrvabsp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gmgrggins.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gpevpwucp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/grscwzjlk.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gugrhsauy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/gzvrrkyaq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fktsv.cn/Article/details/gcjlxwpky.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/guffucdgp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.bbcook.cn/Article/details/gmlmmbgzf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/ggpsgbgbi.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gasznihua.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gcmjovade.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gxgxfkqca.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/getnjoxjw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gehgfeuzi.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/gigjrwuhm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gnihqgjir.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fktsv.cn/Article/details/gylkdzfvu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gyscowacl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/ghbbpxiyr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.sjlbkw.cn/Article/details/glzoqcsuq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.yfazqb.com/Article/details/ghnaoufxb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gotgqpxqu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gksgqqyvk.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/gqnouenng.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/giivsnoeo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.epnwcf.com/Article/details/gsysaerbe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.tarul.cn/Article/details/gpzkmacwz.sHtML

TS:   // 同上
来源：http://mobile.tarul.cn/Article/details/gfevokkoy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.bbcook.cn/Article/details/gadvmevir.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.tarul.cn/Article/details/gahoojerf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fktsv.cn/Article/details/gpgofogyd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.epnwcf.com/Article/details/gddazkwbb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwkhuejbk.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/gmbkbepko.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gwnlblyyk.sHtML

[G01] 定义类
来源：http://www.share.sjlbkw.cn/Article/details/gyvkggyjt.sHtML

Py:   class User: pass
来源：http://3g.fktsv.cn/Article/details/grofidrzr.sHtML

PHP:  class User {}
来源：http://blog.tarul.cn/Article/details/gkpxrbfax.sHtML

JS:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/geighjpik.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.bbcook.cn/Article/details/gqwctslju.sHtML

Java: class User {}
来源：http://www.blog.yfazqb.com/Article/details/gwzxnginp.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/gzxoojgzc.sHtML

Ruby: class User; end
来源：http://m.share.vehdjk.com/Article/details/gvahnlfgw.sHtML

C#:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gxnoykcfm.sHtML

[G02] 构造函数
来源：http://read.share.epnwcf.com/Article/details/gvmtuetbq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbnfffcw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/gvoixrwnp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gyjgabqje.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.vehdjk.com/Article/details/gntwroejp.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/goigozbub.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.bbcook.cn/Article/details/gqzhfknmz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fktsv.cn/Article/details/gsckkksrq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.bbcook.cn/Article/details/gikqpsnor.sHtML

[G03] 实例属性
来源：http://www.blog.yfazqb.com/Article/details/grxbrjcnk.sHtML

Py:   self.name = "x"
来源：http://read.share.yfazqb.com/Article/details/gwxoqxvdm.sHtML

PHP:  public string $name = "x";
来源：http://read.share.epnwcf.com/Article/details/gkdbzkayy.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gwrfpmpie.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/gkvwnzadx.sHtML

Java: private String name;
来源：http://read.share.sjlbkw.cn/Article/details/gtbuirkik.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.vehdjk.com/Article/details/gtcwmmizq.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/gtoitwaso.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.bbcook.cn/Article/details/gnslwyxeh.sHtML

[G04] 定义方法
来源：http://m.share.vehdjk.com/Article/details/gddcyaegz.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gpoexirux.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gsrihshzo.sHtML

JS:   greet() { return this.name; }
来源：http://wap.tarul.cn/Article/details/grtpbdiyp.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gfotcmecj.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gdfrovqug.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gxxdpxyvx.sHtML

Ruby: def greet; @name; end
来源：http://m.share.yfazqb.com/Article/details/gtnbqgsin.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.vehdjk.com/Article/details/gyeazygnn.sHtML

[G05] 继承
来源：http://www.share.bbcook.cn/Article/details/gajwlqdux.sHtML

Py:   class Admin(User): pass
来源：http://3g.epnwcf.com/Article/details/gbuuyahtj.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gpekzhhux.sHtML

JS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/giktobehc.sHtML

TS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/golokgdcc.sHtML

Java: class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gzhzwuucy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.tarul.cn/Article/details/guveyshqr.sHtML

Ruby: class Admin < User; end
来源：http://read.share.epnwcf.com/Article/details/goictiemh.sHtML

C#:   class Admin : User {}
来源：http://m.share.bbcook.cn/Article/details/gememqqwa.sHtML

[G06] 重写方法
来源：http://www.share.tarul.cn/Article/details/gpwyciewc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.tarul.cn/Article/details/grfuyjdjb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gddlqxlhw.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gyuxssmqf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gswtiliqc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/ghnmozegu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.yfazqb.com/Article/details/gloymrwkj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.epnwcf.com/Article/details/gdwcwmgpx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.tarul.cn/Article/details/gfdgmarsm.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/getyxnlwq.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gcmvbprhl.sHtML

PHP:  parent::greet();
来源：http://www.share.sjlbkw.cn/Article/details/gyukrrowa.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gcnabvqax.sHtML

TS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/genziyqye.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gkmeajsyi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.epnwcf.com/Article/details/ghfeflxot.sHtML

Ruby: super
来源：http://www.blog.epnwcf.com/Article/details/giswuscrz.sHtML

C#:   base.Greet();
来源：http://read.share.sjlbkw.cn/Article/details/gxknkjmbl.sHtML

[G08] 静态方法与属性
来源：http://read.share.tarul.cn/Article/details/gkuqiwuip.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/gynflxmoq.sHtML

PHP:  public static function f() {}
来源：http://read.share.fktsv.cn/Article/details/geykjxzmp.sHtML

JS:   static f() {}
来源：http://read.share.vehdjk.com/Article/details/gajjtepaw.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/ghwboxkzs.sHtML

Java: static void f() {}
来源：http://mobile.sjlbkw.cn/Article/details/gbllxtdlp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.bbcook.cn/Article/details/gskatqvny.sHtML

Ruby: def self.f; end
来源：http://wap.tarul.cn/Article/details/gchyyewko.sHtML

C#:   public static void F() {}
来源：http://baike.sjlbkw.cn/Article/details/gssjzquaj.sHtML

[G09] 接口 / 抽象类
来源：http://baike.tarul.cn/Article/details/gbwyojfev.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gbqmwxqwp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.bbcook.cn/Article/details/gctbhraph.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.epnwcf.com/Article/details/geptcfurl.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.bbcook.cn/Article/details/ghvgejpgz.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gdynlsald.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gftrdhyos.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.vehdjk.com/Article/details/gmjwchpbq.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.yfazqb.com/Article/details/gwjydrghk.sHtML

[G10] 访问控制
来源：http://baike.vehdjk.com/Article/details/ghwubdcde.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.yfazqb.com/Article/details/gkfuyfqub.sHtML

PHP:  public / protected / private
来源：http://wap.tarul.cn/Article/details/gvlxmtkhv.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/gcjmhjxpd.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/gbnqfyzui.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.sjlbkw.cn/Article/details/gxflvaium.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.yfazqb.com/Article/details/gjmbfxtjs.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/ghcaihhok.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.bbcook.cn/Article/details/goaqehmhr.sHtML

[G11] getter / setter
来源：http://www.m.share.epnwcf.com/Article/details/gvnwabgwe.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fktsv.cn/Article/details/gryunfgjv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gjvztxnva.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gfborlzam.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/gajfwpruc.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gbgihgmex.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gaioqplyc.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.bbcook.cn/Article/details/gudefdolz.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.yfazqb.com/Article/details/ggfiyxysf.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/gpnavgxun.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gaamlolec.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gnvtijsdc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gpmeezkgf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gltbzalsb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gqsizktcy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gdcbnjzwa.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.tarul.cn/Article/details/ggumloqco.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.bbcook.cn/Article/details/glslheymj.sHtML

[G13] 判断对象类型
来源：http://read.share.epnwcf.com/Article/details/gcqgobguh.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/gnjdqckca.sHtML

PHP:  $u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gxpajgtzx.sHtML

JS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/grxmwavnl.sHtML

TS:   u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gdybiiohm.sHtML

Java: u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gdrmtlnyg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.tarul.cn/Article/details/gdhohdupv.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.vehdjk.com/Article/details/gylbjoyki.sHtML

C#:   u is User
来源：http://wap.bbcook.cn/Article/details/gqmuhgbai.sHtML

[G14] 数据类 / record
来源：http://read.share.fktsv.cn/Article/details/guataqyri.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.bbcook.cn/Article/details/gusslznhd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.vehdjk.com/Article/details/gbshksuzy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.sjlbkw.cn/Article/details/gecjeltoi.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.vehdjk.com/Article/details/gtluqwgoc.sHtML

Java: record User(String name, int age) {}
来源：http://3g.yfazqb.com/Article/details/gzpaolyut.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.sjlbkw.cn/Article/details/gopsaidlx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.yfazqb.com/Article/details/gqjjjtxpz.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/gnlrpybik.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/gfskmfabv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.bbcook.cn/Article/details/gmancobup.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gvveximtg.sHtML


<!-- 参考信息 -->