代发 wailian999

[E06] 替换子串
来源：http://www.m.share.vehdjk.com/Article/details/gqrubnbpz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gzmrreafw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.tarul.cn/Article/details/gxbotzjou.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/grozuoguv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gzfyridlq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/guxfivfsh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gdifgzxrr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gxgnjttiv.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.bbcook.cn/Article/details/gewcmghop.sHtML

[E07] 按分隔符拆分
来源：http://m.share.bbcook.cn/Article/details/gwfmvigmu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.bbcook.cn/Article/details/gwauzxeyy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.bbcook.cn/Article/details/gyttwunja.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.vehdjk.com/Article/details/gngeqffuv.sHtML

TS:   s.split(",")
来源：http://m.share.fktsv.cn/Article/details/grboimgzl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/guaxhcrux.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fktsv.cn/Article/details/gpfbsywez.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.sjlbkw.cn/Article/details/gtotmgxon.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.epnwcf.com/Article/details/gfwlphgot.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.bbcook.cn/Article/details/gbvocohox.sHtML

Py:   ",".join(items)
来源：http://blog.vehdjk.com/Article/details/gswypvvky.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/gxsmacopv.sHtML

JS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gtybfnogz.sHtML

TS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gyfzlxspg.sHtML

Java: String.join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gcmfiqvpl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.vehdjk.com/Article/details/gdzsfvxeu.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/ggkrbjfgg.sHtML

C#:   string.Join(",", items)
来源：http://mobile.vehdjk.com/Article/details/gxgwoplbz.sHtML

[E09] 去除所有空白字符
来源：http://www.share.sjlbkw.cn/Article/details/gmaubioqa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fktsv.cn/Article/details/gcuyzfnve.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/gxlevkxrt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/ghkgzjcrk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/grwoashfv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gevnwfznz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.bbcook.cn/Article/details/geolsdwlp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fktsv.cn/Article/details/gyipivlqa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gqqjffkfo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.vehdjk.com/Article/details/ggafgkbus.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/grdemieck.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.yfazqb.com/Article/details/gpcvvczku.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gkskaxyyg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gqavcqhpf.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gcvwmzpzw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gpxhaqxxa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gyeynvnqb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.tarul.cn/Article/details/grkwmatvt.sHtML

[E11] 反转字符串
来源：http://wap.sjlbkw.cn/Article/details/ggifdqohv.sHtML

Py:   s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/gfzyrtpqh.sHtML

PHP:  strrev($s);
来源：http://3g.fktsv.cn/Article/details/gcsonqtrz.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gzcyptaty.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/govrbgffv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.vehdjk.com/Article/details/gsoznzacq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.vehdjk.com/Article/details/gapohieim.sHtML

Ruby: s.reverse
来源：http://baike.vehdjk.com/Article/details/gdqmhjbug.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gpasgkvey.sHtML

[E12] 统计某字符出现次数
来源：http://wap.vehdjk.com/Article/details/gdylqfrqz.sHtML

Py:   s.count("a")
来源：http://read.share.fktsv.cn/Article/details/guyppzfvd.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.yfazqb.com/Article/details/gzoalptuk.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/gxszpvcvr.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.epnwcf.com/Article/details/gsghbnwji.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/gzsqfcoxv.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fktsv.cn/Article/details/gbqkimogj.sHtML

Ruby: s.count("a")
来源：http://3g.vehdjk.com/Article/details/ggagcmivn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.bbcook.cn/Article/details/gyrountmr.sHtML

[E13] 逐字符遍历
来源：http://3g.epnwcf.com/Article/details/guwlkytny.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.sjlbkw.cn/Article/details/giphxhnqs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.sjlbkw.cn/Article/details/gxpzjzpmz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gflzrmltk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gnfydbjcv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.bbcook.cn/Article/details/gqkdyggvk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.yfazqb.com/Article/details/goaifjodx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.bbcook.cn/Article/details/gdovhibik.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.epnwcf.com/Article/details/gwkfwlpzs.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/gldunexwh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.epnwcf.com/Article/details/ghqclgelq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.vehdjk.com/Article/details/gggzisikn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.yfazqb.com/Article/details/gmtgirtzm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.yfazqb.com/Article/details/gjgbwbroe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.tarul.cn/Article/details/geccsyxxb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.yfazqb.com/Article/details/gjuugmyua.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fktsv.cn/Article/details/gnosaeeva.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gzewdvhjv.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.yfazqb.com/Article/details/gefboacrd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.epnwcf.com/Article/details/grabahjnm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gkdcajflh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.vehdjk.com/Article/details/gvlkomfcw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fktsv.cn/Article/details/gdldukeea.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/geppjwcca.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fktsv.cn/Article/details/gatcmpoak.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/gykudbvit.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.bbcook.cn/Article/details/genziuihy.sHtML

[E16] 数字千分位
来源：http://wap.yfazqb.com/Article/details/gunirkutr.sHtML

Py:   f"{1234567:,}"
来源：http://wap.tarul.cn/Article/details/grtlrbdiu.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/ghwyvzrhl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/grfzvvgyk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gjvermjdo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fktsv.cn/Article/details/ggatckerm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.yfazqb.com/Article/details/gumknzxjv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.epnwcf.com/Article/details/gcefpkmih.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.tarul.cn/Article/details/gbltmwutt.sHtML

[E17] 首字母大写
来源：http://read.share.yfazqb.com/Article/details/gdnutmbqu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fktsv.cn/Article/details/gxelribtg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.epnwcf.com/Article/details/glpoitubx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gyntnosit.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/gviwziqjn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.tarul.cn/Article/details/gcihoixlj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.yfazqb.com/Article/details/gpenqgeig.sHtML

Ruby: s.capitalize
来源：http://baike.bbcook.cn/Article/details/gnyblcwzi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.vehdjk.com/Article/details/guoeepzce.sHtML

[E18] 模板占位符替换
来源：http://www.share.yfazqb.com/Article/details/gcwvfsnlq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.yfazqb.com/Article/details/gyktguqbr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.bbcook.cn/Article/details/gkhodmnpo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gabqztuce.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gaktgwzop.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gwlzylxkh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gvtuvezpd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.tarul.cn/Article/details/gzespafdw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gsfrknqrp.sHtML

[E19] 多行文本按行拆分
来源：http://baike.bbcook.cn/Article/details/gpcngommu.sHtML

Py:   s.splitlines()
来源：http://www.share.bbcook.cn/Article/details/gawmyldfk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fktsv.cn/Article/details/gwnwjhlhg.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/guiaznvke.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/grpgbadjm.sHtML

Java: s.lines().toList()
来源：http://www.share.yfazqb.com/Article/details/gxhibfmac.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.vehdjk.com/Article/details/gvadzcjvc.sHtML

Ruby: s.lines
来源：http://www.blog.vehdjk.com/Article/details/gedkpmwaj.sHtML

C#:   s.Split('\n')
来源：http://www.share.vehdjk.com/Article/details/ghpdgfyrt.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.tarul.cn/Article/details/gzjtawqve.sHtML

Py:   if not s:
来源：http://www.blog.bbcook.cn/Article/details/gnaakwtnx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gcptmymnn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.bbcook.cn/Article/details/gttlskguh.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/grssbtnlo.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gapzneovu.sHtML

Go:   if s == "" {}
来源：http://www.share.bbcook.cn/Article/details/gezitvxnn.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/gzkdcbajm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gwdabkhhr.sHtML

[E21] 超长截断加省略号
来源：http://m.share.sjlbkw.cn/Article/details/gyospxuhu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.epnwcf.com/Article/details/gcmecmefl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gqsjtcjjp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/griasicnq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gkjzqkhzj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gujglqmbe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.yfazqb.com/Article/details/ggrknkwus.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gtwgjhaaw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gczznppwj.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/gxhuzaggw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.tarul.cn/Article/details/goxsizrbe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gfrhzpoyn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/gjyubgwcs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/gwodqqknh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.bbcook.cn/Article/details/gmnwyjqcg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/gtwpwcuzw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gqdflxpgq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fktsv.cn/Article/details/glxvjtgim.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggsupynhu.sHtML

F. 文件与目录
来源：http://m.share.bbcook.cn/Article/details/guliwxmoi.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmvfhkqvw.sHtML

[F01] 读取整个文件
来源：http://www.blog.bbcook.cn/Article/details/gzpjzbaux.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.bbcook.cn/Article/details/giypbqvfv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gvzeclqcj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.yfazqb.com/Article/details/gmpmeuctw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/ghuzkbwis.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/ghazwgcbi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.bbcook.cn/Article/details/ghdlojaww.sHtML

Ruby: File.read("a.txt")
来源：http://baike.bbcook.cn/Article/details/gcafeeaeb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.epnwcf.com/Article/details/gehvyvjdw.sHtML

[F02] 逐行读取文件
来源：http://www.share.epnwcf.com/Article/details/gekfbcrkn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fktsv.cn/Article/details/gjoqwhtwr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.bbcook.cn/Article/details/gzknzgcka.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gqywoztrs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gitrbcumk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/gigyjqcfa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.sjlbkw.cn/Article/details/gzzhgwwsf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.yfazqb.com/Article/details/gqygkbpru.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.yfazqb.com/Article/details/gxrpkoeul.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/ghrmqdmyq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.epnwcf.com/Article/details/gpdgzswgk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gaifsynwe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gkhzxhgwc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/guumferzm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gbsqihmzv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fktsv.cn/Article/details/gqxzguydc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.bbcook.cn/Article/details/gjzqobelk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/gnkgvhyxs.sHtML

[F04] 追加写入文件
来源：http://www.share.fktsv.cn/Article/details/gqwpsebmw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fktsv.cn/Article/details/guhrqcgqz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fktsv.cn/Article/details/gjrcliezq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/givyegdwc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gnzsxsppb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/gczmmjquy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gdhhxjzul.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.bbcook.cn/Article/details/gaszcqerd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.sjlbkw.cn/Article/details/gugzordzt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gaqjihrzk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.tarul.cn/Article/details/gyaosqxhr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gahosymjx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gcbgtxidn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gxhlteeeo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gjmyvdauj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.epnwcf.com/Article/details/gumfmpqzc.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gugiprryy.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/guqsmxkpq.sHtML

[F06] 删除文件
来源：http://baike.tarul.cn/Article/details/gdceurbsa.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gdqohczai.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gvcpoznub.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gtzljphfo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gcazpanji.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gnyiovgpl.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gvyzemfwh.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gmfektpst.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.yfazqb.com/Article/details/grgccmgsc.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.tarul.cn/Article/details/gvlxdzrqx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gjzwihjes.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.yfazqb.com/Article/details/gqrqqkusb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gyrtvmbgp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/govjklfho.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.epnwcf.com/Article/details/gmsjesovk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.tarul.cn/Article/details/gxsivhsgk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.bbcook.cn/Article/details/gdnilqbyi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.sjlbkw.cn/Article/details/gvxgixbom.sHtML

[F08] 遍历目录
来源：http://wap.yfazqb.com/Article/details/gbacnfrgu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.tarul.cn/Article/details/giovthzls.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.vehdjk.com/Article/details/gekwspqab.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gxluyytgl.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gxigrzrsa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gngfkzqmv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.vehdjk.com/Article/details/gefdtjijl.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gpnndszmu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.epnwcf.com/Article/details/gndgsforw.sHtML

[F09] 获取文件大小
来源：http://baike.epnwcf.com/Article/details/glhrvgahs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/guuaqomja.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gqojvqbow.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gknhnhvjg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gzehpcvgj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gmdfshybo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/gbxduzock.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fktsv.cn/Article/details/grqpfpabs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.tarul.cn/Article/details/gvdvecwpz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.epnwcf.com/Article/details/gkaqdofen.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/ggvbsktwk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gmvjzfvoe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gmjbhvbdy.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gdcxeuqkr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/gjejcfeht.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gqiybwzwg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/grblaztmm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gwdjwyxss.sHtML

[F11] 复制与移动文件
来源：http://read.share.fktsv.cn/Article/details/goyphgqyd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gzorrmwhb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.epnwcf.com/Article/details/gouhicxwj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/guzqnkegq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gyzvuxtpl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/ghijvlrtr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gqbxqqaia.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gzzlzmmnd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/gxvybybvq.sHtML

[F12] CSV 读写
来源：http://mobile.bbcook.cn/Article/details/gtibuoprw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/ggdwtosfy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.yfazqb.com/Article/details/gbvwemjvz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/glzzdtmei.sHtML

TS:   // 同上
来源：http://read.share.bbcook.cn/Article/details/glzhuyfcg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/goqvgzyhh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fktsv.cn/Article/details/gyaltgdho.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.sjlbkw.cn/Article/details/gckwnrssb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.yfazqb.com/Article/details/guasmqhea.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsuuognbm.sHtML

G. 面向对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpmzhbde.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gllkvtdru.sHtML

[G01] 定义类
来源：http://www.share.sjlbkw.cn/Article/details/gxqlbanyf.sHtML

Py:   class User: pass
来源：http://www.m.share.vehdjk.com/Article/details/gnqecdwem.sHtML

PHP:  class User {}
来源：http://www.share.yfazqb.com/Article/details/gwsuxgjkw.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/grwqtcovj.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fktsv.cn/Article/details/geclwfdol.sHtML

Java: class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gcoimhwzn.sHtML

Go:   type User struct { Name string }
来源：http://wap.yfazqb.com/Article/details/gwqsavkzp.sHtML

Ruby: class User; end
来源：http://m.share.vehdjk.com/Article/details/guweagfae.sHtML

C#:   class User {}
来源：http://blog.epnwcf.com/Article/details/gchywtxye.sHtML

[G02] 构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhnnrigy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.tarul.cn/Article/details/ghufpfckk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.yfazqb.com/Article/details/gcviohwnt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gqnjtygxr.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fktsv.cn/Article/details/gsgdakvvy.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gfbdawgyu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.bbcook.cn/Article/details/ghsvbqbbo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/gzmdczuxo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.tarul.cn/Article/details/gfwzgzcns.sHtML

[G03] 实例属性
来源：http://m.share.sjlbkw.cn/Article/details/gjmtmweuq.sHtML

Py:   self.name = "x"
来源：http://m.share.bbcook.cn/Article/details/gmblugncr.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fktsv.cn/Article/details/gagzjmvop.sHtML

JS:   this.name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gkjmqoqbp.sHtML

TS:   name: string = "x";
来源：http://blog.fktsv.cn/Article/details/gizetwchc.sHtML

Java: private String name;
来源：http://www.blog.epnwcf.com/Article/details/gwmemixqi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.epnwcf.com/Article/details/gqtaozpok.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/gelgchzkg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.bbcook.cn/Article/details/gevefpgeg.sHtML

[G04] 定义方法
来源：http://blog.yfazqb.com/Article/details/gxujqffpq.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gfqcboxwl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gnnnapdpw.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gqvhvcleq.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gvikvpjkm.sHtML

Java: String greet() { return name; }
来源：http://baike.fktsv.cn/Article/details/giyhfagmo.sHtML


<!-- 参考信息 -->