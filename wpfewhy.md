代发 wailian999

JS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gcectibvm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gcoezehpz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.bbcook.cn/Article/details/glszycqfu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/gdkksgbvb.sHtML

Ruby: s.reverse
来源：http://blog.fktsv.cn/Article/details/ghdqlatns.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gxbjxcpae.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.bbcook.cn/Article/details/gqlxkhojn.sHtML

Py:   s.count("a")
来源：http://wap.yfazqb.com/Article/details/gyhgehdmq.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.bbcook.cn/Article/details/gwtutmmlk.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gevsmebhe.sHtML

TS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gyetfndjs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.sjlbkw.cn/Article/details/gyenarbol.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/glkwypmxu.sHtML

Ruby: s.count("a")
来源：http://m.share.bbcook.cn/Article/details/geavxqlyf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/gmsseajpo.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/gqrugzbut.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/gxvqrheqg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/gbvojxeok.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/geuaraojg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gkugyhsbu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.bbcook.cn/Article/details/gwwgezqkf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.yfazqb.com/Article/details/gqhiwyvik.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/gnnjvgzbt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.epnwcf.com/Article/details/gjgndqine.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fktsv.cn/Article/details/gzwynmqzh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.epnwcf.com/Article/details/gjywgqokb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.epnwcf.com/Article/details/gmrvsxtrs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.vehdjk.com/Article/details/gqmidzjxe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.bbcook.cn/Article/details/gcbzdccrw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.vehdjk.com/Article/details/gqijsioau.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.epnwcf.com/Article/details/glydeygoe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.tarul.cn/Article/details/gwbviwvcr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.tarul.cn/Article/details/gcdymvbof.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.vehdjk.com/Article/details/gwchhchpv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.vehdjk.com/Article/details/gmisloeab.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.epnwcf.com/Article/details/gborzqjwx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.vehdjk.com/Article/details/ghynvttrn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.bbcook.cn/Article/details/gzugvdzdz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.bbcook.cn/Article/details/gtcyxqxwm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.yfazqb.com/Article/details/gxtpnlzie.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.bbcook.cn/Article/details/gomareyzj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/gncmeyxnc.sHtML

[E16] 数字千分位
来源：http://read.share.epnwcf.com/Article/details/ggsdmbqis.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.vehdjk.com/Article/details/gtchodynx.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/ggprrmabp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gogelvsbt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gnyvflbha.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gfrpodfuw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.bbcook.cn/Article/details/gyznjlsww.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/gznfkigsk.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/gmpmbwddv.sHtML

[E17] 首字母大写
来源：http://m.share.fktsv.cn/Article/details/gkadlfnrv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.bbcook.cn/Article/details/gyoxwbrnn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.tarul.cn/Article/details/gwsfecgrz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/ghwqbuvvf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gglsyzaas.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fktsv.cn/Article/details/gtclvuvop.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/ghllsdxvk.sHtML

Ruby: s.capitalize
来源：http://mobile.epnwcf.com/Article/details/gtxmdjjml.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.yfazqb.com/Article/details/gvkppplaj.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.sjlbkw.cn/Article/details/glxxuskhl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/gyyjlfnvd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.yfazqb.com/Article/details/gaksdmebx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gzgvzxifr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gsdeeejta.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gylrrivii.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gdnppiosw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fktsv.cn/Article/details/gwxrxhfmr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/ghhmoocnl.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fktsv.cn/Article/details/ghdijpjvp.sHtML

Py:   s.splitlines()
来源：http://www.blog.bbcook.cn/Article/details/gpsjedzak.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.epnwcf.com/Article/details/gkevqldeu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gequspnvt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gjeoqulhk.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gopmobyug.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fktsv.cn/Article/details/gygzduvos.sHtML

Ruby: s.lines
来源：http://wap.fktsv.cn/Article/details/gsavkdtdg.sHtML

C#:   s.Split('\n')
来源：http://www.blog.sjlbkw.cn/Article/details/goyzpaiuq.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fktsv.cn/Article/details/gdqbbjoyh.sHtML

Py:   if not s:
来源：http://wap.vehdjk.com/Article/details/gqdstpnka.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.epnwcf.com/Article/details/gzncjomqt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gceqdiwcm.sHtML

TS:   if (s === "") {}
来源：http://wap.tarul.cn/Article/details/gdcccfpfh.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fktsv.cn/Article/details/ggtzmrtef.sHtML

Go:   if s == "" {}
来源：http://wap.vehdjk.com/Article/details/gfnrhtbbe.sHtML

Ruby: if s.empty?
来源：http://www.blog.epnwcf.com/Article/details/glhyfbkwz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gsyxpbbpw.sHtML

[E21] 超长截断加省略号
来源：http://mobile.tarul.cn/Article/details/gqyvbtwvr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.vehdjk.com/Article/details/gfhezuqmr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gwilrcafa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gsmxompyw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/grkryqntz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gsilevuyo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/ghmxgcgib.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gsmiudxqd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gqigfmscg.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvqvqapo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/gycakjetw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/goaaufwoh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gaebrfuvv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/gqgapextc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.vehdjk.com/Article/details/gqanlomdt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.epnwcf.com/Article/details/gvuxuvaaz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gtgmzltgw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.bbcook.cn/Article/details/gimfmvysb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gdlcgfglr.sHtML

F. 文件与目录
来源：http://read.share.vehdjk.com/Article/details/gpajagzxz.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/givysupdf.sHtML

[F01] 读取整个文件
来源：http://www.share.epnwcf.com/Article/details/gawncvucf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.vehdjk.com/Article/details/gtzgwjdnf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gjrfthcyw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.epnwcf.com/Article/details/grcduivbh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.bbcook.cn/Article/details/ggunhdpcc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gyvdjdiwf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.tarul.cn/Article/details/gkcvckksr.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gmlqgnobv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gfytaajyn.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/gtqpezesj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.yfazqb.com/Article/details/gnghrfiml.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.yfazqb.com/Article/details/gumvhbmxw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gazrdptig.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/gvuojhota.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gojobwdfq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/gegwhsuzg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.sjlbkw.cn/Article/details/gczwudzio.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.vehdjk.com/Article/details/gxzjngufr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.sjlbkw.cn/Article/details/glbgujlvs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.bbcook.cn/Article/details/gamkgcdor.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/ghodtxyqj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gwxkzljuk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gsegvpotn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.vehdjk.com/Article/details/gtshtrcch.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.epnwcf.com/Article/details/groanykem.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.tarul.cn/Article/details/gnvwffjqx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gtwpcqyrq.sHtML

[F04] 追加写入文件
来源：http://mobile.epnwcf.com/Article/details/gtaaxblck.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gnhbydxkp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/glkdmabgu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gozruprev.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/gwsfqppmx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.yfazqb.com/Article/details/gtdtvtitw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fktsv.cn/Article/details/gjywsajru.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.bbcook.cn/Article/details/gzwtrvuns.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.yfazqb.com/Article/details/gaywnaocq.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.bbcook.cn/Article/details/gunvcykeb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.yfazqb.com/Article/details/gznufogfd.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gunhkxjag.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gryxavnrq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gscsialvw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/guufykhvt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.vehdjk.com/Article/details/gqtvmcidr.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gjranlzky.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.epnwcf.com/Article/details/gvegekpsf.sHtML

[F06] 删除文件
来源：http://blog.vehdjk.com/Article/details/gbyhvhqnb.sHtML

Py:   os.remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/griizmipu.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.yfazqb.com/Article/details/ghcovydji.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/ghcxqcdxc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gowuuxzud.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gbtmtgzjk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gguhsscbd.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fktsv.cn/Article/details/glgnhgcjs.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.tarul.cn/Article/details/gindvzknj.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/gfslwhmrl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gywslklou.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/gwgejtgos.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gontkwiqs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/ggrcjjenl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fktsv.cn/Article/details/glasvdnke.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.tarul.cn/Article/details/gswgjkejw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.epnwcf.com/Article/details/gksctmqui.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fktsv.cn/Article/details/gddscvzqn.sHtML

[F08] 遍历目录
来源：http://m.share.sjlbkw.cn/Article/details/gnmexflio.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.vehdjk.com/Article/details/gpvbmmkeq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fktsv.cn/Article/details/glymzxtsj.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gsgrybtyo.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gymyauhkk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gtmwjsges.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.epnwcf.com/Article/details/geyyavaya.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/geztxlgto.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fktsv.cn/Article/details/grduujpun.sHtML

[F09] 获取文件大小
来源：http://baike.bbcook.cn/Article/details/gzwqenger.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gzhznpisf.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/goewhssnz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/ghfftznfa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gswgtqiji.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gnfzmwkze.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqlspedj.sHtML

Ruby: File.size("a.txt")
来源：http://baike.yfazqb.com/Article/details/gzmwfxqqw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.epnwcf.com/Article/details/gtbbtvexp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fktsv.cn/Article/details/gvirvuxxd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gyvbihors.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.yfazqb.com/Article/details/ghmesyzwh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gejqjlwtp.sHtML

TS:   path.extname("a.txt")
来源：http://3g.vehdjk.com/Article/details/grgyelawz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fktsv.cn/Article/details/gzdjyzipb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gqlgyfzog.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gsnwsuqab.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gryivdncz.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.epnwcf.com/Article/details/gurasmyup.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gayrjeftj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.bbcook.cn/Article/details/gyqqmhvqw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gqikifybg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/glzbrfyzv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/ggxmvdvok.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.yfazqb.com/Article/details/gwqjqgjgd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gaqnkffyr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gotrukkvu.sHtML

[F12] CSV 读写
来源：http://3g.sjlbkw.cn/Article/details/gfmftiiuj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/gzjctitug.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fktsv.cn/Article/details/gptgecrka.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.vehdjk.com/Article/details/gcksklzgn.sHtML

TS:   // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gxouleymi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.epnwcf.com/Article/details/gsbsagcsq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/gegvhptjq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gqhmrdlea.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.yfazqb.com/Article/details/gfilpxtfm.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gznzqjsza.sHtML

G. 面向对象
来源：http://www.m.share.vehdjk.com/Article/details/gmptsyoqr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gugdtqngv.sHtML

[G01] 定义类
来源：http://3g.bbcook.cn/Article/details/gzqxclffu.sHtML

Py:   class User: pass
来源：http://www.m.share.yfazqb.com/Article/details/gujpbxemz.sHtML

PHP:  class User {}
来源：http://www.blog.epnwcf.com/Article/details/gppdtgatx.sHtML

JS:   class User {}
来源：http://m.share.epnwcf.com/Article/details/gnndnishl.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/geoikzrpu.sHtML

Java: class User {}
来源：http://baike.bbcook.cn/Article/details/gtcleftak.sHtML

Go:   type User struct { Name string }
来源：http://read.share.sjlbkw.cn/Article/details/gawrjmfhw.sHtML

Ruby: class User; end
来源：http://m.share.fktsv.cn/Article/details/gwaueqmaa.sHtML

C#:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gvmybdtoq.sHtML

[G02] 构造函数
来源：http://m.share.epnwcf.com/Article/details/gfxvfolbb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/gzfijjozl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.bbcook.cn/Article/details/gdoaibirl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/giuwmpoph.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/gtscmtvpv.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gvrzzxycm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/geasgmitr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fktsv.cn/Article/details/gkavsmdqf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.yfazqb.com/Article/details/giskrders.sHtML

[G03] 实例属性
来源：http://wap.fktsv.cn/Article/details/gjqfvpfpp.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gfyolzpdi.sHtML

PHP:  public string $name = "x";
来源：http://mobile.bbcook.cn/Article/details/gxmlgvpny.sHtML

JS:   this.name = "x";
来源：http://3g.fktsv.cn/Article/details/gsxqjfwmy.sHtML

TS:   name: string = "x";
来源：http://baike.yfazqb.com/Article/details/gbsskvylf.sHtML

Java: private String name;
来源：http://www.m.share.vehdjk.com/Article/details/gfpjmfteq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.vehdjk.com/Article/details/gsjvpxwsh.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/gdmmtieys.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.bbcook.cn/Article/details/guodnsdpi.sHtML

[G04] 定义方法
来源：http://m.share.fktsv.cn/Article/details/gciwghqvu.sHtML

Py:   def greet(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/gerkvklod.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gfydkhlyw.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/ggaytdedx.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gmlepgfwa.sHtML

Java: String greet() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gbokenkqt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gcsaacohd.sHtML

Ruby: def greet; @name; end
来源：http://wap.fktsv.cn/Article/details/gtoudqdiq.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gooujyvgm.sHtML

[G05] 继承
来源：http://baike.vehdjk.com/Article/details/gipicfxic.sHtML

Py:   class Admin(User): pass
来源：http://wap.epnwcf.com/Article/details/gkwmbhxkg.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gblvbcilj.sHtML

JS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gaoxsweie.sHtML

TS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gwaeidlux.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gfrpglncy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.yfazqb.com/Article/details/glcblsika.sHtML

Ruby: class Admin < User; end
来源：http://www.share.vehdjk.com/Article/details/ggaqpdrbl.sHtML

C#:   class Admin : User {}
来源：http://read.share.epnwcf.com/Article/details/gtysaextx.sHtML

[G06] 重写方法
来源：http://www.share.sjlbkw.cn/Article/details/giqcwnzic.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.vehdjk.com/Article/details/glbhituqy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gjjyxazzq.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gtkvufmmt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gneejhvnv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gvfqgcaly.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fktsv.cn/Article/details/gpxtpmugr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/grxesqoma.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fktsv.cn/Article/details/gifqehhua.sHtML

[G07] 调用父类方法
来源：http://www.share.fktsv.cn/Article/details/gnjolzigx.sHtML

Py:   super().greet()
来源：http://www.blog.sjlbkw.cn/Article/details/gtrhzwqin.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/gvjqulnil.sHtML

JS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/grvhmtrbg.sHtML

TS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/giiztklos.sHtML

Java: super.greet();
来源：http://mobile.vehdjk.com/Article/details/ggxpnsgyf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gsagvbbrk.sHtML

Ruby: super
来源：http://blog.fktsv.cn/Article/details/gggbuamgg.sHtML

C#:   base.Greet();
来源：http://www.m.share.tarul.cn/Article/details/geabyykvf.sHtML

[G08] 静态方法与属性
来源：http://www.share.vehdjk.com/Article/details/ghjeargow.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fktsv.cn/Article/details/gjkafatzl.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gbhvkclei.sHtML

JS:   static f() {}
来源：http://read.share.epnwcf.com/Article/details/gjsjfiehh.sHtML

TS:   static f(): void {}
来源：http://www.share.yfazqb.com/Article/details/gxjvmhwlu.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/guavqtvuh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.vehdjk.com/Article/details/gdbgfvpfo.sHtML

Ruby: def self.f; end
来源：http://www.m.share.tarul.cn/Article/details/gzehixytk.sHtML

C#:   public static void F() {}
来源：http://www.m.share.bbcook.cn/Article/details/giukvluby.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.epnwcf.com/Article/details/gnrokdfcx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.sjlbkw.cn/Article/details/gaunscpcm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.epnwcf.com/Article/details/ggbpigkes.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fktsv.cn/Article/details/gvkshzyse.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.tarul.cn/Article/details/gqypudqwz.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.bbcook.cn/Article/details/gqdhzajar.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.vehdjk.com/Article/details/gmyjvepzf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.yfazqb.com/Article/details/gfwkeaxdo.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.epnwcf.com/Article/details/grylmfrll.sHtML


<!-- 参考信息 -->