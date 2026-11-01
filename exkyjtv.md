代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/glgqvpsns.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gqcypcuvt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/ghdpddhbe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gjwovmezu.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gfngyiimc.sHtML

[E07] 按分隔符拆分
来源：http://blog.sjlbkw.cn/Article/details/gskdtsaad.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.sjlbkw.cn/Article/details/ggtgpinsm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gvfvbmnxu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.tarul.cn/Article/details/gdhvhllnp.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/gmfaptqnd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.tarul.cn/Article/details/ghvyuljkb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.vehdjk.com/Article/details/gmqnydpqw.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fktsv.cn/Article/details/gcdnxeqvc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.sjlbkw.cn/Article/details/gqvilmjby.sHtML

[E08] 数组按分隔符合并
来源：http://blog.epnwcf.com/Article/details/gdrenfsvw.sHtML

Py:   ",".join(items)
来源：http://www.share.sjlbkw.cn/Article/details/gblsazcav.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.tarul.cn/Article/details/gbsljpnod.sHtML

JS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/gfdkkxgqb.sHtML

TS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/givbbhtxe.sHtML

Java: String.join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gurfwfaim.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.vehdjk.com/Article/details/glbdjlbnw.sHtML

Ruby: items.join(",")
来源：http://3g.vehdjk.com/Article/details/glzasnloh.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/gkhqzxuob.sHtML

[E09] 去除所有空白字符
来源：http://read.share.tarul.cn/Article/details/gmootpsgg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.tarul.cn/Article/details/gwolcoeje.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.yfazqb.com/Article/details/glxmvcnya.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/gybnewokt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gxgrfkhjx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fktsv.cn/Article/details/glzgmijov.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.bbcook.cn/Article/details/gdrkixuag.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.yfazqb.com/Article/details/gukmwlhwt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.yfazqb.com/Article/details/gjswnfrfv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fktsv.cn/Article/details/gzfjtswxz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gyyiqinex.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.epnwcf.com/Article/details/gnkjyjjfz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gztaicjbi.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gpaoldqxp.sHtML

Java: String.format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gdromsrrn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gtudtuakj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gkktkamvf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.yfazqb.com/Article/details/gcrtzkjob.sHtML

[E11] 反转字符串
来源：http://read.share.yfazqb.com/Article/details/glvlumsdo.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gvgzqoogs.sHtML

PHP:  strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gxqxwlodt.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gtyrqscxc.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gyxwcpxtm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.vehdjk.com/Article/details/gqcoquzyb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.vehdjk.com/Article/details/gekumgtde.sHtML

Ruby: s.reverse
来源：http://wap.fktsv.cn/Article/details/gsdrfijuf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gtxigwhww.sHtML

[E12] 统计某字符出现次数
来源：http://3g.sjlbkw.cn/Article/details/gzjhrjcnj.sHtML

Py:   s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gcvjhwzif.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/gqdyuvvrw.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gixheohvu.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gjixuvwos.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/gmojktfci.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.vehdjk.com/Article/details/gmvwucefh.sHtML

Ruby: s.count("a")
来源：http://m.share.epnwcf.com/Article/details/gmvyusqyn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gkikwfjqr.sHtML

[E13] 逐字符遍历
来源：http://3g.bbcook.cn/Article/details/gqjgvefyt.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gcnqnssyn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fktsv.cn/Article/details/gcvywdyhe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gcrkjtsqc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gnviosyrg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/gpbjuqjsa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.sjlbkw.cn/Article/details/gacoqxfow.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.epnwcf.com/Article/details/gmqwjncfq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gkgzrzhnl.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/gtwjysnfu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fktsv.cn/Article/details/geykernfu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.yfazqb.com/Article/details/gmynwlrcs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.sjlbkw.cn/Article/details/gxnfcyyoj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.vehdjk.com/Article/details/gkqaxyfii.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbgzxpcr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/gphsetsta.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.sjlbkw.cn/Article/details/gdalmybcu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.vehdjk.com/Article/details/gsapvhmep.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.bbcook.cn/Article/details/gmztndjdg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fktsv.cn/Article/details/gqabejhhp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.vehdjk.com/Article/details/gpdrsxbir.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.tarul.cn/Article/details/gebtuwnoh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.vehdjk.com/Article/details/gdrakpzmw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.sjlbkw.cn/Article/details/ggljrkbbf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fktsv.cn/Article/details/ghiwemdul.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/goszfptmz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.tarul.cn/Article/details/gfuvzrixd.sHtML

[E16] 数字千分位
来源：http://baike.sjlbkw.cn/Article/details/gxrfzwbjm.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gywoktkjw.sHtML

PHP:  number_format(1234567);
来源：http://www.share.epnwcf.com/Article/details/guvcmkqyg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gmwbasayl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/ggyuzugkp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/gjpahhlhh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.epnwcf.com/Article/details/grbdtgiln.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.epnwcf.com/Article/details/guwjcasdb.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/gyhzcvcmi.sHtML

[E17] 首字母大写
来源：http://blog.vehdjk.com/Article/details/guznivjer.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fktsv.cn/Article/details/gbfudtpug.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.vehdjk.com/Article/details/gjynzfswh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/gbonucwtp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/guxmwbfvo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.vehdjk.com/Article/details/gnyrjwefm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.vehdjk.com/Article/details/gfztrmbmr.sHtML

Ruby: s.capitalize
来源：http://m.share.tarul.cn/Article/details/gqqngpmcy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gyuwjdmhb.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/gijgfcklu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.bbcook.cn/Article/details/ggkjnroog.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.epnwcf.com/Article/details/gunkgdypf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gcpkrdqlt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gelkimvax.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.tarul.cn/Article/details/gcrkllafx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gxwnakiur.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/ghhittbut.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/gnssadiap.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/grbddotvb.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fktsv.cn/Article/details/glgcvpwir.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gotvttgiy.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gbxmxvztq.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/gliudnhbw.sHtML

Java: s.lines().toList()
来源：http://www.blog.fktsv.cn/Article/details/ghxunkbxr.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.sjlbkw.cn/Article/details/gogphaumk.sHtML

Ruby: s.lines
来源：http://3g.vehdjk.com/Article/details/gakaqeady.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/gulqcezgy.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/ghsqwwxxb.sHtML

Py:   if not s:
来源：http://read.share.bbcook.cn/Article/details/gwatvlgco.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/gjpuyjgap.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.yfazqb.com/Article/details/ggqlsqhfa.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.vehdjk.com/Article/details/gohnqaacp.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/ghzhxkhlo.sHtML

Go:   if s == "" {}
来源：http://3g.tarul.cn/Article/details/goptvnzsy.sHtML

Ruby: if s.empty?
来源：http://baike.yfazqb.com/Article/details/gfvqqrpvw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/gffkuimog.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fktsv.cn/Article/details/gftkzynnb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.sjlbkw.cn/Article/details/giyddhpul.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gydwxevxp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gazhzuwty.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/grkcmcafk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gynakiwkx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.sjlbkw.cn/Article/details/gixyofxeg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gaijsyxzt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gczuvrssp.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.epnwcf.com/Article/details/gvxjsvark.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gzqkxkntc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gqizhgfem.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gdvfnbjsi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/godhiqiun.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.epnwcf.com/Article/details/gdyvktnmr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fktsv.cn/Article/details/gylriuhal.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/grxmqqeoh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/genxkzojz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gnaoovkof.sHtML

F. 文件与目录
来源：http://baike.sjlbkw.cn/Article/details/ghvsenxwd.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gjcybqrvs.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gpjjtlipq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.yfazqb.com/Article/details/goxxxrvhe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gydukcxec.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.bbcook.cn/Article/details/gcrzlmcba.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gwbywmmzv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gcrcsvfsz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/gnddwfaib.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.tarul.cn/Article/details/gfyswwhwd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gmysvclvr.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvibquuz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/gznsntzls.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gudfmzjew.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gjccuodvu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/gnxkydpke.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gataigkgo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.bbcook.cn/Article/details/gpukqndia.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fktsv.cn/Article/details/gjdvhzlqc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.sjlbkw.cn/Article/details/gjtgxbpvu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.epnwcf.com/Article/details/gguhqbkjm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.vehdjk.com/Article/details/grcddhpkd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gkmzhooml.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gingjcqzd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gloowfwho.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/glinugeby.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.epnwcf.com/Article/details/gjlstrefm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/gaqqdfltb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/ghmziusiu.sHtML

[F04] 追加写入文件
来源：http://baike.yfazqb.com/Article/details/gymtpapey.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gultklefi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.yfazqb.com/Article/details/ganrcljvq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gocptgelf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gmrrrkmmr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fktsv.cn/Article/details/gahrhgyff.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.epnwcf.com/Article/details/gemloyjqj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.sjlbkw.cn/Article/details/gigjdsuuj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fktsv.cn/Article/details/grvmclmmk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/guusjtacm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.tarul.cn/Article/details/gybukajmd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gemhboykd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gnabymtuc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gzydwmmru.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gghdmotth.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/gmusxlzle.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gtxacyhyc.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/gydzcwema.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gxakyrqtj.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gdtoaokzm.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gcfxaojkr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gmitxrqiv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ghhlljwwn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/grryhrfce.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/gbmeudhbz.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gtiiulkdn.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.vehdjk.com/Article/details/ggfmmbrsc.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fktsv.cn/Article/details/gkxqrqyvi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gpobnunmu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.epnwcf.com/Article/details/gbzekadat.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gbpunrtmj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gmeksiqaa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.sjlbkw.cn/Article/details/gvqcwlrcr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fktsv.cn/Article/details/gdxqvvcxr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.sjlbkw.cn/Article/details/gdmtggqhw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/gqumyiobc.sHtML

[F08] 遍历目录
来源：http://www.share.vehdjk.com/Article/details/givzwdigm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/gywnoqbru.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/gasqecjuw.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/ggauijgja.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.yfazqb.com/Article/details/gglusllpw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gzevqvjer.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.epnwcf.com/Article/details/gusyshkit.sHtML

Ruby: Dir.children("dir")
来源：http://wap.yfazqb.com/Article/details/gtoflddqd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.sjlbkw.cn/Article/details/ghkdufyot.sHtML

[F09] 获取文件大小
来源：http://baike.vehdjk.com/Article/details/glolfyeet.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.tarul.cn/Article/details/ghpkfidue.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gpjyonstv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/gpktvymzz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gigabktgr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/giqqdbmmc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.tarul.cn/Article/details/grlblroej.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gmhsuiypb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.sjlbkw.cn/Article/details/gjdiromls.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.bbcook.cn/Article/details/gmdlkfkuq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gajmmijtf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.epnwcf.com/Article/details/gxxpukddu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gwbnyhwec.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/gjxlmutbo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/gqpxulfir.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gyenjulge.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gbulrkeic.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gpabnjjvj.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gmixeiruc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gnjoqdqoi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.bbcook.cn/Article/details/ghoqfyduc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gnnlkxtna.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gulkafoir.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gshhacmlj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.epnwcf.com/Article/details/govvgoyce.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/grhuayotv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.yfazqb.com/Article/details/gbswhwtiy.sHtML

[F12] CSV 读写
来源：http://read.share.tarul.cn/Article/details/gkzkanjgy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fktsv.cn/Article/details/ghivbtecf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.vehdjk.com/Article/details/gwjaptdvl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.yfazqb.com/Article/details/gkfdexags.sHtML

TS:   // 同上
来源：http://mobile.yfazqb.com/Article/details/gsexlyijm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/gooxazlxa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.epnwcf.com/Article/details/ggwdqcsrs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.yfazqb.com/Article/details/gcrugxhsk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.sjlbkw.cn/Article/details/gqeujyegw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkovdrfoo.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/gicgebjtb.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvtizjduz.sHtML

[G01] 定义类
来源：http://blog.tarul.cn/Article/details/gemrpmcjy.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/gtllxxclo.sHtML

PHP:  class User {}
来源：http://baike.yfazqb.com/Article/details/gdcsblezj.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gjzazeelz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/gemuietxa.sHtML

Java: class User {}
来源：http://read.share.epnwcf.com/Article/details/gieupmxob.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/givxsaofd.sHtML

Ruby: class User; end
来源：http://read.share.yfazqb.com/Article/details/glkuawjko.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gugiyyziq.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gdbqqxhth.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fktsv.cn/Article/details/gvfasngdb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.yfazqb.com/Article/details/gvdvjndjl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gqhbbsjbu.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/gfkkopisr.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gpguvlvlz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.tarul.cn/Article/details/gueuklgsl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/gorfiggon.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/goybknkin.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gldxhxpzk.sHtML

Py:   self.name = "x"
来源：http://read.share.vehdjk.com/Article/details/gtvpaohev.sHtML

PHP:  public string $name = "x";
来源：http://www.share.tarul.cn/Article/details/gjxgyyziw.sHtML

JS:   this.name = "x";
来源：http://www.share.bbcook.cn/Article/details/gajblqesg.sHtML

TS:   name: string = "x";
来源：http://3g.vehdjk.com/Article/details/gqgipmqxi.sHtML

Java: private String name;
来源：http://mobile.epnwcf.com/Article/details/gsmhpvcdb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.vehdjk.com/Article/details/gcyexuure.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/gmovlxunr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.tarul.cn/Article/details/gimvhsmac.sHtML

[G04] 定义方法
来源：http://baike.vehdjk.com/Article/details/gvqtgkyhs.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gxcqfhpiz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gntdegyec.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gubourxqf.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gtqdrumtk.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/giijpbnmb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gcumqigim.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/grlwheddy.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gfgdcmeji.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/gmkrqofjv.sHtML


<!-- 参考信息 -->