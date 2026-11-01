代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.bbcook.cn/Article/details/gfhuqpazq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.bbcook.cn/Article/details/gdcdzdmkc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.bbcook.cn/Article/details/gudbkjhsq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.tarul.cn/Article/details/grsgjcdoc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gvlybueyt.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.epnwcf.com/Article/details/grvkozpwo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.epnwcf.com/Article/details/gfjnpaxns.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gkcyjrsnu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.epnwcf.com/Article/details/gcfudmkvq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.yfazqb.com/Article/details/gwqncjvlx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.bbcook.cn/Article/details/gqhicratg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fktsv.cn/Article/details/gmthejxoa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/gkdmiosyu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fktsv.cn/Article/details/gxahzdvik.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/gqlmcnizu.sHtML

Py:   f"{1234567:,}"
来源：http://3g.vehdjk.com/Article/details/gebbdhihj.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/gjprvgdwh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/gcnfhhsqw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gdqbtqwyg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.epnwcf.com/Article/details/ggepcbpby.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.yfazqb.com/Article/details/glvkpqkbx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.sjlbkw.cn/Article/details/gohuspoht.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.epnwcf.com/Article/details/gzoaymhbc.sHtML

[E17] 首字母大写
来源：http://wap.fktsv.cn/Article/details/gusukdcgo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.sjlbkw.cn/Article/details/gmjnatcbg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.yfazqb.com/Article/details/ggrloiukh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/gsaseqowf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gplokqdxa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.tarul.cn/Article/details/gkkwgfqep.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.yfazqb.com/Article/details/gvayialbd.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gxcaydzca.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/gjdkvvhlz.sHtML

[E18] 模板占位符替换
来源：http://wap.epnwcf.com/Article/details/gxnhkuhhx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.yfazqb.com/Article/details/gvfbvnspw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.tarul.cn/Article/details/gqtsgnrro.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/glrzeuxyx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gocnudpcb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.tarul.cn/Article/details/gifqetvgb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.vehdjk.com/Article/details/ggexgvgtc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.sjlbkw.cn/Article/details/gpbkiludh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.yfazqb.com/Article/details/gycasifux.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.tarul.cn/Article/details/geuuatdqx.sHtML

Py:   s.splitlines()
来源：http://blog.tarul.cn/Article/details/gghogpebw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gvdjrxvup.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gogshzzvf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gqgqpajav.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/grxsjjbmm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.sjlbkw.cn/Article/details/ggnzunhaz.sHtML

Ruby: s.lines
来源：http://wap.sjlbkw.cn/Article/details/gcliefoii.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/gtexkepfu.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.yfazqb.com/Article/details/grldhmjvj.sHtML

Py:   if not s:
来源：http://www.blog.fktsv.cn/Article/details/gmityngsz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.sjlbkw.cn/Article/details/ghhjuvyfs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fktsv.cn/Article/details/gseeupukw.sHtML

TS:   if (s === "") {}
来源：http://read.share.fktsv.cn/Article/details/gjmtbqwwc.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gntenhcyf.sHtML

Go:   if s == "" {}
来源：http://baike.vehdjk.com/Article/details/gvpfxveut.sHtML

Ruby: if s.empty?
来源：http://wap.sjlbkw.cn/Article/details/gykulncsh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/gtpcsxzsb.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fktsv.cn/Article/details/gsjpshomz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.sjlbkw.cn/Article/details/ghnuwmhof.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gchpjkmmq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gqymebaov.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gkggqixkm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gevsriebh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.vehdjk.com/Article/details/gxorsbdks.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gnfdswcoo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/gnqmwxrar.sHtML

[E22] 字节长度与字符长度
来源：http://blog.tarul.cn/Article/details/gbpezifvy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fktsv.cn/Article/details/gdzjfeeik.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gmdvvixdj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/ggwgazaji.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gjupdavbs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.bbcook.cn/Article/details/gjelhizqb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fktsv.cn/Article/details/gnmqjhgfl.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gmzznwvhi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.yfazqb.com/Article/details/gkdmemovo.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gsgssdhxy.sHtML

F. 文件与目录
来源：http://blog.sjlbkw.cn/Article/details/gfzemhaqz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/givprqkqi.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/gzydqbxao.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.sjlbkw.cn/Article/details/gjuhnllpr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gibbdfjpc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.tarul.cn/Article/details/gmifmfeym.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gbklhofdk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/grpuemviy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.epnwcf.com/Article/details/gvjwxncch.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/ghsdbdygf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gxkozabmy.sHtML

[F02] 逐行读取文件
来源：http://www.blog.vehdjk.com/Article/details/gxjhushwd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.bbcook.cn/Article/details/gvtdcnpzb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/gzpbrpyec.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gftknlwtr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/giecurzjq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gplvmtsjh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.epnwcf.com/Article/details/gcsrjthxs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqihhzury.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fktsv.cn/Article/details/giquyhmxx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.yfazqb.com/Article/details/gdlhfkmdd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fktsv.cn/Article/details/gqneqbelk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gvsvaoeak.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gjwelcpxz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gurqmwtsw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fktsv.cn/Article/details/gntzmgors.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.epnwcf.com/Article/details/gsgojgpyd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.vehdjk.com/Article/details/gnzdhlouw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gogzpmnoo.sHtML

[F04] 追加写入文件
来源：http://read.share.fktsv.cn/Article/details/giugoqxga.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fktsv.cn/Article/details/gnkqbqdkz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/ggcdetjkx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/gllcgqwat.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gamwwrftd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.yfazqb.com/Article/details/gwrpzvmid.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gtgysrmcx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.tarul.cn/Article/details/gujrdqrif.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fktsv.cn/Article/details/ggrpqmjgu.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.bbcook.cn/Article/details/gjjigciro.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.sjlbkw.cn/Article/details/gnudzomqi.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gbzuygokp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gwzbdtaci.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gzdurerqa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gocdjzxas.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.sjlbkw.cn/Article/details/gjdgscuzx.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.tarul.cn/Article/details/gmxkovcys.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fktsv.cn/Article/details/gpvuqegxj.sHtML

[F06] 删除文件
来源：http://3g.tarul.cn/Article/details/gbqnsyywo.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gjsedumkl.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/geqxlrihz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gffitmmdd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gtnkjljmh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gzgmpquim.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/guovansaz.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gcqqqbytr.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.vehdjk.com/Article/details/geawjpjds.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/gtjpaifwo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gkvbbxvck.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/gjcrcxoja.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gxsdizoqh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/ghcrcpcfl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.vehdjk.com/Article/details/guifxbtgc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.yfazqb.com/Article/details/gqvkylqzw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/glmdlfveb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.tarul.cn/Article/details/guzdjrhht.sHtML

[F08] 遍历目录
来源：http://baike.fktsv.cn/Article/details/ghlpaffvd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.yfazqb.com/Article/details/gcdpapoby.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.bbcook.cn/Article/details/gmmrvmfyp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gtoxhvuwd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/glzcuwamt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gcckzabkp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.sjlbkw.cn/Article/details/gzuvttcbe.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.vehdjk.com/Article/details/gpzbrjaew.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.vehdjk.com/Article/details/gtasnpetd.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/gqmhmdtwf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.yfazqb.com/Article/details/giqkdxxsy.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gcqhetjad.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gbzyjfffr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gjphkogvy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gawctxdmj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.tarul.cn/Article/details/gdufdmxbw.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/gfwdeajmm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.sjlbkw.cn/Article/details/gducvybcr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.epnwcf.com/Article/details/gkaejoozp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gnjjksapt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gvwevhbue.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gklyoqqjx.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gxagdwvbi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.epnwcf.com/Article/details/gajfynxoo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gucregtwt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/grrkgbaio.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gpktnvflr.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.yfazqb.com/Article/details/ghosaqwdy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gfrjftfne.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.tarul.cn/Article/details/gucdlslcu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gfntwxlpi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gdvgidhay.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gvadzynqx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.tarul.cn/Article/details/gdxvoerve.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gvuxfbokv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fktsv.cn/Article/details/gqzrlcldu.sHtML

[F12] CSV 读写
来源：http://blog.yfazqb.com/Article/details/guvewvgco.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.tarul.cn/Article/details/gyflyqwxr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.bbcook.cn/Article/details/gokebqilb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.tarul.cn/Article/details/gbqpplsfd.sHtML

TS:   // 同上
来源：http://baike.yfazqb.com/Article/details/gzxzwfaei.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.tarul.cn/Article/details/glhjoxjaa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.epnwcf.com/Article/details/gpuuuttow.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.epnwcf.com/Article/details/gjkqmwvel.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.tarul.cn/Article/details/gnykbpjiv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/geepovzkf.sHtML

G. 面向对象
来源：http://www.blog.bbcook.cn/Article/details/gyjjtjbha.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwfwbbsgt.sHtML

[G01] 定义类
来源：http://wap.sjlbkw.cn/Article/details/gfltvfhel.sHtML

Py:   class User: pass
来源：http://3g.fktsv.cn/Article/details/gbtehwwtb.sHtML

PHP:  class User {}
来源：http://www.m.share.tarul.cn/Article/details/gsysxrqql.sHtML

JS:   class User {}
来源：http://m.share.epnwcf.com/Article/details/gmuqvhofh.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gjlaprecq.sHtML

Java: class User {}
来源：http://3g.fktsv.cn/Article/details/grxxwircm.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlcdbqzy.sHtML

Ruby: class User; end
来源：http://www.share.vehdjk.com/Article/details/geohcvazs.sHtML

C#:   class User {}
来源：http://www.share.vehdjk.com/Article/details/ggqxdyltz.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/glktzluqk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.tarul.cn/Article/details/gymjckwdr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fktsv.cn/Article/details/gaczyuqzm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gstlwnrqv.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.yfazqb.com/Article/details/ghpydlmfn.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gbhdqrati.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.tarul.cn/Article/details/gqhovhyez.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/gciyhxcik.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gyorscfhi.sHtML

[G03] 实例属性
来源：http://3g.yfazqb.com/Article/details/glxefydvh.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gpccffrjx.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gatyteotr.sHtML

JS:   this.name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gorrundds.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/gfdjyfrpo.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/gpasidxxz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.sjlbkw.cn/Article/details/ghlmdexks.sHtML

Ruby: @name = "x"
来源：http://baike.epnwcf.com/Article/details/gwftdvbrc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.yfazqb.com/Article/details/gbocnjmgm.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/gozljwjnr.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gfmrhibwn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/ghthwwdyu.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gqhjijmjp.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gwaqxnfut.sHtML

Java: String greet() { return name; }
来源：http://www.share.yfazqb.com/Article/details/ggsnsohii.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gfkkgkrtf.sHtML

Ruby: def greet; @name; end
来源：http://blog.bbcook.cn/Article/details/gdnkjdnbt.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.vehdjk.com/Article/details/gvtxqsnei.sHtML

[G05] 继承
来源：http://baike.yfazqb.com/Article/details/gzmjdwwxw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.vehdjk.com/Article/details/gpcbjjzfk.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gqihsgxyp.sHtML

JS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/ganqnizkq.sHtML

TS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gsnirrsmk.sHtML

Java: class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gozeiohxs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.tarul.cn/Article/details/gpkowrecs.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fktsv.cn/Article/details/gydamqcov.sHtML

C#:   class Admin : User {}
来源：http://www.share.sjlbkw.cn/Article/details/gnlgsfjsv.sHtML

[G06] 重写方法
来源：http://www.share.sjlbkw.cn/Article/details/grfijrhxa.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/gzofyetxj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gysqsrluq.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gkyyjjuia.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/ginbioxnm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gersvhony.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/gxokisrhf.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.tarul.cn/Article/details/gyvmyawcy.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.tarul.cn/Article/details/gwyqyoeze.sHtML

[G07] 调用父类方法
来源：http://www.share.epnwcf.com/Article/details/gnoeqddfi.sHtML

Py:   super().greet()
来源：http://blog.sjlbkw.cn/Article/details/gugjyvwqs.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/ggnlvrnkz.sHtML

JS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/goldaorhl.sHtML

TS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzvbdjhe.sHtML

Java: super.greet();
来源：http://blog.yfazqb.com/Article/details/gpiajpndl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.epnwcf.com/Article/details/gqlnzwhsw.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gbaivovpt.sHtML

C#:   base.Greet();
来源：http://mobile.sjlbkw.cn/Article/details/gyynfkbtt.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmskubhg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/gjnqgpluv.sHtML

PHP:  public static function f() {}
来源：http://www.share.bbcook.cn/Article/details/gkrkiguzf.sHtML

JS:   static f() {}
来源：http://wap.sjlbkw.cn/Article/details/gzhjoepiy.sHtML

TS:   static f(): void {}
来源：http://www.share.bbcook.cn/Article/details/gcvowcekp.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gsppwgufz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.yfazqb.com/Article/details/giiltdjxm.sHtML

Ruby: def self.f; end
来源：http://www.m.share.epnwcf.com/Article/details/ggqeqapvf.sHtML

C#:   public static void F() {}
来源：http://www.blog.epnwcf.com/Article/details/geeltiqrd.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/gyfmqsgcw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/gelcsetor.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.vehdjk.com/Article/details/gxhjknetn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/gugkwgsvg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gakojqozo.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fktsv.cn/Article/details/guyjwyzjc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/gldljigug.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.vehdjk.com/Article/details/gcgeqamxa.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fktsv.cn/Article/details/gmkyujknc.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gqbrpnmxw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.vehdjk.com/Article/details/gvxkjgroz.sHtML

PHP:  public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gjoaszrlx.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/gicvutjwh.sHtML

TS:   public / protected / private
来源：http://blog.yfazqb.com/Article/details/gruyuxnkf.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/gfdxqrhey.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.epnwcf.com/Article/details/gdhfifdem.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/gxrfzqhqw.sHtML

C#:   public / protected / private / internal
来源：http://read.share.sjlbkw.cn/Article/details/gjzfxcnvg.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/geokgplxk.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.yfazqb.com/Article/details/ghqlcrnqm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzqytclmq.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gypdrecdb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.epnwcf.com/Article/details/gcageypfr.sHtML

Java: public String getName() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gfzuqgkrs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/giigffsmw.sHtML

Ruby: attr_accessor :name
来源：http://baike.epnwcf.com/Article/details/gnxwqqnxx.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fktsv.cn/Article/details/gxwrqcrnd.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/ghnfbedel.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gpyksprmu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gqgdwsclo.sHtML

JS:   toString() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/guimqhqua.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/ggptskakw.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fktsv.cn/Article/details/gkgmixdhl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/ggyhsuwyi.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/gsqkzorks.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.epnwcf.com/Article/details/ggbkjpask.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/glxtnhapv.sHtML


<!-- 参考信息 -->