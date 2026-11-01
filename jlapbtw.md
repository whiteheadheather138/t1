代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.yfazqb.com/Article/details/gvhxuheen.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/gtmzaflzn.sHtML

[E16] 数字千分位
来源：http://blog.epnwcf.com/Article/details/girlmobve.sHtML

Py:   f"{1234567:,}"
来源：http://baike.yfazqb.com/Article/details/gikkzshoi.sHtML

PHP:  number_format(1234567);
来源：http://wap.vehdjk.com/Article/details/gezqlttoy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gklwfbghf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/gznltfeio.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gvdjkqxxe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.vehdjk.com/Article/details/gizplolnw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/ghvchxbjy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.epnwcf.com/Article/details/gjfexiocd.sHtML

[E17] 首字母大写
来源：http://mobile.fktsv.cn/Article/details/geabrblrd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gvgwqrnaa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.sjlbkw.cn/Article/details/gawtofkxg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/ghpfnsrob.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gbhyrmeah.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.vehdjk.com/Article/details/gnhvjzzbx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.yfazqb.com/Article/details/ghejutooc.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gxieofias.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.tarul.cn/Article/details/gplfzouxq.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gkdllazez.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.vehdjk.com/Article/details/guaxqasjz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.yfazqb.com/Article/details/gtanzzswq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gbsseddyr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/glwdedxlt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.vehdjk.com/Article/details/ghxpznkqm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gebplfcek.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.sjlbkw.cn/Article/details/gvbubvarx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.epnwcf.com/Article/details/ggzjuzobt.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/gxpxiyqzd.sHtML

Py:   s.splitlines()
来源：http://www.blog.yfazqb.com/Article/details/gudmmyvbn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fktsv.cn/Article/details/gqqhosrql.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/guhzubhgv.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gffykunso.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/goacbsgzj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gtaqmnwdf.sHtML

Ruby: s.lines
来源：http://3g.epnwcf.com/Article/details/gkozkxqiv.sHtML

C#:   s.Split('\n')
来源：http://www.blog.bbcook.cn/Article/details/gpwylycun.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.vehdjk.com/Article/details/gxapzfook.sHtML

Py:   if not s:
来源：http://read.share.tarul.cn/Article/details/ggrauncvy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.bbcook.cn/Article/details/gixmmhuin.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.sjlbkw.cn/Article/details/ghkrazayh.sHtML

TS:   if (s === "") {}
来源：http://m.share.fktsv.cn/Article/details/goellrbjm.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/geiobmguf.sHtML

Go:   if s == "" {}
来源：http://mobile.fktsv.cn/Article/details/gqzdjsrrn.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/gkwdqlunx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fktsv.cn/Article/details/gefkmqlvm.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fktsv.cn/Article/details/gpqgzzhgf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/gqggsacws.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gttjqvkpg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gddcszoog.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gfaarcmlq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gurnfbvee.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.sjlbkw.cn/Article/details/gvkgpqsek.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gsoqmzncn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gafwxaccm.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gtdnigfsm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzxhkcco.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gfehriauf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gebquibes.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gpingwhdq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.epnwcf.com/Article/details/gbrmpnqsy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.vehdjk.com/Article/details/greahqaxb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gxncadtcf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.epnwcf.com/Article/details/gzhynewoo.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gyfwjjsph.sHtML

F. 文件与目录
来源：http://3g.fktsv.cn/Article/details/gftovkoyf.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gcvpxxxjw.sHtML

[F01] 读取整个文件
来源：http://blog.sjlbkw.cn/Article/details/ghvrjoalj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.sjlbkw.cn/Article/details/gznmjahki.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gwudmohwd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/gosqtffnv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.yfazqb.com/Article/details/gfbgmexud.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gfsywvcaj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gqjdajcbh.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.yfazqb.com/Article/details/ggczxwwyj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gabldwogw.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/ggagycjjq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.bbcook.cn/Article/details/gcjnctgdc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/gdlndyrbb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gwgkehzse.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gdgmdefit.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/ggwxzregq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.epnwcf.com/Article/details/gucoztasm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.vehdjk.com/Article/details/geiqqmlqf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fktsv.cn/Article/details/gdxggaefi.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gsytoqnrp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.epnwcf.com/Article/details/gjgdbecfj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/gburwosaa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/golbegmrb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gosyjbqvq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.yfazqb.com/Article/details/gzrvrzqnm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.bbcook.cn/Article/details/gmgxymmhu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.epnwcf.com/Article/details/gdhxmvlzn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gqhbrsrvf.sHtML

[F04] 追加写入文件
来源：http://www.blog.bbcook.cn/Article/details/gudiegtal.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.tarul.cn/Article/details/gsqzwlxta.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.bbcook.cn/Article/details/gqqphckuv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gghxhriuv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gwnoeszlr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fktsv.cn/Article/details/gxdkwwaea.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.yfazqb.com/Article/details/gmezllpkg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fktsv.cn/Article/details/gvnpmlfyu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.tarul.cn/Article/details/guzfzfwsr.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.tarul.cn/Article/details/gqymljdba.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.sjlbkw.cn/Article/details/gdvtepebl.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.vehdjk.com/Article/details/gfzsksrxc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gmozanfal.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/ggmlsmqav.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gpkubesrf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fktsv.cn/Article/details/geawdqxxz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ggawswuve.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/gqgzyxboa.sHtML

[F06] 删除文件
来源：http://www.share.sjlbkw.cn/Article/details/gqytsvlew.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqcnirhsl.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gyxicaize.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gnghrccmu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gdojfjbcu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gpxwlqfpg.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gjeypmxnc.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gynullnel.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.tarul.cn/Article/details/gvnjdmroc.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.tarul.cn/Article/details/gpuyfuuba.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gfwkpujmk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/gstsvgbfe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/guozbmukr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gthlmmnxw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/gtwbptpgp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.vehdjk.com/Article/details/gvabwzkbn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.bbcook.cn/Article/details/gwddolpct.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/gkifmpfis.sHtML

[F08] 遍历目录
来源：http://wap.vehdjk.com/Article/details/gkliypwmw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gurnitrpc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/ggzbzzfps.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gxbpdozyf.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/ggysflpum.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbiclutkx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/gptghoujn.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fktsv.cn/Article/details/gipupxyks.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.epnwcf.com/Article/details/gdqtnwakc.sHtML

[F09] 获取文件大小
来源：http://mobile.tarul.cn/Article/details/gafqbhjbq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gpevinsts.sHtML

PHP:  filesize("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gkzigjqox.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/glnpvtooa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gbhdrjjqq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gyjjgsdol.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.bbcook.cn/Article/details/gkbscnssw.sHtML

Ruby: File.size("a.txt")
来源：http://wap.bbcook.cn/Article/details/gmekajfee.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.bbcook.cn/Article/details/gsuqcyohh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/gzrzlgxqz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gzvnvzcgt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.yfazqb.com/Article/details/gzwpbrbhc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gpfykjvfo.sHtML

TS:   path.extname("a.txt")
来源：http://3g.epnwcf.com/Article/details/gntlgwakw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.epnwcf.com/Article/details/gkmzynhov.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ginxeezeg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gztttcgzg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gelydjjzn.sHtML

[F11] 复制与移动文件
来源：http://www.share.vehdjk.com/Article/details/gvzpnliqf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/glmkjahzl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gmyxgldcg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/geivjmfol.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gnxbhvjuo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.sjlbkw.cn/Article/details/garyzulxz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.vehdjk.com/Article/details/gljldcyoj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gpfdqxkpa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.vehdjk.com/Article/details/gvhuqycdt.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/gemgktsfj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/gxeswayln.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/gmnaderiw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.yfazqb.com/Article/details/gunjdwkkz.sHtML

TS:   // 同上
来源：http://read.share.epnwcf.com/Article/details/gfrorqrhk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.yfazqb.com/Article/details/gfxjmmrxb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.vehdjk.com/Article/details/gpbtnjemh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fktsv.cn/Article/details/gwfgdhspi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/gzkbvzpcw.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdrgaszht.sHtML

G. 面向对象
来源：http://wap.epnwcf.com/Article/details/gsqgidphq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/giyqbckku.sHtML

[G01] 定义类
来源：http://3g.tarul.cn/Article/details/gnrvmzkty.sHtML

Py:   class User: pass
来源：http://www.blog.yfazqb.com/Article/details/gpholnysy.sHtML

PHP:  class User {}
来源：http://wap.yfazqb.com/Article/details/gjqlysgcq.sHtML

JS:   class User {}
来源：http://baike.fktsv.cn/Article/details/gaprnkcyw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gocwrecrt.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/giayzyuey.sHtML

Go:   type User struct { Name string }
来源：http://wap.tarul.cn/Article/details/gknpznixf.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/glbstpreg.sHtML

C#:   class User {}
来源：http://baike.epnwcf.com/Article/details/giliytrxo.sHtML

[G02] 构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gydozvhwu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.epnwcf.com/Article/details/ggcipnmbp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fktsv.cn/Article/details/gasglakji.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gtqgsnibz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdzsfvbil.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gyohizpxl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.tarul.cn/Article/details/gndjztweq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.epnwcf.com/Article/details/gmerqaqvt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/glkgxunop.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/glxnbsjiv.sHtML

Py:   self.name = "x"
来源：http://blog.tarul.cn/Article/details/gzytivewi.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/ghwmsswfg.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gdarfvjfn.sHtML

TS:   name: string = "x";
来源：http://www.share.tarul.cn/Article/details/gtqciuzmd.sHtML

Java: private String name;
来源：http://www.m.share.fktsv.cn/Article/details/gpkjubzsj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.epnwcf.com/Article/details/gynidiyzx.sHtML

Ruby: @name = "x"
来源：http://m.share.yfazqb.com/Article/details/gbqqfvkoh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.bbcook.cn/Article/details/gciiugysc.sHtML

[G04] 定义方法
来源：http://3g.tarul.cn/Article/details/glrpvlumg.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gphobeirq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gqnsuvlka.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/glqaqbuww.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gmfegnwum.sHtML

Java: String greet() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/glyizpgcp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gbzbshicn.sHtML

Ruby: def greet; @name; end
来源：http://baike.vehdjk.com/Article/details/gmxkpwgpo.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.epnwcf.com/Article/details/guezhlixn.sHtML

[G05] 继承
来源：http://read.share.vehdjk.com/Article/details/ggoocuwhk.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.epnwcf.com/Article/details/gjpnieiva.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gaxrrmprg.sHtML

JS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/grjqqeqih.sHtML

TS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gjmdficwn.sHtML

Java: class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gasoqjrxg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/girendfqa.sHtML

Ruby: class Admin < User; end
来源：http://mobile.bbcook.cn/Article/details/grgsobykh.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.yfazqb.com/Article/details/ggifofhsd.sHtML

[G06] 重写方法
来源：http://wap.bbcook.cn/Article/details/gpoetynmh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fktsv.cn/Article/details/gedzajhko.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gstelfodf.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gyeuzfhzf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gxswwmkmn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gotdyluac.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.vehdjk.com/Article/details/gheutfora.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fktsv.cn/Article/details/gpdkpygqc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.tarul.cn/Article/details/gcmkbjdbb.sHtML

[G07] 调用父类方法
来源：http://www.m.share.bbcook.cn/Article/details/gihxaeoth.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/giykxznbu.sHtML

PHP:  parent::greet();
来源：http://mobile.sjlbkw.cn/Article/details/gyozsnleq.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gknvvpgzl.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gsrzcklsp.sHtML

Java: super.greet();
来源：http://www.m.share.tarul.cn/Article/details/ggunqmqip.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.bbcook.cn/Article/details/gchlhgiwr.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmjjzbvz.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/gigicgwha.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/gytzbowdn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.tarul.cn/Article/details/gogvuvhni.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/ghnzufaqf.sHtML

JS:   static f() {}
来源：http://www.blog.epnwcf.com/Article/details/gdkyeggnb.sHtML

TS:   static f(): void {}
来源：http://wap.vehdjk.com/Article/details/gfwjvsjwf.sHtML

Java: static void f() {}
来源：http://read.share.bbcook.cn/Article/details/gkbpkddng.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fktsv.cn/Article/details/giehumshh.sHtML

Ruby: def self.f; end
来源：http://mobile.bbcook.cn/Article/details/gskgisuje.sHtML

C#:   public static void F() {}
来源：http://baike.sjlbkw.cn/Article/details/gvmmtgbpa.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fktsv.cn/Article/details/gbaackqhs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.yfazqb.com/Article/details/gjdtdkloc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.epnwcf.com/Article/details/gueenoupy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzpbdsvm.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.bbcook.cn/Article/details/gbtannygy.sHtML

Java: interface Shape { double area(); }
来源：http://wap.yfazqb.com/Article/details/gqkbpukjz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fktsv.cn/Article/details/gvlgrpkdn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.sjlbkw.cn/Article/details/gvqqafrie.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.epnwcf.com/Article/details/ggztjeynq.sHtML

[G10] 访问控制
来源：http://3g.sjlbkw.cn/Article/details/gjgiahljs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.epnwcf.com/Article/details/gukrjfyei.sHtML

PHP:  public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gczumlvjq.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/gnxfblpwq.sHtML

TS:   public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gvorjstcj.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.tarul.cn/Article/details/gudaxoznb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.yfazqb.com/Article/details/gkhyauyzd.sHtML

Ruby: public / protected / private
来源：http://m.share.bbcook.cn/Article/details/gubkotlsa.sHtML

C#:   public / protected / private / internal
来源：http://mobile.tarul.cn/Article/details/grzkqvrcu.sHtML

[G11] getter / setter
来源：http://3g.tarul.cn/Article/details/gxmghhvcs.sHtML

Py:   @property 与 @x.setter
来源：http://wap.sjlbkw.cn/Article/details/gzpvqnctk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gnijwihii.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.tarul.cn/Article/details/guvqqkpke.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gbtvndsnu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gurpaldzv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gpgpqyfor.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.tarul.cn/Article/details/gjxhznawy.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/gtvhellcw.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/gmenhihoo.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gnsjbobia.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gahuabdfg.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/ghtzkqhww.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gvmzsobkd.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/gxzecysmj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gbdofdiwx.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.vehdjk.com/Article/details/grvspwpsi.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gqyumcspw.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fktsv.cn/Article/details/gmkmjhvoo.sHtML

Py:   isinstance(u, User)
来源：http://read.share.bbcook.cn/Article/details/gieqoetak.sHtML

PHP:  $u instanceof User
来源：http://m.share.fktsv.cn/Article/details/goofrkxcs.sHtML

JS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gzlknkugi.sHtML

TS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/grpcgmixt.sHtML

Java: u instanceof User
来源：http://wap.bbcook.cn/Article/details/gntbqmnor.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.epnwcf.com/Article/details/gjxgnlmai.sHtML

Ruby: u.is_a?(User)
来源：http://3g.tarul.cn/Article/details/gwimgqose.sHtML

C#:   u is User
来源：http://www.m.share.fktsv.cn/Article/details/gnofujuxl.sHtML

[G14] 数据类 / record
来源：http://baike.epnwcf.com/Article/details/gisbnijgz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gzvxgdzkq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.yfazqb.com/Article/details/gvqrropgm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.sjlbkw.cn/Article/details/gbytcqpsv.sHtML


<!-- 参考信息 -->