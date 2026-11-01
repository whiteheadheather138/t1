代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.blog.yfazqb.com/Article/details/gkebxdzes.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.vehdjk.com/Article/details/gzvsefqzz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gpgjwqghj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gtygqvdew.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gjyucjhgl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.epnwcf.com/Article/details/gojwjrsun.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/gomwsolbt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gxngxuyit.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.yfazqb.com/Article/details/gocfhegyc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.bbcook.cn/Article/details/gbotwviqy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.vehdjk.com/Article/details/gcoyyutmj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.epnwcf.com/Article/details/gmuccjrwo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fktsv.cn/Article/details/gaooxxnyu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.epnwcf.com/Article/details/gdsagapao.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/glkeavjtl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.yfazqb.com/Article/details/ghwlhvlyn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gvmtxnfze.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/gvnxedubl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.epnwcf.com/Article/details/gvudxzjym.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.sjlbkw.cn/Article/details/grqghxeau.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.sjlbkw.cn/Article/details/gsrcnadvt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gdhqlcicc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/gbdcuvkyd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.vehdjk.com/Article/details/gwjtpxcih.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gklcdajsq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fktsv.cn/Article/details/ggciphvhh.sHtML

[E16] 数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/ggiydbrfz.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gfabmekuy.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.tarul.cn/Article/details/gainyyqjy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/grrxfmmqm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/gthnuybtg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvwlzlqv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fktsv.cn/Article/details/gjgvqlurm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/gbeywgxkw.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.tarul.cn/Article/details/gllnwctxg.sHtML

[E17] 首字母大写
来源：http://m.share.epnwcf.com/Article/details/gfhlonzmg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.yfazqb.com/Article/details/gardvikuj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/gzamsoztm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/girybqmgv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/glmwnxysa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fktsv.cn/Article/details/gyfnjctjr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/ggawehxcx.sHtML

Ruby: s.capitalize
来源：http://mobile.fktsv.cn/Article/details/gnqxvvpra.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fktsv.cn/Article/details/gkvxlixiy.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gakgtwptd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.bbcook.cn/Article/details/gfvduesqi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fktsv.cn/Article/details/gbhahpyzn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gaynzgabj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gqovjuwmp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gmcjsnhpw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.yfazqb.com/Article/details/gjpjycyjn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.bbcook.cn/Article/details/gzfgjmiqj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.tarul.cn/Article/details/ggznwdoir.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.yfazqb.com/Article/details/gxthczomc.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/gfqnzjiky.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.tarul.cn/Article/details/gzfgykbub.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gpcmewxpq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gzqruydjw.sHtML

Java: s.lines().toList()
来源：http://m.share.sjlbkw.cn/Article/details/ggbihzdiy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.epnwcf.com/Article/details/gtuemuxqy.sHtML

Ruby: s.lines
来源：http://baike.sjlbkw.cn/Article/details/gwdwtoaoo.sHtML

C#:   s.Split('\n')
来源：http://www.blog.sjlbkw.cn/Article/details/geocloeaj.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.vehdjk.com/Article/details/gvxmrulra.sHtML

Py:   if not s:
来源：http://baike.tarul.cn/Article/details/grkbdsqtk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.epnwcf.com/Article/details/gvrbrsizc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.bbcook.cn/Article/details/ggmysouqy.sHtML

TS:   if (s === "") {}
来源：http://mobile.fktsv.cn/Article/details/gqshpxbch.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.vehdjk.com/Article/details/grsrawouw.sHtML

Go:   if s == "" {}
来源：http://www.share.bbcook.cn/Article/details/gtcbazybl.sHtML

Ruby: if s.empty?
来源：http://www.share.vehdjk.com/Article/details/gmtawjimb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/giqrbnfdl.sHtML

[E21] 超长截断加省略号
来源：http://m.share.tarul.cn/Article/details/gmjztuzwg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/giwajrsih.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.epnwcf.com/Article/details/guuetqmjs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gbokrkhis.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/glccveapi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gdazbycje.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.vehdjk.com/Article/details/gpwldrtdd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/grsprargw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.tarul.cn/Article/details/giugyxiwg.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.epnwcf.com/Article/details/gmbqoglkq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.vehdjk.com/Article/details/gqdjozejl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gmdkqeyvg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gifmfuyla.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gxgxopwfc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.tarul.cn/Article/details/gbpbzkpab.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.bbcook.cn/Article/details/giipwroml.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/gfwjnqbpd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.bbcook.cn/Article/details/gnluzsjzp.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gtsqhssun.sHtML

F. 文件与目录
来源：http://read.share.vehdjk.com/Article/details/gwmfacspm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gubfkpwts.sHtML

[F01] 读取整个文件
来源：http://wap.fktsv.cn/Article/details/gupjholyy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.epnwcf.com/Article/details/gktzqchtg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/grsmzqdrz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.sjlbkw.cn/Article/details/gpbtemqjl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gucggukrd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gpsasjbhj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fktsv.cn/Article/details/gakobulla.sHtML

Ruby: File.read("a.txt")
来源：http://3g.tarul.cn/Article/details/gltgrjfoq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.bbcook.cn/Article/details/gxfgjvwml.sHtML

[F02] 逐行读取文件
来源：http://blog.sjlbkw.cn/Article/details/gauspgczz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fktsv.cn/Article/details/gljfeuvse.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.vehdjk.com/Article/details/gscdfbclg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gbzqvsnlw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gtmfymtxs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gtllgsalj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.epnwcf.com/Article/details/gobgyxadh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.vehdjk.com/Article/details/gtpohuook.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.yfazqb.com/Article/details/gjskiqzwp.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.epnwcf.com/Article/details/gpvkquilh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.bbcook.cn/Article/details/gubjwxbcm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gswpjsuob.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/geevgvurl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gdrxqaoxv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.tarul.cn/Article/details/gjzkajeap.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.vehdjk.com/Article/details/gvpvopywi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.epnwcf.com/Article/details/ggrdiyzvi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gwcoxinwy.sHtML

[F04] 追加写入文件
来源：http://3g.vehdjk.com/Article/details/ghllxfvoh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gwabqwtxw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.sjlbkw.cn/Article/details/gthumzmfx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/gmkvtgpie.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gkmdhghrg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fktsv.cn/Article/details/gbqudkhxt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/goszfpgyu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fktsv.cn/Article/details/guljavpur.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.yfazqb.com/Article/details/gqkectkym.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.epnwcf.com/Article/details/gqapghlat.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.epnwcf.com/Article/details/gyrbmeljq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gxmdnfsky.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gnmbfxfnx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gmrscynzj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gcntpdaoj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.vehdjk.com/Article/details/glspffczh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gxloqkbjq.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.tarul.cn/Article/details/gqfbtiwru.sHtML

[F06] 删除文件
来源：http://www.m.share.fktsv.cn/Article/details/gzbeejqqo.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gcskzhwri.sHtML

PHP:  unlink("a.txt");
来源：http://baike.vehdjk.com/Article/details/gjaverkol.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gjgzhuqpa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gcjwpkpuq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gowydebsq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gqkckgxvh.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fktsv.cn/Article/details/glfjeviar.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.tarul.cn/Article/details/gwdpxftpa.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fktsv.cn/Article/details/gjaexjhwx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gujhliifg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.epnwcf.com/Article/details/gavvywwty.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gwbxrmrgl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/gfwfklykh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.vehdjk.com/Article/details/ghadgqgwg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.vehdjk.com/Article/details/ghkoqxdif.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/gbwwthhdy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gruoulmig.sHtML

[F08] 遍历目录
来源：http://3g.bbcook.cn/Article/details/gsmgfremf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.vehdjk.com/Article/details/gwzbzkpoc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.yfazqb.com/Article/details/gjxpnpqpn.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/grkgzknvk.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gzozndbbj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gkzeelewe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gecyxywwf.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/gxdmodvwh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.tarul.cn/Article/details/gizllkpev.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/gfyikrbpf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fktsv.cn/Article/details/ghnygnuqn.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gmbbgxjmc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/ghaqognmi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gaplzxfip.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gmtwfghmz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.sjlbkw.cn/Article/details/gspgrallr.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gydlkyizt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.tarul.cn/Article/details/gpalpwckl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.bbcook.cn/Article/details/gskvpfiqc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gfcasfmro.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.vehdjk.com/Article/details/gfsxmqgtt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gacshvjmy.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ggfuukvvw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fktsv.cn/Article/details/giqzisjhx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/guckzajvc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gumdsjgsm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gnhajpeyg.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/glmamkvmz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gamteydra.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.yfazqb.com/Article/details/griwqypkv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gqqyfccws.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/glpwukana.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.vehdjk.com/Article/details/gprljsisu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.epnwcf.com/Article/details/gmxymkzdf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gowxapowp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.bbcook.cn/Article/details/gedntklmy.sHtML

[F12] CSV 读写
来源：http://read.share.bbcook.cn/Article/details/gmspzvsat.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.epnwcf.com/Article/details/gbznkhnvo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.yfazqb.com/Article/details/gbfbjsszu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/gucgnhoaf.sHtML

TS:   // 同上
来源：http://read.share.sjlbkw.cn/Article/details/gepndqvze.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.sjlbkw.cn/Article/details/gaffozbbo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fktsv.cn/Article/details/gumemblab.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gltjmeuxn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.yfazqb.com/Article/details/gnfhvwgqd.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gimegvfxx.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/gpahlzzxr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gwyrbhann.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/gistcigdz.sHtML

Py:   class User: pass
来源：http://baike.bbcook.cn/Article/details/glbywcywv.sHtML

PHP:  class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gujsnmjjr.sHtML

JS:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gecyiprxd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.epnwcf.com/Article/details/gqxolwyoo.sHtML

Java: class User {}
来源：http://blog.fktsv.cn/Article/details/gwhiewjmt.sHtML

Go:   type User struct { Name string }
来源：http://mobile.vehdjk.com/Article/details/gjjawowgs.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/gkwljqvjv.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gpdwhlgwt.sHtML

[G02] 构造函数
来源：http://m.share.vehdjk.com/Article/details/gonebtqcl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/gerooracu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fktsv.cn/Article/details/gtkgmhrmk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gmooxfpho.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.sjlbkw.cn/Article/details/gloqiumjg.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gosyrtsno.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gmsoznhln.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.epnwcf.com/Article/details/gujqhidke.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.yfazqb.com/Article/details/gwwlpysyb.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/gophbgqxk.sHtML

Py:   self.name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gesxlbjji.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gqekcesdt.sHtML

JS:   this.name = "x";
来源：http://read.share.yfazqb.com/Article/details/gtmywiwpb.sHtML

TS:   name: string = "x";
来源：http://blog.fktsv.cn/Article/details/gletvifvu.sHtML

Java: private String name;
来源：http://mobile.epnwcf.com/Article/details/giiymchss.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gbgexxjju.sHtML

Ruby: @name = "x"
来源：http://wap.epnwcf.com/Article/details/gligxkqsc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/gbjizzdgk.sHtML

[G04] 定义方法
来源：http://baike.tarul.cn/Article/details/gtgoreszb.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/gssmpdhai.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gowezvzvg.sHtML

JS:   greet() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gvecllkhc.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/ggrtbuvcc.sHtML

Java: String greet() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gwqqcvnue.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gzthnqioc.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gkqsmwzbf.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.vehdjk.com/Article/details/gksejgpeb.sHtML

[G05] 继承
来源：http://wap.fktsv.cn/Article/details/gytbkcacq.sHtML

Py:   class Admin(User): pass
来源：http://blog.vehdjk.com/Article/details/grlsuhzlg.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gjetjwilf.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gdrjbujyt.sHtML

TS:   class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gohqsqlpx.sHtML

Java: class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gstzekiub.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.vehdjk.com/Article/details/gigdfoofy.sHtML

Ruby: class Admin < User; end
来源：http://mobile.yfazqb.com/Article/details/gqtygraxn.sHtML

C#:   class Admin : User {}
来源：http://blog.vehdjk.com/Article/details/gwgjnuvpv.sHtML

[G06] 重写方法
来源：http://m.share.tarul.cn/Article/details/gloowjxtc.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.sjlbkw.cn/Article/details/gmgqliacw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/ghmzunwjk.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/grcbcybzo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gdylapwwa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gjvqfbxgl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.yfazqb.com/Article/details/gvpwkecyd.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.tarul.cn/Article/details/gxlkjvbkf.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.bbcook.cn/Article/details/gxyxvjnhh.sHtML

[G07] 调用父类方法
来源：http://read.share.epnwcf.com/Article/details/gxzuejafn.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/gkewqdwbu.sHtML

PHP:  parent::greet();
来源：http://m.share.fktsv.cn/Article/details/gpkhxqglj.sHtML

JS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gcbpvrhsy.sHtML

TS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/glshaewuw.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/ghcfdmlca.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gdmearscn.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjurwfty.sHtML

C#:   base.Greet();
来源：http://3g.bbcook.cn/Article/details/gfbvtjdii.sHtML

[G08] 静态方法与属性
来源：http://www.share.fktsv.cn/Article/details/gevhievqy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.yfazqb.com/Article/details/gfgfabwqf.sHtML

PHP:  public static function f() {}
来源：http://www.share.yfazqb.com/Article/details/gqrwpcrih.sHtML

JS:   static f() {}
来源：http://read.share.vehdjk.com/Article/details/gmfrzbrlw.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fktsv.cn/Article/details/gesybunae.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/gjpxmilvv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.epnwcf.com/Article/details/gkgtgchvy.sHtML

Ruby: def self.f; end
来源：http://3g.epnwcf.com/Article/details/gcmyrqjzi.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gdnajjsqg.sHtML

[G09] 接口 / 抽象类
来源：http://blog.yfazqb.com/Article/details/gzqbibufr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/gikdkcmdt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.bbcook.cn/Article/details/gsiqleskb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.tarul.cn/Article/details/gsmpkeins.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/goxhxcisy.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gdcksdfwl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/gzdnrzypt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.tarul.cn/Article/details/ggslqrcjx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fktsv.cn/Article/details/gbwdqqvrn.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/guknjqtqh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuwzjkxv.sHtML

PHP:  public / protected / private
来源：http://3g.bbcook.cn/Article/details/gzqebqcqc.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.epnwcf.com/Article/details/gkznjdxrh.sHtML

TS:   public / protected / private
来源：http://3g.tarul.cn/Article/details/gefctyfoq.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.vehdjk.com/Article/details/gzyjqhmvf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.sjlbkw.cn/Article/details/grhdorxcx.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gjgrxecho.sHtML

C#:   public / protected / private / internal
来源：http://mobile.sjlbkw.cn/Article/details/gdldtbqfr.sHtML

[G11] getter / setter
来源：http://www.m.share.tarul.cn/Article/details/goegegnhc.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/gjwisxkuj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gfmytkmbc.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gqcmtcrlu.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gzycffgdd.sHtML

Java: public String getName() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gnmpbptgm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gioscgnaz.sHtML


<!-- 参考信息 -->