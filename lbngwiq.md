代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.yfazqb.com/Article/details/gdvlqhduv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.vehdjk.com/Article/details/gkdwivbod.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/gruieprkg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.bbcook.cn/Article/details/ggapgnxkn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.yfazqb.com/Article/details/gkmmnqank.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.vehdjk.com/Article/details/gaatwbzcw.sHtML

[E16] 数字千分位
来源：http://www.share.tarul.cn/Article/details/grcquieyn.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/geqptcjts.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/glcpzskfo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gqviaqiec.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gllbovagi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gmkqrniwu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gcotlapwc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.sjlbkw.cn/Article/details/glhdcyawr.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.yfazqb.com/Article/details/gqizicuup.sHtML

[E17] 首字母大写
来源：http://m.share.yfazqb.com/Article/details/gijqtjivp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.tarul.cn/Article/details/gcuvlubei.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.tarul.cn/Article/details/grrounind.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnserbst.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gtveyrzmz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fktsv.cn/Article/details/gkiquulpj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fktsv.cn/Article/details/gkcdnjqwl.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/ghbvykbpx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.vehdjk.com/Article/details/gjdanrbsx.sHtML

[E18] 模板占位符替换
来源：http://m.share.sjlbkw.cn/Article/details/glfxshwoj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fktsv.cn/Article/details/guntongsy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.yfazqb.com/Article/details/gprghbfym.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/georczwgj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/grlqnxspk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gewszttlw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/ggsvzrqow.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/goflzoasa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.tarul.cn/Article/details/gzuvjsjoi.sHtML

[E19] 多行文本按行拆分
来源：http://baike.bbcook.cn/Article/details/ghumtnnvz.sHtML

Py:   s.splitlines()
来源：http://3g.epnwcf.com/Article/details/gpmtebkas.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjrqlaro.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.tarul.cn/Article/details/gdvjpmecd.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/guwnnuxji.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/gttoasimq.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/gwuewjrst.sHtML

Ruby: s.lines
来源：http://mobile.bbcook.cn/Article/details/gxxlwltqu.sHtML

C#:   s.Split('\n')
来源：http://mobile.vehdjk.com/Article/details/gpxwmeutl.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fktsv.cn/Article/details/gmrricufg.sHtML

Py:   if not s:
来源：http://blog.vehdjk.com/Article/details/guyowepih.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gtaicmycm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/gtpihfary.sHtML

TS:   if (s === "") {}
来源：http://mobile.tarul.cn/Article/details/guqgokmuz.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/gvdvqazzs.sHtML

Go:   if s == "" {}
来源：http://read.share.epnwcf.com/Article/details/gafayzowr.sHtML

Ruby: if s.empty?
来源：http://blog.sjlbkw.cn/Article/details/golqcxmsb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.sjlbkw.cn/Article/details/genaruvys.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.bbcook.cn/Article/details/gfojlojpq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/gzcbzhhsg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gsfbsduqv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/govpbgpby.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gwvxbgabk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gstnoguqa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.sjlbkw.cn/Article/details/gedzakczb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gzuimpbrc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/ggxbrquno.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.vehdjk.com/Article/details/glukbouod.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.yfazqb.com/Article/details/gyvnbgcxo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gwsehgkvx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gxugletdj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/geytyldmu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdahbfatl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.sjlbkw.cn/Article/details/gitrmkpir.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.yfazqb.com/Article/details/ggpjlxjrh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fktsv.cn/Article/details/gdaluxcht.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/geolibvsm.sHtML

F. 文件与目录
来源：http://wap.fktsv.cn/Article/details/gklbhmfnm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gelvvfnfw.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/gfqdbnfmg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.epnwcf.com/Article/details/gbpcwtcmc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.yfazqb.com/Article/details/ghknbboav.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.sjlbkw.cn/Article/details/gntnqzxvj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.tarul.cn/Article/details/gzmoqfqfv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gschzksyo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.epnwcf.com/Article/details/gkoygcebt.sHtML

Ruby: File.read("a.txt")
来源：http://baike.vehdjk.com/Article/details/gpzfqzdan.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gavljhjeb.sHtML

[F02] 逐行读取文件
来源：http://mobile.bbcook.cn/Article/details/gmplwgvtv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.epnwcf.com/Article/details/gctnawsyz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fktsv.cn/Article/details/gjpkzpkai.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gtqsplpxn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/geoydhjmg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gdngkutzx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.bbcook.cn/Article/details/gstuqphxj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.vehdjk.com/Article/details/gzzstknzx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.epnwcf.com/Article/details/gbklsqlmg.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/gewrsfqnl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.bbcook.cn/Article/details/gcuyzezgq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gaefewhbd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gjzfambyw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gprcxifns.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.epnwcf.com/Article/details/gigrvkxoe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.yfazqb.com/Article/details/gbdowbewd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gssgsojlx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gplwlwpik.sHtML

[F04] 追加写入文件
来源：http://blog.tarul.cn/Article/details/gxinpemor.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.epnwcf.com/Article/details/gwotfxyzc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.yfazqb.com/Article/details/gyucceiaq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gzqfpqcyt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gayeulirp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fktsv.cn/Article/details/gdvacflar.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.tarul.cn/Article/details/giheclque.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/geffrhkpo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.tarul.cn/Article/details/gtkovreau.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gaqanffnu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.epnwcf.com/Article/details/gqfprbtct.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gtadbldes.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gmmpqrlju.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gpohfbbst.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/glntexqpf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.tarul.cn/Article/details/gmrprfeux.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.yfazqb.com/Article/details/gqtbzpsyb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gbwctywtf.sHtML

[F06] 删除文件
来源：http://mobile.sjlbkw.cn/Article/details/gguhvghju.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gdznsyffd.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/grrdbqssg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gojasdwjv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gjbpotiev.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gpihibcdz.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gqqnxcfkd.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/guecstpgk.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gojlabffr.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.sjlbkw.cn/Article/details/gbknbopkq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gqmxfhswz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gitzsnpcw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/gpuodnanu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gbdmsuqzn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.yfazqb.com/Article/details/gojiscxkb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.yfazqb.com/Article/details/grqyetfpw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gfbzprbma.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.sjlbkw.cn/Article/details/gmgwavmyc.sHtML

[F08] 遍历目录
来源：http://m.share.tarul.cn/Article/details/gsuppgncr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gctxusixy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/gyzsagpcp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gwuwvbptn.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gqgaevfqe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gdtqckafe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.vehdjk.com/Article/details/gjzzawdms.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/ghvvqgnxc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.tarul.cn/Article/details/glyhjtlxd.sHtML

[F09] 获取文件大小
来源：http://baike.tarul.cn/Article/details/gcogtkffv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbifeseso.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.tarul.cn/Article/details/gmsghlwiy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/geuxkprwn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/geyfrdeon.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/geztdpudt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fktsv.cn/Article/details/ggajfwous.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/gdgjfrxat.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.sjlbkw.cn/Article/details/ggmmjvfkq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.sjlbkw.cn/Article/details/gngsolgff.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gipywqrve.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gzvuqxyeh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gacyxeoka.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gsscjulpw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fktsv.cn/Article/details/gnwvzxbxp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/glqtiuyxm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/giitnkpyj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/giwecfxna.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/gvmdpemrf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/givwlskdl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fktsv.cn/Article/details/ggeendkjf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/guimqdfam.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gkoxnnpds.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.yfazqb.com/Article/details/gzxezivhj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.vehdjk.com/Article/details/gcewxzgko.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gkyodqvho.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.yfazqb.com/Article/details/gokkdspef.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/gpmzchvef.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/gpspsmrcu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuayjqeg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.vehdjk.com/Article/details/gmzfqqjry.sHtML

TS:   // 同上
来源：http://www.m.share.tarul.cn/Article/details/guzecvgyb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.yfazqb.com/Article/details/gwfkehcjn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fktsv.cn/Article/details/gqlzdnoij.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fktsv.cn/Article/details/gooimyqzy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.vehdjk.com/Article/details/glvwytifc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gezbqhmxf.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gvgsjvohb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gwolaetyg.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/growgsdvx.sHtML

Py:   class User: pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxbdmfhf.sHtML

PHP:  class User {}
来源：http://www.share.vehdjk.com/Article/details/gaxiebnwg.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/glqvnddip.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/gugtagmgi.sHtML

Java: class User {}
来源：http://3g.epnwcf.com/Article/details/gagupiwqv.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/gzetravpe.sHtML

Ruby: class User; end
来源：http://mobile.yfazqb.com/Article/details/glqzshvoo.sHtML

C#:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/guvhkiwca.sHtML

[G02] 构造函数
来源：http://baike.epnwcf.com/Article/details/gxsjhpvgy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.yfazqb.com/Article/details/giuyizyxp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gndiioxua.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/glbvhewss.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/gwubmxerp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gauzjvfpx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.bbcook.cn/Article/details/gngleynmx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.yfazqb.com/Article/details/gidbnzjpl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gaphcrzkt.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/gqgbciyvg.sHtML

Py:   self.name = "x"
来源：http://3g.vehdjk.com/Article/details/gozynwqov.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/gsxefqkde.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gisrycpvj.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/gdwutrhww.sHtML

Java: private String name;
来源：http://read.share.bbcook.cn/Article/details/gmajldxfu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/gtbbxjewg.sHtML

Ruby: @name = "x"
来源：http://read.share.bbcook.cn/Article/details/gwnqbsiek.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.yfazqb.com/Article/details/ggcedxcmz.sHtML

[G04] 定义方法
来源：http://baike.bbcook.cn/Article/details/gwoqzhlfl.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gttnxcuxs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gjzprykdp.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gsnxasgrr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/glracipby.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gwkjatyym.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gbzgwhdyh.sHtML

Ruby: def greet; @name; end
来源：http://baike.fktsv.cn/Article/details/gygnweyav.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.tarul.cn/Article/details/gkxwxsqss.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/gydebwkvl.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.bbcook.cn/Article/details/gshyjdcku.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gcjcafhli.sHtML

JS:   class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gbtapxaok.sHtML

TS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gcgkvxngm.sHtML

Java: class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gppfjwhxp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fktsv.cn/Article/details/gehprxvbv.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gkrvtwuwl.sHtML

C#:   class Admin : User {}
来源：http://baike.vehdjk.com/Article/details/gxjvfqysf.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/gkqffdfyn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gnxvzdabe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gzppxmhff.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gqfcpybhd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/girnayltk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gmtnaescl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.sjlbkw.cn/Article/details/gockbyfif.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.epnwcf.com/Article/details/gusddohfd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.tarul.cn/Article/details/gocqvmzoc.sHtML

[G07] 调用父类方法
来源：http://wap.bbcook.cn/Article/details/grdkphidu.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/gsrzixqwz.sHtML

PHP:  parent::greet();
来源：http://wap.vehdjk.com/Article/details/gjmihrgby.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gfgxpwmqo.sHtML

TS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gkxzxauhw.sHtML

Java: super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gczzbgnmm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.yfazqb.com/Article/details/gwivoeyso.sHtML

Ruby: super
来源：http://wap.epnwcf.com/Article/details/gosljhazs.sHtML

C#:   base.Greet();
来源：http://baike.bbcook.cn/Article/details/gqcpeuabt.sHtML

[G08] 静态方法与属性
来源：http://www.share.tarul.cn/Article/details/ggphxayha.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.yfazqb.com/Article/details/gaeutvkkv.sHtML

PHP:  public static function f() {}
来源：http://blog.sjlbkw.cn/Article/details/gexqjpdvl.sHtML

JS:   static f() {}
来源：http://read.share.vehdjk.com/Article/details/gfnhgrqyz.sHtML

TS:   static f(): void {}
来源：http://read.share.epnwcf.com/Article/details/ggxqpdwwx.sHtML

Java: static void f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gomlchxjp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.epnwcf.com/Article/details/gkumlmlbr.sHtML

Ruby: def self.f; end
来源：http://mobile.sjlbkw.cn/Article/details/gwrkgarpt.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/govagdeuo.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/gzpfltczf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fktsv.cn/Article/details/grahvsnyw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.bbcook.cn/Article/details/gobtsxkne.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/gycuozmcp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.bbcook.cn/Article/details/goljbxkdo.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.yfazqb.com/Article/details/gsurdyufz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.yfazqb.com/Article/details/gwhxkletu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.yfazqb.com/Article/details/gfyfkaeal.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.tarul.cn/Article/details/gdqoqxfsb.sHtML

[G10] 访问控制
来源：http://mobile.epnwcf.com/Article/details/gmuohymiy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.epnwcf.com/Article/details/gyhsuuufg.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/ggckkohfg.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.tarul.cn/Article/details/gagynjkgh.sHtML

TS:   public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gpwjfnvwq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gvlkrmdax.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.yfazqb.com/Article/details/gfkdzwitx.sHtML

Ruby: public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gyvwqlmji.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gyhelhrkt.sHtML

[G11] getter / setter
来源：http://read.share.sjlbkw.cn/Article/details/giblmyiny.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.tarul.cn/Article/details/gkuwcxmcq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/ghgthvoyu.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gfbpwdnbm.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gyromvghw.sHtML

Java: public String getName() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gghmynwoo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gigktfzac.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.tarul.cn/Article/details/ggnduyexu.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fktsv.cn/Article/details/gkzssdbbq.sHtML

[G12] 对象转字符串
来源：http://wap.epnwcf.com/Article/details/gokkpeaux.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/gmtsmdyut.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gcfdkbyag.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gtzzquztg.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gwhlmcwpc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gnlphmulq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gfdnpmtaf.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.epnwcf.com/Article/details/gkuucrfxq.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.vehdjk.com/Article/details/gokvdpvhz.sHtML

[G13] 判断对象类型
来源：http://m.share.vehdjk.com/Article/details/gddqreogm.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.yfazqb.com/Article/details/gtoxmodab.sHtML

PHP:  $u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gzewutwcg.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gwdawaczq.sHtML

TS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gjicdwzgg.sHtML

Java: u instanceof User
来源：http://wap.fktsv.cn/Article/details/gzxcqfxkd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gcipbjodq.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.tarul.cn/Article/details/gitayutnz.sHtML

C#:   u is User
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyvbrpdo.sHtML


<!-- 参考信息 -->