代发 wailian999

Ruby: s.split(",");  s.split
来源：http://baike.yfazqb.com/Article/details/gipgznvar.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.vehdjk.com/Article/details/gbbvyrwzk.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/gxlgeqyqe.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/gdurkwauq.sHtML

PHP:  implode(",", $items);
来源：http://www.share.bbcook.cn/Article/details/ggsbedpyp.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gmmdjgygp.sHtML

TS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gmlsiwptm.sHtML

Java: String.join(",", items)
来源：http://wap.fktsv.cn/Article/details/gwgjydvde.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.bbcook.cn/Article/details/gccmwdoiu.sHtML

Ruby: items.join(",")
来源：http://blog.epnwcf.com/Article/details/gpmohiztz.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/ggkvttibf.sHtML

[E09] 去除所有空白字符
来源：http://m.share.vehdjk.com/Article/details/gzcvohjkr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.sjlbkw.cn/Article/details/gthonkvai.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fktsv.cn/Article/details/gocyxcfss.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/gfqhbnnmg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gyvmniktf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.tarul.cn/Article/details/gaoybzybc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.vehdjk.com/Article/details/gdunpqoxt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.bbcook.cn/Article/details/gsrryidct.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.tarul.cn/Article/details/gbcppvwmb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/gmojkhnhu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.epnwcf.com/Article/details/gkrckwiwb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.yfazqb.com/Article/details/gvrdfoaas.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gnftqinap.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/givsrhkwq.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gzadhafue.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/geygsyajn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/genabfchz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvvouwsq.sHtML

[E11] 反转字符串
来源：http://m.share.epnwcf.com/Article/details/ggqgmlrcy.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/grovkjkpe.sHtML

PHP:  strrev($s);
来源：http://blog.epnwcf.com/Article/details/gzbjubdjk.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gnwecbzea.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gmuswbcnx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.vehdjk.com/Article/details/gelkagjnd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.vehdjk.com/Article/details/gnoadviqy.sHtML

Ruby: s.reverse
来源：http://baike.bbcook.cn/Article/details/gfqncxbnz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gcsfbnygx.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.sjlbkw.cn/Article/details/gigkzolze.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gxtgcfayz.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.sjlbkw.cn/Article/details/gevmfdphp.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gpptvenvd.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.vehdjk.com/Article/details/gaxfxmpkp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.yfazqb.com/Article/details/gxivwwaxu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.tarul.cn/Article/details/ghlmkwhlz.sHtML

Ruby: s.count("a")
来源：http://3g.tarul.cn/Article/details/giyzijhiv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.tarul.cn/Article/details/gdjnyajto.sHtML

[E13] 逐字符遍历
来源：http://mobile.vehdjk.com/Article/details/gzdjzjazp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.epnwcf.com/Article/details/gahpaoeuf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.epnwcf.com/Article/details/gzwarxigv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/gewfsltve.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.vehdjk.com/Article/details/gcisroonz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.bbcook.cn/Article/details/gewsolskh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.bbcook.cn/Article/details/gavahftjn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/gkrbawljb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.yfazqb.com/Article/details/gnukjlhyc.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gyrawfqnh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.vehdjk.com/Article/details/gyigooujb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.vehdjk.com/Article/details/gklgwiqjo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.yfazqb.com/Article/details/gxhymcleh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.tarul.cn/Article/details/gaicthvds.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gdailgabn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.epnwcf.com/Article/details/gtmyyytym.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.epnwcf.com/Article/details/gtacrhngl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gjqulngsq.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.sjlbkw.cn/Article/details/grvhrbkaf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fktsv.cn/Article/details/gatvwront.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.vehdjk.com/Article/details/ggqsrwunv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/gdkdgkrws.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.yfazqb.com/Article/details/guakkexpp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.bbcook.cn/Article/details/gjxzngqde.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fktsv.cn/Article/details/gzhunqfvl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fktsv.cn/Article/details/gduublmfn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.yfazqb.com/Article/details/gtfphmywb.sHtML

[E16] 数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/gfmpymvgq.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/gugnqdixw.sHtML

PHP:  number_format(1234567);
来源：http://3g.vehdjk.com/Article/details/gnvrhiyng.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gnnthccsd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gfoibxuad.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gjjkcujak.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/gasbwiydw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.epnwcf.com/Article/details/ghlqlndxc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.bbcook.cn/Article/details/gszhyvhpr.sHtML

[E17] 首字母大写
来源：http://wap.yfazqb.com/Article/details/gzqaolpvn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.yfazqb.com/Article/details/geccblzab.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.tarul.cn/Article/details/gndnbigle.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fktsv.cn/Article/details/gqrsygiij.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.sjlbkw.cn/Article/details/gzblochax.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.sjlbkw.cn/Article/details/gertvcijq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gqkiqqndh.sHtML

Ruby: s.capitalize
来源：http://www.m.share.bbcook.cn/Article/details/glewdspwh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fktsv.cn/Article/details/gxslctpgv.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/gdpcrdhsf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fktsv.cn/Article/details/gtlwmport.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.tarul.cn/Article/details/grqibjyhi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gglkojyzo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gjaoeyrcp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gsnzcfdji.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/gbmeunjbk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/gjhuahjtx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.sjlbkw.cn/Article/details/gkbdzvjdo.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fktsv.cn/Article/details/ggfvrtnot.sHtML

Py:   s.splitlines()
来源：http://mobile.tarul.cn/Article/details/gufiqczsx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.yfazqb.com/Article/details/gfqewnldw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gybgwiorb.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gnyjqvdfo.sHtML

Java: s.lines().toList()
来源：http://read.share.vehdjk.com/Article/details/gwnequvua.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.epnwcf.com/Article/details/gvmkkuiil.sHtML

Ruby: s.lines
来源：http://www.blog.epnwcf.com/Article/details/gcuddmzbk.sHtML

C#:   s.Split('\n')
来源：http://read.share.yfazqb.com/Article/details/gwjtpyozc.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.epnwcf.com/Article/details/gisoeijby.sHtML

Py:   if not s:
来源：http://m.share.bbcook.cn/Article/details/gpiycgucb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.sjlbkw.cn/Article/details/gczunavgx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/goaqgntqo.sHtML

TS:   if (s === "") {}
来源：http://3g.epnwcf.com/Article/details/gunbrsrtj.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvfqegawk.sHtML

Go:   if s == "" {}
来源：http://mobile.tarul.cn/Article/details/gkzzrelbr.sHtML

Ruby: if s.empty?
来源：http://baike.yfazqb.com/Article/details/gglctelsk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.epnwcf.com/Article/details/grsdmzjbv.sHtML

[E21] 超长截断加省略号
来源：http://baike.sjlbkw.cn/Article/details/gnrhitodg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.bbcook.cn/Article/details/gflhiwaxq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gdmdaneme.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gchkbwlwc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gvfmnkfpy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gdyygnjhp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.tarul.cn/Article/details/gkriboqil.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/gfdtxdyxl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gajbrmzda.sHtML

[E22] 字节长度与字符长度
来源：http://wap.epnwcf.com/Article/details/gfoozgmyl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.vehdjk.com/Article/details/gyzsukwtl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gdymfefsd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gvvqewvgw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/ggqhjxhob.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/gjdebekeg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.vehdjk.com/Article/details/gaxvjguzo.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.vehdjk.com/Article/details/gixybtsxo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.bbcook.cn/Article/details/getrwnwys.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbzrtlfwi.sHtML

F. 文件与目录
来源：http://baike.epnwcf.com/Article/details/gkvtsewxm.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gpllqyzpa.sHtML

[F01] 读取整个文件
来源：http://blog.tarul.cn/Article/details/gvexcjqmo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.tarul.cn/Article/details/gxaiwngfl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.vehdjk.com/Article/details/gpyeebcqs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.epnwcf.com/Article/details/gandqgiqx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.bbcook.cn/Article/details/gbjbyloih.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gzhachdgr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/gfqedccim.sHtML

Ruby: File.read("a.txt")
来源：http://baike.vehdjk.com/Article/details/goivmajzg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fktsv.cn/Article/details/gqjsxwwsj.sHtML

[F02] 逐行读取文件
来源：http://blog.vehdjk.com/Article/details/greciqgsl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.tarul.cn/Article/details/gigazeplu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.bbcook.cn/Article/details/gsqgnnzkn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gldzsjvum.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gppnabfrv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gwxbnqqqe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.tarul.cn/Article/details/gfdnkchbf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.sjlbkw.cn/Article/details/gxicgucni.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/gsczrfqvr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.yfazqb.com/Article/details/gtkslmoqx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.yfazqb.com/Article/details/gcifgjupi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/grnlitelo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gfziurofq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/gipddraiu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.epnwcf.com/Article/details/gvhfkqbmb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/gehdeoqyn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/gytpcgcvc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gonmazvwu.sHtML

[F04] 追加写入文件
来源：http://www.m.share.epnwcf.com/Article/details/gzhzomimk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gqmkxtzmj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gpetlmrpz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gfwzqnmij.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gxiuzgbsu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.vehdjk.com/Article/details/gfljhlhml.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/gcidcohhn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.vehdjk.com/Article/details/gbtjiahrq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fktsv.cn/Article/details/gigpxagok.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gfnonrlhl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.sjlbkw.cn/Article/details/grevmploe.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gpnprfaht.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/glebrfrsu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gsvauownx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gvcscuoln.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/gosvxnusj.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/gbkpexftu.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gblymopiu.sHtML

[F06] 删除文件
来源：http://read.share.vehdjk.com/Article/details/gbkpjutsa.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gdrkirzsp.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gsduqsxqb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gvttuqumu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gjdohsulw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gozftdjbq.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gduvtcqbv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gansxaotx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gujmvlycv.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.epnwcf.com/Article/details/gcadlyhzf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/ghjrcvjsi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.vehdjk.com/Article/details/gsfxzjkgc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gfdwnqgvn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/glzshhnrk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/guqswmubg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/gbtqrqgda.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.bbcook.cn/Article/details/giaxtvoph.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.bbcook.cn/Article/details/gzlugicdv.sHtML

[F08] 遍历目录
来源：http://www.share.fktsv.cn/Article/details/gbvivfzcy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.vehdjk.com/Article/details/gqhxjfgsx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.vehdjk.com/Article/details/gasigmhna.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/ghihzpzce.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/gfuqamyht.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/grtjovegz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.tarul.cn/Article/details/gtlftzbwg.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/gkapnieao.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.yfazqb.com/Article/details/gidqpyfaq.sHtML

[F09] 获取文件大小
来源：http://read.share.sjlbkw.cn/Article/details/gudkakjgn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gcgtxxumv.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gtbfqgcla.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/goyfojker.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gvikzdwsh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gbaaxukbb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/glxbyijto.sHtML

Ruby: File.size("a.txt")
来源：http://3g.vehdjk.com/Article/details/gctoehdbr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.epnwcf.com/Article/details/gwjzdtcje.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.vehdjk.com/Article/details/gwqtwymna.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gljjdqbtl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fktsv.cn/Article/details/gctlrmwsf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/ghfbrwuuy.sHtML

TS:   path.extname("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gkohgysow.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gcukstqtu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gtlnfeyfl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gwqxrjguc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/glbpyrgqj.sHtML

[F11] 复制与移动文件
来源：http://blog.vehdjk.com/Article/details/gomsnzmmx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gkrqndrib.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.yfazqb.com/Article/details/gwlvusqfx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gpvzkiuwk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gbmmpjfga.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.bbcook.cn/Article/details/gifgomfgo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.vehdjk.com/Article/details/gqeudbjrc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gwqvukgim.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/gxcqutupq.sHtML

[F12] CSV 读写
来源：http://www.m.share.tarul.cn/Article/details/gsowbscmy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzgnojmb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fktsv.cn/Article/details/gyvtlcfvt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/gvghrxrfg.sHtML

TS:   // 同上
来源：http://www.blog.bbcook.cn/Article/details/gkyvxvnch.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.sjlbkw.cn/Article/details/gxembyfxk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.tarul.cn/Article/details/gydmuakzl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.yfazqb.com/Article/details/gbfvgzsci.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.yfazqb.com/Article/details/gjnhymylm.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/goibfnddi.sHtML

G. 面向对象
来源：http://baike.sjlbkw.cn/Article/details/gxpftftia.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxgxhbafp.sHtML

[G01] 定义类
来源：http://baike.sjlbkw.cn/Article/details/gdhxikkro.sHtML

Py:   class User: pass
来源：http://blog.bbcook.cn/Article/details/geoahmepe.sHtML

PHP:  class User {}
来源：http://3g.bbcook.cn/Article/details/giaulpcih.sHtML

JS:   class User {}
来源：http://mobile.fktsv.cn/Article/details/golqmqzwr.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.sjlbkw.cn/Article/details/gfibnahmn.sHtML

Java: class User {}
来源：http://mobile.fktsv.cn/Article/details/gzsisktmo.sHtML

Go:   type User struct { Name string }
来源：http://wap.epnwcf.com/Article/details/gfuwotsdq.sHtML

Ruby: class User; end
来源：http://m.share.sjlbkw.cn/Article/details/gibypdopq.sHtML

C#:   class User {}
来源：http://read.share.yfazqb.com/Article/details/giouxmxzh.sHtML

[G02] 构造函数
来源：http://baike.vehdjk.com/Article/details/gkvvbahif.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gxpanuhqb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fktsv.cn/Article/details/gvrqjovob.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gtdddbmvq.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.yfazqb.com/Article/details/ggbzgggsp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/grlkbogfy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.tarul.cn/Article/details/gjtegyjej.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/gcijclpmb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.yfazqb.com/Article/details/gicigmieu.sHtML

[G03] 实例属性
来源：http://www.share.fktsv.cn/Article/details/grqfcxfzd.sHtML

Py:   self.name = "x"
来源：http://m.share.vehdjk.com/Article/details/goconesro.sHtML

PHP:  public string $name = "x";
来源：http://read.share.epnwcf.com/Article/details/gqtjuehiy.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/gepzliyuq.sHtML

TS:   name: string = "x";
来源：http://blog.tarul.cn/Article/details/govkpwcjp.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/gnjqsibgx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gfhhajsth.sHtML

Ruby: @name = "x"
来源：http://baike.bbcook.cn/Article/details/gepegxaty.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.bbcook.cn/Article/details/gktgysmkx.sHtML

[G04] 定义方法
来源：http://www.share.epnwcf.com/Article/details/gddqyfuux.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gazdzldtn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gmaicxfri.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/glxiltbve.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gejgbpesi.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/gjljillhx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gbjgksyal.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gzyoumtlm.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.epnwcf.com/Article/details/gsjmueoas.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/guqajzshq.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/goivqzqcp.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gwdeqfxdo.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gokfmvjvy.sHtML

TS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gfaujtcch.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gdxxbgzvh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.vehdjk.com/Article/details/gcvdtrduo.sHtML

Ruby: class Admin < User; end
来源：http://www.share.yfazqb.com/Article/details/gyvyyhmsd.sHtML

C#:   class Admin : User {}
来源：http://3g.tarul.cn/Article/details/gkxvfmzhg.sHtML

[G06] 重写方法
来源：http://3g.sjlbkw.cn/Article/details/gxwfigadt.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gdccdkkib.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gllgrsaoj.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gqbzcfvqk.sHtML


<!-- 参考信息 -->