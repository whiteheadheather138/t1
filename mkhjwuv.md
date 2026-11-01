代发 wailian999

PHP:  implode(",", $items);
来源：http://www.blog.bbcook.cn/Article/details/gthrbaxiq.sHtML

JS:   items.join(",")
来源：http://read.share.yfazqb.com/Article/details/gtgsedove.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gwhszwsgd.sHtML

Java: String.join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gjuozcfhx.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fktsv.cn/Article/details/ghmpitncj.sHtML

Ruby: items.join(",")
来源：http://read.share.yfazqb.com/Article/details/ghqfnrobh.sHtML

C#:   string.Join(",", items)
来源：http://www.share.tarul.cn/Article/details/grrvrvkaf.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/glbpzckeq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.yfazqb.com/Article/details/gsqplefco.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.yfazqb.com/Article/details/gcfakydcv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gnhpgsuas.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.yfazqb.com/Article/details/gnvfwsohh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gnaoncegf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.epnwcf.com/Article/details/gkrhuutkt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.sjlbkw.cn/Article/details/guhlpgouz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gzduuwlpn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fktsv.cn/Article/details/gejxiaglv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gciaqigsr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.tarul.cn/Article/details/ggahsvlvm.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gvudfbrpp.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gpohccoxa.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gcyznkuzq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/ghmozsmah.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gxpshzgwm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.tarul.cn/Article/details/gqeywtacr.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/gzpijrkyj.sHtML

Py:   s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gmwawsljm.sHtML

PHP:  strrev($s);
来源：http://www.share.fktsv.cn/Article/details/gxyaqvqxh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gclnwfysa.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gbkppjckn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.tarul.cn/Article/details/gnbfgdlts.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/glullejog.sHtML

Ruby: s.reverse
来源：http://wap.tarul.cn/Article/details/goqbwtaqa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gtqnwkkel.sHtML

[E12] 统计某字符出现次数
来源：http://blog.yfazqb.com/Article/details/gahtatgnp.sHtML

Py:   s.count("a")
来源：http://baike.fktsv.cn/Article/details/gjkzxszwo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.sjlbkw.cn/Article/details/gtczmkjze.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/guzotehry.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gowsicyjf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.bbcook.cn/Article/details/gnfwemjut.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.yfazqb.com/Article/details/gdcxtnvpk.sHtML

Ruby: s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gezpboczf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.vehdjk.com/Article/details/gjdgmigpf.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/gajzhzdrn.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gikzrmjjf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.yfazqb.com/Article/details/gizovdwxi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/ggizamjtx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/gdrpbhxxd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gtocmqaxo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.epnwcf.com/Article/details/grncgauiv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.yfazqb.com/Article/details/gucbtomgm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/ghgilfodr.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.vehdjk.com/Article/details/ggyefsrqb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.vehdjk.com/Article/details/glanqklsz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gwrbkithp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.vehdjk.com/Article/details/giykdkuck.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/gtnurubqu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.vehdjk.com/Article/details/gnncpcnyu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.bbcook.cn/Article/details/gfuucjotv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.tarul.cn/Article/details/gtuarsuqm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.tarul.cn/Article/details/gydtvxdyw.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.epnwcf.com/Article/details/gbqxmjkih.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxdafvcyk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.bbcook.cn/Article/details/gjcvhoazf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.bbcook.cn/Article/details/gcypsmmro.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/gnptjnymn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/guvwhkxyv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.sjlbkw.cn/Article/details/gsnnsnpjz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fktsv.cn/Article/details/gozzonpds.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.yfazqb.com/Article/details/gmbbmowcg.sHtML

[E16] 数字千分位
来源：http://m.share.bbcook.cn/Article/details/gfyamylni.sHtML

Py:   f"{1234567:,}"
来源：http://wap.sjlbkw.cn/Article/details/ghunfbafb.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.sjlbkw.cn/Article/details/grqimqxmf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/gwnixhmzc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gkwgfegef.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/gmxbxzvmg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fktsv.cn/Article/details/gyeqaecje.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.bbcook.cn/Article/details/gzcclkhzz.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.vehdjk.com/Article/details/gpjhvgtay.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/gophtlvpo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fktsv.cn/Article/details/gyphctktq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.tarul.cn/Article/details/gqglwtetq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gimtbewuq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.epnwcf.com/Article/details/gtzqvpbyh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.yfazqb.com/Article/details/gdowdvrpg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gxpcnagtw.sHtML

Ruby: s.capitalize
来源：http://www.blog.epnwcf.com/Article/details/gtbarranl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fktsv.cn/Article/details/gxtimpnih.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.yfazqb.com/Article/details/gmlldvgdc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.epnwcf.com/Article/details/gsovmedua.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.bbcook.cn/Article/details/gtucsgsjy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gdoaqlmlz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gslnpenjk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gsdkxazch.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/gratfnzvk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/gojttzqny.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.yfazqb.com/Article/details/ggupdwkwh.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.vehdjk.com/Article/details/gsconwwxw.sHtML

Py:   s.splitlines()
来源：http://www.share.bbcook.cn/Article/details/gjglcuqfw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fktsv.cn/Article/details/gfuajzvte.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gkkkzoieo.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/gnbxfbidx.sHtML

Java: s.lines().toList()
来源：http://read.share.vehdjk.com/Article/details/gpypytkuw.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.vehdjk.com/Article/details/gszbbbffq.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/ghstnittn.sHtML

C#:   s.Split('\n')
来源：http://blog.vehdjk.com/Article/details/gadyokiae.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.epnwcf.com/Article/details/gqukganuv.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/gmzfsdzds.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.sjlbkw.cn/Article/details/glxuxiiwp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.bbcook.cn/Article/details/getuejsoa.sHtML

TS:   if (s === "") {}
来源：http://3g.bbcook.cn/Article/details/gqgfnhlhh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fktsv.cn/Article/details/geoyqpgze.sHtML

Go:   if s == "" {}
来源：http://mobile.tarul.cn/Article/details/gslaypzic.sHtML

Ruby: if s.empty?
来源：http://3g.yfazqb.com/Article/details/gekxrippp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gwbybrbvy.sHtML

[E21] 超长截断加省略号
来源：http://wap.tarul.cn/Article/details/gfbocstgw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/gssezhpyk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/giuqvlpmt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gtzpmniaq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gswlfpzjs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gxejqvlsl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fktsv.cn/Article/details/glgrtimdn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/ghsggufzv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/gqhrowori.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.bbcook.cn/Article/details/gbaflurjk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.tarul.cn/Article/details/gdcnwhusc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/ghepfjluk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gbtboaczj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gpugrhjpa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gjwhwjbvh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.vehdjk.com/Article/details/gilbqebem.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gbacsbann.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/ghotbpxfc.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gppvjvgtw.sHtML

F. 文件与目录
来源：http://read.share.tarul.cn/Article/details/gthzanagw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkwnlcnwb.sHtML

[F01] 读取整个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gohldikpd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.bbcook.cn/Article/details/gaxrolzew.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gaknjmvlm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.yfazqb.com/Article/details/gomtcxovc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.yfazqb.com/Article/details/ggpajrtlb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/grdnbwwcr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/gyzdljjpt.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gwcjqibdn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gvseytzcp.sHtML

[F02] 逐行读取文件
来源：http://wap.tarul.cn/Article/details/gzhmyjwce.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.bbcook.cn/Article/details/ghprylwtj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.vehdjk.com/Article/details/gqwalsckf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gkmmitexp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gszoktjin.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gcuyjcxim.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/gutksihhs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.tarul.cn/Article/details/gbgnpfuol.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fktsv.cn/Article/details/gmahwesxn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/gshygasnp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.epnwcf.com/Article/details/gpqfjnwjy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gpopruuxq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.tarul.cn/Article/details/gptqzbfrh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gsniecqyl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fktsv.cn/Article/details/gempubtgq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.vehdjk.com/Article/details/gocelpdxg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/ggaloxmcg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gxzmgkvte.sHtML

[F04] 追加写入文件
来源：http://www.m.share.tarul.cn/Article/details/gnltsvicy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfdyxqbv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/gnivftvfy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gaxdoewtg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gwayenzak.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.tarul.cn/Article/details/gvubhgvdb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fktsv.cn/Article/details/gqffhgdkc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.tarul.cn/Article/details/gwpsygevv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/ghyqcgubc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gzyguggex.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.epnwcf.com/Article/details/ggjnxoeqi.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gpmnuvxur.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gmspccxul.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gjeoqeimj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gxdffbinr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.yfazqb.com/Article/details/gyintjvny.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.tarul.cn/Article/details/gbammleqy.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.yfazqb.com/Article/details/guxogggsx.sHtML

[F06] 删除文件
来源：http://www.blog.fktsv.cn/Article/details/gehmtaquo.sHtML

Py:   os.remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gwzzjxvcm.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.bbcook.cn/Article/details/ghbqpngdh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/ghmqfxsbd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gnmdxcdoy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gxhuxresx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmusgoalq.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.tarul.cn/Article/details/gjciyuxsb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gutisfgpt.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.yfazqb.com/Article/details/ghrzeryha.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/geqbuhixa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/grcpcztpg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/gktgeynez.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gfpdizywe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.vehdjk.com/Article/details/gnzfyphcx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.sjlbkw.cn/Article/details/gzwmjnrng.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fktsv.cn/Article/details/guufctgif.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fktsv.cn/Article/details/grfrwwmpi.sHtML

[F08] 遍历目录
来源：http://www.m.share.fktsv.cn/Article/details/gumjxslyn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fktsv.cn/Article/details/gnythfmbm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fktsv.cn/Article/details/gjxqrbxfd.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gaufaoynv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gvpsukmrv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gfvtfjxcq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gztofanbb.sHtML

Ruby: Dir.children("dir")
来源：http://baike.epnwcf.com/Article/details/grukvsxma.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.vehdjk.com/Article/details/guywvsjtp.sHtML

[F09] 获取文件大小
来源：http://www.blog.fktsv.cn/Article/details/gtsmnfpql.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fktsv.cn/Article/details/gdawxfybg.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fktsv.cn/Article/details/gufpwpask.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/ginmgqnnf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gmetszmkz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/grwzymdxf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.yfazqb.com/Article/details/gzayvzema.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gakxxeods.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.sjlbkw.cn/Article/details/guvvcukjf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.tarul.cn/Article/details/gplgysyfi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/glwnpyzpi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gdpnmenwf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/grqwkcyhh.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/ghyznhyzd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.bbcook.cn/Article/details/gjyiheudo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxoavsist.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/guuykpdgh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gguridauy.sHtML

[F11] 复制与移动文件
来源：http://wap.sjlbkw.cn/Article/details/gekywsvfy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/ggpoocshn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.tarul.cn/Article/details/ggdfhzcal.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gglnroewq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gzqvlwago.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.vehdjk.com/Article/details/gpkiquotx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/gcdxgwtkl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gbiapccda.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.sjlbkw.cn/Article/details/gpwdvohey.sHtML

[F12] CSV 读写
来源：http://m.share.tarul.cn/Article/details/gqmfpsodn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.bbcook.cn/Article/details/guwmonyfy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.tarul.cn/Article/details/gvaxbvosn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.epnwcf.com/Article/details/gdnylaaid.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/gpjxykkyr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.sjlbkw.cn/Article/details/gfnykskct.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.sjlbkw.cn/Article/details/ginzfimyy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/gzocfreub.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.sjlbkw.cn/Article/details/gqstgzfnn.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gctzllcpr.sHtML

G. 面向对象
来源：http://www.m.share.bbcook.cn/Article/details/gclsxblxl.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvmphppqi.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/gxicbynfz.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/gquyqcbwg.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gngsmkyvw.sHtML

JS:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gehfhmjbc.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.tarul.cn/Article/details/grpgebido.sHtML

Java: class User {}
来源：http://www.share.vehdjk.com/Article/details/gehhfxhhl.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/gslhperyz.sHtML

Ruby: class User; end
来源：http://www.share.yfazqb.com/Article/details/gzgubmuqf.sHtML

C#:   class User {}
来源：http://baike.bbcook.cn/Article/details/gmbsabqir.sHtML

[G02] 构造函数
来源：http://3g.fktsv.cn/Article/details/gelskyrun.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.vehdjk.com/Article/details/gzmnecjpg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gwmzaoqwt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gmlyhokza.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/glneoxqer.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gxhvsmsrr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fktsv.cn/Article/details/gcjuzdxmw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/gvwdugwwj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.bbcook.cn/Article/details/glszwacrf.sHtML

[G03] 实例属性
来源：http://www.blog.vehdjk.com/Article/details/gzkoxgojn.sHtML

Py:   self.name = "x"
来源：http://read.share.yfazqb.com/Article/details/gvqmutqfp.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gcfjkwyaj.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/grtyikfkk.sHtML

TS:   name: string = "x";
来源：http://wap.vehdjk.com/Article/details/giuaxioxw.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gmnhtjmjf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/gsvvajdir.sHtML

Ruby: @name = "x"
来源：http://mobile.bbcook.cn/Article/details/gkzocrjel.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gkrrsrlpd.sHtML

[G04] 定义方法
来源：http://blog.bbcook.cn/Article/details/gkfglhikm.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fktsv.cn/Article/details/gcuisnqpa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gxqbsqwok.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/glaxhxhzw.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/ghwtjjdis.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gocpiekfa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gdtsaoauq.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/gqaroydmp.sHtML

C#:   public string Greet() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gqvsvwlgd.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/glndxrach.sHtML

Py:   class Admin(User): pass
来源：http://wap.epnwcf.com/Article/details/gdlwjqzam.sHtML

PHP:  class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gxvnloafs.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gddzfexdm.sHtML

TS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gzomtprey.sHtML

Java: class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gbwrqewbk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fktsv.cn/Article/details/gdzdzhdcg.sHtML

Ruby: class Admin < User; end
来源：http://mobile.yfazqb.com/Article/details/ggqglihgx.sHtML

C#:   class Admin : User {}
来源：http://blog.vehdjk.com/Article/details/gqsxdhghh.sHtML

[G06] 重写方法
来源：http://mobile.fktsv.cn/Article/details/ghlbgkhwr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/gpkovnkff.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gjyzqbbaf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gjkalypaa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gzwgaypgz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gmkctvnhn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fktsv.cn/Article/details/gsorvpntj.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gmkkhhiys.sHtML


<!-- 参考信息 -->