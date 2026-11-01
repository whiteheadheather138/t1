代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fktsv.cn/Article/details/geirwlwlk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/gtuclstmi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gpscomhhj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gdemyvbcx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.bbcook.cn/Article/details/gjxfwibyt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/gfhfmjboh.sHtML

Ruby: s.capitalize
来源：http://read.share.fktsv.cn/Article/details/goedyuuyv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/gbxnueqmg.sHtML

[E18] 模板占位符替换
来源：http://www.share.epnwcf.com/Article/details/gepxbgwcx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.tarul.cn/Article/details/ggtsanmjj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.yfazqb.com/Article/details/ggtkgjbhf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gtapyolri.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gjhtldcxg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gztrhydmz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.epnwcf.com/Article/details/glhwqfulr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.vehdjk.com/Article/details/gnnewgvjt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.vehdjk.com/Article/details/geybuwskf.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.bbcook.cn/Article/details/gmcbzxfzm.sHtML

Py:   s.splitlines()
来源：http://www.share.vehdjk.com/Article/details/gkcaqpcez.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gcilmjxsd.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gcvjfkowt.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gznnykokg.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/gvkgoozey.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.epnwcf.com/Article/details/gynbnlhvt.sHtML

Ruby: s.lines
来源：http://blog.bbcook.cn/Article/details/gaceevdwa.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.epnwcf.com/Article/details/gfzooruze.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/gfhygqacn.sHtML

Py:   if not s:
来源：http://www.m.share.fktsv.cn/Article/details/guugsmcqr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.vehdjk.com/Article/details/gvlafzikr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.vehdjk.com/Article/details/gvuvkyhlt.sHtML

TS:   if (s === "") {}
来源：http://wap.epnwcf.com/Article/details/gpxnsebfc.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gozmqhacd.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/gejejbivf.sHtML

Ruby: if s.empty?
来源：http://blog.fktsv.cn/Article/details/gatnnsfsd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gdbeixzeo.sHtML

[E21] 超长截断加省略号
来源：http://wap.yfazqb.com/Article/details/gwrrkekhb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/gxllabfpj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/giktviivp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/ghyqlzvzp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gdyzfognl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gqcsdsmdo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.epnwcf.com/Article/details/gdomksryo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gxxgdatxh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gmjxzhjzs.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.yfazqb.com/Article/details/gjwirqtxd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.bbcook.cn/Article/details/gdsufddcf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gtjvnaeuc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gbwxaomcl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gkafwkaig.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.yfazqb.com/Article/details/gyzsazpgu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/gnlclmcre.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.yfazqb.com/Article/details/gailgiryf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.vehdjk.com/Article/details/gnyuducbt.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gxovbyaol.sHtML

F. 文件与目录
来源：http://www.share.epnwcf.com/Article/details/gjftdbsnd.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gpdkxedsk.sHtML

[F01] 读取整个文件
来源：http://wap.yfazqb.com/Article/details/gamrxgunu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.sjlbkw.cn/Article/details/gxqaldxmu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gwtruxkbe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.tarul.cn/Article/details/gwycxtqku.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.yfazqb.com/Article/details/gbrzurnla.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gpojrjqjo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.epnwcf.com/Article/details/gqjmwsmhg.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gaknfoksx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.vehdjk.com/Article/details/ghfqswrgh.sHtML

[F02] 逐行读取文件
来源：http://www.blog.tarul.cn/Article/details/glaibukja.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.sjlbkw.cn/Article/details/galczhoxs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fktsv.cn/Article/details/gislocgkg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gwdejedww.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gpmzptafr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/gahrxjwpg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/gihvercgd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.bbcook.cn/Article/details/gxpvsztwa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.yfazqb.com/Article/details/gowoitrqr.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/glhdiolgq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.bbcook.cn/Article/details/gexyclivh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gdqvsygni.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gypriimre.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/glzkrkvcb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.yfazqb.com/Article/details/gslvlfdwg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.yfazqb.com/Article/details/gzevspufd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.vehdjk.com/Article/details/gzsoyfihp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gvfswvtfp.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gxjvseinr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.tarul.cn/Article/details/gvolrjuqp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/ghmwxknpn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/ganovhxyq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gnvbfrkru.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/gnechdgbw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.tarul.cn/Article/details/gbahqjxkh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.vehdjk.com/Article/details/gxzewqdhg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.vehdjk.com/Article/details/goyyityle.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gabcgrtrl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.bbcook.cn/Article/details/gsqhehrqs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.tarul.cn/Article/details/ghczwmgvs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gmowoyhsh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gpoeivpws.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gkizcszxe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.sjlbkw.cn/Article/details/galtrntpt.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gtzoopngv.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gznnaplbj.sHtML

[F06] 删除文件
来源：http://mobile.tarul.cn/Article/details/givxvznxb.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gjisbwmpl.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gzhkwclzu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gyfkwxgqg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gvkiyavxm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gdgkcyoiw.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gkztgpmgz.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.epnwcf.com/Article/details/gsbkjnizf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gfxrwvkds.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.tarul.cn/Article/details/gplzuetkk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/gxlovynns.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.sjlbkw.cn/Article/details/gzbutkiqo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gzjemlrry.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/ggerxqmuj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.epnwcf.com/Article/details/gcchmpghk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.sjlbkw.cn/Article/details/gfxizbjsm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.tarul.cn/Article/details/gqtvglepf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.tarul.cn/Article/details/gikukvhgn.sHtML

[F08] 遍历目录
来源：http://mobile.tarul.cn/Article/details/gpmzpihfv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.epnwcf.com/Article/details/ggjtaofwe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.sjlbkw.cn/Article/details/gdjoicnsi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqdzioge.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gsioheele.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/gsmcoyfjr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gzvxkxcih.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/grsivdejl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gdmdxicel.sHtML

[F09] 获取文件大小
来源：http://read.share.yfazqb.com/Article/details/gmrlvouex.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gsbsmlqdz.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gbkqasqvd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gupnwqhbt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gfqdbkzie.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gzvzczvhr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gnenixgwf.sHtML

Ruby: File.size("a.txt")
来源：http://blog.bbcook.cn/Article/details/gwcitehdm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.yfazqb.com/Article/details/grmuewmmi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.bbcook.cn/Article/details/gcmzhvymb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gbcfekqrd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/gqrusncaa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/ggqfotuxl.sHtML

TS:   path.extname("a.txt")
来源：http://blog.yfazqb.com/Article/details/ghcwrcdlj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gknpqaanj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwkrbfspe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gqaguymwk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gncxjgktb.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gssknsdwd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gmuiuifih.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.vehdjk.com/Article/details/gprnisvzm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gsqwmxlqb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjjovnkyn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.bbcook.cn/Article/details/gmifvgrvi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.epnwcf.com/Article/details/gjuooothh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gppvfijxn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.vehdjk.com/Article/details/gscgdzwni.sHtML

[F12] CSV 读写
来源：http://3g.bbcook.cn/Article/details/goyvvocai.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fktsv.cn/Article/details/gmteaclaq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.epnwcf.com/Article/details/gxwyowjmc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.tarul.cn/Article/details/ggwrtnzvc.sHtML

TS:   // 同上
来源：http://wap.fktsv.cn/Article/details/gtieniczh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.epnwcf.com/Article/details/gzthknllh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.bbcook.cn/Article/details/gxnixvwvs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.yfazqb.com/Article/details/gueevnyeb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fktsv.cn/Article/details/giunkluvw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxatttpvd.sHtML

G. 面向对象
来源：http://www.m.share.epnwcf.com/Article/details/gnkuuavqq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gskkzwadv.sHtML

[G01] 定义类
来源：http://mobile.fktsv.cn/Article/details/gzsiuwgux.sHtML

Py:   class User: pass
来源：http://read.share.epnwcf.com/Article/details/gewmstbie.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gzayhalba.sHtML

JS:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gbjeyrivb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/gbgbnnxzn.sHtML

Java: class User {}
来源：http://wap.fktsv.cn/Article/details/gsguqqspu.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/gmrhgbvlu.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/gvuzlefbb.sHtML

C#:   class User {}
来源：http://wap.fktsv.cn/Article/details/giuooccdq.sHtML

[G02] 构造函数
来源：http://mobile.fktsv.cn/Article/details/gyblffjwl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.vehdjk.com/Article/details/ghcpfkndu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/gqvkalqwd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gqzytfyqn.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.yfazqb.com/Article/details/gfbdvyghd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/glijmbxpq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.yfazqb.com/Article/details/gzahuenyl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fktsv.cn/Article/details/gprilrche.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.epnwcf.com/Article/details/gxdzabkeg.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/guhmuaeas.sHtML

Py:   self.name = "x"
来源：http://wap.vehdjk.com/Article/details/ghofmrnkq.sHtML

PHP:  public string $name = "x";
来源：http://blog.fktsv.cn/Article/details/glkpyqwge.sHtML

JS:   this.name = "x";
来源：http://wap.tarul.cn/Article/details/gxtppttcz.sHtML

TS:   name: string = "x";
来源：http://m.share.epnwcf.com/Article/details/gukvyruch.sHtML

Java: private String name;
来源：http://wap.epnwcf.com/Article/details/gysscwmuv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fktsv.cn/Article/details/gllayrism.sHtML

Ruby: @name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gpbcysdxu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fktsv.cn/Article/details/gdjoigwpu.sHtML

[G04] 定义方法
来源：http://www.share.sjlbkw.cn/Article/details/guekrftqg.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gsiunecos.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/ggkybrbqv.sHtML

JS:   greet() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gnrkmaedj.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gvklhocic.sHtML

Java: String greet() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gjcnnmdli.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gegvychen.sHtML

Ruby: def greet; @name; end
来源：http://wap.fktsv.cn/Article/details/gqpmdlsth.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/giizenkpy.sHtML

[G05] 继承
来源：http://read.share.yfazqb.com/Article/details/gdwueyxtv.sHtML

Py:   class Admin(User): pass
来源：http://www.share.tarul.cn/Article/details/gncxstigb.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gtoytwydx.sHtML

JS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gisltcpat.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gmlkijeul.sHtML

Java: class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gvervmjgu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/ghtitpxvg.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/gxddtjylx.sHtML

C#:   class Admin : User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfpronunr.sHtML

[G06] 重写方法
来源：http://3g.fktsv.cn/Article/details/gywekrxnb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.vehdjk.com/Article/details/gsihexivt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gpsoiftpl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gpqfuqhno.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/glpzxytkq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gtgsystvs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.epnwcf.com/Article/details/gcxlbucdu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.bbcook.cn/Article/details/glwupxdpp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.epnwcf.com/Article/details/gigemzian.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/gxbuujznw.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/gfyfsqzom.sHtML

PHP:  parent::greet();
来源：http://www.blog.fktsv.cn/Article/details/gssgpxcku.sHtML

JS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gwbonbrvw.sHtML

TS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gokghfnqh.sHtML

Java: super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gdswumnut.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.epnwcf.com/Article/details/gveblzfst.sHtML

Ruby: super
来源：http://read.share.bbcook.cn/Article/details/glzjywtja.sHtML

C#:   base.Greet();
来源：http://baike.epnwcf.com/Article/details/gujmnxcbg.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/ggipsjnly.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.bbcook.cn/Article/details/gklotzkch.sHtML

PHP:  public static function f() {}
来源：http://baike.fktsv.cn/Article/details/gxvwiwqxs.sHtML

JS:   static f() {}
来源：http://baike.sjlbkw.cn/Article/details/gtdqsljlh.sHtML

TS:   static f(): void {}
来源：http://mobile.epnwcf.com/Article/details/gadwfhtah.sHtML

Java: static void f() {}
来源：http://3g.vehdjk.com/Article/details/gijblwmsh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.sjlbkw.cn/Article/details/grhaanqyw.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/gshflliwt.sHtML

C#:   public static void F() {}
来源：http://mobile.bbcook.cn/Article/details/gvhugqmhl.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/gbdqvmotm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fktsv.cn/Article/details/gglvykrbf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.yfazqb.com/Article/details/gzejlxvqv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/glcszsjti.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.vehdjk.com/Article/details/gibpavdpt.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/gapalsfgq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gisvqczyy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/girnuesni.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gaiulbbcn.sHtML

[G10] 访问控制
来源：http://mobile.tarul.cn/Article/details/gkbcpwkqg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.sjlbkw.cn/Article/details/ggavydkyd.sHtML

PHP:  public / protected / private
来源：http://mobile.tarul.cn/Article/details/gflqircze.sHtML

JS:   #private 字段；其余公开
来源：http://baike.sjlbkw.cn/Article/details/gfhvvujaw.sHtML

TS:   public / protected / private
来源：http://read.share.yfazqb.com/Article/details/giwqkxnrj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.bbcook.cn/Article/details/gxyuojljn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fktsv.cn/Article/details/gcfenietb.sHtML

Ruby: public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gdxheeeen.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fktsv.cn/Article/details/gvwomevqv.sHtML

[G11] getter / setter
来源：http://read.share.tarul.cn/Article/details/gtdxnfzxm.sHtML

Py:   @property 与 @x.setter
来源：http://3g.yfazqb.com/Article/details/gxlrojfsc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gkeoqoxek.sHtML

JS:   get name() { return this._name; }
来源：http://baike.epnwcf.com/Article/details/gwrwllmov.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/gdtmwlamh.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gnrscfwbk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gecqkfmfa.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/gdklvymwh.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.epnwcf.com/Article/details/gsjqeucdd.sHtML

[G12] 对象转字符串
来源：http://baike.fktsv.cn/Article/details/gsvugqfgh.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/gwlqktvjs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/ggbrjiqte.sHtML

JS:   toString() { return this.name; }
来源：http://wap.tarul.cn/Article/details/gzozzmkol.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gsaljokyy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gidgggsjz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/glciyrgna.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fktsv.cn/Article/details/gguwrxtzl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gsfqxhqjc.sHtML

[G13] 判断对象类型
来源：http://m.share.fktsv.cn/Article/details/gbndmjnvk.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/gtznntbyt.sHtML

PHP:  $u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gtbkpvvuq.sHtML

JS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/grzvftdev.sHtML

TS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gibxkdxpy.sHtML

Java: u instanceof User
来源：http://baike.yfazqb.com/Article/details/gztybhecr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.sjlbkw.cn/Article/details/giaugkiwl.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fktsv.cn/Article/details/gmyamsrhi.sHtML

C#:   u is User
来源：http://3g.sjlbkw.cn/Article/details/gaaawrano.sHtML

[G14] 数据类 / record
来源：http://3g.sjlbkw.cn/Article/details/gkjozvukb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.vehdjk.com/Article/details/grmatbcwd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.vehdjk.com/Article/details/gvhscntlc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fktsv.cn/Article/details/gkfupcnnl.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fktsv.cn/Article/details/gkrqttbzt.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.tarul.cn/Article/details/ghufgsbfk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.tarul.cn/Article/details/gitysoriz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.sjlbkw.cn/Article/details/gcgyycaja.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.tarul.cn/Article/details/gaeyzmszr.sHtML

[G15] 枚举
来源：http://www.share.vehdjk.com/Article/details/gjunnbivc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fktsv.cn/Article/details/gqmyafdvp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.vehdjk.com/Article/details/ghsgqjbvr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.bbcook.cn/Article/details/gxlojebuw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gvobcsuce.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/gffvlhtds.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.epnwcf.com/Article/details/gddaxdsvn.sHtML


<!-- 参考信息 -->