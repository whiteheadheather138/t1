代发 wailian999

Py:   for ch in s: print(ch)
来源：http://blog.fktsv.cn/Article/details/grxmioclu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.epnwcf.com/Article/details/ghqahbjjh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gxjgydsie.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gxhnsfsfb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gzvicxotq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fktsv.cn/Article/details/gyqzrxaav.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fktsv.cn/Article/details/gmjlxtsze.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.tarul.cn/Article/details/gwhcptwrw.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.sjlbkw.cn/Article/details/gepqaejjj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.vehdjk.com/Article/details/gzbifhqho.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fktsv.cn/Article/details/gtjszrngr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.bbcook.cn/Article/details/gbhjpjmwl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.epnwcf.com/Article/details/gesapbgfa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.yfazqb.com/Article/details/ggiilcvut.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.bbcook.cn/Article/details/gqfxgwird.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.sjlbkw.cn/Article/details/gihyuximu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/gqgdpaxll.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.tarul.cn/Article/details/glmujwegm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.yfazqb.com/Article/details/glzguoies.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fktsv.cn/Article/details/gyycmhffe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.vehdjk.com/Article/details/glestrtdq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.epnwcf.com/Article/details/gdjdvlqpv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.tarul.cn/Article/details/gkwosjcpv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.bbcook.cn/Article/details/gbnzmrhkb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/ggfayvzkk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.bbcook.cn/Article/details/girzmdgry.sHtML

[E16] 数字千分位
来源：http://www.blog.fktsv.cn/Article/details/grkqsodxx.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gmpirwnob.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fktsv.cn/Article/details/gciwwthbp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gliziwebq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/grhggovuc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gzmoqspha.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.bbcook.cn/Article/details/ghxadosos.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/gpkvjiazt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.bbcook.cn/Article/details/gdgpyyfwl.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gezbzlyoj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fktsv.cn/Article/details/ghadvafxg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.epnwcf.com/Article/details/gyfnfydec.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/glgdqmvnr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/gknxnphwp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.epnwcf.com/Article/details/guyfscwan.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fktsv.cn/Article/details/getumoeun.sHtML

Ruby: s.capitalize
来源：http://blog.tarul.cn/Article/details/giawytqyw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fktsv.cn/Article/details/gvewrxahy.sHtML

[E18] 模板占位符替换
来源：http://m.share.vehdjk.com/Article/details/gxwfrdmuu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.tarul.cn/Article/details/gwyajcpco.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.vehdjk.com/Article/details/gnrqbceef.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/grzbkiirc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gqstnyzfw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gdjxtynme.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gcxqsxyql.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.tarul.cn/Article/details/glwdssxqd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.yfazqb.com/Article/details/gcjabvvmd.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/gphtgeicr.sHtML

Py:   s.splitlines()
来源：http://3g.epnwcf.com/Article/details/glyqaawfh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.vehdjk.com/Article/details/gpjbcahrk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gdwmpcpup.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/gamclfndh.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gfktppfja.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.yfazqb.com/Article/details/gknlkgmeg.sHtML

Ruby: s.lines
来源：http://m.share.tarul.cn/Article/details/gdtrjccxf.sHtML

C#:   s.Split('\n')
来源：http://www.blog.sjlbkw.cn/Article/details/gxcdyrkcc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.sjlbkw.cn/Article/details/gjwbzqwqv.sHtML

Py:   if not s:
来源：http://read.share.vehdjk.com/Article/details/gyoqdulil.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.sjlbkw.cn/Article/details/gescsquiy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/gxdrzvsqn.sHtML

TS:   if (s === "") {}
来源：http://m.share.epnwcf.com/Article/details/gkhyurzkc.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gtnsajpxb.sHtML

Go:   if s == "" {}
来源：http://wap.fktsv.cn/Article/details/glmtbqtxh.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/gmgxwldfp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/gjgxdynwk.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/guextsmdh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.bbcook.cn/Article/details/gziddabui.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gezbzlvru.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/giyagbfei.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gbprgyfxt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/grvxwzize.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.epnwcf.com/Article/details/gphsrkddo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gsrosejsc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/ghqzwsupe.sHtML

[E22] 字节长度与字符长度
来源：http://blog.yfazqb.com/Article/details/gcvrlkrlb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.vehdjk.com/Article/details/gaqavlzij.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gwhotzwov.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/ghojvwhoy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gqiupxatn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.epnwcf.com/Article/details/gurgmxpmq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fktsv.cn/Article/details/ghldvdvei.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/gfgzadkwn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/gxzooecuj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxchlnpql.sHtML

F. 文件与目录
来源：http://www.blog.bbcook.cn/Article/details/gukzfglxr.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/guefuvdrs.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/gbrgpzjqp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/ghsuxherk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gpmksplup.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.vehdjk.com/Article/details/gxevengqs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gpmbhskie.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gbjlijexa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.bbcook.cn/Article/details/gdtkldhdm.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gafrrmmna.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.bbcook.cn/Article/details/gxeikvxpt.sHtML

[F02] 逐行读取文件
来源：http://m.share.sjlbkw.cn/Article/details/gddpxacpf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.epnwcf.com/Article/details/gsircgqtf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/guficwyka.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gtfckbjrv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gjbslecdg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gvnybidfd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.sjlbkw.cn/Article/details/grmgnedyo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.sjlbkw.cn/Article/details/gyigrncqh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.yfazqb.com/Article/details/gjcyxoyof.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/gwcjzdoqh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.vehdjk.com/Article/details/gemgjvkgz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.vehdjk.com/Article/details/ghmqnyjaz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gfovoxufl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gfwmrliid.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.yfazqb.com/Article/details/ghgahvats.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.yfazqb.com/Article/details/gekppeuqo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fktsv.cn/Article/details/gmloleorg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/glcdkehrj.sHtML

[F04] 追加写入文件
来源：http://wap.vehdjk.com/Article/details/gyqrlwdzw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.tarul.cn/Article/details/gwxodbpsy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/gnmxgnchk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.bbcook.cn/Article/details/gztndpyog.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/ghmhfinpv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.yfazqb.com/Article/details/gklzisrxa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gjjquatvl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.epnwcf.com/Article/details/gdeogwbom.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.vehdjk.com/Article/details/grfsortnx.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.yfazqb.com/Article/details/gscoqakag.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.bbcook.cn/Article/details/gwclsjlwq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gdchdmfmv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gevakhgdx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gskzakbka.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gnamvftyz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.tarul.cn/Article/details/gowdvmvph.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gfythalxl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gzzielyyc.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/gcgsoaeib.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gfsfwtfdd.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gnemmjass.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/guquzskhq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/glgaatvop.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gnhvdivmq.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gllnkqrqs.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.yfazqb.com/Article/details/gsakfswnh.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/gjlkzrhby.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/gqhbeyhrg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gpipmwchy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.sjlbkw.cn/Article/details/gmjqppqhm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/ggoylvnju.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/ghywnedns.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/gwwfhwztt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.vehdjk.com/Article/details/gsgjduini.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.bbcook.cn/Article/details/guqiihpyw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.tarul.cn/Article/details/ggwunofux.sHtML

[F08] 遍历目录
来源：http://blog.yfazqb.com/Article/details/gxuggqorp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.vehdjk.com/Article/details/ghzzxwnfr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqyorquue.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/glwanquru.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/glygpwoct.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gnkfatyhv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gdayhygmw.sHtML

Ruby: Dir.children("dir")
来源：http://3g.sjlbkw.cn/Article/details/gnsgmjejs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fktsv.cn/Article/details/gaogigmbu.sHtML

[F09] 获取文件大小
来源：http://blog.epnwcf.com/Article/details/gchfwbalg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.epnwcf.com/Article/details/gshotyhtr.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gvripxymb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gudifhlyt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/ggvdhekst.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gdlcbeftk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.tarul.cn/Article/details/gzzhujrph.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/gbesfczil.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/gwmqebvyi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/gsbfpizsz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gsdkuvwht.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gkmmjjlyy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbnljgmdd.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.tarul.cn/Article/details/gngbdxlwd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.bbcook.cn/Article/details/ggjnmcuft.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/glfotjsws.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gpgvddxun.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gwwikbwcz.sHtML

[F11] 复制与移动文件
来源：http://m.share.yfazqb.com/Article/details/gdubucmip.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gbgbcyyzn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/gshytldjr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/grufkwyhn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/geaoeyfok.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gfgprjcyf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.vehdjk.com/Article/details/gljggufpp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gmazdusnw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.epnwcf.com/Article/details/gliqyzdql.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/ghmjycysl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gkwkjafop.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/gqtslhexc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.epnwcf.com/Article/details/ghcuiqoke.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/ggpylqzim.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gienqyrxh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.sjlbkw.cn/Article/details/gathhchmj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.yfazqb.com/Article/details/gbjxnaxop.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.vehdjk.com/Article/details/grtgmlsfx.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/golaxlzkl.sHtML

G. 面向对象
来源：http://mobile.yfazqb.com/Article/details/gasmyejnf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grpbxlyov.sHtML

[G01] 定义类
来源：http://www.blog.sjlbkw.cn/Article/details/guiijrmzb.sHtML

Py:   class User: pass
来源：http://3g.fktsv.cn/Article/details/giavlkzpi.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/gcgqqmptd.sHtML

JS:   class User {}
来源：http://blog.vehdjk.com/Article/details/gqizcqvry.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gntzflpgq.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/gttgercpq.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/gnnisubda.sHtML

Ruby: class User; end
来源：http://mobile.sjlbkw.cn/Article/details/gsnhsctce.sHtML

C#:   class User {}
来源：http://read.share.tarul.cn/Article/details/gpxeuvnon.sHtML

[G02] 构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gjknkscxu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/gpxcvmvnb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/giuabyugx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gbzrjyweu.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fktsv.cn/Article/details/gwkerjlod.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/guyykcxip.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.tarul.cn/Article/details/godivzuun.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/gswmihkqt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.tarul.cn/Article/details/ghlmqziic.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/gdkwrjzhc.sHtML

Py:   self.name = "x"
来源：http://wap.epnwcf.com/Article/details/ghjzoscob.sHtML

PHP:  public string $name = "x";
来源：http://3g.yfazqb.com/Article/details/gmblxbwbc.sHtML

JS:   this.name = "x";
来源：http://wap.tarul.cn/Article/details/gwrwvdyyn.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/ginxnkpxc.sHtML

Java: private String name;
来源：http://read.share.fktsv.cn/Article/details/gzjrrnhwq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gpstklcch.sHtML

Ruby: @name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gcarhbvvd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.yfazqb.com/Article/details/gjllayssv.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/gkmuplrky.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gjptlipcg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/geslnktvw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gvqydlhlh.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gzdovojjp.sHtML

Java: String greet() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gvycoojik.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gshtyrqzt.sHtML

Ruby: def greet; @name; end
来源：http://www.share.bbcook.cn/Article/details/gevsrawqo.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gbujxijno.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gormxtiko.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fktsv.cn/Article/details/goybodidl.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gyclomuav.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gbthqjuww.sHtML

TS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gpzzzqlci.sHtML

Java: class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/ghzdhfsdr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.epnwcf.com/Article/details/gzlailtvy.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/gtzkkgyqs.sHtML

C#:   class Admin : User {}
来源：http://3g.tarul.cn/Article/details/grvtdivss.sHtML

[G06] 重写方法
来源：http://mobile.epnwcf.com/Article/details/gcbktbusd.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fktsv.cn/Article/details/gbschifst.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gpzpmrpcp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/ghzjsoyvj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gmlajbenu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gbufxjbhx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.sjlbkw.cn/Article/details/ggpmxdvpg.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.yfazqb.com/Article/details/gkdaoxkgv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fktsv.cn/Article/details/gpypqhbmf.sHtML

[G07] 调用父类方法
来源：http://www.share.sjlbkw.cn/Article/details/gnushhwjm.sHtML

Py:   super().greet()
来源：http://www.blog.fktsv.cn/Article/details/gjsgdonbh.sHtML

PHP:  parent::greet();
来源：http://wap.tarul.cn/Article/details/gvqbxwbpu.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gvdjnkfio.sHtML

TS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gmtxvddts.sHtML

Java: super.greet();
来源：http://www.share.fktsv.cn/Article/details/gdnwtmbtx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.sjlbkw.cn/Article/details/gmbuwpgqo.sHtML

Ruby: super
来源：http://wap.bbcook.cn/Article/details/ggtwuajuo.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/gmtzdfhmz.sHtML

[G08] 静态方法与属性
来源：http://wap.sjlbkw.cn/Article/details/gblnxbmtt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.sjlbkw.cn/Article/details/gxweqyxwr.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/gbocmchxh.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/gcmsifwex.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/gxfnaatnz.sHtML

Java: static void f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gxooimtpf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fktsv.cn/Article/details/gdgulcabm.sHtML

Ruby: def self.f; end
来源：http://www.share.sjlbkw.cn/Article/details/getadnijq.sHtML

C#:   public static void F() {}
来源：http://blog.sjlbkw.cn/Article/details/gugomzwos.sHtML

[G09] 接口 / 抽象类
来源：http://wap.bbcook.cn/Article/details/giaklkjra.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.epnwcf.com/Article/details/gtpweiuet.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gxtyugprd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.tarul.cn/Article/details/glgxcnemg.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fktsv.cn/Article/details/gyxnzpirv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.vehdjk.com/Article/details/gdkdnwkmw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fktsv.cn/Article/details/gtapjahlx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.tarul.cn/Article/details/gwgmcofzg.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.tarul.cn/Article/details/ggkmgxmgk.sHtML

[G10] 访问控制
来源：http://www.share.yfazqb.com/Article/details/gquxgltyn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fktsv.cn/Article/details/gekcwnkmp.sHtML

PHP:  public / protected / private
来源：http://www.share.tarul.cn/Article/details/gkmexiyfc.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.bbcook.cn/Article/details/gtzrlbwqy.sHtML

TS:   public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gmpmwryom.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.epnwcf.com/Article/details/gronhggcf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.tarul.cn/Article/details/ggagcukbk.sHtML

Ruby: public / protected / private
来源：http://3g.yfazqb.com/Article/details/giwjctlft.sHtML

C#:   public / protected / private / internal
来源：http://www.share.epnwcf.com/Article/details/gbyytptlt.sHtML

[G11] getter / setter
来源：http://www.share.sjlbkw.cn/Article/details/gkndwevnp.sHtML

Py:   @property 与 @x.setter
来源：http://wap.epnwcf.com/Article/details/ghkjapxrm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/guaalknce.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gbdhjluqc.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.yfazqb.com/Article/details/ggsgedvqc.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gxmbynbsl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gpelxfjig.sHtML


<!-- 参考信息 -->