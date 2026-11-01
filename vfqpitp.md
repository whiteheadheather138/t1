代发 wailian999

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/gyrtpkyhe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.epnwcf.com/Article/details/gbekqxobu.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.sjlbkw.cn/Article/details/gminaofaz.sHtML

Py:   ",".join(items)
来源：http://www.blog.fktsv.cn/Article/details/gquovposw.sHtML

PHP:  implode(",", $items);
来源：http://m.share.epnwcf.com/Article/details/goqnbfnye.sHtML

JS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gclwxjjwh.sHtML

TS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gnxxqoami.sHtML

Java: String.join(",", items)
来源：http://wap.tarul.cn/Article/details/gcikidpat.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.yfazqb.com/Article/details/gbkivzygy.sHtML

Ruby: items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gnapxsdwz.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gcjwuszlp.sHtML

[E09] 去除所有空白字符
来源：http://blog.vehdjk.com/Article/details/govbuiamh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.epnwcf.com/Article/details/gxgzbehqx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.epnwcf.com/Article/details/gmrxjicyi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/guzorryal.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gynlcgxks.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/goxnoityk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.epnwcf.com/Article/details/gfcpqhrbw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.yfazqb.com/Article/details/ggnazmjvq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gmehdtmeh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.sjlbkw.cn/Article/details/gieyqooop.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gnmdmhdng.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.yfazqb.com/Article/details/glzlemjcr.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gthzsunoz.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gcvtlmxrh.sHtML

Java: String.format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gagjvbnwx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gvsprhhfo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gyikolkzn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/gnpcydtnl.sHtML

[E11] 反转字符串
来源：http://baike.tarul.cn/Article/details/gswgftwzh.sHtML

Py:   s[::-1]
来源：http://wap.tarul.cn/Article/details/gasjioowu.sHtML

PHP:  strrev($s);
来源：http://baike.epnwcf.com/Article/details/gxowswncz.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gbcxhkgux.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/ggwtohxhm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gsazicsci.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/ggiycaosi.sHtML

Ruby: s.reverse
来源：http://mobile.vehdjk.com/Article/details/gzweawbwo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/guvexcigw.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gvllhshpz.sHtML

Py:   s.count("a")
来源：http://www.share.yfazqb.com/Article/details/grcqouuoo.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fktsv.cn/Article/details/gvkjkpgtf.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gojcvcsdq.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gezsnlnsu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.tarul.cn/Article/details/gajukwyas.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.vehdjk.com/Article/details/gvfqgrwsc.sHtML

Ruby: s.count("a")
来源：http://baike.epnwcf.com/Article/details/gnzaczwtu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.epnwcf.com/Article/details/gntwasuds.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.epnwcf.com/Article/details/gzotgzrgc.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.sjlbkw.cn/Article/details/gazojhofu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.epnwcf.com/Article/details/gvaaydwnu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.bbcook.cn/Article/details/gysvvgbuv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/gthbnmyea.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gjhjgbgxp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.epnwcf.com/Article/details/gumqwmstp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.vehdjk.com/Article/details/gyrfjcmae.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.tarul.cn/Article/details/gjprtgezc.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fktsv.cn/Article/details/gnknlqzmz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.yfazqb.com/Article/details/gwysfalki.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcuxoono.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fktsv.cn/Article/details/gvqrbbhsm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fktsv.cn/Article/details/gsatndrfy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fktsv.cn/Article/details/ggrfsgyem.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.tarul.cn/Article/details/gbjwulrgk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fktsv.cn/Article/details/gxeqflilp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.bbcook.cn/Article/details/ghntdnzun.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/gwhhefufv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.yfazqb.com/Article/details/ghujndcky.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.yfazqb.com/Article/details/gzxifmpui.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/gopuozfkm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.yfazqb.com/Article/details/gkdmlnlro.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.yfazqb.com/Article/details/gldgbrtyk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.bbcook.cn/Article/details/gyhelojkk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/glscvnaxh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/gchyzdfjp.sHtML

[E16] 数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/gfyfktfwk.sHtML

Py:   f"{1234567:,}"
来源：http://wap.bbcook.cn/Article/details/gvcyodmyc.sHtML

PHP:  number_format(1234567);
来源：http://baike.bbcook.cn/Article/details/glhhqzbcc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/godlxmdhw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gncelnsqi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/gxqavfyau.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.epnwcf.com/Article/details/gremvtcjj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.tarul.cn/Article/details/gapobhoai.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.epnwcf.com/Article/details/gmophlmsb.sHtML

[E17] 首字母大写
来源：http://www.m.share.tarul.cn/Article/details/gkwnxlsve.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.yfazqb.com/Article/details/gllmcqczj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.bbcook.cn/Article/details/grounbzdu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gkepcofcq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/geruelxxt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/ghrfbbevf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.yfazqb.com/Article/details/gvpnkhwjn.sHtML

Ruby: s.capitalize
来源：http://3g.yfazqb.com/Article/details/gjbfdggbb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.yfazqb.com/Article/details/gjldruptk.sHtML

[E18] 模板占位符替换
来源：http://blog.tarul.cn/Article/details/gfmdaposs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.tarul.cn/Article/details/gdlbilyqf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.sjlbkw.cn/Article/details/gsbohbjvb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gfykfaqqu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gfbrttgpx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gqztxuawn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fktsv.cn/Article/details/gnccsnfsb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fktsv.cn/Article/details/giqpckkuh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.bbcook.cn/Article/details/geedoelhs.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/gzhmmpseq.sHtML

Py:   s.splitlines()
来源：http://blog.yfazqb.com/Article/details/goulmooeg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/grsjoegjj.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/ggirkosae.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gcfeyzuat.sHtML

Java: s.lines().toList()
来源：http://baike.yfazqb.com/Article/details/gqhpvpyrr.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.sjlbkw.cn/Article/details/ggjcpcdzs.sHtML

Ruby: s.lines
来源：http://blog.sjlbkw.cn/Article/details/gkovcarcn.sHtML

C#:   s.Split('\n')
来源：http://mobile.yfazqb.com/Article/details/gfiqmabxr.sHtML

[E20] 判断字符串是否为空
来源：http://baike.yfazqb.com/Article/details/gybqatmuo.sHtML

Py:   if not s:
来源：http://read.share.sjlbkw.cn/Article/details/giuajuaie.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.vehdjk.com/Article/details/gclcmtywh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.vehdjk.com/Article/details/gwbtcuqro.sHtML

TS:   if (s === "") {}
来源：http://blog.fktsv.cn/Article/details/gdpgltbbk.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fktsv.cn/Article/details/gkcwribtu.sHtML

Go:   if s == "" {}
来源：http://wap.tarul.cn/Article/details/glikhkcvb.sHtML

Ruby: if s.empty?
来源：http://read.share.epnwcf.com/Article/details/guxqqomxa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fktsv.cn/Article/details/gnntbhytr.sHtML

[E21] 超长截断加省略号
来源：http://blog.bbcook.cn/Article/details/gjvhgjtpj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/gumuksvbf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gmdvibqhz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gnepznlwt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gbaoomdve.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gkrzmpjkz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.tarul.cn/Article/details/ghkindvln.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gssqmpndk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gyeakmqww.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.tarul.cn/Article/details/gapbsphoh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gzcpjewbq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/giuoiwhkg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gkzwzepfs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gyfihlthd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.bbcook.cn/Article/details/gwrmvbmmk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fktsv.cn/Article/details/gdhkrvlhu.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.tarul.cn/Article/details/gqhztnnhl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.tarul.cn/Article/details/gjjvubtlt.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/grwftgmcz.sHtML

F. 文件与目录
来源：http://mobile.epnwcf.com/Article/details/ggawwehjy.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gwtuxiyjw.sHtML

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/grjiduivz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.sjlbkw.cn/Article/details/gbfdjjjqm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/grupngmua.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.epnwcf.com/Article/details/gvmomfdkp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gkgsifnvg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/grkepeylr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.tarul.cn/Article/details/gshhavgki.sHtML

Ruby: File.read("a.txt")
来源：http://baike.bbcook.cn/Article/details/gifbooluz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.yfazqb.com/Article/details/guoexvsrx.sHtML

[F02] 逐行读取文件
来源：http://www.blog.vehdjk.com/Article/details/grvmgeqxi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.vehdjk.com/Article/details/gkajbkdgq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fktsv.cn/Article/details/ghbfrscmf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyiiprbp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gzgpzmxpq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gjukvaijr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.vehdjk.com/Article/details/gsfwhseml.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gfyjtmgsr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqstkocr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.bbcook.cn/Article/details/gsilpelik.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.tarul.cn/Article/details/gkmrqdhhg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gocptoasu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gsriwvocz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gddmimnyy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.sjlbkw.cn/Article/details/gzesibeyp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.sjlbkw.cn/Article/details/gtebtimru.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gtcjfgmei.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/guhusfxjk.sHtML

[F04] 追加写入文件
来源：http://baike.sjlbkw.cn/Article/details/gkqubnzcz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.bbcook.cn/Article/details/gwcsofvud.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.epnwcf.com/Article/details/gbyoepozn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gggulbtnp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gkiedhnvv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fktsv.cn/Article/details/gkaqmswyy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gtdziyxqq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.epnwcf.com/Article/details/glnodhanh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.epnwcf.com/Article/details/gylrkmntu.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.tarul.cn/Article/details/gzujsfbmg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.vehdjk.com/Article/details/gxjzzfbsi.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gweygezsv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gliicnhvt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gqhvfmifo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwudmbeu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.yfazqb.com/Article/details/gmpyfxhzs.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gyxfwfwoi.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.tarul.cn/Article/details/gnlcpeitp.sHtML

[F06] 删除文件
来源：http://baike.yfazqb.com/Article/details/gvajfsfay.sHtML

Py:   os.remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gmciiunts.sHtML

PHP:  unlink("a.txt");
来源：http://blog.yfazqb.com/Article/details/gojbviddm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gwynjtrfi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gfhtudglq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gsqxuhavj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ghkohrtjr.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.yfazqb.com/Article/details/ghyrhuwnr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gbjavpkih.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.bbcook.cn/Article/details/gbgcocsta.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gjuokzjpp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/goosspcyb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/goixpekxe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gvcjdkhdn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.bbcook.cn/Article/details/gcwycyxwr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.vehdjk.com/Article/details/gartxfeoe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.vehdjk.com/Article/details/guwzpqgkh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gwnasalnf.sHtML

[F08] 遍历目录
来源：http://blog.vehdjk.com/Article/details/gkrdanfim.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fktsv.cn/Article/details/groiwjxtj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fktsv.cn/Article/details/gwtuehffu.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gsezcarac.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gizlntgzp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gjfuadcld.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.yfazqb.com/Article/details/gqxdsrjht.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gjyxzoinq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.tarul.cn/Article/details/gthbgnvqq.sHtML

[F09] 获取文件大小
来源：http://baike.tarul.cn/Article/details/gpjzsdgup.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.yfazqb.com/Article/details/ggylfscek.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fktsv.cn/Article/details/glafpgvaf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gdecimueo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gugozqvcj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gcpenynuc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.sjlbkw.cn/Article/details/gxgsujjbl.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwhglujrz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.vehdjk.com/Article/details/gdprlffgf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.epnwcf.com/Article/details/glmhwzwbt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gvqmygsba.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.vehdjk.com/Article/details/grobvlxtt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gbdgrirci.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/goqybvtqq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.tarul.cn/Article/details/gtwgpzfic.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gukcaueuj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gqccagdsd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gjhtikdwc.sHtML

[F11] 复制与移动文件
来源：http://m.share.sjlbkw.cn/Article/details/gpbbosvip.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gmyqljxuj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gvurazkzw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gicvaeaps.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gxgkkbbpa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gnabcwbag.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.yfazqb.com/Article/details/gtieecaci.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gdwwiufgg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.bbcook.cn/Article/details/gctcbymmz.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/grlrwbylv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.epnwcf.com/Article/details/gqlksocac.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.sjlbkw.cn/Article/details/gthebunzx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.vehdjk.com/Article/details/glnvnsrfg.sHtML

TS:   // 同上
来源：http://3g.fktsv.cn/Article/details/geovwasey.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/gcwtgmssu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxvukxoc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/ghmnhvgub.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.bbcook.cn/Article/details/gbdxkxrnq.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gaorbbmfn.sHtML

G. 面向对象
来源：http://www.m.share.vehdjk.com/Article/details/gurnkrpxs.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gyghtkopv.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/gesxtnuxb.sHtML

Py:   class User: pass
来源：http://m.share.bbcook.cn/Article/details/gpybdmytb.sHtML

PHP:  class User {}
来源：http://baike.sjlbkw.cn/Article/details/gqpbgcyxv.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/ggwnpjlgv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsuvcwwko.sHtML

Java: class User {}
来源：http://3g.bbcook.cn/Article/details/gxedbqpvn.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/gefixqxqg.sHtML

Ruby: class User; end
来源：http://blog.tarul.cn/Article/details/gnoyslizy.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gxaxwrhms.sHtML

[G02] 构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqhfadax.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.vehdjk.com/Article/details/gqugvvagx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.sjlbkw.cn/Article/details/ghvwoezmz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gzxhpszfi.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.epnwcf.com/Article/details/gnxqlojwh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gqezptpuo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.yfazqb.com/Article/details/gxicwazyy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.yfazqb.com/Article/details/gnhexhqbb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gbrdwgale.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/gfimxkfse.sHtML

Py:   self.name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/getlgiunk.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/gvnorexhp.sHtML

JS:   this.name = "x";
来源：http://www.share.fktsv.cn/Article/details/gcbvusmqn.sHtML

TS:   name: string = "x";
来源：http://www.blog.epnwcf.com/Article/details/goyqjcjfy.sHtML

Java: private String name;
来源：http://m.share.yfazqb.com/Article/details/gjghvxnzp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.yfazqb.com/Article/details/gnqzsacxg.sHtML

Ruby: @name = "x"
来源：http://mobile.fktsv.cn/Article/details/geffnkmne.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.epnwcf.com/Article/details/gyvlqrrlb.sHtML

[G04] 定义方法
来源：http://www.m.share.tarul.cn/Article/details/gvosfhhnt.sHtML

Py:   def greet(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gnutfhlfk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gnazscjdi.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/guxxclkzy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gkziwokiz.sHtML

Java: String greet() { return name; }
来源：http://baike.tarul.cn/Article/details/giqrtzjic.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gyilnfjzr.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/glybcivjv.sHtML

C#:   public string Greet() => Name;
来源：http://blog.yfazqb.com/Article/details/gpqzilfsc.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/gfefwwfqu.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.yfazqb.com/Article/details/gorvbxxdl.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/ghoooedik.sHtML

JS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gbcstlqus.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gyqtkmmok.sHtML

Java: class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/ghxssxdds.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.yfazqb.com/Article/details/glckcjlxg.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/gunekielc.sHtML

C#:   class Admin : User {}
来源：http://wap.fktsv.cn/Article/details/gjsyyigwk.sHtML

[G06] 重写方法
来源：http://wap.fktsv.cn/Article/details/gakuwwjlb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.yfazqb.com/Article/details/glprsbrdm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gxutkapuf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gxbqeynxp.sHtML


<!-- 参考信息 -->