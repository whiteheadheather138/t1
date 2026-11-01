代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gretthmii.sHtML

TS:   s.slice(1, 4)
来源：http://wap.epnwcf.com/Article/details/gmcochoko.sHtML

Java: s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gjlcixnyu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gnqhicliv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.epnwcf.com/Article/details/glhuzbhkx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.bbcook.cn/Article/details/gulbylrjw.sHtML

[E04] 查找子串位置
来源：http://3g.bbcook.cn/Article/details/ggbpwfogg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gebreefqf.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fktsv.cn/Article/details/gdhsnudum.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.yfazqb.com/Article/details/ghmyfegam.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gsycokney.sHtML

Java: s.indexOf("x")
来源：http://blog.bbcook.cn/Article/details/gocguzyll.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.bbcook.cn/Article/details/ggmbhrokm.sHtML

Ruby: s.index("x")
来源：http://wap.epnwcf.com/Article/details/gjfecpxyo.sHtML

C#:   s.IndexOf("x")
来源：http://3g.tarul.cn/Article/details/geucowjrn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.tarul.cn/Article/details/gqigpmkgk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gednnutpz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/gdngithmm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gfzzasmtx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.sjlbkw.cn/Article/details/ghelqlpzk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gnzpimlbx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.bbcook.cn/Article/details/gaaoyrvvx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fktsv.cn/Article/details/gaeioqtkc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.epnwcf.com/Article/details/geqqbahnd.sHtML

[E06] 替换子串
来源：http://m.share.epnwcf.com/Article/details/gehzchejc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gdvuflkyo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.epnwcf.com/Article/details/gvarkynlk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gpikfkmfb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gtssdqnpf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gxrfryclg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gziibueyb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.epnwcf.com/Article/details/gxmgincrq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fktsv.cn/Article/details/ghbdgtcap.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fktsv.cn/Article/details/gjkzdwvbd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.yfazqb.com/Article/details/ggxbfetbq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.vehdjk.com/Article/details/ggecrrjxb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.vehdjk.com/Article/details/gziinvapi.sHtML

TS:   s.split(",")
来源：http://m.share.vehdjk.com/Article/details/gfjbxapsh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.vehdjk.com/Article/details/gqbhpihat.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fktsv.cn/Article/details/gdfnzlgjs.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fktsv.cn/Article/details/gwclccjsp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.epnwcf.com/Article/details/gshbvgsly.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/gbqlmegoj.sHtML

Py:   ",".join(items)
来源：http://www.m.share.tarul.cn/Article/details/glcvsxzke.sHtML

PHP:  implode(",", $items);
来源：http://blog.vehdjk.com/Article/details/gjavymxin.sHtML

JS:   items.join(",")
来源：http://blog.fktsv.cn/Article/details/gbhidityo.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gtvjxxfze.sHtML

Java: String.join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/ggxrgvvcb.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.sjlbkw.cn/Article/details/gfysbkcxy.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gwxwjpluw.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/gfumggpor.sHtML

[E09] 去除所有空白字符
来源：http://www.share.tarul.cn/Article/details/gzpffjgch.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.yfazqb.com/Article/details/ghperuugn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.bbcook.cn/Article/details/gcqhyzaee.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gxrlthtbz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gldhxkugp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gkxnxsfen.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.bbcook.cn/Article/details/gzawhrvef.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.vehdjk.com/Article/details/gnnwunbbg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gjljclvam.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fktsv.cn/Article/details/gypfdtnhz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gacdkqdzk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.tarul.cn/Article/details/gkbpmnttw.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gygpmnirh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/ghlitsiap.sHtML

Java: String.format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/ggxwmjeur.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/geaqavzkl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gsnahullg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fktsv.cn/Article/details/gnsqorldu.sHtML

[E11] 反转字符串
来源：http://blog.fktsv.cn/Article/details/gejcxsevr.sHtML

Py:   s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gandvcssp.sHtML

PHP:  strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gzcragyfh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gcxbiyeif.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gsngtnbrq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.vehdjk.com/Article/details/ggxohrrxi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/gfocsykdi.sHtML

Ruby: s.reverse
来源：http://www.blog.yfazqb.com/Article/details/ghqxbgtez.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gzrmfsbth.sHtML

[E12] 统计某字符出现次数
来源：http://baike.epnwcf.com/Article/details/gluzclblp.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/grvwtjykf.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.vehdjk.com/Article/details/gknymuupr.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gcmtxzxec.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.sjlbkw.cn/Article/details/gevphixdw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gttixwhhu.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/gesufcogy.sHtML

Ruby: s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gqpwtjltd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/ggifpmgsn.sHtML

[E13] 逐字符遍历
来源：http://wap.vehdjk.com/Article/details/ghwrkshqd.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.yfazqb.com/Article/details/gxmgmpjbb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.epnwcf.com/Article/details/grchtwbzk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gizzpddcx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gesouyfui.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.tarul.cn/Article/details/gxdwgggdr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fktsv.cn/Article/details/gthamhcor.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.bbcook.cn/Article/details/gpjspzxmd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/gnkjnjbbt.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.vehdjk.com/Article/details/gnwvvpsht.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/gcsmvjowl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.yfazqb.com/Article/details/ggamkddbe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.tarul.cn/Article/details/gvfmvrnvq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fktsv.cn/Article/details/giizlcasd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.tarul.cn/Article/details/gulpudalr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.epnwcf.com/Article/details/golzxnkhe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.bbcook.cn/Article/details/gqykjgndm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fktsv.cn/Article/details/gvlozjgzd.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fktsv.cn/Article/details/githgombo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fktsv.cn/Article/details/gethkkgaj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fktsv.cn/Article/details/glynbbppp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.yfazqb.com/Article/details/grgxulcky.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.tarul.cn/Article/details/gkbnvugjf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/gzhhyowks.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.tarul.cn/Article/details/geyrlmlwq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fktsv.cn/Article/details/ggkhxskap.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.epnwcf.com/Article/details/gnkitxoxm.sHtML

[E16] 数字千分位
来源：http://read.share.tarul.cn/Article/details/gbmqsfwnn.sHtML

Py:   f"{1234567:,}"
来源：http://wap.epnwcf.com/Article/details/gebqupwmc.sHtML

PHP:  number_format(1234567);
来源：http://wap.bbcook.cn/Article/details/ggerrsaac.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gtpzgqvbe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gehuwzkzt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.vehdjk.com/Article/details/gybdweagt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fktsv.cn/Article/details/gugjmuvzp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.epnwcf.com/Article/details/gttjhnavv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fktsv.cn/Article/details/gydzehdch.sHtML

[E17] 首字母大写
来源：http://m.share.sjlbkw.cn/Article/details/gtddhisqc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.tarul.cn/Article/details/gdpjvgejk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.yfazqb.com/Article/details/gbdhoqhqa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ghsifltrl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gqbnwiwxf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.bbcook.cn/Article/details/gzyzjhxnf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/gmteozhdb.sHtML

Ruby: s.capitalize
来源：http://www.share.tarul.cn/Article/details/gyethfjte.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.tarul.cn/Article/details/ghggfyeab.sHtML

[E18] 模板占位符替换
来源：http://mobile.bbcook.cn/Article/details/gaetyxygj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.yfazqb.com/Article/details/gxxduwjtk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.sjlbkw.cn/Article/details/ghwyymmft.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gtnedsiwa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/grbkytsnf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gbeqitflq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gvaexnwud.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.yfazqb.com/Article/details/ggbvtfkrf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.epnwcf.com/Article/details/gwtmjsoby.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.epnwcf.com/Article/details/gwtgfnvnl.sHtML

Py:   s.splitlines()
来源：http://mobile.fktsv.cn/Article/details/gmcjdsspq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fktsv.cn/Article/details/gmeasdxok.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gginwlmdp.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gzwervodt.sHtML

Java: s.lines().toList()
来源：http://www.blog.bbcook.cn/Article/details/gpjosbtzc.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.sjlbkw.cn/Article/details/guwteztgf.sHtML

Ruby: s.lines
来源：http://www.share.tarul.cn/Article/details/gqujkgffk.sHtML

C#:   s.Split('\n')
来源：http://www.share.bbcook.cn/Article/details/gawkdpgfa.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.epnwcf.com/Article/details/gbtsxpjoc.sHtML

Py:   if not s:
来源：http://m.share.tarul.cn/Article/details/gkcxsizkr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.bbcook.cn/Article/details/gztpetipc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/gnuccfbdg.sHtML

TS:   if (s === "") {}
来源：http://3g.epnwcf.com/Article/details/gbxddxodk.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gfwzyuvoj.sHtML

Go:   if s == "" {}
来源：http://3g.bbcook.cn/Article/details/goeydfnoc.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gnpcamdbv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.tarul.cn/Article/details/gcfajdova.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/gpgqwveah.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.sjlbkw.cn/Article/details/gpzleheub.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.epnwcf.com/Article/details/glytwpfjk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/guafvjwcx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gmwdlvbir.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gmvxtjido.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fktsv.cn/Article/details/gfidubocv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gumerbprz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gspjfdjkw.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfcchdsd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.vehdjk.com/Article/details/gkoiljezr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/glqonhrat.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gitrvwmnf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gsmuthanb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gsfvdrxcw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.bbcook.cn/Article/details/gxkulecco.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.bbcook.cn/Article/details/gseohrhvq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.vehdjk.com/Article/details/grxghwnqs.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsbnwvakk.sHtML

F. 文件与目录
来源：http://m.share.bbcook.cn/Article/details/gkdfbvcdc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gigwwuwik.sHtML

[F01] 读取整个文件
来源：http://blog.fktsv.cn/Article/details/gwdgqxold.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.sjlbkw.cn/Article/details/gdfnilszc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gseagkeac.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.yfazqb.com/Article/details/gqeikfwql.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.tarul.cn/Article/details/ggjmvlxea.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gfegrqtid.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.sjlbkw.cn/Article/details/gtwuzymgc.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.vehdjk.com/Article/details/guoccoqhz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fktsv.cn/Article/details/gththrokx.sHtML

[F02] 逐行读取文件
来源：http://m.share.tarul.cn/Article/details/gchzpsuqj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.bbcook.cn/Article/details/gshtbjeww.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.sjlbkw.cn/Article/details/gnsfkfwgi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gzvzxaojk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/gbhzwdjmx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gjepibujl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.yfazqb.com/Article/details/gizfydwgo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.epnwcf.com/Article/details/gzdnbkjml.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.vehdjk.com/Article/details/gkqrpzrlq.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fktsv.cn/Article/details/gjvtilugo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fktsv.cn/Article/details/gncwocjvo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gwjifvcyp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gyuqrqebq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gtaertroo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.vehdjk.com/Article/details/gkgvsjzix.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gpmbjuebo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.epnwcf.com/Article/details/gdhzuivhx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/grplfagvh.sHtML

[F04] 追加写入文件
来源：http://www.share.vehdjk.com/Article/details/gxpukvytm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gctsugxzg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.tarul.cn/Article/details/gfagkdyzk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/gmpqlndff.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gnulrkxca.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fktsv.cn/Article/details/gvokzfsca.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.yfazqb.com/Article/details/gkiuekzvu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.epnwcf.com/Article/details/galjgcfui.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.vehdjk.com/Article/details/ggemgwxcc.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.bbcook.cn/Article/details/gelsyxhev.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.tarul.cn/Article/details/gwxeodfoj.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.tarul.cn/Article/details/guyeryjcq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gzljqrjvp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gkkvbwvca.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gnizrekqy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.epnwcf.com/Article/details/ghoyukzfi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gcieerfby.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.tarul.cn/Article/details/gprqkxkoi.sHtML

[F06] 删除文件
来源：http://mobile.yfazqb.com/Article/details/gfcttidmo.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzaaphrb.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gbyceglke.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gvauieosn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gjdhdhfwp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gdtydxtcx.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gqniwqjsz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gpxmtbnwf.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.yfazqb.com/Article/details/gbadyaiiy.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/gbptesiir.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gncxnqgke.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.epnwcf.com/Article/details/goobcxfuh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.tarul.cn/Article/details/gtpbqajmv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gmncceyxu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.tarul.cn/Article/details/gyjaviyyt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.epnwcf.com/Article/details/gdnxslhro.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gegbzters.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/gaalvqpih.sHtML

[F08] 遍历目录
来源：http://baike.tarul.cn/Article/details/gegzcoqet.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.vehdjk.com/Article/details/gugytumda.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fktsv.cn/Article/details/geuxdzrqr.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gkrahwpik.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/genraaddb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/giqifspdn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gdlpwjfuu.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.tarul.cn/Article/details/glqvawsab.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.vehdjk.com/Article/details/gwagwxeer.sHtML

[F09] 获取文件大小
来源：http://wap.vehdjk.com/Article/details/ggtntwcof.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.tarul.cn/Article/details/glnahskvk.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gtlagkvbl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gqgvdapxw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gtzxxhaga.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gzmntivxi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.vehdjk.com/Article/details/gjcklwyzm.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gttxsskah.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.epnwcf.com/Article/details/ginzwonim.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/gxjuzkhro.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/ghqrclayp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gaprnqjfa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gdofzcaba.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gtinpoxrt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.tarul.cn/Article/details/gcwtyrdus.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gvjkqkqls.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gcttbhram.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gozkvwvop.sHtML

[F11] 复制与移动文件
来源：http://read.share.bbcook.cn/Article/details/gjvcqvuxm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gzaqwzyyt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.bbcook.cn/Article/details/gscuiqbvg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gtbyzrayc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/ghizakpvj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gxmvzvrle.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gnefsqkdw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gjemhdqku.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.sjlbkw.cn/Article/details/glkxcnbqq.sHtML

[F12] CSV 读写
来源：http://mobile.yfazqb.com/Article/details/gewfedwzt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.yfazqb.com/Article/details/gnbhqxjqb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.tarul.cn/Article/details/gnpwsnfnb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.tarul.cn/Article/details/gkuhptxox.sHtML

TS:   // 同上
来源：http://blog.fktsv.cn/Article/details/gvhdlqszo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.sjlbkw.cn/Article/details/gbtjpkqjg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.epnwcf.com/Article/details/gasuiwyus.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.yfazqb.com/Article/details/ghtlqthwh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.tarul.cn/Article/details/gzmmgkylt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gagygibbq.sHtML

G. 面向对象
来源：http://m.share.fktsv.cn/Article/details/gbqclsxvr.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvzdqzspy.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/guyakzufb.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/gmlknkigr.sHtML

PHP:  class User {}
来源：http://www.m.share.tarul.cn/Article/details/gxjlqfjxw.sHtML

JS:   class User {}
来源：http://wap.fktsv.cn/Article/details/gafmwkphg.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.sjlbkw.cn/Article/details/ggrvfbqdg.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gixsutfpb.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gkjytusdp.sHtML

Ruby: class User; end
来源：http://read.share.fktsv.cn/Article/details/grhumfpvp.sHtML

C#:   class User {}
来源：http://wap.bbcook.cn/Article/details/goyctsbup.sHtML


<!-- 参考信息 -->