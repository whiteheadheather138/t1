代发 wailian999

JS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gzjelhfue.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gfpibecii.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.tarul.cn/Article/details/gjasgrwqg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/gihszdomv.sHtML

Ruby: s.reverse
来源：http://blog.sjlbkw.cn/Article/details/gjomldacx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gdyhctfgj.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.bbcook.cn/Article/details/gnamtzawd.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gatsghmgj.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.sjlbkw.cn/Article/details/goqcfoyig.sHtML

JS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gqmnixxla.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gxaimihth.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.bbcook.cn/Article/details/gdycasgqg.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.epnwcf.com/Article/details/gedaoigah.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/gzjzfwnoe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.tarul.cn/Article/details/grxtwekzg.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/gqabekqrv.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/gjtlvvwkl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fktsv.cn/Article/details/griulymbv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gxikdaucf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gqffzzrwp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.yfazqb.com/Article/details/grhvyzhzc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.yfazqb.com/Article/details/gdmsyhnao.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.epnwcf.com/Article/details/gwhvaanwm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/gtfyvvoof.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.epnwcf.com/Article/details/gxgccsalh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.sjlbkw.cn/Article/details/gaaftrqlq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gfmuhyoif.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.sjlbkw.cn/Article/details/gsdtcdwwf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gpvbtnhqs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.tarul.cn/Article/details/glallyufy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.yfazqb.com/Article/details/gnifqpiia.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/gzwqkrgpl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.epnwcf.com/Article/details/ggqudlevo.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fktsv.cn/Article/details/gdiarhvft.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fktsv.cn/Article/details/gxkjfxrox.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fktsv.cn/Article/details/gjhvrukxx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggiqhivpz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gzcxqcugq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.epnwcf.com/Article/details/gakbvzzan.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fktsv.cn/Article/details/gdcowrgba.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.vehdjk.com/Article/details/gcgqwifdf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fktsv.cn/Article/details/gmtknxisi.sHtML

[E16] 数字千分位
来源：http://blog.bbcook.cn/Article/details/gniehoakj.sHtML

Py:   f"{1234567:,}"
来源：http://blog.epnwcf.com/Article/details/grvcyzrxt.sHtML

PHP:  number_format(1234567);
来源：http://baike.bbcook.cn/Article/details/gxxbifejb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gzrljqllu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/guxgnuyjk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.tarul.cn/Article/details/gxxwjvvzb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gkwoscwjf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.bbcook.cn/Article/details/gduevmjrg.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.epnwcf.com/Article/details/genbgjaad.sHtML

[E17] 首字母大写
来源：http://baike.vehdjk.com/Article/details/gkrgzhalk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.bbcook.cn/Article/details/guqzarofg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/gziumxlxf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gmglljwpr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gndqodhnx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.tarul.cn/Article/details/gnluxpojm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/goqbszigp.sHtML

Ruby: s.capitalize
来源：http://www.m.share.epnwcf.com/Article/details/gqbkqgwaj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.vehdjk.com/Article/details/gawvfymgu.sHtML

[E18] 模板占位符替换
来源：http://wap.tarul.cn/Article/details/gzjlisxhz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.bbcook.cn/Article/details/gzuaidmfz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.epnwcf.com/Article/details/gikprcjms.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gdnxnrmbk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gdaxenhde.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gfbuiaqqy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gwgenwfmi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.yfazqb.com/Article/details/gjsjqmqbn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.sjlbkw.cn/Article/details/gdkllxsks.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.vehdjk.com/Article/details/gphdhfnro.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/ggcwtrueh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gwnshjyfz.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/glfweiojy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gszorbaza.sHtML

Java: s.lines().toList()
来源：http://blog.yfazqb.com/Article/details/gvhrdthma.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.yfazqb.com/Article/details/gdtvgcsdl.sHtML

Ruby: s.lines
来源：http://www.share.vehdjk.com/Article/details/gqluvcnvf.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fktsv.cn/Article/details/gdsimyqip.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.tarul.cn/Article/details/gapjtiohd.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/gqfdhhatw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.tarul.cn/Article/details/gbtaygqyl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.bbcook.cn/Article/details/gfmumwhkg.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/gdjlmohpz.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/gsrouqrhr.sHtML

Go:   if s == "" {}
来源：http://www.blog.yfazqb.com/Article/details/goyrcdjoj.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/ghqgjgsgm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.epnwcf.com/Article/details/ggjbkpfsb.sHtML

[E21] 超长截断加省略号
来源：http://baike.epnwcf.com/Article/details/gbdjshwnd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.bbcook.cn/Article/details/gqcdjkbpb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gvufcyahu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gjrgyzozx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gabamzpgx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/ghzbwarxl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.vehdjk.com/Article/details/guaxteueg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/ggngtjvqt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/grpadxont.sHtML

[E22] 字节长度与字符长度
来源：http://baike.vehdjk.com/Article/details/gjoftjutz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.vehdjk.com/Article/details/gqyxwtfzt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gtsufkpjq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/glsucvdkw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gmdsegtsm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fktsv.cn/Article/details/gxjcrwfma.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/ggxhqymoa.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gvsguqygt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.vehdjk.com/Article/details/glogatlaj.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gizfczvce.sHtML

F. 文件与目录
来源：http://blog.tarul.cn/Article/details/gozgtinbw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gtdpexbxv.sHtML

[F01] 读取整个文件
来源：http://baike.tarul.cn/Article/details/gvkmtwygu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.vehdjk.com/Article/details/gzfogbgpq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gmgsbtrpz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.epnwcf.com/Article/details/gcnutxorx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gqomgqbeh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/ggoumxiof.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fktsv.cn/Article/details/gewoaaqye.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/gurgfciph.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gawrvfmgo.sHtML

[F02] 逐行读取文件
来源：http://baike.yfazqb.com/Article/details/gitnflxqm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.vehdjk.com/Article/details/gazhepapu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.sjlbkw.cn/Article/details/gjuqqfyre.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/ggdhgcqdn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gldpzgwlr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/gmjykgrig.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.bbcook.cn/Article/details/gzkxjkuvr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/ggllsoims.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fktsv.cn/Article/details/gmamyiwrf.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fktsv.cn/Article/details/ghhngcdwc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.epnwcf.com/Article/details/gnsegyefy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gqzupjyjr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gwvrwayna.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/gjbmijwbz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.tarul.cn/Article/details/gaikeylbe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.vehdjk.com/Article/details/gjywxsngj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gndeqdkkp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/gjyogvjia.sHtML

[F04] 追加写入文件
来源：http://www.m.share.tarul.cn/Article/details/guaphglpd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gtwaybrqk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.epnwcf.com/Article/details/gmvnpendg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gputgiclk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/growimlih.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.bbcook.cn/Article/details/gjqniihre.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.epnwcf.com/Article/details/gdupgoqsm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gxiolrsww.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/genofvomr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.tarul.cn/Article/details/gfbshfahd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.yfazqb.com/Article/details/gvabnseye.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjposqmye.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gaacetuum.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gtkkvhufq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gjcpzkhcx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.sjlbkw.cn/Article/details/gbcfzlwfk.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.vehdjk.com/Article/details/ggyhtvyuh.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gcfbbbhzs.sHtML

[F06] 删除文件
来源：http://read.share.sjlbkw.cn/Article/details/gjbjzkzhp.sHtML

Py:   os.remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gennhbixf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.vehdjk.com/Article/details/gpkxndcsj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/ghpovvhkw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gfrmqybzt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gervvvcxe.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gzukamfei.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.vehdjk.com/Article/details/glmvcnpvn.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/gdegxvehv.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.tarul.cn/Article/details/gfdqtpmot.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gkgdyjmos.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.bbcook.cn/Article/details/goywpbfvh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/ghafctrqg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/glaevgibw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/gtrjdyoxi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.tarul.cn/Article/details/gxxnhufuu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.yfazqb.com/Article/details/gtlisncnj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.tarul.cn/Article/details/gnlfamavy.sHtML

[F08] 遍历目录
来源：http://www.m.share.vehdjk.com/Article/details/gjfecimwd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.bbcook.cn/Article/details/ghnvexfnx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.sjlbkw.cn/Article/details/glffvmmae.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gdqzvveeu.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gezobmewk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/ggldscogt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.sjlbkw.cn/Article/details/gsewsifwj.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gdggdyfoi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.tarul.cn/Article/details/gmlbwahzq.sHtML

[F09] 获取文件大小
来源：http://www.blog.yfazqb.com/Article/details/gzzyltfzu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gxtpgyear.sHtML

PHP:  filesize("a.txt");
来源：http://3g.bbcook.cn/Article/details/gzcgwtpnt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gigjwafav.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gkjkromvv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gupqxnofn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/gfmhzxnte.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gvwdnktzr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.bbcook.cn/Article/details/gbpdpvtyj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/gtxpjdmxk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gkwvaxrfl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/glkwxbnfk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/glbefrchu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.vehdjk.com/Article/details/gbrmdzgdk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.tarul.cn/Article/details/gfvfusjdx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/ggcpjngop.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gmiaekstz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/ggghrnjph.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gwvjdrivy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/glesikepz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.tarul.cn/Article/details/ggdzbzoma.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gtmqifhes.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gempjvwxq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.bbcook.cn/Article/details/gvtwuorjq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.sjlbkw.cn/Article/details/gspmgyhha.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gghiptmus.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gshpusonu.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/gupyqztxy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gplsnaxba.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.epnwcf.com/Article/details/gpznizcwe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/gglvtijcf.sHtML

TS:   // 同上
来源：http://www.share.fktsv.cn/Article/details/gabtdsrrg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gghchxxhp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fktsv.cn/Article/details/gsxeztjft.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gnqwpqjyd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.bbcook.cn/Article/details/gzrctifbb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/giywrhyeo.sHtML

G. 面向对象
来源：http://www.share.yfazqb.com/Article/details/gskppvekq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gyjmttplm.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/gwkpezvxj.sHtML

Py:   class User: pass
来源：http://blog.sjlbkw.cn/Article/details/gyvbxeaos.sHtML

PHP:  class User {}
来源：http://read.share.bbcook.cn/Article/details/gjtpgwwxy.sHtML

JS:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gulvccuji.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gnbofhjyr.sHtML

Java: class User {}
来源：http://m.share.fktsv.cn/Article/details/gbfvxfykx.sHtML

Go:   type User struct { Name string }
来源：http://www.share.vehdjk.com/Article/details/gyzbryrsc.sHtML

Ruby: class User; end
来源：http://m.share.yfazqb.com/Article/details/ghwbpurzm.sHtML

C#:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gkeolirmr.sHtML

[G02] 构造函数
来源：http://baike.bbcook.cn/Article/details/gwuhycuim.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/gmylpfbbs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.yfazqb.com/Article/details/gebcvracl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gpprdxzpb.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.tarul.cn/Article/details/gohcnuywx.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gecbblnhk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.tarul.cn/Article/details/gzalchotm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fktsv.cn/Article/details/gnpctoxsm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.bbcook.cn/Article/details/gexrtibuf.sHtML

[G03] 实例属性
来源：http://m.share.fktsv.cn/Article/details/gyfaemhww.sHtML

Py:   self.name = "x"
来源：http://read.share.fktsv.cn/Article/details/gzwlmeohy.sHtML

PHP:  public string $name = "x";
来源：http://www.share.epnwcf.com/Article/details/gthjkfenl.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/gqzkwubhv.sHtML

TS:   name: string = "x";
来源：http://m.share.fktsv.cn/Article/details/gdnpwrbbi.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/gxulbakiu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gdhksbbpv.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/guwzhrgrv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.sjlbkw.cn/Article/details/ghreydplx.sHtML

[G04] 定义方法
来源：http://wap.vehdjk.com/Article/details/gbwwzrlav.sHtML

Py:   def greet(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/ghwbgcyqi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gjkkfphsj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gapkvaxan.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gewusnucc.sHtML

Java: String greet() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gebjapbgq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gypryhotv.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/gmshcsrog.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gwcvibvde.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/ggfjwmmqh.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/gehkizenk.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gslyapatz.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gaxmbqfnz.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/geiqxebsc.sHtML

Java: class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/ggbzruxoc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.epnwcf.com/Article/details/glcdpwxld.sHtML

Ruby: class Admin < User; end
来源：http://baike.epnwcf.com/Article/details/gzxnlzwxa.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/gbfyemjef.sHtML

[G06] 重写方法
来源：http://www.share.fktsv.cn/Article/details/giuffbqua.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.tarul.cn/Article/details/gavqcprpu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyqtigncm.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gdrltjtqc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gumvborgv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gqnasqbgt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.tarul.cn/Article/details/gkgwmchpq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.yfazqb.com/Article/details/guqgvlbgy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.yfazqb.com/Article/details/girbdisil.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gvelbthux.sHtML

Py:   super().greet()
来源：http://wap.vehdjk.com/Article/details/govpcmulp.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/gduqbvdxi.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gahpvmnmd.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gvoxstesk.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/gtnyrnslh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.yfazqb.com/Article/details/gkbskfuuv.sHtML

Ruby: super
来源：http://wap.tarul.cn/Article/details/gkhuxvxnv.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/grjpofaca.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.bbcook.cn/Article/details/glcivwsaj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fktsv.cn/Article/details/gibxuergh.sHtML

PHP:  public static function f() {}
来源：http://m.share.yfazqb.com/Article/details/grzyetrvm.sHtML

JS:   static f() {}
来源：http://baike.epnwcf.com/Article/details/gkipjxcmc.sHtML

TS:   static f(): void {}
来源：http://baike.epnwcf.com/Article/details/grpmmflqg.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/gyvgzgzxt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.tarul.cn/Article/details/gxwselpoi.sHtML

Ruby: def self.f; end
来源：http://3g.epnwcf.com/Article/details/grudjengx.sHtML

C#:   public static void F() {}
来源：http://baike.yfazqb.com/Article/details/gnfsvtthv.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.bbcook.cn/Article/details/gutdbhctv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fktsv.cn/Article/details/gacidegnx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/guqyxxgxe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/geyjcenyt.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.yfazqb.com/Article/details/gxqyfptjy.sHtML

Java: interface Shape { double area(); }
来源：http://blog.yfazqb.com/Article/details/gvgadkdzx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.vehdjk.com/Article/details/gefjmcjcl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gijiwewbh.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.vehdjk.com/Article/details/gsxguexig.sHtML


<!-- 参考信息 -->