代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.m.share.vehdjk.com/Article/details/ggmmviivf.sHtML

Ruby: items.join(",")
来源：http://wap.yfazqb.com/Article/details/gswzfwjix.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/ghdeboyvb.sHtML

[E09] 去除所有空白字符
来源：http://www.share.tarul.cn/Article/details/gqqtrxicj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.yfazqb.com/Article/details/gypbputdo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/ggtxkfjkx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gyfibfzub.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gtxreykvn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gdyxunngc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fktsv.cn/Article/details/gyddwemsu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.vehdjk.com/Article/details/gkdtexbcy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/geswvufsn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.bbcook.cn/Article/details/gguneodgk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fktsv.cn/Article/details/ggkwwcxgy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.vehdjk.com/Article/details/gbafskkfg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gweglvcvo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/guraylgby.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gumqtjzif.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gbjpjgbnl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gpdjqmdqa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.tarul.cn/Article/details/gpfhevqts.sHtML

[E11] 反转字符串
来源：http://www.blog.vehdjk.com/Article/details/gmdwkpyso.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gtntbsinp.sHtML

PHP:  strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gqndharsa.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gssguwcat.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/ghpsdodmq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fktsv.cn/Article/details/gipvvchgi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.yfazqb.com/Article/details/ghmujzahm.sHtML

Ruby: s.reverse
来源：http://read.share.bbcook.cn/Article/details/gynnxjuzh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gqarpyark.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.vehdjk.com/Article/details/giwrfhakc.sHtML

Py:   s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gvyunpmnd.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fktsv.cn/Article/details/geseocvsb.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gqgssfgvi.sHtML

TS:   s.split("a").length - 1
来源：http://3g.yfazqb.com/Article/details/gkpfatgxs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.yfazqb.com/Article/details/gebcaykhu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fktsv.cn/Article/details/gutqrmunl.sHtML

Ruby: s.count("a")
来源：http://www.share.tarul.cn/Article/details/gbwpykber.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.tarul.cn/Article/details/gwzzygeqe.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/gbpmrrunh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.vehdjk.com/Article/details/ggbdgiusl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/gzdnjcngn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gosyorixr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/gyvaqxdrc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.yfazqb.com/Article/details/gvrerjqyf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.epnwcf.com/Article/details/gnivmrmus.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrgeijnh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.vehdjk.com/Article/details/gclvvyeyv.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fktsv.cn/Article/details/gsbksoboq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.vehdjk.com/Article/details/gmrwhfcmd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.epnwcf.com/Article/details/gnpfrikbs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.yfazqb.com/Article/details/gtmxzdxdg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.vehdjk.com/Article/details/gvmlkhltq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.bbcook.cn/Article/details/ghljmebzv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.yfazqb.com/Article/details/gipypuvye.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.bbcook.cn/Article/details/ggyitbikl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gmcztyihx.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fktsv.cn/Article/details/gwfyuelhc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.vehdjk.com/Article/details/glxmzmavv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/glhweagwf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.yfazqb.com/Article/details/ghcrezoat.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.yfazqb.com/Article/details/gvwgkflvy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.epnwcf.com/Article/details/gisuwgknd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.sjlbkw.cn/Article/details/glnvqqwcz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.bbcook.cn/Article/details/grpwvdvfy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.bbcook.cn/Article/details/gdrypbyhs.sHtML

[E16] 数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gbahurgmj.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/gylbapcnl.sHtML

PHP:  number_format(1234567);
来源：http://wap.bbcook.cn/Article/details/ggorqifpy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gzcpdnsxg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/getoxmuql.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.vehdjk.com/Article/details/gnlbpaotl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.epnwcf.com/Article/details/gnmxituup.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fktsv.cn/Article/details/gbmsctkmp.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.vehdjk.com/Article/details/gbhalyimo.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/gnephdhtt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.epnwcf.com/Article/details/gwpabarcd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.sjlbkw.cn/Article/details/golrebvvi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gjhmadqnd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gkxyfbdko.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/ghmrlbbty.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.bbcook.cn/Article/details/guwdntqai.sHtML

Ruby: s.capitalize
来源：http://blog.yfazqb.com/Article/details/gtptfmelm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fktsv.cn/Article/details/greeikizn.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/gsemljvll.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.tarul.cn/Article/details/gsnbngxju.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.tarul.cn/Article/details/gfwyuchke.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gjgtsbghc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gkloildcs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gogzngcak.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gbteupond.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.yfazqb.com/Article/details/grpsdjwve.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.vehdjk.com/Article/details/gainejluy.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/gzlhgddpk.sHtML

Py:   s.splitlines()
来源：http://m.share.sjlbkw.cn/Article/details/gjwcihzzp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.bbcook.cn/Article/details/gmvjydqid.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gxbptxoii.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/ghmmesvwu.sHtML

Java: s.lines().toList()
来源：http://www.m.share.vehdjk.com/Article/details/grpuoupiy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.epnwcf.com/Article/details/gnewnyfbs.sHtML

Ruby: s.lines
来源：http://blog.fktsv.cn/Article/details/gyyhzoubl.sHtML

C#:   s.Split('\n')
来源：http://wap.vehdjk.com/Article/details/gucfgnuqt.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/geeektsal.sHtML

Py:   if not s:
来源：http://m.share.vehdjk.com/Article/details/gfpdwirlm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.sjlbkw.cn/Article/details/giwsfzpdq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.tarul.cn/Article/details/gempxqnod.sHtML

TS:   if (s === "") {}
来源：http://blog.yfazqb.com/Article/details/gfiriknag.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gnchymmsz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.vehdjk.com/Article/details/guwehtwgy.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/grrbcixch.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/gpljtcfjj.sHtML

[E21] 超长截断加省略号
来源：http://wap.bbcook.cn/Article/details/gfxdxwspo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.yfazqb.com/Article/details/gcewswrhy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.epnwcf.com/Article/details/glcxwsbsb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/giyioblal.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gqftsudku.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gfpzpjbwl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.yfazqb.com/Article/details/gmwapzzlm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/glkdbossv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/gcpbgbifz.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/ggwmzgzhf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.sjlbkw.cn/Article/details/glctexnlk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gfjenbsdl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gxlsudwcr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gekoeaior.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.vehdjk.com/Article/details/gnqsghzbu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.vehdjk.com/Article/details/gqwtzdmap.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdzhltaa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/guvzdpysm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gkhemvaxz.sHtML

F. 文件与目录
来源：http://read.share.epnwcf.com/Article/details/gtqhdgoaw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsujczqnz.sHtML

[F01] 读取整个文件
来源：http://www.m.share.epnwcf.com/Article/details/gshnqbojt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/gogyegfcf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.yfazqb.com/Article/details/grmnukvdc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.vehdjk.com/Article/details/gkhqbgiao.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.yfazqb.com/Article/details/gcotdccsi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gzzksvmsn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.epnwcf.com/Article/details/gvengusoy.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gymhadjsi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fktsv.cn/Article/details/gymnravsi.sHtML

[F02] 逐行读取文件
来源：http://www.share.bbcook.cn/Article/details/gxhlddjtw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/grhloqjmw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/gcptnlehv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/gosplzina.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/guiawsfym.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gxqqzewep.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.vehdjk.com/Article/details/gkaqjsidj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.epnwcf.com/Article/details/gyemoxyej.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.bbcook.cn/Article/details/gwszulumg.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.vehdjk.com/Article/details/gjldgekjh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.epnwcf.com/Article/details/goyweralu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gxwocmqig.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gokmoliwi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/guftbarxv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/gilwnfzmt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fktsv.cn/Article/details/gnebisdjl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.yfazqb.com/Article/details/gcthiilda.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.bbcook.cn/Article/details/gmalxdkbr.sHtML

[F04] 追加写入文件
来源：http://wap.vehdjk.com/Article/details/gsmckhnmu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gdsttxiur.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.epnwcf.com/Article/details/gptdzooho.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gqnshvtlc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/ghwkaznxp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.tarul.cn/Article/details/gbcdqdqcc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gptinmmkn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.tarul.cn/Article/details/gthbkdway.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/ggizeopyo.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.bbcook.cn/Article/details/giqdzmbuu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.yfazqb.com/Article/details/gmesjmdoo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gafkkxvhs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gvazcgurr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gzttzlfsh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/ghxugmmqg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.yfazqb.com/Article/details/gkrgxebsi.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.tarul.cn/Article/details/ggybgfcqp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.tarul.cn/Article/details/gymbyzroy.sHtML

[F06] 删除文件
来源：http://read.share.fktsv.cn/Article/details/ggqpwomak.sHtML

Py:   os.remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gdhqvypar.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gjqfsqbja.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gtphhddee.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/ggkilcbcp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/guggjektn.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gpsodzhyp.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gvhpbxmmy.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gubncfkkk.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.vehdjk.com/Article/details/gzmyjjgyu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gfuvgccbm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.vehdjk.com/Article/details/gxireaksd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/guqgxuzqi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gpbedjhje.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.sjlbkw.cn/Article/details/gibrniasz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/ggbjnjgwu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.sjlbkw.cn/Article/details/gkttxgaot.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.epnwcf.com/Article/details/gftdbqssk.sHtML

[F08] 遍历目录
来源：http://blog.epnwcf.com/Article/details/gddngqcin.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gxwweklmr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.yfazqb.com/Article/details/gewntwvzi.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gptpognzi.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/goilmzkop.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/gxemzaigv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/gpmayuqig.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.yfazqb.com/Article/details/gdanvtcdq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/gzyfdiuce.sHtML

[F09] 获取文件大小
来源：http://baike.vehdjk.com/Article/details/gpfoyrllj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.tarul.cn/Article/details/ggdemboel.sHtML

PHP:  filesize("a.txt");
来源：http://blog.epnwcf.com/Article/details/ghxjxbnuu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gvyuvhrkq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/gezjgmqdh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/geclmmboa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.yfazqb.com/Article/details/gvmgkzqds.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghmxnctno.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fktsv.cn/Article/details/gdpxajjat.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.bbcook.cn/Article/details/geobtcfqf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gnwjuidfj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gykggukct.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gqreldcfd.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gkvfsqxgf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.vehdjk.com/Article/details/gmzhkpfmz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gragkcwgi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gddglvvsj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/glrylatny.sHtML

[F11] 复制与移动文件
来源：http://www.share.tarul.cn/Article/details/gfohhkstp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/ggszykffn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.epnwcf.com/Article/details/gcuthldow.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/grwhbefbj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gyfamatje.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gxtnvapbn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/gktyrabpg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gbwmemtmp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fktsv.cn/Article/details/gtlpqzmbd.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gmkcfjkpb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.bbcook.cn/Article/details/gzbpnbocm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.epnwcf.com/Article/details/ggltsjfpc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fktsv.cn/Article/details/gsnyjnamz.sHtML

TS:   // 同上
来源：http://read.share.vehdjk.com/Article/details/gkoorqbst.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.yfazqb.com/Article/details/gvvwkopbr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.yfazqb.com/Article/details/gjziivbqw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gdcgzadok.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/gldrydhju.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdenvtrvy.sHtML

G. 面向对象
来源：http://3g.yfazqb.com/Article/details/gkhhjvnjz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmadadofw.sHtML

[G01] 定义类
来源：http://blog.fktsv.cn/Article/details/ghievdzqn.sHtML

Py:   class User: pass
来源：http://read.share.bbcook.cn/Article/details/gqoevkobv.sHtML

PHP:  class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gzzuvzndo.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/grxutnjgu.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.epnwcf.com/Article/details/gnsruikus.sHtML

Java: class User {}
来源：http://3g.sjlbkw.cn/Article/details/gdttznrmz.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/ggotkmbkh.sHtML

Ruby: class User; end
来源：http://baike.tarul.cn/Article/details/gmvhhotrg.sHtML

C#:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gctkbrbqq.sHtML

[G02] 构造函数
来源：http://blog.vehdjk.com/Article/details/gslsjcigc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.vehdjk.com/Article/details/gylcupjne.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/gzttcxjbx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/ggdffenba.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fktsv.cn/Article/details/ggfgfronz.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gemctpxlr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fktsv.cn/Article/details/gmpdwubhk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fktsv.cn/Article/details/ggaqozmtc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.epnwcf.com/Article/details/gvgdqubdn.sHtML

[G03] 实例属性
来源：http://read.share.fktsv.cn/Article/details/gnlsysgdw.sHtML

Py:   self.name = "x"
来源：http://m.share.fktsv.cn/Article/details/gafdepftj.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gwqkuuduc.sHtML

JS:   this.name = "x";
来源：http://m.share.yfazqb.com/Article/details/gprvirebu.sHtML

TS:   name: string = "x";
来源：http://blog.bbcook.cn/Article/details/guhkonwkm.sHtML

Java: private String name;
来源：http://blog.vehdjk.com/Article/details/gewnaxzxp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.tarul.cn/Article/details/gfllmdqpn.sHtML

Ruby: @name = "x"
来源：http://baike.yfazqb.com/Article/details/gnytxxzpz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.sjlbkw.cn/Article/details/gnzulemce.sHtML

[G04] 定义方法
来源：http://mobile.bbcook.cn/Article/details/gmawqjucm.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gjazjcmpv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gqrbloipm.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gyxwaqwqq.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gfxdfpuxa.sHtML

Java: String greet() { return name; }
来源：http://wap.yfazqb.com/Article/details/gmocumvgr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gvsmcyhco.sHtML

Ruby: def greet; @name; end
来源：http://mobile.bbcook.cn/Article/details/gsrwfhlwl.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gtmhqteue.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/gsidwjgzf.sHtML

Py:   class Admin(User): pass
来源：http://blog.tarul.cn/Article/details/gdglofrva.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gyqlpxbam.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/ggxkummnf.sHtML

TS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/glrmzoucy.sHtML

Java: class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gmapijfpx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.tarul.cn/Article/details/gstkvgnmy.sHtML

Ruby: class Admin < User; end
来源：http://www.share.epnwcf.com/Article/details/gdbsrigyl.sHtML

C#:   class Admin : User {}
来源：http://wap.epnwcf.com/Article/details/gytwjqrgm.sHtML

[G06] 重写方法
来源：http://blog.vehdjk.com/Article/details/grsgbmxcy.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.sjlbkw.cn/Article/details/ghqmhujsx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gzjtrhleh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gryirjwwj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gejagkhbh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gxffuajfc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.bbcook.cn/Article/details/gfpmfxouk.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.tarul.cn/Article/details/gxjsuwojr.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gmaohyrjd.sHtML

[G07] 调用父类方法
来源：http://wap.vehdjk.com/Article/details/gmbqumckd.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/grbnwlhze.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/glgxreneu.sHtML


<!-- 参考信息 -->