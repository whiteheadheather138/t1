代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gjgshmqnd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gnihxnbuy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gblfnrdcn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.yfazqb.com/Article/details/gvszioefv.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/gakjveysp.sHtML

[E07] 按分隔符拆分
来源：http://3g.bbcook.cn/Article/details/gfunrhrhn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.bbcook.cn/Article/details/gnjlopmni.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gsikvsycl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.epnwcf.com/Article/details/gsrdrhqpy.sHtML

TS:   s.split(",")
来源：http://baike.sjlbkw.cn/Article/details/gcqtjqmuv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.sjlbkw.cn/Article/details/gbssexcis.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.bbcook.cn/Article/details/gprfxdhzl.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.vehdjk.com/Article/details/glqkfrizn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.bbcook.cn/Article/details/gymlpbstc.sHtML

[E08] 数组按分隔符合并
来源：http://wap.vehdjk.com/Article/details/greoangyz.sHtML

Py:   ",".join(items)
来源：http://www.share.sjlbkw.cn/Article/details/gicieeqpb.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.yfazqb.com/Article/details/gcrrfmnsq.sHtML

JS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gbszgtwdl.sHtML

TS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gvcjpwlqi.sHtML

Java: String.join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gvzruxcrj.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.vehdjk.com/Article/details/gwvqwglva.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gdikdbtqh.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/ghttmdrgj.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/grbqcdsjg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.vehdjk.com/Article/details/ghgvqxtsi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gthgajexr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.bbcook.cn/Article/details/gfqxwrfzh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gvnnadoti.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/gmydzkpdx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.tarul.cn/Article/details/gffidjvat.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.vehdjk.com/Article/details/gaxkhxfgl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gvjysovcc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.sjlbkw.cn/Article/details/gtswyqbmt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.epnwcf.com/Article/details/grynorcfm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.yfazqb.com/Article/details/gnmorklux.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gnfqlcsuq.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gppoboaqm.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gqubbesro.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gnjfdddor.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gumalzcxj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fktsv.cn/Article/details/gckbgpign.sHtML

[E11] 反转字符串
来源：http://mobile.bbcook.cn/Article/details/gzlnwefnf.sHtML

Py:   s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/gpriqoakj.sHtML

PHP:  strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gmuesuvil.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gymswtcmq.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gopzwpspv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.epnwcf.com/Article/details/gvquyhiha.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/guogacjtk.sHtML

Ruby: s.reverse
来源：http://read.share.tarul.cn/Article/details/gxbqzzhgw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gixfvswqz.sHtML

[E12] 统计某字符出现次数
来源：http://3g.sjlbkw.cn/Article/details/gqawjrrkl.sHtML

Py:   s.count("a")
来源：http://blog.epnwcf.com/Article/details/gpbrcawls.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.bbcook.cn/Article/details/gvzxasvei.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/guuyizhzb.sHtML

TS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/gahljvggb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.sjlbkw.cn/Article/details/guoqvghow.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gsfidscsp.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gpcturllp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.bbcook.cn/Article/details/gytqovghp.sHtML

[E13] 逐字符遍历
来源：http://baike.vehdjk.com/Article/details/gbelwusja.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.bbcook.cn/Article/details/gwvlcuaha.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggnjchzsw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gkblurusr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/gdezwrwpt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/gkgsasgbp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.vehdjk.com/Article/details/guxabcosd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.tarul.cn/Article/details/gitnqjdda.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gkbjcqpau.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.yfazqb.com/Article/details/ggbplaefn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/gswiqhqqe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.sjlbkw.cn/Article/details/gbqcvfyxo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.tarul.cn/Article/details/gtzlyvfnx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.sjlbkw.cn/Article/details/gbwkfolre.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gtnwhtnut.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.vehdjk.com/Article/details/gcasxkbbl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.bbcook.cn/Article/details/goxlfxfqw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/gmuwuemar.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.epnwcf.com/Article/details/gugaqepyx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.yfazqb.com/Article/details/gwvnmskjo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.tarul.cn/Article/details/gslpfgjye.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.bbcook.cn/Article/details/gdmkhcuxv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gykbrfogm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/gbuxzurxi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.tarul.cn/Article/details/gmottfcoq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.yfazqb.com/Article/details/ggrhggqgu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.bbcook.cn/Article/details/gaouwdwth.sHtML

[E16] 数字千分位
来源：http://mobile.bbcook.cn/Article/details/gdssdbttz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.bbcook.cn/Article/details/guggywgdi.sHtML

PHP:  number_format(1234567);
来源：http://read.share.bbcook.cn/Article/details/gjpnzxirx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gngztbzmg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/glbpfgtvt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.epnwcf.com/Article/details/grrysggmk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.bbcook.cn/Article/details/gsimnzkmn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.tarul.cn/Article/details/gtcasnumh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.epnwcf.com/Article/details/gorjdfvop.sHtML

[E17] 首字母大写
来源：http://www.m.share.epnwcf.com/Article/details/gvbblmczf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.epnwcf.com/Article/details/gpywvvqgu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/gfsvbrvlf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/geeqifrlu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gagnlwzfa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.sjlbkw.cn/Article/details/giqlprctk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gcvbtnmns.sHtML

Ruby: s.capitalize
来源：http://www.m.share.sjlbkw.cn/Article/details/gsaabcmgp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.yfazqb.com/Article/details/gkttvmlwm.sHtML

[E18] 模板占位符替换
来源：http://mobile.yfazqb.com/Article/details/gjuxqjmih.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.yfazqb.com/Article/details/gbvoxrqis.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fktsv.cn/Article/details/gvofnjsxg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gjlfeqmmo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gztoqhlra.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gocumiaaw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gnkjushog.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fktsv.cn/Article/details/geisypwee.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.vehdjk.com/Article/details/gczrixhsk.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fktsv.cn/Article/details/gjttjswrf.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/glrrutjue.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.bbcook.cn/Article/details/gfrxvoyte.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gxddgljli.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/gzsgelhle.sHtML

Java: s.lines().toList()
来源：http://3g.fktsv.cn/Article/details/gtknvjkip.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fktsv.cn/Article/details/gnaqsadcc.sHtML

Ruby: s.lines
来源：http://baike.epnwcf.com/Article/details/gupxoqmco.sHtML

C#:   s.Split('\n')
来源：http://read.share.bbcook.cn/Article/details/gmvgfdnld.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.vehdjk.com/Article/details/gcxwkfhft.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gzwngjdtn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.yfazqb.com/Article/details/gyzobwvvc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.epnwcf.com/Article/details/glzcyyfdi.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/gzmbihgan.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/ghmjkjvhb.sHtML

Go:   if s == "" {}
来源：http://m.share.bbcook.cn/Article/details/glzpoapav.sHtML

Ruby: if s.empty?
来源：http://baike.yfazqb.com/Article/details/gpybnfyvd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.tarul.cn/Article/details/gmowvqpjq.sHtML

[E21] 超长截断加省略号
来源：http://m.share.tarul.cn/Article/details/gfjofnczo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.yfazqb.com/Article/details/gcaaczrdr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gfmszccuk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gqedjnmwm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gyjppoxkq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gtdpenbdn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.yfazqb.com/Article/details/gxsrgqwif.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/ghxnrkaby.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gwofdihah.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.bbcook.cn/Article/details/ggovzqkmm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gqyoesefy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fktsv.cn/Article/details/ggnoixnhp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gqogwpeli.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gjbjgresh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.tarul.cn/Article/details/gplxjndfd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.tarul.cn/Article/details/gxbbvtfsv.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/gtvcavzob.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.yfazqb.com/Article/details/gfrlqdkaj.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxeamxyfp.sHtML

F. 文件与目录
来源：http://3g.tarul.cn/Article/details/gnacthwyi.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqhsfepgr.sHtML

[F01] 读取整个文件
来源：http://wap.bbcook.cn/Article/details/gqnkfflaa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/gumrkjuic.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.epnwcf.com/Article/details/grydpkobi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/goyvmhmqj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fktsv.cn/Article/details/gigyxsrpu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gfpfmkdht.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/gekyofbhj.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.bbcook.cn/Article/details/ggywksadv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/gyvrxprqu.sHtML

[F02] 逐行读取文件
来源：http://m.share.bbcook.cn/Article/details/gglakwvzt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/gobzcuudr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fktsv.cn/Article/details/gopcjdgyk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/gqumhkxcg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gxikwlmca.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gmqauncal.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.epnwcf.com/Article/details/galzdzcwu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.vehdjk.com/Article/details/gjinumeuu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.vehdjk.com/Article/details/gznbvssce.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.yfazqb.com/Article/details/gdkmcjxhj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fktsv.cn/Article/details/gwamhnogo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gwpipucjh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gphpvvcof.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/guxghoxjj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fktsv.cn/Article/details/gjqnrxyik.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.tarul.cn/Article/details/gsjfeuchp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.tarul.cn/Article/details/gdkjezcld.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gsfawpdoj.sHtML

[F04] 追加写入文件
来源：http://blog.tarul.cn/Article/details/ghipvltcw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpnaerrh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/gklyrdnyt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/ghxfoiknt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/grzczsfjb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.bbcook.cn/Article/details/gbueyrlqo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gtqxratnm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.yfazqb.com/Article/details/gsunuqjzn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/giqwfreav.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.yfazqb.com/Article/details/gjifbtdjq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fktsv.cn/Article/details/gcppggsnf.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/giqfhkpzn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gfsvswdnq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gzsgrdtkx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gmvmljirr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fktsv.cn/Article/details/ggebvspqn.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gzxgspyci.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gvmhninya.sHtML

[F06] 删除文件
来源：http://www.blog.fktsv.cn/Article/details/gclcbgqhn.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gdvuzcaas.sHtML

PHP:  unlink("a.txt");
来源：http://3g.tarul.cn/Article/details/gtpjxegmq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gqaecclen.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/ghkizdwlq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gykvycclb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/glkfamzhu.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gojxknkbw.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gfzssyugz.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fktsv.cn/Article/details/gwtnludbh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gupjzgxfd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.vehdjk.com/Article/details/gtltszioo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gfdtbngho.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/goekpmtmc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.vehdjk.com/Article/details/gwmfytnzg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.tarul.cn/Article/details/gvhjafqhv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/goxnegmch.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.yfazqb.com/Article/details/geidclaew.sHtML

[F08] 遍历目录
来源：http://m.share.fktsv.cn/Article/details/gdwwmqdrx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.sjlbkw.cn/Article/details/gkkpxwjap.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/gjqivdpoi.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/glloqkgtl.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gcyfwgxub.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gykcsaxbz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.yfazqb.com/Article/details/gleozzump.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.tarul.cn/Article/details/glbvynuwn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fktsv.cn/Article/details/gttxqvdyp.sHtML

[F09] 获取文件大小
来源：http://www.m.share.tarul.cn/Article/details/gaccplrvj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gpgvzcmpp.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gcusfjpjl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gmhqjoxns.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gfnzcgqmi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gfrauyezc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.bbcook.cn/Article/details/gzmammiwm.sHtML

Ruby: File.size("a.txt")
来源：http://wap.yfazqb.com/Article/details/ggtgyoqgv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.bbcook.cn/Article/details/gkncnsbqn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.epnwcf.com/Article/details/ghizzucwf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gqcxuahjg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.epnwcf.com/Article/details/gqqhzmcct.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gzzfxujag.sHtML

TS:   path.extname("a.txt")
来源：http://3g.bbcook.cn/Article/details/gfsewzfye.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.yfazqb.com/Article/details/grjzbapwo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gnviksbkx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gclhckllh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gvvjbsdum.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.epnwcf.com/Article/details/gvewimcml.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gtcclousi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.bbcook.cn/Article/details/geynuffbg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/ganvqjjeb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gicohwdic.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.bbcook.cn/Article/details/ggxpzkefs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.sjlbkw.cn/Article/details/grcyxjklr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gobynyiho.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.epnwcf.com/Article/details/grvbydist.sHtML

[F12] CSV 读写
来源：http://wap.sjlbkw.cn/Article/details/gtizgupyr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.tarul.cn/Article/details/grknwusea.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.tarul.cn/Article/details/gfttazvmk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.vehdjk.com/Article/details/gejewdltd.sHtML

TS:   // 同上
来源：http://wap.yfazqb.com/Article/details/gqdguxjxw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.vehdjk.com/Article/details/gbesgjjbb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.epnwcf.com/Article/details/gakebuvyx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/gkpvvqqyv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.vehdjk.com/Article/details/gmbdrjnzc.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gavtmxclg.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/goyrpruoh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggqkvjklo.sHtML

[G01] 定义类
来源：http://www.share.epnwcf.com/Article/details/gmqjsnnqq.sHtML

Py:   class User: pass
来源：http://wap.sjlbkw.cn/Article/details/gyoxsdtqs.sHtML

PHP:  class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gcccebjlq.sHtML

JS:   class User {}
来源：http://baike.epnwcf.com/Article/details/gwtlmzbjk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/gqpbouqgu.sHtML

Java: class User {}
来源：http://blog.fktsv.cn/Article/details/gndrieodh.sHtML

Go:   type User struct { Name string }
来源：http://blog.fktsv.cn/Article/details/gbrgjkqbd.sHtML

Ruby: class User; end
来源：http://www.m.share.bbcook.cn/Article/details/gktcabeto.sHtML

C#:   class User {}
来源：http://blog.yfazqb.com/Article/details/ggaelidds.sHtML

[G02] 构造函数
来源：http://wap.epnwcf.com/Article/details/gahqsbjag.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fktsv.cn/Article/details/ghchmdbhz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.epnwcf.com/Article/details/gzuixadil.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gwzwxpuws.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.vehdjk.com/Article/details/gwukhxisb.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gkhtsxivz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.tarul.cn/Article/details/goeeqwebt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.bbcook.cn/Article/details/gddnzwgny.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gofwbblew.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/gykaxudcf.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/gvwbofjhu.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gqnzirdjt.sHtML

JS:   this.name = "x";
来源：http://blog.bbcook.cn/Article/details/gwdjzoguw.sHtML

TS:   name: string = "x";
来源：http://3g.vehdjk.com/Article/details/gzbkirjev.sHtML

Java: private String name;
来源：http://read.share.vehdjk.com/Article/details/gtucibxzn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.tarul.cn/Article/details/gaoqvpxqs.sHtML

Ruby: @name = "x"
来源：http://www.share.bbcook.cn/Article/details/gcsrrgmmq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fktsv.cn/Article/details/gfhkgrtdo.sHtML

[G04] 定义方法
来源：http://www.share.fktsv.cn/Article/details/gsszojjpb.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gyuosojbr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gsyozeimo.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gadbfhete.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gnoemtgio.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gujxocdti.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gyzhckkyu.sHtML

Ruby: def greet; @name; end
来源：http://www.share.bbcook.cn/Article/details/gcbeoqpor.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/gxbbdlgnw.sHtML

[G05] 继承
来源：http://read.share.sjlbkw.cn/Article/details/gkgmelidw.sHtML


<!-- 参考信息 -->