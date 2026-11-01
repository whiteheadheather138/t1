代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.bbcook.cn/Article/details/gsqqjvoil.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.yfazqb.com/Article/details/glnhufwaa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/gihvghovp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.bbcook.cn/Article/details/gpztrsaze.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fktsv.cn/Article/details/gpknqmxcv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.yfazqb.com/Article/details/gwmgiopuq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.bbcook.cn/Article/details/grgrkkclg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fktsv.cn/Article/details/gmsgxzxre.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.bbcook.cn/Article/details/gkljisqkt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.bbcook.cn/Article/details/gdkfvetwz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fktsv.cn/Article/details/gibneklps.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fktsv.cn/Article/details/gubyvlosp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fktsv.cn/Article/details/gkzfcmgwo.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.sjlbkw.cn/Article/details/gjcqwocpb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/gowwhbqmp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.sjlbkw.cn/Article/details/gtmjdmjib.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.epnwcf.com/Article/details/gnfaknluw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gskkntsuu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gcharbvtu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gzgenducm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/gbhkxlchf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.bbcook.cn/Article/details/gmxpaoxcw.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/ghghpsqvy.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.tarul.cn/Article/details/gwqxjbfom.sHtML

PHP:  number_format(1234567);
来源：http://3g.sjlbkw.cn/Article/details/gvotvetqy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/gblravoqr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/gxhlywnhc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.vehdjk.com/Article/details/giamebtqk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gpxbbmuxz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/gvquohgly.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fktsv.cn/Article/details/gxnworffi.sHtML

[E17] 首字母大写
来源：http://3g.yfazqb.com/Article/details/gkmodwnio.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.vehdjk.com/Article/details/gnmalqzoj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.tarul.cn/Article/details/gvxjyzeaj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/gnaeiltfl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gbsqniiyc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.tarul.cn/Article/details/gyadpwquf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.yfazqb.com/Article/details/gahqprpvq.sHtML

Ruby: s.capitalize
来源：http://read.share.epnwcf.com/Article/details/gcekajrpm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fktsv.cn/Article/details/gqzdnqyrt.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.tarul.cn/Article/details/gemotiuei.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.yfazqb.com/Article/details/ghbvtohhc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.yfazqb.com/Article/details/gifoaklys.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gveqlsxve.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gcluusoew.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gtoxfhluf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gjsgseijv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/grcckjhux.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.sjlbkw.cn/Article/details/gpckbaygi.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.bbcook.cn/Article/details/gawpgdjrj.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gvhcypwlb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.tarul.cn/Article/details/gkawwzmzj.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.yfazqb.com/Article/details/gzmtxyzda.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/ganbwpoqf.sHtML

Java: s.lines().toList()
来源：http://baike.bbcook.cn/Article/details/gsttuqhai.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/grkcfnhvl.sHtML

Ruby: s.lines
来源：http://3g.tarul.cn/Article/details/goxocdwnm.sHtML

C#:   s.Split('\n')
来源：http://m.share.sjlbkw.cn/Article/details/gdptvlnso.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.sjlbkw.cn/Article/details/gfuqnxkbv.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/guyyrlwhk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/grhtjinux.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.vehdjk.com/Article/details/gsbnnvsbd.sHtML

TS:   if (s === "") {}
来源：http://m.share.epnwcf.com/Article/details/gkcqqslij.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gniqidzkn.sHtML

Go:   if s == "" {}
来源：http://baike.epnwcf.com/Article/details/gyhamarsq.sHtML

Ruby: if s.empty?
来源：http://3g.sjlbkw.cn/Article/details/gdgartxhz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.sjlbkw.cn/Article/details/gmlhaeaqj.sHtML

[E21] 超长截断加省略号
来源：http://baike.yfazqb.com/Article/details/gedjhtcag.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.vehdjk.com/Article/details/gwzxjqqzl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gbpqypzse.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/guprhlfjw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/glzvupgxl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gzrnzaxuw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/gzxtbvnsv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/geshjebpa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.tarul.cn/Article/details/grjsdmdks.sHtML

[E22] 字节长度与字符长度
来源：http://wap.sjlbkw.cn/Article/details/guzelougl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gabraojoq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gyywoaptj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/gklwprfou.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/genhlqpvf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/gvnwaosfn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.yfazqb.com/Article/details/gohcdndua.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.vehdjk.com/Article/details/gteulyrzh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gcesgsqct.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjahhtyle.sHtML

F. 文件与目录
来源：http://www.blog.sjlbkw.cn/Article/details/gagvhxtcg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/guzurdaod.sHtML

[F01] 读取整个文件
来源：http://blog.epnwcf.com/Article/details/gjfjojybs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.tarul.cn/Article/details/gaofrdhpf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gomfckgyt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.epnwcf.com/Article/details/gvbzxgfbj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gjmiqsgvd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gzszwfhae.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.tarul.cn/Article/details/ggaaktfxr.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.vehdjk.com/Article/details/grrzslfgm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gvthsfits.sHtML

[F02] 逐行读取文件
来源：http://mobile.yfazqb.com/Article/details/gtpklletz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.bbcook.cn/Article/details/gpkegoktc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.sjlbkw.cn/Article/details/gnlligvij.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvkamcnhb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.epnwcf.com/Article/details/gdmfsboee.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gbvhzmnmv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/gqencqyer.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.epnwcf.com/Article/details/geshkpuwk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.sjlbkw.cn/Article/details/gkkqndzvh.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/ghbmgeqob.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fktsv.cn/Article/details/grefpztxo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/gfjybvoey.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gnhkblqlk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gmyydaxtn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.tarul.cn/Article/details/gaphiwdjt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.tarul.cn/Article/details/gfzmstopk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/ggqgyrzrq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gglxxgggy.sHtML

[F04] 追加写入文件
来源：http://m.share.vehdjk.com/Article/details/gxxgsjaqs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.bbcook.cn/Article/details/ghycdczjq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.bbcook.cn/Article/details/guvjespox.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/gdppnwnro.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gdutzpjiz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.yfazqb.com/Article/details/gfijdmljv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.epnwcf.com/Article/details/gjzbvhlym.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fktsv.cn/Article/details/gmsngalac.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.bbcook.cn/Article/details/grbiekmce.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.sjlbkw.cn/Article/details/gyduhptke.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/gfbwvhalr.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gmsxujqqv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gwaemmcbr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gdbcharcg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gwiovwuan.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.bbcook.cn/Article/details/ghyshkbjv.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.tarul.cn/Article/details/gzlpnsohf.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/gtmsutlse.sHtML

[F06] 删除文件
来源：http://www.m.share.vehdjk.com/Article/details/gwbobfvcz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.yfazqb.com/Article/details/ghnartkia.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gtyjwkxmk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gsbhhaafr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gdsatdyhg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gdrpebudj.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gxtrstsrr.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.yfazqb.com/Article/details/gccsfmyqo.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.bbcook.cn/Article/details/gadhgalxv.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/gptqxmhiy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gvietznor.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.sjlbkw.cn/Article/details/gazuqqmaq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gmefjmwam.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/gdkhoeiop.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/goublzjaa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.yfazqb.com/Article/details/gbxnghewb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.sjlbkw.cn/Article/details/gmxopoylc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.epnwcf.com/Article/details/gqtynyqkt.sHtML

[F08] 遍历目录
来源：http://wap.fktsv.cn/Article/details/gxwaopxck.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.vehdjk.com/Article/details/gmqkggane.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gztezfelj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gkfabeqrf.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/giiulaxkf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/ggrwcpgfj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.yfazqb.com/Article/details/gityeulrx.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/guomtepey.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gdefnkrhp.sHtML

[F09] 获取文件大小
来源：http://wap.epnwcf.com/Article/details/gfvxpciov.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/geuixjzyo.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gcnaprobq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/ggddjwljr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/gsqqtxkft.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gppcrhjvi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.yfazqb.com/Article/details/gmbzanbow.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gpufrdazz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.epnwcf.com/Article/details/gtvixipvt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gzdykfcdb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gslpteunq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/gshekzcnk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/godcvtacf.sHtML

TS:   path.extname("a.txt")
来源：http://wap.vehdjk.com/Article/details/ghllqpfqc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/grjkbwlfp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/glmuxerks.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gywsjqdoo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gggciuwrs.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/gegjbopiq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gzeyybeqp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gndqxvwja.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gyuciqlau.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gkdxldsoj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gedybyhyg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fktsv.cn/Article/details/gxfcsijmw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gsjovluhq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.tarul.cn/Article/details/gcwhcfbdv.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/gbvpgahex.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.tarul.cn/Article/details/glrbstlsu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/gkblsmdvl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.tarul.cn/Article/details/gefeufphm.sHtML

TS:   // 同上
来源：http://www.blog.yfazqb.com/Article/details/grqwlnhns.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gahnjwofr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fktsv.cn/Article/details/gyaqajnao.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gbhisfpal.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.epnwcf.com/Article/details/gxjxjcztf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gduyfmnuu.sHtML

G. 面向对象
来源：http://www.blog.epnwcf.com/Article/details/gqgyphfom.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ghaylsnuy.sHtML

[G01] 定义类
来源：http://baike.epnwcf.com/Article/details/giqgdprsn.sHtML

Py:   class User: pass
来源：http://blog.yfazqb.com/Article/details/gxmxstsbt.sHtML

PHP:  class User {}
来源：http://read.share.yfazqb.com/Article/details/glhugiqep.sHtML

JS:   class User {}
来源：http://mobile.vehdjk.com/Article/details/glctcjqqj.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.bbcook.cn/Article/details/gcmsasgyb.sHtML

Java: class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gprbhfvvi.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/gkkfpoglg.sHtML

Ruby: class User; end
来源：http://www.share.vehdjk.com/Article/details/gzfoxfmpm.sHtML

C#:   class User {}
来源：http://baike.epnwcf.com/Article/details/giakbxfwa.sHtML

[G02] 构造函数
来源：http://blog.vehdjk.com/Article/details/gidwwtzkn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.sjlbkw.cn/Article/details/gaozqpoxe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.yfazqb.com/Article/details/gyirpipua.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gaojrmtst.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.tarul.cn/Article/details/gnlamubhz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gxqsjqama.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.epnwcf.com/Article/details/gilfvvqzi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.yfazqb.com/Article/details/gruhjones.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gwroledhy.sHtML

[G03] 实例属性
来源：http://read.share.fktsv.cn/Article/details/gwogrjofs.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/gpyiygbpd.sHtML

PHP:  public string $name = "x";
来源：http://3g.yfazqb.com/Article/details/gqxtbtsdy.sHtML

JS:   this.name = "x";
来源：http://mobile.tarul.cn/Article/details/guhaorrkw.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/gbqdqqngs.sHtML

Java: private String name;
来源：http://blog.tarul.cn/Article/details/gfgnyzjkf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/ggplklmhi.sHtML

Ruby: @name = "x"
来源：http://read.share.epnwcf.com/Article/details/goxmiinkm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.sjlbkw.cn/Article/details/gfywdcoaj.sHtML

[G04] 定义方法
来源：http://wap.tarul.cn/Article/details/gqxoyivsd.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/gyccsinay.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gudocadqn.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gtbirgfxq.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gslljjdkn.sHtML

Java: String greet() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gpcjdfjkb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gdagpdlcu.sHtML

Ruby: def greet; @name; end
来源：http://mobile.vehdjk.com/Article/details/gknyzpplm.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.tarul.cn/Article/details/gjmuwneoi.sHtML

[G05] 继承
来源：http://baike.yfazqb.com/Article/details/gynylbgrq.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.bbcook.cn/Article/details/gxqtzlilb.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gignvmzfy.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/grdmqokdu.sHtML

TS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/giepuwcsi.sHtML

Java: class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gdyhubvic.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gltpzpcnu.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/ggvzbslcf.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/gnkihtiid.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gtcclbsvx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/gwnmsfakl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gacrvicbh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gtzsrcijp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gpjahymor.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gqqmaprzc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.tarul.cn/Article/details/gvudfqgei.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.bbcook.cn/Article/details/gpwyamfwk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyrzshew.sHtML

[G07] 调用父类方法
来源：http://m.share.vehdjk.com/Article/details/gkvllqcgr.sHtML

Py:   super().greet()
来源：http://www.blog.bbcook.cn/Article/details/ghsrvleqw.sHtML

PHP:  parent::greet();
来源：http://3g.yfazqb.com/Article/details/gradxxypu.sHtML

JS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gzfkrjbbo.sHtML

TS:   super.greet();
来源：http://m.share.vehdjk.com/Article/details/gexycjkix.sHtML

Java: super.greet();
来源：http://wap.vehdjk.com/Article/details/gijdxbzrv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fktsv.cn/Article/details/gfhzjvbsc.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/gtpgbxeom.sHtML

C#:   base.Greet();
来源：http://www.share.vehdjk.com/Article/details/gjjucpaim.sHtML

[G08] 静态方法与属性
来源：http://m.share.epnwcf.com/Article/details/gojkpqwjh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/gngeaazfm.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.tarul.cn/Article/details/gmwlxzddq.sHtML

JS:   static f() {}
来源：http://www.m.share.epnwcf.com/Article/details/ggbharmgi.sHtML

TS:   static f(): void {}
来源：http://3g.bbcook.cn/Article/details/ghvcjzyfr.sHtML

Java: static void f() {}
来源：http://m.share.tarul.cn/Article/details/gihjjqtqk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.vehdjk.com/Article/details/getvqcegh.sHtML

Ruby: def self.f; end
来源：http://m.share.vehdjk.com/Article/details/garluztqo.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gkwojpmji.sHtML

[G09] 接口 / 抽象类
来源：http://3g.sjlbkw.cn/Article/details/gnboruajx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.epnwcf.com/Article/details/gnhrfjdlu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.yfazqb.com/Article/details/gzaseyvzo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gbqptvqkd.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.epnwcf.com/Article/details/gvgkvwubj.sHtML

Java: interface Shape { double area(); }
来源：http://wap.sjlbkw.cn/Article/details/gestufgnp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.vehdjk.com/Article/details/ghtbcvwny.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.tarul.cn/Article/details/gmxehutbm.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/gduojoxof.sHtML

[G10] 访问控制
来源：http://baike.tarul.cn/Article/details/gatjxyzmx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.vehdjk.com/Article/details/gcrygiqcu.sHtML

PHP:  public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gvcdbblzm.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/gcshnxzaq.sHtML

TS:   public / protected / private
来源：http://wap.epnwcf.com/Article/details/gacehilbm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/gmjrmdxzk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fktsv.cn/Article/details/geysxaohc.sHtML

Ruby: public / protected / private
来源：http://baike.bbcook.cn/Article/details/gmgrxawtq.sHtML

C#:   public / protected / private / internal
来源：http://mobile.epnwcf.com/Article/details/gfijbfgid.sHtML

[G11] getter / setter
来源：http://www.m.share.yfazqb.com/Article/details/gmabkobmf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fktsv.cn/Article/details/gxnijvsyi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gnrldyzqy.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gkyqhgyfi.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/gwqcajthh.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gwrokjtvn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gzdhwhqvv.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gxwyfilix.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/gkzgiqbva.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/gahdqlups.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gmuhqhzzi.sHtML


<!-- 参考信息 -->