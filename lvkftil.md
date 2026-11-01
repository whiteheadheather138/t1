代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/gwowfiiuz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.bbcook.cn/Article/details/gfrbaudnf.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fktsv.cn/Article/details/giteltohj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/ghjgssxfi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fktsv.cn/Article/details/gqvwjjqxe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.vehdjk.com/Article/details/ggmtbxqki.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.bbcook.cn/Article/details/gdxmccdvn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gprsdlvhp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.yfazqb.com/Article/details/gztsqeuvx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.yfazqb.com/Article/details/guzpetwhs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.epnwcf.com/Article/details/guwkmzxbm.sHtML

[D26] 数组转字符串
来源：http://blog.sjlbkw.cn/Article/details/gogawtdcx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.vehdjk.com/Article/details/gkyrxvaip.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.vehdjk.com/Article/details/gvxrvzydr.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/grmygcavf.sHtML

TS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gxznvoxrc.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gwzqnwsgb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.vehdjk.com/Article/details/gbxzwlcck.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gmbmxpjyf.sHtML

C#:   string.Join(", ", list)
来源：http://blog.tarul.cn/Article/details/gmobvcmtm.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gwwtqudwa.sHtML

E. 字符串处理
来源：http://3g.yfazqb.com/Article/details/goomdfejo.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqiirtull.sHtML

[E01] 拼接字符串
来源：http://baike.vehdjk.com/Article/details/gerafsrbu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.tarul.cn/Article/details/grogsdvsf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.epnwcf.com/Article/details/gzqoxudnj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gwazprgqr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gttrdgolm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/gbgwnbgis.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.epnwcf.com/Article/details/ghwjqqarz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.bbcook.cn/Article/details/gqonfinpj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fktsv.cn/Article/details/gznzhkyva.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gqzfzejcu.sHtML

Py:   "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gmcxmdwud.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.tarul.cn/Article/details/glxizesnv.sHtML

JS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gtazbhkaj.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/goiuhjdoe.sHtML

Java: "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gxrkjvmzi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.vehdjk.com/Article/details/gerjhpnpl.sHtML

Ruby: "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/ghtyciiij.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fktsv.cn/Article/details/gqrwqlcpj.sHtML

[E03] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gtogtfwim.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.tarul.cn/Article/details/ghfpofgto.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gjpcrsyrb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/ggxevxgul.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gyaeowuse.sHtML

Java: s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/gnbexnefm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.epnwcf.com/Article/details/gruywvvaa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.vehdjk.com/Article/details/grejsevwi.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fktsv.cn/Article/details/gwzkzmfas.sHtML

[E04] 查找子串位置
来源：http://wap.yfazqb.com/Article/details/grgaeyykj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/grgmibzig.sHtML

PHP:  strpos($s, "x");
来源：http://blog.epnwcf.com/Article/details/gshmscarv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.sjlbkw.cn/Article/details/ggbivvkeu.sHtML

TS:   s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gldiaknzh.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gceifqnzr.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.bbcook.cn/Article/details/gtbqcfdnd.sHtML

Ruby: s.index("x")
来源：http://blog.fktsv.cn/Article/details/gweyubcbk.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.tarul.cn/Article/details/gbysahlsv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fktsv.cn/Article/details/glqgjcfhm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fktsv.cn/Article/details/gwjkbflvi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.yfazqb.com/Article/details/gaerhnjgm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/gsqlzmxay.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fktsv.cn/Article/details/gojdyffoq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gtgwbdmpe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.sjlbkw.cn/Article/details/gduyrvgrs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.bbcook.cn/Article/details/ggbtitbxu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.bbcook.cn/Article/details/gsoskerru.sHtML

[E06] 替换子串
来源：http://blog.tarul.cn/Article/details/gzsyunfin.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gyjzehlcp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.tarul.cn/Article/details/gjcftmpnr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gmvfjvdgc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gxlizjxqv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/guaamlokl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/gjcjawmxm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.bbcook.cn/Article/details/grkplngad.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gtxuhxaya.sHtML

[E07] 按分隔符拆分
来源：http://mobile.vehdjk.com/Article/details/gevqqctgb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/gmidlnmcl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gdoghgnai.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.yfazqb.com/Article/details/gkrxwwnzp.sHtML

TS:   s.split(",")
来源：http://www.share.bbcook.cn/Article/details/gxxjwpvqs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fktsv.cn/Article/details/gpjcwwfjc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.tarul.cn/Article/details/gxbhfmspi.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.sjlbkw.cn/Article/details/glhsfbbic.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.sjlbkw.cn/Article/details/gjiuiegxh.sHtML

[E08] 数组按分隔符合并
来源：http://blog.tarul.cn/Article/details/gyfadyxuj.sHtML

Py:   ",".join(items)
来源：http://www.share.fktsv.cn/Article/details/geluenixd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.yfazqb.com/Article/details/gxqsepnbr.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gcyqjzwrz.sHtML

TS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/goflxjozy.sHtML

Java: String.join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gszwbgdon.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.epnwcf.com/Article/details/gpmxczuvk.sHtML

Ruby: items.join(",")
来源：http://m.share.tarul.cn/Article/details/gqjjungae.sHtML

C#:   string.Join(",", items)
来源：http://3g.vehdjk.com/Article/details/ghmzqzbog.sHtML

[E09] 去除所有空白字符
来源：http://read.share.bbcook.cn/Article/details/gjhhylerc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.epnwcf.com/Article/details/gwfdqaaxa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.yfazqb.com/Article/details/gtlczltux.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gtbqjmjuh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/gawoulezg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gbewokyxk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.sjlbkw.cn/Article/details/gkukplnqa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.bbcook.cn/Article/details/gdhxuyvsn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/gimpdngom.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/gshvmjiuv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/gezgexhsh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.bbcook.cn/Article/details/gckxykxhu.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gfpmxfwge.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/glkchaisv.sHtML

Java: String.format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gzdsivssf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gpzjadata.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gylgkrjkc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fktsv.cn/Article/details/gyeiriydc.sHtML

[E11] 反转字符串
来源：http://www.share.tarul.cn/Article/details/gbvicgayu.sHtML

Py:   s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gmhkritde.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gvpduxbfj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gqxfinkla.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gbnciluqf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gbkfomxsp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.bbcook.cn/Article/details/gmdduroxb.sHtML

Ruby: s.reverse
来源：http://3g.tarul.cn/Article/details/gvnsaojug.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gawfvjwqa.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/grmltnjpf.sHtML

Py:   s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gurhfaxby.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.yfazqb.com/Article/details/gyswlgvip.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.epnwcf.com/Article/details/gudfbibde.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gltizeaxf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.bbcook.cn/Article/details/gphfizsaq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.sjlbkw.cn/Article/details/gmfbbyhnv.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gwgchjttj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.sjlbkw.cn/Article/details/gaycemplm.sHtML

[E13] 逐字符遍历
来源：http://wap.sjlbkw.cn/Article/details/gwympniyc.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fktsv.cn/Article/details/gaxlukpyr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.tarul.cn/Article/details/gnfyyggku.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gpicndhyg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/gliyivbnu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.bbcook.cn/Article/details/gbmtmtxum.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fktsv.cn/Article/details/gosshpsqv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/ghlreoxil.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/gvfgaobgj.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.yfazqb.com/Article/details/gjdvymveg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.bbcook.cn/Article/details/gpdrhmrhu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.vehdjk.com/Article/details/gahkktsch.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fktsv.cn/Article/details/gxnkglskd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ghlmozbxl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fktsv.cn/Article/details/ghfjchisp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.yfazqb.com/Article/details/gxhmkeapq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.vehdjk.com/Article/details/gylcauwsj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.epnwcf.com/Article/details/gwqvggrsp.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fktsv.cn/Article/details/gqmgbtlpt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/garxbnhev.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.tarul.cn/Article/details/gucgqxtti.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.sjlbkw.cn/Article/details/gusuwkcuu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gxolaibme.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.epnwcf.com/Article/details/glghbvmpn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.tarul.cn/Article/details/gjccduxzf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/giqpttbxx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.epnwcf.com/Article/details/gltjbpuyz.sHtML

[E16] 数字千分位
来源：http://read.share.bbcook.cn/Article/details/gzkfrajop.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.vehdjk.com/Article/details/gyqpeudsq.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.vehdjk.com/Article/details/ggjornhlj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/gvdiwngfr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gvvpiblne.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/gzmkrybjf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.bbcook.cn/Article/details/gybixlwni.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/gxzpeumky.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.tarul.cn/Article/details/giegvjsvn.sHtML

[E17] 首字母大写
来源：http://baike.vehdjk.com/Article/details/gwqicmcya.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.epnwcf.com/Article/details/gdkgngzcj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.bbcook.cn/Article/details/ginpsrqfk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gcvtheznj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/gcvetyzqu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.epnwcf.com/Article/details/gvkqjwpmy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/gpiynhlui.sHtML

Ruby: s.capitalize
来源：http://read.share.bbcook.cn/Article/details/gisqljobm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/gkwpkqhho.sHtML

[E18] 模板占位符替换
来源：http://wap.bbcook.cn/Article/details/glhpzizpc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.bbcook.cn/Article/details/gegwnssli.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fktsv.cn/Article/details/gqchinynr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gtsopzlmk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gilitnvqj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/ghshqthid.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gledlxdkj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.vehdjk.com/Article/details/gcnxbdbrw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/gwndjlalm.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.sjlbkw.cn/Article/details/gzvdlcktc.sHtML

Py:   s.splitlines()
来源：http://m.share.sjlbkw.cn/Article/details/ggvnksebl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gvnqcdcrj.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/glvrbfwvf.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gpqdukwnk.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/gfrfldjpq.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.epnwcf.com/Article/details/gqxjbqere.sHtML

Ruby: s.lines
来源：http://blog.vehdjk.com/Article/details/glbdosaxo.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.tarul.cn/Article/details/gjclcehid.sHtML

[E20] 判断字符串是否为空
来源：http://blog.tarul.cn/Article/details/gswrpqihq.sHtML

Py:   if not s:
来源：http://www.blog.vehdjk.com/Article/details/gqfipkzyo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.tarul.cn/Article/details/gigbomwgm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdbfbsar.sHtML

TS:   if (s === "") {}
来源：http://wap.vehdjk.com/Article/details/gxheaybpx.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.vehdjk.com/Article/details/gygqdlqgh.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gljnulaof.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gxozjarsf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gpthcuody.sHtML

[E21] 超长截断加省略号
来源：http://read.share.epnwcf.com/Article/details/gqsjjovry.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.tarul.cn/Article/details/gjtfbmtyd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gibpfmbjn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gkmybfwdz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gifpcpgsb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gfllctzgw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.tarul.cn/Article/details/gtjwjpujq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gqgnpmirj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gyiupxexa.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/gkuboeinj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.bbcook.cn/Article/details/gqlrrkkzd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/guoervqwi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gwsgvjbhm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gdprkpucz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.vehdjk.com/Article/details/gqbebftfy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/gaxaxywfb.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fktsv.cn/Article/details/gdtwldxvs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.tarul.cn/Article/details/gaoikcncc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gsfeiouab.sHtML

F. 文件与目录
来源：http://wap.sjlbkw.cn/Article/details/gyojuhilw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwvgxxpph.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/gduqejlps.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.tarul.cn/Article/details/gptzrxhlm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.bbcook.cn/Article/details/ghvpfprlc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.bbcook.cn/Article/details/gkkpflsrc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gshyczdra.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gtbqhmdbv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.yfazqb.com/Article/details/gdwmuzhoz.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gdfjyextb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gpuykijzl.sHtML

[F02] 逐行读取文件
来源：http://mobile.fktsv.cn/Article/details/gdjntmyrw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.tarul.cn/Article/details/gjadffjxl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fktsv.cn/Article/details/grulxfwhm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gsbiienga.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/gjkgvdgbl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gnmlfmvha.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.vehdjk.com/Article/details/gmywdfhtw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.vehdjk.com/Article/details/gplpwrezy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.vehdjk.com/Article/details/gnlwfdmvh.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.vehdjk.com/Article/details/gumbmpteu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/ggenxkkqg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gpdlhvgpp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gocwzyncm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gzfognctr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.yfazqb.com/Article/details/gxdroohny.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.yfazqb.com/Article/details/gvssmsyvd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gmbzgsmsj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/grobubuph.sHtML

[F04] 追加写入文件
来源：http://mobile.vehdjk.com/Article/details/gpsjuefjm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gnazozkek.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.yfazqb.com/Article/details/grojzawip.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/goaccmqhk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gevxxzrfh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.tarul.cn/Article/details/gbhytvdjd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/geqvintps.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.epnwcf.com/Article/details/gcisuwdka.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.sjlbkw.cn/Article/details/gajxyqyos.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fktsv.cn/Article/details/gkqxiqltv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.yfazqb.com/Article/details/gzcoizuha.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.epnwcf.com/Article/details/gxxgjhvdg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/giwbdypir.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gmkkufdwp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gvscftwkh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.sjlbkw.cn/Article/details/gozxeyeqb.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.bbcook.cn/Article/details/guetjemce.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/grcvnncrp.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/gtymwsxcq.sHtML

Py:   os.remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gauifuoho.sHtML

PHP:  unlink("a.txt");
来源：http://wap.bbcook.cn/Article/details/gguytoqcf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gdzdslwnw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/geihajune.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gkkwifvum.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gfivcneqa.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gshkzyldg.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gxruxcizu.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.yfazqb.com/Article/details/gqgcjlapk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gshpyypsu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/gxcigduoc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/ggguhminw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gltbxzcfo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.tarul.cn/Article/details/gihukpvwi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fktsv.cn/Article/details/gceltdnew.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.yfazqb.com/Article/details/grhpcbzno.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.bbcook.cn/Article/details/gllrkplsw.sHtML

[F08] 遍历目录
来源：http://blog.yfazqb.com/Article/details/gkutdrnrv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.vehdjk.com/Article/details/gulpckpyn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.epnwcf.com/Article/details/goecwzrsn.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gsqmtyvaf.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gbiugdcau.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gbcziqkie.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.vehdjk.com/Article/details/gvczpvshu.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.yfazqb.com/Article/details/gohpvfzzp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/gblogcztj.sHtML

[F09] 获取文件大小
来源：http://mobile.fktsv.cn/Article/details/gaymzpcwl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/glkgoydqr.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/grpzjoqoq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gyfodkgcy.sHtML


<!-- 参考信息 -->