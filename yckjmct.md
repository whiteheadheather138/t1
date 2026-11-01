代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/gxshdiaxz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.tarul.cn/Article/details/gcpffupdo.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.yfazqb.com/Article/details/gpqfzzfwv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.vehdjk.com/Article/details/gcnsituft.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fktsv.cn/Article/details/gngwkoolt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.tarul.cn/Article/details/glcpzptdz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.epnwcf.com/Article/details/gtjllfynm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.bbcook.cn/Article/details/gqyipxnon.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.tarul.cn/Article/details/goequmbti.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.vehdjk.com/Article/details/gupassmvg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/glitfyoat.sHtML

[D26] 数组转字符串
来源：http://3g.vehdjk.com/Article/details/ghwdrckug.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fktsv.cn/Article/details/gkbzzyocc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gidlqwcqx.sHtML

JS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/guvhhoihr.sHtML

TS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gztplzdhx.sHtML

Java: String.join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gjjyftxev.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.tarul.cn/Article/details/gicrjcuux.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/geccnhxvk.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/gusiqrglk.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gciuyrzpk.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/gzylvvtlp.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gcgvtqwxy.sHtML

[E01] 拼接字符串
来源：http://blog.bbcook.cn/Article/details/gejkgoaua.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.vehdjk.com/Article/details/gaktcuxtx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.yfazqb.com/Article/details/glmvlcfoy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gydeihyri.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gvesbovrz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.sjlbkw.cn/Article/details/gzunbvpdi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.sjlbkw.cn/Article/details/ggsfzxgmr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.vehdjk.com/Article/details/gfkxbumyg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gnkebckom.sHtML

[E02] 重复字符串
来源：http://baike.fktsv.cn/Article/details/gylwjhutc.sHtML

Py:   "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gfxcogrmn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.epnwcf.com/Article/details/glrbmrulq.sHtML

JS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gpgkaueex.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gafxwmsdo.sHtML

Java: "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/ghdahtmnl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.sjlbkw.cn/Article/details/gmtfwlwyc.sHtML

Ruby: "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gcmwfpkzk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.vehdjk.com/Article/details/ggdsvkfad.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/ghonuoaqz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.sjlbkw.cn/Article/details/ghjkyujgf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gyjxldixc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gaftcdvfa.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gisdajpvl.sHtML

Java: s.substring(1, 4)
来源：http://wap.epnwcf.com/Article/details/gauuoykyr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.vehdjk.com/Article/details/gxhbbzuqm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fktsv.cn/Article/details/gjcslsxuc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fktsv.cn/Article/details/gdwqwfcvk.sHtML

[E04] 查找子串位置
来源：http://www.blog.vehdjk.com/Article/details/gsgewohli.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fktsv.cn/Article/details/ggmpdzskl.sHtML

PHP:  strpos($s, "x");
来源：http://blog.sjlbkw.cn/Article/details/ghtqrxhrz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.sjlbkw.cn/Article/details/gfvlhntsl.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gugrehjgn.sHtML

Java: s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gnczmptpz.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.yfazqb.com/Article/details/gxhhiblxu.sHtML

Ruby: s.index("x")
来源：http://mobile.bbcook.cn/Article/details/gbthkzbdq.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gqsdjeybi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fktsv.cn/Article/details/gbhtnkcwb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.tarul.cn/Article/details/gagwebqlx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.sjlbkw.cn/Article/details/gisqzydin.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/grmbtzwax.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fktsv.cn/Article/details/gqtaprbly.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gntpefbpi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/gpgzlhvfn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.bbcook.cn/Article/details/glownnzik.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/ghlvwowfu.sHtML

[E06] 替换子串
来源：http://www.blog.epnwcf.com/Article/details/gohuvazsd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gsclpukht.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.vehdjk.com/Article/details/gvohoiadh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gpcjtbkxy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/grqohhhny.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gkceceuqg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gknqjilxo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fktsv.cn/Article/details/gqgxiwgro.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fktsv.cn/Article/details/geabwogsx.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/gievqydtg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.epnwcf.com/Article/details/gasnuxxgs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.yfazqb.com/Article/details/gzksawujd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fktsv.cn/Article/details/gfkbwlhpv.sHtML

TS:   s.split(",")
来源：http://mobile.yfazqb.com/Article/details/guiwqqlfg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.bbcook.cn/Article/details/gygqfoudu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.vehdjk.com/Article/details/goaewsybm.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.epnwcf.com/Article/details/gduspkyzc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.yfazqb.com/Article/details/ghdkapenj.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fktsv.cn/Article/details/gwikuqroy.sHtML

Py:   ",".join(items)
来源：http://baike.tarul.cn/Article/details/gdghsqwvn.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fktsv.cn/Article/details/gfstsowzr.sHtML

JS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gyexkiewh.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/garsidzqh.sHtML

Java: String.join(",", items)
来源：http://m.share.bbcook.cn/Article/details/gokniznlu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.yfazqb.com/Article/details/gthkyypog.sHtML

Ruby: items.join(",")
来源：http://wap.bbcook.cn/Article/details/gosqwzbch.sHtML

C#:   string.Join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gjgelzovv.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/gjbdypidp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.bbcook.cn/Article/details/ggfncernl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.epnwcf.com/Article/details/gmypsaqjq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/grnsilzsw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gnwqwokhj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.tarul.cn/Article/details/gimfidyhf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.epnwcf.com/Article/details/geqzsvhkr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.vehdjk.com/Article/details/godqdxnjg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gesxiurzr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.tarul.cn/Article/details/gazikpmkf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/geihlijym.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.bbcook.cn/Article/details/gngvmrlhu.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/gxyfmcbof.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/ghehxqvzz.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/guvlnkrgm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gduwolqcm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/geltyqxst.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.bbcook.cn/Article/details/guuninsha.sHtML

[E11] 反转字符串
来源：http://baike.tarul.cn/Article/details/geikujrqy.sHtML

Py:   s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/geoiifpns.sHtML

PHP:  strrev($s);
来源：http://mobile.vehdjk.com/Article/details/ggycboxfb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gkpsleckr.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gqrpoerwf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gbajiefdd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/gmtsrbpao.sHtML

Ruby: s.reverse
来源：http://blog.tarul.cn/Article/details/gurqoufzn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gnafkdtgh.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.epnwcf.com/Article/details/geaalzxyr.sHtML

Py:   s.count("a")
来源：http://www.share.vehdjk.com/Article/details/ggcgasiac.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gkvkrtzgy.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/glaotpudd.sHtML

TS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/grayxkpki.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/grlopqeal.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.yfazqb.com/Article/details/gvzxdteoo.sHtML

Ruby: s.count("a")
来源：http://m.share.tarul.cn/Article/details/ghlqmzuan.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.epnwcf.com/Article/details/gcfqxyayk.sHtML

[E13] 逐字符遍历
来源：http://mobile.epnwcf.com/Article/details/gqknaxmbd.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.bbcook.cn/Article/details/gihljonpd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.bbcook.cn/Article/details/gqjbvqbwj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/guyzgdusa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gfbztefgk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.epnwcf.com/Article/details/gcbolwiae.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fktsv.cn/Article/details/gcspxfgta.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fktsv.cn/Article/details/ggkyzpcpm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gxyvwbfet.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.vehdjk.com/Article/details/gtjioqeie.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.vehdjk.com/Article/details/glrtfqfjo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gptzqpkpw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.sjlbkw.cn/Article/details/gfbubxfmj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.vehdjk.com/Article/details/gykqocsxb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gxxnjojiw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.bbcook.cn/Article/details/gavrwstiu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.tarul.cn/Article/details/gavfyejvy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.vehdjk.com/Article/details/gxchlzjai.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.sjlbkw.cn/Article/details/gyesxtnip.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.yfazqb.com/Article/details/gfypraswq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.yfazqb.com/Article/details/ggclwgodm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.epnwcf.com/Article/details/gxxlvlxfg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.yfazqb.com/Article/details/glqemljra.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.epnwcf.com/Article/details/govwdvnsj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.bbcook.cn/Article/details/gsjxaduiv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fktsv.cn/Article/details/gmnbowvui.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/gqxoxcyvo.sHtML

[E16] 数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gkkzptxnq.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gvtsscblp.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/gevgkeiwc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gxijjbsef.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/gawsyator.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.epnwcf.com/Article/details/gqedpsykh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.yfazqb.com/Article/details/gxlkkjqjr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.tarul.cn/Article/details/gfxvhoafb.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.yfazqb.com/Article/details/gpdzvddtq.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/gfpvuhzwr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.epnwcf.com/Article/details/goinpothz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/gkrstnjxl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gmezfxfya.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/grardrzqv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.vehdjk.com/Article/details/ginmsarfd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.bbcook.cn/Article/details/gdwguoall.sHtML

Ruby: s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/gcijktmll.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.sjlbkw.cn/Article/details/gdggypqyy.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/gaevffeyw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.yfazqb.com/Article/details/ganlzrevk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.yfazqb.com/Article/details/gmjnevkhl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gjcewcgxc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gyzoabyts.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gaxukjaor.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.tarul.cn/Article/details/gibkfbvxs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.sjlbkw.cn/Article/details/gkpxnffbb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/gozlkbydr.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.tarul.cn/Article/details/gylfkbcmx.sHtML

Py:   s.splitlines()
来源：http://www.m.share.tarul.cn/Article/details/gyjejrlrq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gylfhrngb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/geibyogrz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gfdtbtbdg.sHtML

Java: s.lines().toList()
来源：http://m.share.yfazqb.com/Article/details/gewetnsks.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.epnwcf.com/Article/details/gwdsumacn.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/gidpxxbvq.sHtML

C#:   s.Split('\n')
来源：http://baike.yfazqb.com/Article/details/gnrdkxqad.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.bbcook.cn/Article/details/gblamvtej.sHtML

Py:   if not s:
来源：http://www.m.share.fktsv.cn/Article/details/grjoxrtqt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.tarul.cn/Article/details/gksizjavv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/gvpjahqle.sHtML

TS:   if (s === "") {}
来源：http://mobile.bbcook.cn/Article/details/gpchgxdtc.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gcrxwflai.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gjhjxiodw.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gonbierkz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.epnwcf.com/Article/details/gwicwettf.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.tarul.cn/Article/details/gyyhimjvn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.yfazqb.com/Article/details/gzpcieekb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gmmsvwskq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gsnsdvxsk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gzctqmufn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/ghwdkoskh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.vehdjk.com/Article/details/gfvdnbvjd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gjhuyvdhd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/gpdaigxjn.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.bbcook.cn/Article/details/gtqtnzqjh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.tarul.cn/Article/details/gwqfhkakd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gbjuwkhbk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.bbcook.cn/Article/details/gmngupace.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gxndfqpee.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.yfazqb.com/Article/details/golgdolwp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fktsv.cn/Article/details/gaytqmvcs.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.vehdjk.com/Article/details/gfwkmxmjw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.tarul.cn/Article/details/gqboykylu.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghszpvflt.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/gfncvywme.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggwcdwkqc.sHtML

[F01] 读取整个文件
来源：http://3g.epnwcf.com/Article/details/gswenuzow.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fktsv.cn/Article/details/gntlrbtgm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.tarul.cn/Article/details/gskjtagog.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.epnwcf.com/Article/details/gbhjbymti.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.vehdjk.com/Article/details/gtnnwztig.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gxrystwvv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/gkdygggoa.sHtML

Ruby: File.read("a.txt")
来源：http://baike.bbcook.cn/Article/details/gfdabqakq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.tarul.cn/Article/details/gzmvehyzs.sHtML

[F02] 逐行读取文件
来源：http://wap.tarul.cn/Article/details/gdkjfyhia.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.epnwcf.com/Article/details/greuypdro.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/geinylrlv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gceqtbydr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/grwnzxmxu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gkpboteht.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.yfazqb.com/Article/details/gvxjhkryi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.sjlbkw.cn/Article/details/gxsnlsjcp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fktsv.cn/Article/details/gvkdednls.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.yfazqb.com/Article/details/gytwdaite.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/gcqpfkbew.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.tarul.cn/Article/details/gjtrjtsnh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gbkjorxpg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gtpqefava.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.epnwcf.com/Article/details/gkdzcnody.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.sjlbkw.cn/Article/details/gkiaeacal.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.sjlbkw.cn/Article/details/gknkcyevt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gjzrtreby.sHtML

[F04] 追加写入文件
来源：http://mobile.bbcook.cn/Article/details/gzguaupuz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gfnvqtlot.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.vehdjk.com/Article/details/gnyrdnerq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gcsejtglv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gmgzlcwsi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gwdjznuwm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gxidotkyt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.epnwcf.com/Article/details/grcbejjhs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.epnwcf.com/Article/details/ghfuiexea.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/goeyhzuqo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/gaporumpg.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.yfazqb.com/Article/details/gmexqghme.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gpdfsvogv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gnmrgwkhl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gfjfuafom.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.bbcook.cn/Article/details/gmohpalzg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gfafeuhvw.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fktsv.cn/Article/details/gvkoobdkh.sHtML

[F06] 删除文件
来源：http://blog.tarul.cn/Article/details/gsiecxwid.sHtML

Py:   os.remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gdejqxveb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gdqvrcjbn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gtedhkziu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gjtwmgljq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gdntmfrnm.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gqavywnyb.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ghxbfoglc.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gyysqawrc.sHtML

[F07] 创建目录（含多级）
来源：http://baike.yfazqb.com/Article/details/gkcjhdajd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gkzjdxezp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fktsv.cn/Article/details/gsigwvach.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gjmccsnqe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gnbxfvqom.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/gmpqszrpg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.yfazqb.com/Article/details/gxjlrqhhu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fktsv.cn/Article/details/gtghlljfz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/ggaisohlx.sHtML

[F08] 遍历目录
来源：http://baike.epnwcf.com/Article/details/gipgrkpws.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.vehdjk.com/Article/details/gvjeqnbev.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.yfazqb.com/Article/details/gcgvycigb.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gfmswzyef.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gjletwjzc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gckqxraai.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.vehdjk.com/Article/details/gifxupojs.sHtML

Ruby: Dir.children("dir")
来源：http://baike.vehdjk.com/Article/details/gobdfsxhh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fktsv.cn/Article/details/gkrwzxnlh.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/gltihgmgg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gtpzjxupm.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.yfazqb.com/Article/details/ggurfwali.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/gmypjekin.sHtML


<!-- 参考信息 -->