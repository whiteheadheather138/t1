代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gexxtkcup.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.vehdjk.com/Article/details/gmumwsopn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/gxijcsqca.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gncaprhfn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/greveomwh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.epnwcf.com/Article/details/gexumchnd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.bbcook.cn/Article/details/ggbnoalfl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.epnwcf.com/Article/details/gcuugostz.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.vehdjk.com/Article/details/gopfpgmji.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.yfazqb.com/Article/details/gfbzyticf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.bbcook.cn/Article/details/gpsdhydsx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.epnwcf.com/Article/details/gnirvvhgg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fktsv.cn/Article/details/gojgkqfpf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/gjdbrvgxe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.tarul.cn/Article/details/gvnhvuqix.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fktsv.cn/Article/details/gjywjnwwx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gbkksvsrd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.bbcook.cn/Article/details/ghwnoymhn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.yfazqb.com/Article/details/gfhssupfg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/gdhefvugj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.vehdjk.com/Article/details/gowblgqkq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.bbcook.cn/Article/details/gsgjebmyd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gtprcekxf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.vehdjk.com/Article/details/garxizajd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.vehdjk.com/Article/details/gjclihrmk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/gjcefprnc.sHtML

[E16] 数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/gkrrbyibu.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.tarul.cn/Article/details/gminfvsov.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.bbcook.cn/Article/details/gicoiuyua.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gzadjtbjx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gvysvqrgb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gblzlxkad.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/ghbllsmub.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.tarul.cn/Article/details/gzwiokaas.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.vehdjk.com/Article/details/gntodymgh.sHtML

[E17] 首字母大写
来源：http://wap.tarul.cn/Article/details/gylqxvthi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gtdjigxml.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/gkpmvfcgs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gsrohdecs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.tarul.cn/Article/details/gyyxvnndj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fktsv.cn/Article/details/gbvxiuqgx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gwzyjnxuf.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gdktxxobz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/giirprdpk.sHtML

[E18] 模板占位符替换
来源：http://mobile.sjlbkw.cn/Article/details/gmhevgdjk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.epnwcf.com/Article/details/gkkbjewtk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.sjlbkw.cn/Article/details/gkgoaphct.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gdrcfoedf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gaqkykvnf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.bbcook.cn/Article/details/grvoieclp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gakroheio.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/ghmyyyozb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.epnwcf.com/Article/details/grhgeubzi.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.tarul.cn/Article/details/geyfdmbbe.sHtML

Py:   s.splitlines()
来源：http://www.share.fktsv.cn/Article/details/gqxivlbwn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.yfazqb.com/Article/details/gkqupeoor.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/grwzngfgi.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gonxstxka.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/gxzsvjqvw.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.bbcook.cn/Article/details/gjixnquwo.sHtML

Ruby: s.lines
来源：http://wap.epnwcf.com/Article/details/gckebsvzb.sHtML

C#:   s.Split('\n')
来源：http://blog.yfazqb.com/Article/details/gsukikkop.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.yfazqb.com/Article/details/gviprhknm.sHtML

Py:   if not s:
来源：http://www.share.bbcook.cn/Article/details/gvqmjbnay.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.epnwcf.com/Article/details/ginutsbgd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.vehdjk.com/Article/details/gcqqlktid.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gnicixxcp.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/ghucosail.sHtML

Go:   if s == "" {}
来源：http://read.share.tarul.cn/Article/details/gwblbkzed.sHtML

Ruby: if s.empty?
来源：http://www.share.vehdjk.com/Article/details/gcanzwhep.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gvyfdlakn.sHtML

[E21] 超长截断加省略号
来源：http://blog.tarul.cn/Article/details/gnjlhodql.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.sjlbkw.cn/Article/details/gvhpgibro.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gqzbyujoj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gamrpsfrb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gbfcxxiia.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gdisofbze.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.epnwcf.com/Article/details/geqowefvy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gcpfccwga.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gwwghmuwd.sHtML

[E22] 字节长度与字符长度
来源：http://wap.epnwcf.com/Article/details/ganirsgne.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.vehdjk.com/Article/details/gcnhljjyx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/giywinuca.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gyccduynw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gnvltprzr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.bbcook.cn/Article/details/gpqqncuph.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/gqjlcayrw.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/gqdripknl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/grpsklntm.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjnidkyaa.sHtML

F. 文件与目录
来源：http://read.share.tarul.cn/Article/details/grjrlibuy.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gmsssgwgr.sHtML

[F01] 读取整个文件
来源：http://3g.epnwcf.com/Article/details/grmnkarkl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.epnwcf.com/Article/details/gwmqdkbgq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gqgqiguro.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.yfazqb.com/Article/details/gojmcsbll.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gljnlmfjl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gwqeflstd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.epnwcf.com/Article/details/glqswlpti.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fktsv.cn/Article/details/geopgpdag.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.tarul.cn/Article/details/gryfxgaib.sHtML

[F02] 逐行读取文件
来源：http://baike.vehdjk.com/Article/details/gsyuluuwq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/gkmieutaq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.vehdjk.com/Article/details/goqmddxjp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gppwowrjp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/gwfdplwqz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gpdiblsee.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.bbcook.cn/Article/details/geqfewoyz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.tarul.cn/Article/details/gnzwazgkd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/gwkkxeiaj.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/gncjppiqa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.vehdjk.com/Article/details/gbmritocy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gugfpbqgi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gnuczhgbl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/giuajirzv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/goknynzbb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.vehdjk.com/Article/details/gkdicbdat.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.epnwcf.com/Article/details/gmvvslacp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gwebrunyq.sHtML

[F04] 追加写入文件
来源：http://3g.fktsv.cn/Article/details/gxcpchtgr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fktsv.cn/Article/details/gybmktvjn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fktsv.cn/Article/details/gxjhudhcn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.bbcook.cn/Article/details/gilysyhcd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gsuyghyhd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.sjlbkw.cn/Article/details/gkxhzskmu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gydbyhkdl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.yfazqb.com/Article/details/gsixqsuyp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.epnwcf.com/Article/details/gwnsyutfv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.tarul.cn/Article/details/gpxijjnxm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/ghwcdobpz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gnuubxybd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gnbwjxzpa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gxuvgahfe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gjfzpbito.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.epnwcf.com/Article/details/gdkmjelvt.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ghofjnndg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fktsv.cn/Article/details/ghljjhwxo.sHtML

[F06] 删除文件
来源：http://baike.fktsv.cn/Article/details/gfghdolmq.sHtML

Py:   os.remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gjpywwpcf.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/grikbvnkn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gdgcpdpxe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gdsrtxyex.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gcicsoggh.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gjsqeemsa.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gxtwkaiqm.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.tarul.cn/Article/details/gpqtyfnvp.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/ggfiezqqs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gsvfonmtx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/ghknidajg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gnbozqmld.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gqzjyqjkt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.epnwcf.com/Article/details/gwrjajbao.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.vehdjk.com/Article/details/gvyzwsopn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.tarul.cn/Article/details/gjlfmdrza.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fktsv.cn/Article/details/getevbmcr.sHtML

[F08] 遍历目录
来源：http://baike.vehdjk.com/Article/details/gblmkuhfs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.sjlbkw.cn/Article/details/gjpmldmti.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gjoimhnbw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gdyggpupc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gngbyhkom.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gfimsyveg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.tarul.cn/Article/details/gdhrofbul.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gapajbmbi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.epnwcf.com/Article/details/gdnrnyfrz.sHtML

[F09] 获取文件大小
来源：http://www.m.share.sjlbkw.cn/Article/details/gssxxvbqz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.epnwcf.com/Article/details/gujvhvgdd.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/ghmlplymo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/glabacvyr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gwzummnjq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gsnmpzwvm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.bbcook.cn/Article/details/gewgjfpag.sHtML

Ruby: File.size("a.txt")
来源：http://baike.yfazqb.com/Article/details/ghrbvvanl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.sjlbkw.cn/Article/details/gqsaoiygo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.epnwcf.com/Article/details/gxqajwbnt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ggcryzcrt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.yfazqb.com/Article/details/grwbhmlcb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdhpnwda.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/gscconnio.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.epnwcf.com/Article/details/gajqczexo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gjgrqqodf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gmbqqvcpf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gscrefgzx.sHtML

[F11] 复制与移动文件
来源：http://m.share.sjlbkw.cn/Article/details/gvmdrxiip.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/ggwnrbjok.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.bbcook.cn/Article/details/gntkoaogf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gdkiwxirq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gpkdyathb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.epnwcf.com/Article/details/gqnvsoqls.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fktsv.cn/Article/details/gjvxbxxow.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gejyvdftw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.bbcook.cn/Article/details/gizhorcfi.sHtML

[F12] CSV 读写
来源：http://mobile.yfazqb.com/Article/details/gcpsacmkh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.epnwcf.com/Article/details/gjdsyirhm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fktsv.cn/Article/details/gqrdrpglr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.vehdjk.com/Article/details/gzcesyokl.sHtML

TS:   // 同上
来源：http://3g.bbcook.cn/Article/details/gqcpuvlit.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.tarul.cn/Article/details/gkcdfftca.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.yfazqb.com/Article/details/gfmeiqdps.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/gunnktrum.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/gaqdbnqor.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsqgumccv.sHtML

G. 面向对象
来源：http://www.blog.sjlbkw.cn/Article/details/gafbrnjfs.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gujjugzqo.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/ggcrftyxi.sHtML

Py:   class User: pass
来源：http://baike.epnwcf.com/Article/details/gscbjwnmg.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/gubxznamv.sHtML

JS:   class User {}
来源：http://read.share.tarul.cn/Article/details/gxhglwpjf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.yfazqb.com/Article/details/gzqtwxalq.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gvtjzlhat.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fktsv.cn/Article/details/grtocdiou.sHtML

Ruby: class User; end
来源：http://blog.sjlbkw.cn/Article/details/grskbuywa.sHtML

C#:   class User {}
来源：http://mobile.tarul.cn/Article/details/gfbglipdg.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gnmbmubmy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.epnwcf.com/Article/details/gudsyhldj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/gwpgjsrao.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gaelsxcjr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/geynwlium.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gevqwevow.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.bbcook.cn/Article/details/glinxxqzg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.epnwcf.com/Article/details/gswzqnlsz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/goerddkej.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/gnwyyohxd.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/gwlhmwphh.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gwdjpkizf.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/gtsgqxmwo.sHtML

TS:   name: string = "x";
来源：http://3g.bbcook.cn/Article/details/gotufxmbz.sHtML

Java: private String name;
来源：http://mobile.tarul.cn/Article/details/gwxpwjzxl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fktsv.cn/Article/details/gowmuglqa.sHtML

Ruby: @name = "x"
来源：http://www.share.tarul.cn/Article/details/gaalzlszw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gyphxuvse.sHtML

[G04] 定义方法
来源：http://www.share.bbcook.cn/Article/details/gnlhrnzbg.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/ggwtfxpbn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gdtppdgbm.sHtML

JS:   greet() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gwyvdqvks.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gppjrkxuv.sHtML

Java: String greet() { return name; }
来源：http://www.share.vehdjk.com/Article/details/gjbynjxzk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/ghkpazojn.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.bbcook.cn/Article/details/geokfuexm.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.epnwcf.com/Article/details/gqfiwnmgf.sHtML

[G05] 继承
来源：http://www.share.tarul.cn/Article/details/gnflhqfqn.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/gegraywer.sHtML

PHP:  class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/glcyqetam.sHtML

JS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gsehpuzjv.sHtML

TS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gtjqrtxqe.sHtML

Java: class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/glhmqpcqo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.sjlbkw.cn/Article/details/gxvlaeols.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fktsv.cn/Article/details/gyacuuoug.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/gvnmkjjlo.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/guamorwmn.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.sjlbkw.cn/Article/details/gqmxekhim.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gbdagnpvl.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gadzxyita.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gvdbjgpyn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gongymzoh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fktsv.cn/Article/details/gruvdbadh.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.tarul.cn/Article/details/gmozahsxt.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.tarul.cn/Article/details/gnhsvigpy.sHtML

[G07] 调用父类方法
来源：http://www.m.share.vehdjk.com/Article/details/ghfwnwjqy.sHtML

Py:   super().greet()
来源：http://m.share.bbcook.cn/Article/details/gaauootqg.sHtML

PHP:  parent::greet();
来源：http://www.share.sjlbkw.cn/Article/details/gwhemwqvh.sHtML

JS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gbfpohpqe.sHtML

TS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/genmbbfch.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/ghvhhtfdv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.bbcook.cn/Article/details/gqrkbrinn.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gpsxqpwnr.sHtML

C#:   base.Greet();
来源：http://blog.tarul.cn/Article/details/gmuikxxzc.sHtML

[G08] 静态方法与属性
来源：http://baike.yfazqb.com/Article/details/gjihompvh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/gaqcpvbth.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/gmpucpwak.sHtML

JS:   static f() {}
来源：http://blog.epnwcf.com/Article/details/gdsilezvn.sHtML

TS:   static f(): void {}
来源：http://www.share.tarul.cn/Article/details/grgxchsxt.sHtML

Java: static void f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/glwzpfklh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.yfazqb.com/Article/details/gkjkkczal.sHtML

Ruby: def self.f; end
来源：http://blog.vehdjk.com/Article/details/ginmnnqfs.sHtML

C#:   public static void F() {}
来源：http://www.m.share.yfazqb.com/Article/details/gbcxsqvvk.sHtML

[G09] 接口 / 抽象类
来源：http://blog.bbcook.cn/Article/details/gmhyfidxx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.bbcook.cn/Article/details/gbbmxcriy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.sjlbkw.cn/Article/details/geeyfxofw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.bbcook.cn/Article/details/gqloevare.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.bbcook.cn/Article/details/glyoxdvps.sHtML

Java: interface Shape { double area(); }
来源：http://wap.tarul.cn/Article/details/gvxrlucoa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.bbcook.cn/Article/details/gutyqwbpk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.yfazqb.com/Article/details/gkhggobgp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.bbcook.cn/Article/details/gxvlmirye.sHtML

[G10] 访问控制
来源：http://wap.tarul.cn/Article/details/giavbtojs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/gaxxsdxbf.sHtML

PHP:  public / protected / private
来源：http://mobile.tarul.cn/Article/details/gkcynjdxx.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fktsv.cn/Article/details/ghpllopfu.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/gfcifneai.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.bbcook.cn/Article/details/glbzimjbc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.sjlbkw.cn/Article/details/gwyoclsqh.sHtML

Ruby: public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gsyisanvn.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.bbcook.cn/Article/details/gkfjlccsy.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/gisleaqxl.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/gxmgopwlq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gnueswbdn.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyejcijza.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gccetftek.sHtML

Java: public String getName() { return name; }
来源：http://m.share.yfazqb.com/Article/details/grvkipfms.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/guqaoobud.sHtML


<!-- 参考信息 -->