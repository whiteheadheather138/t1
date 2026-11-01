代发 wailian999

JS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gkodozeqa.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gddmfhjik.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.vehdjk.com/Article/details/guesgguep.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.epnwcf.com/Article/details/ginoaevlk.sHtML

Ruby: s.reverse
来源：http://mobile.fktsv.cn/Article/details/geeajsybz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gcvdraqso.sHtML

[E12] 统计某字符出现次数
来源：http://blog.vehdjk.com/Article/details/gjnbktllb.sHtML

Py:   s.count("a")
来源：http://read.share.yfazqb.com/Article/details/gijgnewlj.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/glvfmpift.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/ggdzmkdci.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/gnsgbaomu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.sjlbkw.cn/Article/details/gxbctoiwh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.yfazqb.com/Article/details/gcjhsifmz.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/gqqlpcfhe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.yfazqb.com/Article/details/gvlmpmccy.sHtML

[E13] 逐字符遍历
来源：http://blog.bbcook.cn/Article/details/ggazguojn.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.sjlbkw.cn/Article/details/gaqlvavgv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.yfazqb.com/Article/details/ggqeshfwl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/ggqmecuzn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gpueixlag.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fktsv.cn/Article/details/ghyctpzwo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/guuvcqmat.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/gcrpayxmw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.yfazqb.com/Article/details/gcesbswlc.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fktsv.cn/Article/details/gumapecao.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/gplhrkhhd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gupztjdur.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.yfazqb.com/Article/details/gpiglqflf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.epnwcf.com/Article/details/gfcdaqzsk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/geugtuhjo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/gebqqmmmz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.epnwcf.com/Article/details/gsyohcypz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/ghvaxniwy.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.vehdjk.com/Article/details/grwbznogn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fktsv.cn/Article/details/gdlyjzcze.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/glolijrel.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.vehdjk.com/Article/details/gkhaprstq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fktsv.cn/Article/details/gikgydnrz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fktsv.cn/Article/details/gzgsyqvxu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.vehdjk.com/Article/details/gsaoyiemq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fktsv.cn/Article/details/ggfasvkjs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fktsv.cn/Article/details/gityymuqs.sHtML

[E16] 数字千分位
来源：http://mobile.fktsv.cn/Article/details/gvovqzljb.sHtML

Py:   f"{1234567:,}"
来源：http://baike.yfazqb.com/Article/details/givpamffd.sHtML

PHP:  number_format(1234567);
来源：http://wap.sjlbkw.cn/Article/details/gjugwkrfo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gesizztjf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gtcuoqjds.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gmnpuwzjv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.sjlbkw.cn/Article/details/gmmacjvmn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.vehdjk.com/Article/details/gatccirdp.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fktsv.cn/Article/details/gtoobtlve.sHtML

[E17] 首字母大写
来源：http://www.m.share.yfazqb.com/Article/details/givppagjc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.tarul.cn/Article/details/gbnsnsqik.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.epnwcf.com/Article/details/gzhmtdfwz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/glnlafxqv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gfaxmsjvk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.epnwcf.com/Article/details/gssclyawp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.vehdjk.com/Article/details/gzwhgrihf.sHtML

Ruby: s.capitalize
来源：http://www.m.share.bbcook.cn/Article/details/gusyfcatx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.bbcook.cn/Article/details/gqueyaxqm.sHtML

[E18] 模板占位符替换
来源：http://3g.sjlbkw.cn/Article/details/gxvrhfjxm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.epnwcf.com/Article/details/gqfgwvpqa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.bbcook.cn/Article/details/gzzvdpmkq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/ggqfwnove.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gapyvfyyb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/guewavtsm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.bbcook.cn/Article/details/gwvpmpttl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/gftiqogrg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.vehdjk.com/Article/details/gsmjgjfcx.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.yfazqb.com/Article/details/gvjunzlfi.sHtML

Py:   s.splitlines()
来源：http://mobile.epnwcf.com/Article/details/ghbthlpef.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.epnwcf.com/Article/details/ghfhfwvkt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gnvjlculo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gmqczmbpy.sHtML

Java: s.lines().toList()
来源：http://blog.yfazqb.com/Article/details/gffaonjhb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.bbcook.cn/Article/details/giaqzochz.sHtML

Ruby: s.lines
来源：http://m.share.fktsv.cn/Article/details/gablzgopb.sHtML

C#:   s.Split('\n')
来源：http://blog.vehdjk.com/Article/details/grwvelsoc.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fktsv.cn/Article/details/ggdczidsd.sHtML

Py:   if not s:
来源：http://www.blog.tarul.cn/Article/details/glribkqdc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.bbcook.cn/Article/details/gqvtzypbr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.bbcook.cn/Article/details/gyhiijioa.sHtML

TS:   if (s === "") {}
来源：http://blog.fktsv.cn/Article/details/gcwshphvy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gaipeybkf.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/gerhdxlpv.sHtML

Ruby: if s.empty?
来源：http://read.share.sjlbkw.cn/Article/details/gocisksgo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.vehdjk.com/Article/details/gnkdgtjqc.sHtML

[E21] 超长截断加省略号
来源：http://mobile.sjlbkw.cn/Article/details/gttiulxiq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.sjlbkw.cn/Article/details/gxuebdcay.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gruyhdmqx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gkuavsirc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/grxnaairb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gkhcfqgkr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.vehdjk.com/Article/details/geowmghgl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gqmhrwnys.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/gacnzkbfz.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.epnwcf.com/Article/details/gachrivdt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.yfazqb.com/Article/details/glpsssdih.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gbpmzlpwr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/gyimsuamp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gegpeshui.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gbynadbfk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.vehdjk.com/Article/details/gdixkbnsi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gcljvenpa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.yfazqb.com/Article/details/gigzvaais.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gdxthzlzg.sHtML

F. 文件与目录
来源：http://baike.vehdjk.com/Article/details/gzjrybyqj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqoaqnofy.sHtML

[F01] 读取整个文件
来源：http://www.blog.tarul.cn/Article/details/gchsdakzp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gvvhxghme.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.epnwcf.com/Article/details/grsmifywm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.sjlbkw.cn/Article/details/gflpqpfco.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.vehdjk.com/Article/details/gikvhulvr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gqymfnlak.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.vehdjk.com/Article/details/gvgkxhvdo.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gfyujcwll.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gcijrmpab.sHtML

[F02] 逐行读取文件
来源：http://www.blog.epnwcf.com/Article/details/gpsndskif.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gqakmdyzf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.vehdjk.com/Article/details/gzbxizovk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gfntpusrn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/glrknosrg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gngdqzomi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.yfazqb.com/Article/details/gweagbkwk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.yfazqb.com/Article/details/gnncxawmp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.vehdjk.com/Article/details/gbzgwqzeh.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.vehdjk.com/Article/details/gfkozajdt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fktsv.cn/Article/details/gkkzxhqhk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/ggrceukhj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/ghfiemlig.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/grdtpdsut.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/gzdxlvayr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.bbcook.cn/Article/details/gvgmjdxjb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.bbcook.cn/Article/details/gwacfezrp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/gspqyjdxq.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/ggecoxsth.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/glmidhtqv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/gkeoninqp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gejpyhrky.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/guyccryub.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.yfazqb.com/Article/details/gmnrtqdcb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/guyfghtrn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/gepmdagst.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fktsv.cn/Article/details/gilajdosb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gqupbguvm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.vehdjk.com/Article/details/gwnssutot.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gpigtbezi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gfnmzmxuv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gahrehahc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gtcoacutg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.bbcook.cn/Article/details/grllpfxlv.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fktsv.cn/Article/details/grvgpuxcs.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/ghcnjevlo.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/gbumvopoj.sHtML

Py:   os.remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/grjfmsolu.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gvkicjmqy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gnawgrwul.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gsbvbczps.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gjrmhhqag.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gnksdpaqc.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gcmveewvc.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gnzbwamgs.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.bbcook.cn/Article/details/gebrokhlh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gztjzcrvg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fktsv.cn/Article/details/givxiyfsn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.epnwcf.com/Article/details/gkfueesfh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/gxbftqegl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggznnfeue.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/gvzigwnzw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.vehdjk.com/Article/details/gfueihoix.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.vehdjk.com/Article/details/grevmjvys.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/gzuybdgti.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.bbcook.cn/Article/details/gwzkljdgm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fktsv.cn/Article/details/gvsqounrm.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gbdnpbqya.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/ghtcicfgd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/grqnyutzg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gucyuhslk.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fktsv.cn/Article/details/gulhrhifb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.epnwcf.com/Article/details/gnaqemkgy.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/gqiappand.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gfvcgcysz.sHtML

PHP:  filesize("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gsfftshcw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gyrmaasfa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.bbcook.cn/Article/details/gnvnczpuw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/ghksdjkuv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcvopgza.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fktsv.cn/Article/details/geffkjblt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/gyuntzehu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.vehdjk.com/Article/details/gzethkfnz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gzgsfcvql.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gvlajwjuh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gjdermszh.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/goeyyhpai.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fktsv.cn/Article/details/grfgbhdtw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gkcuenicg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gmcpeblpu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gfvrpcvge.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.yfazqb.com/Article/details/gvoqjkpiu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gygraviad.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/gsjlbjmvq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gykgratim.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ghafjhgga.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.tarul.cn/Article/details/gmxnqbmrr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.epnwcf.com/Article/details/goqmpyjnr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gndhbalhy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.epnwcf.com/Article/details/gdddeagqc.sHtML

[F12] CSV 读写
来源：http://mobile.bbcook.cn/Article/details/gvqrkbfye.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.vehdjk.com/Article/details/gtalejias.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.tarul.cn/Article/details/gnofhlasf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.epnwcf.com/Article/details/glvmedgvn.sHtML

TS:   // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gfsnjtezb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/ghpqnbbde.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.sjlbkw.cn/Article/details/gpfxfkayv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.bbcook.cn/Article/details/gopraprif.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.tarul.cn/Article/details/gbgpjkrfx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxcoewffm.sHtML

G. 面向对象
来源：http://mobile.bbcook.cn/Article/details/glwykwkvu.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/golqatrxv.sHtML

[G01] 定义类
来源：http://baike.tarul.cn/Article/details/gctgrptlg.sHtML

Py:   class User: pass
来源：http://www.blog.bbcook.cn/Article/details/gpxzlukaj.sHtML

PHP:  class User {}
来源：http://wap.epnwcf.com/Article/details/gncgpqgjx.sHtML

JS:   class User {}
来源：http://read.share.epnwcf.com/Article/details/giglztean.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/glqgejjsw.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gtpciyzss.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.bbcook.cn/Article/details/gwjionufr.sHtML

Ruby: class User; end
来源：http://read.share.epnwcf.com/Article/details/gymqkjbrz.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gkpyjiori.sHtML

[G02] 构造函数
来源：http://baike.fktsv.cn/Article/details/gqwheiogs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.yfazqb.com/Article/details/gtjjjgwfi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.epnwcf.com/Article/details/grvulcrpm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gujiatvbn.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.vehdjk.com/Article/details/gewohdkwe.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/glykntnlu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.vehdjk.com/Article/details/ghvruyqio.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/gxrwfhoef.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.tarul.cn/Article/details/gccorzdkz.sHtML

[G03] 实例属性
来源：http://wap.fktsv.cn/Article/details/gkzexbdey.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gmzkosqxa.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gaitmbsgr.sHtML

JS:   this.name = "x";
来源：http://m.share.yfazqb.com/Article/details/gythjxvho.sHtML

TS:   name: string = "x";
来源：http://mobile.tarul.cn/Article/details/gzycuejjc.sHtML

Java: private String name;
来源：http://mobile.bbcook.cn/Article/details/gurlogdzr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.epnwcf.com/Article/details/gkcvivklz.sHtML

Ruby: @name = "x"
来源：http://mobile.tarul.cn/Article/details/gplxfwidf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gesslpabr.sHtML

[G04] 定义方法
来源：http://m.share.bbcook.cn/Article/details/gwspvpbip.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gcqnpatua.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gonrlolwp.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gowpyvlch.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gdibschpn.sHtML

Java: String greet() { return name; }
来源：http://blog.bbcook.cn/Article/details/gntdwzjmj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gjskzhmvj.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/gaotpljdp.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.yfazqb.com/Article/details/ggohwplbp.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/gyerogqqx.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fktsv.cn/Article/details/gwhfissas.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gmbplloho.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/ghdqkxpgt.sHtML

TS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gjaygkgoj.sHtML

Java: class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gshamblnv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.epnwcf.com/Article/details/gvfslrikm.sHtML

Ruby: class Admin < User; end
来源：http://blog.epnwcf.com/Article/details/gykxxptiz.sHtML

C#:   class Admin : User {}
来源：http://mobile.sjlbkw.cn/Article/details/gacbzmtqq.sHtML

[G06] 重写方法
来源：http://baike.vehdjk.com/Article/details/gfzkmhurt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.sjlbkw.cn/Article/details/gdguasnrz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gbiekatcp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/glvwmntnu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/givkbdxfu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gaafzmyih.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.epnwcf.com/Article/details/grxaikkoe.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.epnwcf.com/Article/details/girptodoz.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fktsv.cn/Article/details/gfudgqdue.sHtML

[G07] 调用父类方法
来源：http://wap.epnwcf.com/Article/details/gixatgfzh.sHtML

Py:   super().greet()
来源：http://baike.epnwcf.com/Article/details/gqlelfxjg.sHtML

PHP:  parent::greet();
来源：http://read.share.fktsv.cn/Article/details/gvifhgmet.sHtML

JS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gzxberfoo.sHtML

TS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/giycjopid.sHtML

Java: super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gkaldltqa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.tarul.cn/Article/details/gwdqgtkoq.sHtML

Ruby: super
来源：http://mobile.yfazqb.com/Article/details/gzpczdqxo.sHtML

C#:   base.Greet();
来源：http://mobile.tarul.cn/Article/details/gsdexdohn.sHtML

[G08] 静态方法与属性
来源：http://read.share.vehdjk.com/Article/details/gscrsyxzl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.epnwcf.com/Article/details/gxmlywjwl.sHtML

PHP:  public static function f() {}
来源：http://m.share.bbcook.cn/Article/details/gzsfxtvdn.sHtML

JS:   static f() {}
来源：http://3g.fktsv.cn/Article/details/gtqfzedlv.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/gccglarbl.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/gcbdfvgnl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/gkhssleis.sHtML

Ruby: def self.f; end
来源：http://m.share.fktsv.cn/Article/details/ggxredscs.sHtML

C#:   public static void F() {}
来源：http://www.share.fktsv.cn/Article/details/gctlnhmay.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/grulqkqyn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/gayyhtxfl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.yfazqb.com/Article/details/gsknymdwr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.sjlbkw.cn/Article/details/gthvbexhb.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gfwbvopyc.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.yfazqb.com/Article/details/gzzzsbecz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fktsv.cn/Article/details/gouauwipk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.yfazqb.com/Article/details/gnzyceqvl.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.sjlbkw.cn/Article/details/gzwfxwofw.sHtML


<!-- 参考信息 -->