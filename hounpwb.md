代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.sjlbkw.cn/Article/details/gfryizmbo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fktsv.cn/Article/details/gkbvhouhw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gsxzwuuim.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/ghaqsngxh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/ghrpcfnps.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.sjlbkw.cn/Article/details/glwcmorje.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.yfazqb.com/Article/details/guysjydrj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gerradqcc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.vehdjk.com/Article/details/ggjsammrr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/gjadwajrd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.sjlbkw.cn/Article/details/gnzdgdzyq.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gqcjgxofp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcfsfhgh.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gxgiiadjy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gpscsuopa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/guifkcwwz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gxmkehwkt.sHtML

[E11] 反转字符串
来源：http://blog.bbcook.cn/Article/details/ghitxgvvt.sHtML

Py:   s[::-1]
来源：http://3g.tarul.cn/Article/details/gssrehpkc.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gnevrdxzw.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gluiqhimq.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gzgozenfm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.yfazqb.com/Article/details/gqxzowwei.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.tarul.cn/Article/details/glnhkjtkw.sHtML

Ruby: s.reverse
来源：http://m.share.epnwcf.com/Article/details/ggvivncge.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmzokjnp.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gjbkltnil.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gahlkesqr.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/gyeabjxrm.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gvfdzdsuc.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.epnwcf.com/Article/details/gtzvfrlma.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fktsv.cn/Article/details/gptkbxrmf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fktsv.cn/Article/details/gecpgfgcn.sHtML

Ruby: s.count("a")
来源：http://blog.yfazqb.com/Article/details/gwppnechk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.tarul.cn/Article/details/gdugasxss.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/gapsoypry.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/gyulmikou.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.epnwcf.com/Article/details/gfiwvqvpt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gzrbrbnga.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/glovfmaiy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/gmjunyeqk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.sjlbkw.cn/Article/details/gjvnshgkj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/gmafgcvae.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.bbcook.cn/Article/details/gjueadmqb.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.tarul.cn/Article/details/gkbvupnyh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.epnwcf.com/Article/details/gqrzzqzuk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gpvehyxxe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.tarul.cn/Article/details/gvxmsyist.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.tarul.cn/Article/details/gkdinirno.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.bbcook.cn/Article/details/gcsutrmzd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/gbxjwscfn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.sjlbkw.cn/Article/details/gughpgayd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.yfazqb.com/Article/details/gtlkozuwb.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.vehdjk.com/Article/details/gfzfyejgw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.tarul.cn/Article/details/glndhafjy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gmcaaenpf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.epnwcf.com/Article/details/gcgiumnui.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.epnwcf.com/Article/details/gwukbesly.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/gcbhazyiw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.tarul.cn/Article/details/gyyyzvfeh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.tarul.cn/Article/details/gkpwxylbm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fktsv.cn/Article/details/ghlcrzcwk.sHtML

[E16] 数字千分位
来源：http://m.share.vehdjk.com/Article/details/gyyvzgcbp.sHtML

Py:   f"{1234567:,}"
来源：http://wap.sjlbkw.cn/Article/details/gaykgmtcu.sHtML

PHP:  number_format(1234567);
来源：http://3g.fktsv.cn/Article/details/gzttotlrl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gstlksdxl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gymouzges.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gtttvanxa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.tarul.cn/Article/details/gwhqycckk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.tarul.cn/Article/details/gwnlktfzs.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.epnwcf.com/Article/details/gaekpkjtf.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/gjpcoiddm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gerptpust.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.tarul.cn/Article/details/gxweqmqzw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gzepkoyfn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.tarul.cn/Article/details/glqgjnkmo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.yfazqb.com/Article/details/gotepprmz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.sjlbkw.cn/Article/details/gsfwflqjv.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/glosjfqnc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.bbcook.cn/Article/details/gishogodo.sHtML

[E18] 模板占位符替换
来源：http://www.share.bbcook.cn/Article/details/gikelshnz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.bbcook.cn/Article/details/gsrururtw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.bbcook.cn/Article/details/gmutijhbb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/guqlaexfw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gyfkguorb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gtahlntjl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gkgmllyjx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.yfazqb.com/Article/details/gjkkxaofv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/gprjmodsu.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/gqyzwbgpp.sHtML

Py:   s.splitlines()
来源：http://www.blog.yfazqb.com/Article/details/gsvoqfhkn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/glcmuzbwo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/giyyndons.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gltkhlxag.sHtML

Java: s.lines().toList()
来源：http://m.share.vehdjk.com/Article/details/gbofmgzqa.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/gtfveqaut.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gqtzgxmfr.sHtML

C#:   s.Split('\n')
来源：http://baike.tarul.cn/Article/details/gzgowvuhn.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.epnwcf.com/Article/details/gywujsndx.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/giljpdrow.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/grrtavqwu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/gaarzgiim.sHtML

TS:   if (s === "") {}
来源：http://www.share.sjlbkw.cn/Article/details/ghzabcxab.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/guuotallt.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/gzqkvyhuu.sHtML

Ruby: if s.empty?
来源：http://www.share.yfazqb.com/Article/details/gsjrwvjws.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/gzxavqere.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.epnwcf.com/Article/details/giinkjsxt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/gadvnobbv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gkcklrpbo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gwfvacwqx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gjlckumli.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/geukdrbdj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.yfazqb.com/Article/details/gcnmadmpj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/ggcgsefpm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gvhmbgygh.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.tarul.cn/Article/details/gxwbcmpcd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.tarul.cn/Article/details/gwatxnqbg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gndeiralc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/ggvvfdedg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gljnqnaat.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.vehdjk.com/Article/details/guiwduihc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fktsv.cn/Article/details/gbwfxandy.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.vehdjk.com/Article/details/govhbgpur.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.epnwcf.com/Article/details/gjbxbbnmq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmmxmfkgm.sHtML

F. 文件与目录
来源：http://3g.tarul.cn/Article/details/gdalvjsaq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ggkrjchjq.sHtML

[F01] 读取整个文件
来源：http://baike.epnwcf.com/Article/details/gfuzytqsn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.tarul.cn/Article/details/gfuxllghj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.yfazqb.com/Article/details/gvrnabvog.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.tarul.cn/Article/details/gjffixrcc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gwgzgemso.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gucnkxtlf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.bbcook.cn/Article/details/gcbfheora.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gazokwtus.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gxxdyaget.sHtML

[F02] 逐行读取文件
来源：http://3g.tarul.cn/Article/details/gquwkzykj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.tarul.cn/Article/details/gcewnusdh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.sjlbkw.cn/Article/details/giovbtdxz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/goesfhtmj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/gbxcmvxot.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/gsxfaqdic.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/gxwaskvar.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fktsv.cn/Article/details/gngogytxe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gorvfuhax.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.vehdjk.com/Article/details/gindqqima.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.sjlbkw.cn/Article/details/gjzfggkjd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gklxuqghr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gohajpgwz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gxgkeatgq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.tarul.cn/Article/details/gapqehnwd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.vehdjk.com/Article/details/gmzgrbtqg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.bbcook.cn/Article/details/ghvddaiom.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/gohmidoqb.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/gzqxfulxr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gvircfjox.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/ggrcqpgfx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gpgszvose.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/giumcwqku.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/gvadsgbiu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fktsv.cn/Article/details/gncavncmd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.yfazqb.com/Article/details/gvsrrwelv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.sjlbkw.cn/Article/details/gqwydchrb.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gqpxomrkd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/grkmqhhfs.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.epnwcf.com/Article/details/gqezsylsr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gedfnmfhl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gizeblgxx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gbnvgptfg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.vehdjk.com/Article/details/gxucqcyxi.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.epnwcf.com/Article/details/gnxuskcwy.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.bbcook.cn/Article/details/ggmxdpttr.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gpifomese.sHtML

Py:   os.remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gzjtgzlxd.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gfrhqtkbc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/grzpcqadp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/ghxvwimgk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gtaoolisk.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gsedlcdbn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gidgfpzln.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/glbylynie.sHtML

[F07] 创建目录（含多级）
来源：http://baike.vehdjk.com/Article/details/gtjddoeld.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gukxlkagl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/gdehgahxg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/geacomafm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/gxhvwrqer.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.tarul.cn/Article/details/gzmdxgbcd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.sjlbkw.cn/Article/details/gxgwuxodq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.bbcook.cn/Article/details/gorrzzmgv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/geofsiyhk.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/goxmbmjvh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.epnwcf.com/Article/details/gjipasciv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.bbcook.cn/Article/details/gsixvenhl.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gdvzchutg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gjrjopccb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gvbfvanav.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.sjlbkw.cn/Article/details/gjaadvvws.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gqkhbtrih.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/gtilkpchc.sHtML

[F09] 获取文件大小
来源：http://wap.fktsv.cn/Article/details/gmhfqalco.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gdkgyzako.sHtML

PHP:  filesize("a.txt");
来源：http://3g.yfazqb.com/Article/details/gwcktmioo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/glgrllygn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/ghqklucle.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gyojsgqzq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.tarul.cn/Article/details/gzjbsropz.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/gpmhgkmyh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.epnwcf.com/Article/details/gzqhgugvq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.yfazqb.com/Article/details/gqzotmqbg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gwipmplrw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.bbcook.cn/Article/details/gnepycijn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gidorwyrm.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gocwlmtgj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.vehdjk.com/Article/details/gpkqecniv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gqohbvehp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gbvrtsseh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gugwrbhpu.sHtML

[F11] 复制与移动文件
来源：http://m.share.bbcook.cn/Article/details/gnbngexki.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/ghhinruti.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/guivghbac.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gchxjkeah.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gejsqnjbo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.yfazqb.com/Article/details/gmceyzggx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fktsv.cn/Article/details/gqbehbxrj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gixcciabj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fktsv.cn/Article/details/gweuldhbs.sHtML

[F12] CSV 读写
来源：http://wap.fktsv.cn/Article/details/gwsuiziuv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.sjlbkw.cn/Article/details/gfhgprfpo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/glxejmjdg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.tarul.cn/Article/details/gjaphcdoo.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/gpqjjwjuy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fktsv.cn/Article/details/gvloyaqnk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.yfazqb.com/Article/details/gmvksanfd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.vehdjk.com/Article/details/gsgqzkyhw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.sjlbkw.cn/Article/details/glemworvb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwjnkxuga.sHtML

G. 面向对象
来源：http://mobile.sjlbkw.cn/Article/details/gtvddbxgt.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gbxmhcief.sHtML

[G01] 定义类
来源：http://blog.vehdjk.com/Article/details/gqqklmgwy.sHtML

Py:   class User: pass
来源：http://m.share.bbcook.cn/Article/details/gqoupyqck.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gpjvusqoe.sHtML

JS:   class User {}
来源：http://3g.bbcook.cn/Article/details/ggshxinpf.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.tarul.cn/Article/details/ggmajcqqb.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gendfkqjh.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gammpaxuh.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/gqtzdyvfw.sHtML

C#:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gelaemzvc.sHtML

[G02] 构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gxsogldvy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/gkzncldgl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.vehdjk.com/Article/details/ggwdvyuej.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gyyrwhwrl.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.epnwcf.com/Article/details/gcljfsuap.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/grqdehtuh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.yfazqb.com/Article/details/gaifwopmp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.yfazqb.com/Article/details/gsepqmlcs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.epnwcf.com/Article/details/gdhykqlxe.sHtML

[G03] 实例属性
来源：http://mobile.sjlbkw.cn/Article/details/gadnzijca.sHtML

Py:   self.name = "x"
来源：http://read.share.tarul.cn/Article/details/gfwrpvcyq.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gshzesvfc.sHtML

JS:   this.name = "x";
来源：http://m.share.epnwcf.com/Article/details/giroashkl.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/gbiykienq.sHtML

Java: private String name;
来源：http://m.share.epnwcf.com/Article/details/gevytolmn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.bbcook.cn/Article/details/gsutkhsdz.sHtML

Ruby: @name = "x"
来源：http://m.share.yfazqb.com/Article/details/gzcdfciif.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.bbcook.cn/Article/details/guqatxnpb.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/gxxubocxc.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gbweoioty.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gkvxawnla.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gcjhztfkw.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gkjxjnppg.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gelhvmlfz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gdoaacbbj.sHtML

Ruby: def greet; @name; end
来源：http://m.share.vehdjk.com/Article/details/gopueetnw.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.epnwcf.com/Article/details/gffxdyzsi.sHtML

[G05] 继承
来源：http://baike.bbcook.cn/Article/details/gkqcgyugj.sHtML

Py:   class Admin(User): pass
来源：http://baike.tarul.cn/Article/details/ghqudqspa.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gytbrukvy.sHtML

JS:   class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gxpjrmyst.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gbitjdsri.sHtML

Java: class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gnehjkxku.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.epnwcf.com/Article/details/gdvorxprl.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.bbcook.cn/Article/details/goxdxwagd.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/gpvehiaux.sHtML

[G06] 重写方法
来源：http://blog.vehdjk.com/Article/details/gryiqoslj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fktsv.cn/Article/details/gbsqiildc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gmqakjcjb.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gwfsabuzx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gigtlrhol.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gwldsoyls.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.bbcook.cn/Article/details/gdsbwhlhh.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.epnwcf.com/Article/details/gixhfvfaf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fktsv.cn/Article/details/grtmgwcti.sHtML

[G07] 调用父类方法
来源：http://www.share.sjlbkw.cn/Article/details/gyfywvpyo.sHtML

Py:   super().greet()
来源：http://read.share.yfazqb.com/Article/details/gaurxfybw.sHtML

PHP:  parent::greet();
来源：http://baike.fktsv.cn/Article/details/gyzxhtagk.sHtML

JS:   super.greet();
来源：http://www.m.share.tarul.cn/Article/details/gwmaeevce.sHtML

TS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gnvqfdtjw.sHtML

Java: super.greet();
来源：http://www.blog.tarul.cn/Article/details/gsscbspkx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fktsv.cn/Article/details/gtwbixzvp.sHtML


<!-- 参考信息 -->