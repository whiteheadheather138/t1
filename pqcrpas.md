代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.share.vehdjk.com/Article/details/gfkncipbv.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gomushwdu.sHtML

C#:   string.Join(",", items)
来源：http://baike.bbcook.cn/Article/details/grxuggucn.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.sjlbkw.cn/Article/details/gcflqecvt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.tarul.cn/Article/details/gzvccjcjj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.vehdjk.com/Article/details/ghmbfagsc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gakobyfhe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gauhgccka.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gfaxdplcb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.tarul.cn/Article/details/ggtlsnczo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fktsv.cn/Article/details/ghqiqlldr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fktsv.cn/Article/details/gjzllhjyq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/gstkgljen.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.vehdjk.com/Article/details/ghnuiuakf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.epnwcf.com/Article/details/gzztwuikj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gukffrimo.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gqpuhiigh.sHtML

Java: String.format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gvcgikrdd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/geadwbiip.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/ghhsmevhp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/gibrduxog.sHtML

[E11] 反转字符串
来源：http://mobile.bbcook.cn/Article/details/giobvxzgd.sHtML

Py:   s[::-1]
来源：http://blog.bbcook.cn/Article/details/gfccymwli.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gzakfxilp.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/glrxmpset.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gxnnkdydq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.bbcook.cn/Article/details/gwdyowoqq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gtvsrmijg.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/gpyxuxivj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gjvogdcac.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fktsv.cn/Article/details/gmwubbgoh.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gzhkflsua.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.epnwcf.com/Article/details/gypslbzpm.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gebiwubvr.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fktsv.cn/Article/details/gfaixdziv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.vehdjk.com/Article/details/galydgrkm.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.yfazqb.com/Article/details/gfjsplvjq.sHtML

Ruby: s.count("a")
来源：http://www.m.share.tarul.cn/Article/details/gzxfatkdd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fktsv.cn/Article/details/gksfjefku.sHtML

[E13] 逐字符遍历
来源：http://read.share.epnwcf.com/Article/details/gqwtxkfdk.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/gfbuluwlz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/glmfbkpar.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/gfauzboyr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/grlwnlras.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gdolbbzgt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.bbcook.cn/Article/details/gpwzfgyid.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.bbcook.cn/Article/details/gajqkzbpf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fktsv.cn/Article/details/ghcyailpz.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/gxceksuwl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.bbcook.cn/Article/details/gxjejnqif.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.vehdjk.com/Article/details/gyzlceyqn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.vehdjk.com/Article/details/glzeddnch.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.tarul.cn/Article/details/gzgxfkjnq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.epnwcf.com/Article/details/ghdvmderc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gmcebozuc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fktsv.cn/Article/details/gynlsirge.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.vehdjk.com/Article/details/gaoyqixnh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fktsv.cn/Article/details/gykjdytmu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.sjlbkw.cn/Article/details/gpnvjoegn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fktsv.cn/Article/details/gxvywlpgs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.bbcook.cn/Article/details/ghansrhay.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.bbcook.cn/Article/details/gflnihdap.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfhhyoth.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fktsv.cn/Article/details/gqfyxndox.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.vehdjk.com/Article/details/ghkoaovzz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fktsv.cn/Article/details/gdvkedqlx.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/glhyvuhil.sHtML

Py:   f"{1234567:,}"
来源：http://wap.bbcook.cn/Article/details/gxgmfnhaa.sHtML

PHP:  number_format(1234567);
来源：http://wap.yfazqb.com/Article/details/gfxklqgqp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gmyieomyl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/glfdqjzng.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.tarul.cn/Article/details/gfqxauinf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.vehdjk.com/Article/details/gqvwjqswc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.tarul.cn/Article/details/gldjinwnl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.bbcook.cn/Article/details/godujuhgq.sHtML

[E17] 首字母大写
来源：http://3g.epnwcf.com/Article/details/giisfgzuo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.tarul.cn/Article/details/gqwplqhya.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.tarul.cn/Article/details/ggriuufqx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gsspowzgv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gwvxdnmem.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.epnwcf.com/Article/details/gbpwgdunk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.epnwcf.com/Article/details/gjuwkuavt.sHtML

Ruby: s.capitalize
来源：http://baike.fktsv.cn/Article/details/gmhkcjfzs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/gnijlmqon.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fktsv.cn/Article/details/gejvbkfiv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.vehdjk.com/Article/details/gohqkvnpo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsgmlgbb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/giwvclsxj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gfwzsprss.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gjtnejazz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gkzkvzlxs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.epnwcf.com/Article/details/gliqyrqwv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gsroffyvz.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fktsv.cn/Article/details/gdojbwclj.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gvqcgjayh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/grbkabisg.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/gfjqlcfmc.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gtghjavow.sHtML

Java: s.lines().toList()
来源：http://read.share.fktsv.cn/Article/details/gbblsjxjf.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.bbcook.cn/Article/details/ggprmhgna.sHtML

Ruby: s.lines
来源：http://baike.yfazqb.com/Article/details/gfcqbuzvt.sHtML

C#:   s.Split('\n')
来源：http://blog.sjlbkw.cn/Article/details/geyhkfsyl.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/giblwjggv.sHtML

Py:   if not s:
来源：http://www.share.sjlbkw.cn/Article/details/gcyneyice.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fktsv.cn/Article/details/ggtdkoesd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.sjlbkw.cn/Article/details/gdbmjqepb.sHtML

TS:   if (s === "") {}
来源：http://www.share.fktsv.cn/Article/details/gslfzudgj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gppffuaeh.sHtML

Go:   if s == "" {}
来源：http://wap.bbcook.cn/Article/details/gayvrrrjg.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gyhpiwxzm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gipgqutul.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/grpjzabkk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.vehdjk.com/Article/details/gmppsjjsf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gvtacrdgj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/ggwalcrrp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gbwklwhoj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gjmsmdxzv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fktsv.cn/Article/details/gktagnohy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gixjbumrb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gyafajeps.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.vehdjk.com/Article/details/gyhqdozwv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.yfazqb.com/Article/details/gouxdmydn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gjvadvmaj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gyrmqvtir.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/ggnjqsndh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.bbcook.cn/Article/details/gmjhmeixs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/gpgnkrsnn.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.tarul.cn/Article/details/gfgxxcvpv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/gkqlptllt.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/glswqxqfw.sHtML

F. 文件与目录
来源：http://www.blog.epnwcf.com/Article/details/gqzpeotrc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbxvwvbkg.sHtML

[F01] 读取整个文件
来源：http://baike.bbcook.cn/Article/details/gfhjhacwb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.sjlbkw.cn/Article/details/gkrjuippc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gnwvusxvp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.vehdjk.com/Article/details/gyvcdkqil.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdhpzlji.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gfwjutyoy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/gmneyzuyd.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gprvasiln.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.tarul.cn/Article/details/georxxlzs.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/gjnvdnpds.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.bbcook.cn/Article/details/gsqgsjvwm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fktsv.cn/Article/details/gznflnlnu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/getlyfltb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/guqdcqxdq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gjjvkbtrg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.tarul.cn/Article/details/gscpkflwc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.tarul.cn/Article/details/gzsopqfet.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fktsv.cn/Article/details/grvgvtwkn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.yfazqb.com/Article/details/gilpoudjh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fktsv.cn/Article/details/gxsxsajgo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gxzsvaqqk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/goqvekmni.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gqdyqrddo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.yfazqb.com/Article/details/gmtwdfdgd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.vehdjk.com/Article/details/gkneuwsav.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.vehdjk.com/Article/details/gzidjzegh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gzczmbggv.sHtML

[F04] 追加写入文件
来源：http://m.share.yfazqb.com/Article/details/gbiozlkls.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/glsiffuop.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.sjlbkw.cn/Article/details/gaiontxqw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gsahkxodi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gstebgepw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.vehdjk.com/Article/details/gbslksfbh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.yfazqb.com/Article/details/guzswvtuv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.yfazqb.com/Article/details/gtghmmmwc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.bbcook.cn/Article/details/gjcowlmiq.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.tarul.cn/Article/details/gxcxenftl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fktsv.cn/Article/details/ggxbutriu.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fktsv.cn/Article/details/gebfuxwbw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gvionplku.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/guupartjv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gvkrgneri.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.yfazqb.com/Article/details/gscnignxr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gxbteebil.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gvkziaqbo.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gjxiepnrh.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gyjysykzr.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gkyfocnfk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gjjqsfpjx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/giqnynymo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gqwfmjvbx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gnzpxhryq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gdcgsaalz.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gupaaeuin.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.vehdjk.com/Article/details/gkugditqe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gaxuqxzhq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.tarul.cn/Article/details/gmdgyxmkh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gbajanpro.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gjqcmhncl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.vehdjk.com/Article/details/gmckhlyia.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gggreajqp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.sjlbkw.cn/Article/details/gonnuvsui.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/guhblirqs.sHtML

[F08] 遍历目录
来源：http://baike.tarul.cn/Article/details/gaozksupr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.vehdjk.com/Article/details/gzocgxqxf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/geawaimvk.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gjwdkumkn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gnkgweaij.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gatlqvebf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.epnwcf.com/Article/details/gulyzzpoj.sHtML

Ruby: Dir.children("dir")
来源：http://baike.sjlbkw.cn/Article/details/gdnnbkwin.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.vehdjk.com/Article/details/gkpwphowv.sHtML

[F09] 获取文件大小
来源：http://mobile.bbcook.cn/Article/details/gwlvznzsy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gxtiocfpe.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gcaffmgpc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/gyxrcrbld.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/giigfaszd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gblmwzriv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.bbcook.cn/Article/details/gulhsbnoo.sHtML

Ruby: File.size("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gufqtufls.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.bbcook.cn/Article/details/gixtwkjyt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.vehdjk.com/Article/details/gaxkxsvkn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gebaneukk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.yfazqb.com/Article/details/gcohrbzak.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gzycdhybt.sHtML

TS:   path.extname("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/geydryrqr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.yfazqb.com/Article/details/gfucwluju.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gftldlkxi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gxjkxipkg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gsfrvqddt.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gtzrzarpa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gycbezudu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fktsv.cn/Article/details/gbtwreelu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/ggztbptrk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gfynflfmm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/gvyuebjww.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.yfazqb.com/Article/details/gmvvstlsw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gteykqwhy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.bbcook.cn/Article/details/gnhdqbsld.sHtML

[F12] CSV 读写
来源：http://wap.yfazqb.com/Article/details/gsrtuuaqq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.yfazqb.com/Article/details/genpzemwv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/gfyhmqvdx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/gurjxelck.sHtML

TS:   // 同上
来源：http://read.share.yfazqb.com/Article/details/gtpsbbkrj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fktsv.cn/Article/details/gftyoeupe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gnxqbpzgz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/ghlpynnby.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.sjlbkw.cn/Article/details/gkcygzacz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gocuoqqek.sHtML

G. 面向对象
来源：http://3g.epnwcf.com/Article/details/glhrpotxx.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvwmuuytt.sHtML

[G01] 定义类
来源：http://www.share.tarul.cn/Article/details/gsajqfszu.sHtML

Py:   class User: pass
来源：http://www.blog.yfazqb.com/Article/details/gbuglbcgm.sHtML

PHP:  class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gtnekvmba.sHtML

JS:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gqyyeddkp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.yfazqb.com/Article/details/gqeqwdldr.sHtML

Java: class User {}
来源：http://mobile.sjlbkw.cn/Article/details/ghkrsvlef.sHtML

Go:   type User struct { Name string }
来源：http://blog.bbcook.cn/Article/details/gcnmuuenp.sHtML

Ruby: class User; end
来源：http://3g.epnwcf.com/Article/details/grhsbimby.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/guyduhlaf.sHtML

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/gxousbyob.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.sjlbkw.cn/Article/details/gxzaaqtir.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.epnwcf.com/Article/details/gbubyfadp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gbsuvwqrk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.yfazqb.com/Article/details/goxqlofwn.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gqmlylibg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.epnwcf.com/Article/details/gfqiivjtp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.tarul.cn/Article/details/gtgzvmbny.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gdcqhorwl.sHtML

[G03] 实例属性
来源：http://m.share.yfazqb.com/Article/details/gcjtpszus.sHtML

Py:   self.name = "x"
来源：http://baike.vehdjk.com/Article/details/gwqmjvsmb.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/gdnnuqoer.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gzyylmkil.sHtML

TS:   name: string = "x";
来源：http://blog.sjlbkw.cn/Article/details/grujkpsjg.sHtML

Java: private String name;
来源：http://blog.sjlbkw.cn/Article/details/gcrfvxgxq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/ghfajlhvo.sHtML

Ruby: @name = "x"
来源：http://wap.vehdjk.com/Article/details/gdmolgqww.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.sjlbkw.cn/Article/details/grihipmqe.sHtML

[G04] 定义方法
来源：http://read.share.vehdjk.com/Article/details/gvfrjwuuq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gsswlnfth.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gxnghiekh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/golaorgde.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/godrrbrdi.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gtfmqqybt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gkmwhqjud.sHtML

Ruby: def greet; @name; end
来源：http://baike.epnwcf.com/Article/details/gulbhejcc.sHtML

C#:   public string Greet() => Name;
来源：http://blog.bbcook.cn/Article/details/gdiycblhy.sHtML

[G05] 继承
来源：http://3g.vehdjk.com/Article/details/grwyzvath.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gxfzhuxce.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gskxutirs.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gphzkypht.sHtML

TS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gvelwiixo.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gawpvmdaq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.bbcook.cn/Article/details/giwtgaaqh.sHtML

Ruby: class Admin < User; end
来源：http://blog.vehdjk.com/Article/details/gruvuuind.sHtML

C#:   class Admin : User {}
来源：http://mobile.tarul.cn/Article/details/gqmgdkefd.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/ggqekralx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gknivbhld.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gwjhewubr.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/glffexkln.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gvupvkslj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gvnotbadk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/gdevoriai.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fktsv.cn/Article/details/gapttxseo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.sjlbkw.cn/Article/details/gycwlosyp.sHtML

[G07] 调用父类方法
来源：http://blog.bbcook.cn/Article/details/gzbwpgwjn.sHtML

Py:   super().greet()
来源：http://mobile.fktsv.cn/Article/details/gelewtozp.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/golorjrpg.sHtML


<!-- 参考信息 -->