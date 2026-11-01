代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.yfazqb.com/Article/details/gmenyvuuh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.vehdjk.com/Article/details/gpfpnssmy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.sjlbkw.cn/Article/details/ghboqraon.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gulwiqycb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.vehdjk.com/Article/details/gpapzmboz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.tarul.cn/Article/details/ghzbfetaf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gmdjkfpcf.sHtML

[D26] 数组转字符串
来源：http://wap.vehdjk.com/Article/details/gvgiofszm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.yfazqb.com/Article/details/gwrsjkljl.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/ghwjdvsjr.sHtML

JS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gnevehtqt.sHtML

TS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gpopfsivh.sHtML

Java: String.join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gqlfadqvh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.epnwcf.com/Article/details/gwirupvsh.sHtML

Ruby: arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gwlcltdmr.sHtML

C#:   string.Join(", ", list)
来源：http://wap.bbcook.cn/Article/details/gbtfypxip.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwubrrxam.sHtML

E. 字符串处理
来源：http://blog.epnwcf.com/Article/details/gyyqyfscl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdunqfuod.sHtML

[E01] 拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gvigpjlir.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/giicwqzmr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.epnwcf.com/Article/details/geeyedsln.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gqtewavtx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gikrtuijl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.tarul.cn/Article/details/gfgrzdjqh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.sjlbkw.cn/Article/details/gtawiprxi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.bbcook.cn/Article/details/gviznhgeu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fktsv.cn/Article/details/ggcxyvsoe.sHtML

[E02] 重复字符串
来源：http://wap.bbcook.cn/Article/details/gomcgdhqu.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gixrrosfz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.tarul.cn/Article/details/gwnzajfpn.sHtML

JS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/ghihhlgub.sHtML

TS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gfhcshpda.sHtML

Java: "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gcuglfpix.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fktsv.cn/Article/details/gclxxmyos.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gjmeaequq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.epnwcf.com/Article/details/gwpmhxktl.sHtML

[E03] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gtueidcnf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.bbcook.cn/Article/details/gdexrrcsk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/guchlootw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/grzogjpcu.sHtML

TS:   s.slice(1, 4)
来源：http://3g.yfazqb.com/Article/details/gkmcvsxsb.sHtML

Java: s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/gazwkqbki.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fktsv.cn/Article/details/gunsaenki.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.epnwcf.com/Article/details/gbeindaue.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gokzcubcd.sHtML

[E04] 查找子串位置
来源：http://blog.epnwcf.com/Article/details/gwewuulah.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.yfazqb.com/Article/details/gffelhqcm.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.epnwcf.com/Article/details/gsfnoedqh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/gnbmuixwb.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gibasrjzn.sHtML

Java: s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gavwldshr.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.yfazqb.com/Article/details/grqpcnctr.sHtML

Ruby: s.index("x")
来源：http://read.share.fktsv.cn/Article/details/gnvxxizgh.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gkmeyhwpo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.epnwcf.com/Article/details/gyhqszthr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.vehdjk.com/Article/details/ggjcblqew.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.sjlbkw.cn/Article/details/gwtivtceb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gjgdbphll.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.epnwcf.com/Article/details/gkjdsglfj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/ginpjizga.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fktsv.cn/Article/details/guuyufuwh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/gvtylfaop.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.epnwcf.com/Article/details/gvdrtquim.sHtML

[E06] 替换子串
来源：http://read.share.sjlbkw.cn/Article/details/gvvsoegtf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gklnfqiqq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/gnxxsikmj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gcmxpfdvc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gklocvxbu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gwqjortcm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/gjgfjchkp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gjmvkxbni.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.bbcook.cn/Article/details/ggwjpdclk.sHtML

[E07] 按分隔符拆分
来源：http://m.share.yfazqb.com/Article/details/gcpmvarxb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.bbcook.cn/Article/details/gukqjbmyp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.epnwcf.com/Article/details/gidfvnegb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gksgwvlqt.sHtML

TS:   s.split(",")
来源：http://blog.bbcook.cn/Article/details/gtltrgdek.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.epnwcf.com/Article/details/gxjyhjaoq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.bbcook.cn/Article/details/gmtsbjqvb.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.sjlbkw.cn/Article/details/gawwjlegn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.sjlbkw.cn/Article/details/gfwnjsske.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/gcvxjwnov.sHtML

Py:   ",".join(items)
来源：http://baike.fktsv.cn/Article/details/gftqfaxvb.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/gvmbefkqi.sHtML

JS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gvlegtern.sHtML

TS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gqoobrygp.sHtML

Java: String.join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gptueklym.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.bbcook.cn/Article/details/gewfytock.sHtML

Ruby: items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gwsekqjel.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gkqmgserj.sHtML

[E09] 去除所有空白字符
来源：http://blog.fktsv.cn/Article/details/gwizoupmo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fktsv.cn/Article/details/gsjhklluy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gvtzptheo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gpvvxsega.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhwfifhf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gvvrquwiv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.epnwcf.com/Article/details/gnvlslkbg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fktsv.cn/Article/details/gqwacapvb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fktsv.cn/Article/details/ghivklvju.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.sjlbkw.cn/Article/details/gjbfhtzkl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gbubzmbru.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.sjlbkw.cn/Article/details/gvmffdodo.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/geqvlgkra.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gjystlnja.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gqsduqwgd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gmnsblxtl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/geognsxmu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.yfazqb.com/Article/details/gtystjikb.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gexuesbnf.sHtML

Py:   s[::-1]
来源：http://blog.yfazqb.com/Article/details/ggqhvrsyi.sHtML

PHP:  strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gtwkisplx.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gnrdgepcg.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gvmbmvdam.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.epnwcf.com/Article/details/galltxaft.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.tarul.cn/Article/details/gvxvikmmk.sHtML

Ruby: s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gvypjdgcb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/grmprtutf.sHtML

[E12] 统计某字符出现次数
来源：http://blog.sjlbkw.cn/Article/details/gncrpinnl.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gycaoaiuw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/gduxhlmme.sHtML

JS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gcgluixaj.sHtML

TS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gdbzukxzw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gupicgxuv.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.sjlbkw.cn/Article/details/ggyxcpegs.sHtML

Ruby: s.count("a")
来源：http://m.share.yfazqb.com/Article/details/ggayyswrc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fktsv.cn/Article/details/gdgjzeylj.sHtML

[E13] 逐字符遍历
来源：http://3g.vehdjk.com/Article/details/gcbjfxugz.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.tarul.cn/Article/details/glftfhohb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.vehdjk.com/Article/details/gwnycldju.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/ghgjckvmq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gfpccudmu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/gurrxtfac.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.epnwcf.com/Article/details/geshvlncr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.bbcook.cn/Article/details/gkhbvzcwd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.yfazqb.com/Article/details/glmdknoke.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fktsv.cn/Article/details/gocsupjvk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.bbcook.cn/Article/details/gwulpdwks.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.tarul.cn/Article/details/ghyfqreud.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.bbcook.cn/Article/details/gevyamhgt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fktsv.cn/Article/details/gcyeharip.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.epnwcf.com/Article/details/gubdrhtbp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.epnwcf.com/Article/details/gqcncmyoo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.epnwcf.com/Article/details/gfiipkaec.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.yfazqb.com/Article/details/gmfhipfmb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fktsv.cn/Article/details/gnusdzogp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.bbcook.cn/Article/details/gsqcfablu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.epnwcf.com/Article/details/gsikrpszp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.bbcook.cn/Article/details/gzzuhkirc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.yfazqb.com/Article/details/gbjyhjwpp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/gafmpbgdt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.tarul.cn/Article/details/gouuokocp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fktsv.cn/Article/details/ghpbnhoyv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.vehdjk.com/Article/details/gjowjrpsk.sHtML

[E16] 数字千分位
来源：http://read.share.fktsv.cn/Article/details/gouhwnibu.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fktsv.cn/Article/details/ghwrhjdil.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/gngoxxjvk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/grqmnqsgt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gjwescgyr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.tarul.cn/Article/details/gaidhebzw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.tarul.cn/Article/details/gshldqsbs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.tarul.cn/Article/details/gthtajede.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.epnwcf.com/Article/details/gsxsucinu.sHtML

[E17] 首字母大写
来源：http://m.share.fktsv.cn/Article/details/gnnwyiwfv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/gpfirojhi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.tarul.cn/Article/details/glpdukbcn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gwdhshfwf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gxdedwqtp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.tarul.cn/Article/details/gadxamvuz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gngvzonvl.sHtML

Ruby: s.capitalize
来源：http://3g.yfazqb.com/Article/details/gtajdzmil.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/goxzeaurj.sHtML

[E18] 模板占位符替换
来源：http://mobile.tarul.cn/Article/details/gyhyzoflz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.epnwcf.com/Article/details/ggpoanyvl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.vehdjk.com/Article/details/gpzrudosu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtldmpohu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gqxnvhyjn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gzamqexdp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/gcjphorex.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.tarul.cn/Article/details/gztryujer.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.yfazqb.com/Article/details/garkwtmzp.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.vehdjk.com/Article/details/gtxikeqxq.sHtML

Py:   s.splitlines()
来源：http://www.blog.epnwcf.com/Article/details/gdtxkyedb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.tarul.cn/Article/details/grwpjncok.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gggohayda.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gsisqvcgv.sHtML

Java: s.lines().toList()
来源：http://blog.bbcook.cn/Article/details/gahqkupaq.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/gkavdokia.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/gfxmeleob.sHtML

C#:   s.Split('\n')
来源：http://mobile.vehdjk.com/Article/details/giywqjkej.sHtML

[E20] 判断字符串是否为空
来源：http://3g.vehdjk.com/Article/details/grmutyaro.sHtML

Py:   if not s:
来源：http://read.share.epnwcf.com/Article/details/gcbimepkz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.yfazqb.com/Article/details/gogledkbw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.tarul.cn/Article/details/ghflikjfq.sHtML

TS:   if (s === "") {}
来源：http://3g.tarul.cn/Article/details/gnuxthqsf.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/gwobwuqlx.sHtML

Go:   if s == "" {}
来源：http://m.share.yfazqb.com/Article/details/gbbijpajl.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/ghaogiujj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.epnwcf.com/Article/details/ginsqiqfc.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/gcnnlsrst.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.bbcook.cn/Article/details/gsantbkhk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gpkqtibxw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/ggzuunumy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gxxqcwoap.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gopmedsek.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.yfazqb.com/Article/details/guppvnjjf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gncygbnww.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gffpgkpma.sHtML

[E22] 字节长度与字符长度
来源：http://baike.bbcook.cn/Article/details/gqubmhtim.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gwjekntjr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gupfrmcln.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gihwyfaxg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gpnzcetgu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fktsv.cn/Article/details/gaciwdlmz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.tarul.cn/Article/details/gegsidvql.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.epnwcf.com/Article/details/ggqbtxuft.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gvesnspme.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gobroagvl.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/ggemvlnce.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gygumnxkr.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/gdaosrjmp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.sjlbkw.cn/Article/details/gtsfkerri.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/gogdicfdd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.sjlbkw.cn/Article/details/gtqbvoqqg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.yfazqb.com/Article/details/gmxicylad.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gwhzqjkyb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.tarul.cn/Article/details/gcfuxnzii.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fktsv.cn/Article/details/gmtpvtkxh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gjjqceqsd.sHtML

[F02] 逐行读取文件
来源：http://m.share.yfazqb.com/Article/details/gncbskcgj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/gcpyzoafr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.tarul.cn/Article/details/guggtkown.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/grnlpqbyc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gwuqqdqmv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/gieowxxtp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.tarul.cn/Article/details/goarhbhnl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.vehdjk.com/Article/details/gjunybvfk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.sjlbkw.cn/Article/details/gbtalameg.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/gtfgpdgqf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.epnwcf.com/Article/details/gquqfztej.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gsztlvrdh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gcbooxkbs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gvsifybux.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.tarul.cn/Article/details/gfemlpcvt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.epnwcf.com/Article/details/ghcoemlhg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/gtlbdqvqg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/geewkozzr.sHtML

[F04] 追加写入文件
来源：http://www.blog.sjlbkw.cn/Article/details/gkynsojtv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gqqbhhjsi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.vehdjk.com/Article/details/gzkvjxuul.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gddufpiti.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gmogsflgp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fktsv.cn/Article/details/gapvlsrku.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/ggageykbg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fktsv.cn/Article/details/gestjfxmc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fktsv.cn/Article/details/gcvlnvljp.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.yfazqb.com/Article/details/gfcvmjveh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/goombqixa.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.bbcook.cn/Article/details/ghmoymjoq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gsexxqncb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gthnetwip.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gchzvtqwp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.yfazqb.com/Article/details/gopubwdei.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.tarul.cn/Article/details/gzzkeiyte.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gozwwxxvt.sHtML

[F06] 删除文件
来源：http://3g.sjlbkw.cn/Article/details/gihstmdiv.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gxcimkrqr.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gdadubsus.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gjuhvzmmo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gsqqzsllp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gaqiufcoa.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gofeesaxj.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.yfazqb.com/Article/details/goqgttgnr.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gyhggqlrb.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fktsv.cn/Article/details/gtubvgwan.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.yfazqb.com/Article/details/ghpazebah.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/gygyyqohi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/ggoqevhop.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gwrlfvqck.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.tarul.cn/Article/details/gjjmgknnk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.sjlbkw.cn/Article/details/gyziqswfl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.bbcook.cn/Article/details/gubdyylpv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.tarul.cn/Article/details/gsnqjjlzh.sHtML

[F08] 遍历目录
来源：http://www.share.vehdjk.com/Article/details/giqusnelh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.tarul.cn/Article/details/ggnfmnvtw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/gkzrzupfd.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/gftlqpuqi.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gwknnsnok.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gijonlkae.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fktsv.cn/Article/details/gzbrmaxfh.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.tarul.cn/Article/details/gpgnrsiut.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fktsv.cn/Article/details/gnsyiklqp.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gtahtgqit.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.yfazqb.com/Article/details/gdhfkyvpv.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.vehdjk.com/Article/details/ghgupesqs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gaxqbjzug.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gomkkkniv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gdfcbznyr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.epnwcf.com/Article/details/gwsgtgffr.sHtML

Ruby: File.size("a.txt")
来源：http://baike.bbcook.cn/Article/details/gesbygcom.sHtML


<!-- 参考信息 -->