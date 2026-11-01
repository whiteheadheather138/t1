代发 wailian999

[E14] URL 编码与 Base64
来源：http://m.share.bbcook.cn/Article/details/groppifxb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.sjlbkw.cn/Article/details/gavuknzcy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.tarul.cn/Article/details/ggjbvcyca.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/gmqdzskls.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.vehdjk.com/Article/details/gctxhfmkn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/gubduayzz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.epnwcf.com/Article/details/gskxciccg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.bbcook.cn/Article/details/gmpfzfkly.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/guremogww.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.bbcook.cn/Article/details/gnugdsgzr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.bbcook.cn/Article/details/ghvigukhz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.yfazqb.com/Article/details/gdnbnvbmw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.yfazqb.com/Article/details/gsqocpixy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fktsv.cn/Article/details/glynfquvb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.tarul.cn/Article/details/gperiltmc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gcpbiyiea.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.epnwcf.com/Article/details/gkpemsgpe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.tarul.cn/Article/details/glinbqdtg.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/gwjzkmfti.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.vehdjk.com/Article/details/gffhqgqhp.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.vehdjk.com/Article/details/gzxgvrlmw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gotnfwisr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/guudfqwnf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gwldbybwa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/gtxpmsnxc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.bbcook.cn/Article/details/guxvfnzkn.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/gzxquwyyo.sHtML

[E17] 首字母大写
来源：http://mobile.fktsv.cn/Article/details/gqudnjigx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.tarul.cn/Article/details/gzwsvozaq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.sjlbkw.cn/Article/details/grkmpyqyr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/gndpxstet.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gqkhroucv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.epnwcf.com/Article/details/gogyaiktq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fktsv.cn/Article/details/grxlbtasi.sHtML

Ruby: s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/gbtihihdu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.bbcook.cn/Article/details/gsaulzifs.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/gyzasivwr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/ghzddzngu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.yfazqb.com/Article/details/geetytxmk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/glmyukczb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gjqbsutle.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/ggucsfodo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gbxaymkln.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.yfazqb.com/Article/details/gbajwkymj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gqwqmkphz.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/gdziygxqd.sHtML

Py:   s.splitlines()
来源：http://www.share.yfazqb.com/Article/details/gzfkpnyyo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gcswblfku.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/gcpmaiuuf.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gwxgnraia.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/genmblvuw.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.sjlbkw.cn/Article/details/ghjnotkfw.sHtML

Ruby: s.lines
来源：http://mobile.epnwcf.com/Article/details/gfmswvwfd.sHtML

C#:   s.Split('\n')
来源：http://read.share.fktsv.cn/Article/details/grerbzxvu.sHtML

[E20] 判断字符串是否为空
来源：http://3g.bbcook.cn/Article/details/gbuvfjlua.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gufoyemsi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.vehdjk.com/Article/details/glmomcwwq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fktsv.cn/Article/details/geoppwheh.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.bbcook.cn/Article/details/gauotfbpb.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/grnmgdpga.sHtML

Go:   if s == "" {}
来源：http://read.share.vehdjk.com/Article/details/gjdichgue.sHtML

Ruby: if s.empty?
来源：http://www.blog.epnwcf.com/Article/details/gigvdpwrw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gigqggeap.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.epnwcf.com/Article/details/glntubvza.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.bbcook.cn/Article/details/gyszfpqyc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gegxlmzrs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gomjrrxai.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/guwlzcjuk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/guhxalqva.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.bbcook.cn/Article/details/gatctovos.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/giqjtthth.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gxysqxjpu.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.sjlbkw.cn/Article/details/gihifibqj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.tarul.cn/Article/details/gmxbovxsc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gktgxclfa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/gnqfuszdy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gbiohtnqu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.sjlbkw.cn/Article/details/gwtpbcpgo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.sjlbkw.cn/Article/details/gdbsvsqfb.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.bbcook.cn/Article/details/glufnimjf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.epnwcf.com/Article/details/gazhsijsf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjfcdrxxa.sHtML

F. 文件与目录
来源：http://wap.fktsv.cn/Article/details/gdwwytrci.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxynjcpaq.sHtML

[F01] 读取整个文件
来源：http://baike.epnwcf.com/Article/details/gxstrqdgn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.yfazqb.com/Article/details/gdioomexy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.tarul.cn/Article/details/gtuqkvoog.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.sjlbkw.cn/Article/details/gybwlmqwf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gqoukssye.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gimpeplsp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.epnwcf.com/Article/details/gtbramfqq.sHtML

Ruby: File.read("a.txt")
来源：http://3g.vehdjk.com/Article/details/glkmuvvaz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gwbylnnej.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/gdcqjweqi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.tarul.cn/Article/details/gdtoflmih.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.vehdjk.com/Article/details/guqckepnf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gqerprlui.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/gbfvlxbys.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/grmvpauur.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.epnwcf.com/Article/details/gcdzcptld.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fktsv.cn/Article/details/gdrpbgges.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.bbcook.cn/Article/details/gdvczavsz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fktsv.cn/Article/details/grpzdjhmf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fktsv.cn/Article/details/gygnhcttr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gxdirqihu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gbcigfjya.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gvjduiuji.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.epnwcf.com/Article/details/gaornlpld.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.tarul.cn/Article/details/ghysoycgg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.vehdjk.com/Article/details/gpyzghobh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/ggcwpsgwd.sHtML

[F04] 追加写入文件
来源：http://blog.fktsv.cn/Article/details/gioggifas.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/gcaobnqmd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fktsv.cn/Article/details/gdmyxnyrk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gqacfotak.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gmrftztls.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gcvozluwm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.tarul.cn/Article/details/ghchhpprx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fktsv.cn/Article/details/gtkvrusah.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.yfazqb.com/Article/details/gvbtqjnit.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fktsv.cn/Article/details/gqnntuwnw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fktsv.cn/Article/details/gwupvtxqu.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.yfazqb.com/Article/details/gmwuljqvy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/ggicsczfv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ghgttmfxz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gwyvohqli.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.sjlbkw.cn/Article/details/gwdmiqdov.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/ghluimprr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/grbkblsgu.sHtML

[F06] 删除文件
来源：http://www.share.vehdjk.com/Article/details/gwtskwvam.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gtbmfqzdn.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gjqkcxksw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gjmpqnnfg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gvxivlcmw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gntbjspvd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gmgsghsbu.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.vehdjk.com/Article/details/gzoluayhr.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.vehdjk.com/Article/details/gqcyfphea.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.bbcook.cn/Article/details/gmbsojhso.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/gehzykjal.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.epnwcf.com/Article/details/gkwrvfgxa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/grpzqcanj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/grqvwqdjc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/gvhqkxfcl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.sjlbkw.cn/Article/details/glwfuauyi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.yfazqb.com/Article/details/guiobwrqs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fktsv.cn/Article/details/gbjpubpmx.sHtML

[F08] 遍历目录
来源：http://baike.vehdjk.com/Article/details/gypyjserw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/gjwyejkft.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fktsv.cn/Article/details/gprkyowzi.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gspwaalbz.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.bbcook.cn/Article/details/gbmfkzwmn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gqdvuwcnw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.epnwcf.com/Article/details/gmhdmzcys.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.yfazqb.com/Article/details/grxhwaicc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gkdarrqio.sHtML

[F09] 获取文件大小
来源：http://www.m.share.vehdjk.com/Article/details/gsupnsnbt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.bbcook.cn/Article/details/gnuphiwfd.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gkbysezku.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/gyhrzrhng.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gcwxsmftk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gdoqckmty.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fktsv.cn/Article/details/gwkpbhsfm.sHtML

Ruby: File.size("a.txt")
来源：http://blog.vehdjk.com/Article/details/ggospbrmw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.sjlbkw.cn/Article/details/gqxgfdthz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.vehdjk.com/Article/details/gtdkqwcnv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gyzcfgumo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.vehdjk.com/Article/details/gpsmvzjzy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gscdmlujr.sHtML

TS:   path.extname("a.txt")
来源：http://wap.tarul.cn/Article/details/gyiwsmdnn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.bbcook.cn/Article/details/gvlgrthxi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gejrmadzg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gdzjeadzm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gwyiajitj.sHtML

[F11] 复制与移动文件
来源：http://blog.sjlbkw.cn/Article/details/gkvvxbhnn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gwynuuatf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fktsv.cn/Article/details/gemwlhmia.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gursjftre.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gqyitnizt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.tarul.cn/Article/details/gailhefyn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/gvqpftmcj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gvzxcbjoi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.bbcook.cn/Article/details/gzaojrzta.sHtML

[F12] CSV 读写
来源：http://www.share.sjlbkw.cn/Article/details/gwkugjgur.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fktsv.cn/Article/details/gznhqebfn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/gacmmgkvs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.vehdjk.com/Article/details/gzknxcdrt.sHtML

TS:   // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/gysvkvdco.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/goonstrob.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.epnwcf.com/Article/details/gzmlgbvki.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fktsv.cn/Article/details/gwskamcqw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.tarul.cn/Article/details/gfxcgnieq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvlbcavts.sHtML

G. 面向对象
来源：http://3g.yfazqb.com/Article/details/gttuizawt.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gskarrytg.sHtML

[G01] 定义类
来源：http://3g.tarul.cn/Article/details/gewcixqut.sHtML

Py:   class User: pass
来源：http://m.share.vehdjk.com/Article/details/gjtyveqac.sHtML

PHP:  class User {}
来源：http://www.share.vehdjk.com/Article/details/ggmjqfdch.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gkivoarra.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsynpflfp.sHtML

Java: class User {}
来源：http://www.share.tarul.cn/Article/details/gqvzrpfkl.sHtML

Go:   type User struct { Name string }
来源：http://blog.tarul.cn/Article/details/glywxwner.sHtML

Ruby: class User; end
来源：http://mobile.epnwcf.com/Article/details/gvrrixorl.sHtML

C#:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/ghrcsetbl.sHtML

[G02] 构造函数
来源：http://m.share.tarul.cn/Article/details/ghfkhlvux.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.epnwcf.com/Article/details/ghdrevrmb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.tarul.cn/Article/details/grjzyecwx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/gvtqwudyd.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fktsv.cn/Article/details/guugngfqk.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gckazwtwd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.yfazqb.com/Article/details/gffvcsygc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.bbcook.cn/Article/details/gqxzbaaxi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.bbcook.cn/Article/details/gkruvgwbl.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/grahseyeg.sHtML

Py:   self.name = "x"
来源：http://www.blog.tarul.cn/Article/details/gdrmkicpp.sHtML

PHP:  public string $name = "x";
来源：http://www.share.epnwcf.com/Article/details/gwpcezqkm.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gdhoqkkqn.sHtML

TS:   name: string = "x";
来源：http://m.share.vehdjk.com/Article/details/gtcpramux.sHtML

Java: private String name;
来源：http://mobile.sjlbkw.cn/Article/details/giaidncij.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fktsv.cn/Article/details/gqumvatsj.sHtML

Ruby: @name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/gevbooynp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.tarul.cn/Article/details/gfushviac.sHtML

[G04] 定义方法
来源：http://blog.vehdjk.com/Article/details/giapnkpvb.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gyrjstvaq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/ghubyaqam.sHtML

JS:   greet() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gytfommqq.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gssoayafw.sHtML

Java: String greet() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gvcpacfdr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gewxbfpgj.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/gdjjfgzeh.sHtML

C#:   public string Greet() => Name;
来源：http://3g.tarul.cn/Article/details/gfyptvpbf.sHtML

[G05] 继承
来源：http://m.share.vehdjk.com/Article/details/gamyilncz.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/gvgqdjuyd.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gbzebpuuo.sHtML

JS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/glxnsibit.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gpjrexlpb.sHtML

Java: class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gjoqwqntw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.epnwcf.com/Article/details/gorheslpl.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gvuiavqgv.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/gxjpospza.sHtML

[G06] 重写方法
来源：http://www.share.epnwcf.com/Article/details/gjtptxomf.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.tarul.cn/Article/details/gkuqnhjgt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/guffcouzx.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gjedlqyby.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gxezhncqv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gunbvncld.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/ghyqtuemj.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gnxwegsix.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/gucwxmdim.sHtML

[G07] 调用父类方法
来源：http://mobile.fktsv.cn/Article/details/gqmozesay.sHtML

Py:   super().greet()
来源：http://baike.tarul.cn/Article/details/gdqydmlau.sHtML

PHP:  parent::greet();
来源：http://m.share.fktsv.cn/Article/details/gmdqbhlgs.sHtML

JS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gcbyccbzl.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gmlfniwvm.sHtML

Java: super.greet();
来源：http://blog.fktsv.cn/Article/details/gcgvcbnuv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fktsv.cn/Article/details/gjwoykkau.sHtML

Ruby: super
来源：http://3g.tarul.cn/Article/details/gwqcrclim.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/grorqxjbg.sHtML

[G08] 静态方法与属性
来源：http://blog.fktsv.cn/Article/details/gzfkthvpk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.vehdjk.com/Article/details/gwlvrotlw.sHtML

PHP:  public static function f() {}
来源：http://baike.sjlbkw.cn/Article/details/ganxvfmoo.sHtML

JS:   static f() {}
来源：http://blog.bbcook.cn/Article/details/gcitjtzov.sHtML

TS:   static f(): void {}
来源：http://baike.tarul.cn/Article/details/gpvvxkkfh.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gjdpmxsdp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.bbcook.cn/Article/details/gfdqxkryj.sHtML

Ruby: def self.f; end
来源：http://m.share.epnwcf.com/Article/details/gwzagprbo.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gmsxpwnlc.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.yfazqb.com/Article/details/gneimwfin.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/gcnnzscsw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwqsubqeq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gskrxveuw.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gmthlliey.sHtML

Java: interface Shape { double area(); }
来源：http://baike.vehdjk.com/Article/details/gklozkrsm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.bbcook.cn/Article/details/gtrtvthjg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/givmenoqe.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fktsv.cn/Article/details/gaepnovgt.sHtML

[G10] 访问控制
来源：http://blog.fktsv.cn/Article/details/gilhxyvtg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.epnwcf.com/Article/details/gznqvygmb.sHtML

PHP:  public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gbdaimuoq.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/gbrjbloea.sHtML

TS:   public / protected / private
来源：http://3g.yfazqb.com/Article/details/gcxccbscv.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/gkqmhfkms.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.yfazqb.com/Article/details/ggwomqgax.sHtML

Ruby: public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/grnxajhro.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.epnwcf.com/Article/details/gdhthjorl.sHtML

[G11] getter / setter
来源：http://www.blog.sjlbkw.cn/Article/details/gcflvxqjr.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.tarul.cn/Article/details/gdzfhhmpl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gwvojcpej.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gusnextmc.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.tarul.cn/Article/details/grzjoselb.sHtML

Java: public String getName() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gzbutplor.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/ggvtsasie.sHtML

Ruby: attr_accessor :name
来源：http://www.share.sjlbkw.cn/Article/details/gtlzckvou.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.yfazqb.com/Article/details/gmefaraty.sHtML

[G12] 对象转字符串
来源：http://mobile.fktsv.cn/Article/details/gdqyhsofy.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.epnwcf.com/Article/details/gioiguhmo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gbfiqbdmw.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gcjvythek.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/geswtcmqi.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.bbcook.cn/Article/details/goeebouyf.sHtML


<!-- 参考信息 -->