代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.vehdjk.com/Article/details/gzkybbrxf.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.sjlbkw.cn/Article/details/gbbmmtnjq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.tarul.cn/Article/details/gwinstsug.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.epnwcf.com/Article/details/gomcqvpuu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.sjlbkw.cn/Article/details/gitoggssu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gllgabbcw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.yfazqb.com/Article/details/gtkurnkfk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.epnwcf.com/Article/details/gdccqfkgd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.vehdjk.com/Article/details/gkzwitmvg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.epnwcf.com/Article/details/gbuxwsiwg.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/gkijjynfr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gqdonlfnn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.yfazqb.com/Article/details/gmfidhxhk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.tarul.cn/Article/details/gmgoghrfv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.tarul.cn/Article/details/gmjqdzeiy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gvmgnsbgq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/gvdqcasav.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.vehdjk.com/Article/details/gxaocoyhc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.bbcook.cn/Article/details/gnewpigez.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/genpziskj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.sjlbkw.cn/Article/details/gzttjolbe.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gzxvasvmn.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gvuhdbrix.sHtML

TS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gtgjbghqw.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gpqyajgvn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.epnwcf.com/Article/details/gjsfbndrg.sHtML

Ruby: arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gnosfylvt.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/gdpcjongw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gnfqnackj.sHtML

E. 字符串处理
来源：http://www.blog.tarul.cn/Article/details/gcyjmqkpr.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghaauvnok.sHtML

[E01] 拼接字符串
来源：http://m.share.yfazqb.com/Article/details/ghdqssyky.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fktsv.cn/Article/details/gemavjmth.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.bbcook.cn/Article/details/gxuenrkbb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/gkvkgakzi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/gvvkopcus.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/ggpiifjhl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.yfazqb.com/Article/details/gacfzwjuc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.yfazqb.com/Article/details/ghxgrbaqp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.tarul.cn/Article/details/gqychutqb.sHtML

[E02] 重复字符串
来源：http://3g.tarul.cn/Article/details/gwtnckkan.sHtML

Py:   "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gfzfagvwi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fktsv.cn/Article/details/gugqmqbjc.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gmspdbhuw.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gcirrbmwv.sHtML

Java: "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gjsreakgc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.bbcook.cn/Article/details/gzaalashj.sHtML

Ruby: "ab" * 3
来源：http://blog.tarul.cn/Article/details/geppjjeet.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.bbcook.cn/Article/details/ggbewkpmc.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gkhexzpje.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/gadvhmssd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gbburfrgw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gsmtmickp.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gcynozhws.sHtML

Java: s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/ggnpnaqse.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.vehdjk.com/Article/details/gtawfepeh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.yfazqb.com/Article/details/gbnzgghwb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.tarul.cn/Article/details/gobbkqmei.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/guhyrcurx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.bbcook.cn/Article/details/gxkkiahhj.sHtML

PHP:  strpos($s, "x");
来源：http://baike.vehdjk.com/Article/details/gooyuxnxp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.bbcook.cn/Article/details/gyckeowec.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/geuziuxzz.sHtML

Java: s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/glvhbcmbb.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fktsv.cn/Article/details/glsqqiqbi.sHtML

Ruby: s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gjcpmvcje.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/giozkmvkx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fktsv.cn/Article/details/grvnzouts.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gnyyrcdqi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.vehdjk.com/Article/details/gcrxmujrn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gnxgfjtbx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.sjlbkw.cn/Article/details/gtxilaesl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gwtikklhq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.tarul.cn/Article/details/gcolctsmr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fktsv.cn/Article/details/gkhljlxru.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gxirnfcwi.sHtML

[E06] 替换子串
来源：http://www.blog.epnwcf.com/Article/details/gmcfkptzw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gcqtpgjxr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.bbcook.cn/Article/details/gksglicoo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gjtafpbwv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gqnvxyufi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gszelpuoq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gujfqpgyo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gctbgohjg.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.yfazqb.com/Article/details/gnpfpioyt.sHtML

[E07] 按分隔符拆分
来源：http://m.share.yfazqb.com/Article/details/ggxezkohm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.yfazqb.com/Article/details/ggcqvdmkx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gxpntyoyb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fktsv.cn/Article/details/gbpqgjssk.sHtML

TS:   s.split(",")
来源：http://mobile.bbcook.cn/Article/details/gosqujyhm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.tarul.cn/Article/details/ghhjvedry.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/gufztgvjs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.vehdjk.com/Article/details/gikigqbwu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.sjlbkw.cn/Article/details/gaaulqcve.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fktsv.cn/Article/details/gxzwfkvvy.sHtML

Py:   ",".join(items)
来源：http://m.share.tarul.cn/Article/details/gxlkobexc.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fktsv.cn/Article/details/gaufugxnr.sHtML

JS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/ghbhhohsy.sHtML

TS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gpkjaqxmx.sHtML

Java: String.join(",", items)
来源：http://baike.fktsv.cn/Article/details/gdozkzcqj.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/gszzkfiga.sHtML

Ruby: items.join(",")
来源：http://blog.vehdjk.com/Article/details/gwckakczf.sHtML

C#:   string.Join(",", items)
来源：http://blog.sjlbkw.cn/Article/details/gucjgrjzb.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.epnwcf.com/Article/details/gnczuswvw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.vehdjk.com/Article/details/gchurfgyr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/gcopihtya.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gchjywzeo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gdcxaoklc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.yfazqb.com/Article/details/guglnfxsr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.bbcook.cn/Article/details/gfmoevpec.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.tarul.cn/Article/details/gqwnibthw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.epnwcf.com/Article/details/glxtauwxf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fktsv.cn/Article/details/goeowqeji.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.yfazqb.com/Article/details/grptfjacv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/gavjhrlii.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrvbuqcl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gmdyoiidr.sHtML

Java: String.format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gihpbhecl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gjfyiyswj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gnlrdvfoy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.bbcook.cn/Article/details/gdxhamzhx.sHtML

[E11] 反转字符串
来源：http://read.share.vehdjk.com/Article/details/gokussmjr.sHtML

Py:   s[::-1]
来源：http://3g.vehdjk.com/Article/details/gwoqbleti.sHtML

PHP:  strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gcspvuaog.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/grliuxuam.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gyscnsbou.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.tarul.cn/Article/details/gaewodsik.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.tarul.cn/Article/details/gawuvnpdr.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/gdzpcfxpb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/ghtybopjw.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.sjlbkw.cn/Article/details/gwrwfceyd.sHtML

Py:   s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gizkpwkrp.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fktsv.cn/Article/details/ghfmcsoqd.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gdccstdaf.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/gufmvarpx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.vehdjk.com/Article/details/glzqhojab.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.tarul.cn/Article/details/gjdccmusc.sHtML

Ruby: s.count("a")
来源：http://baike.tarul.cn/Article/details/grwlkjwkx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.yfazqb.com/Article/details/giaxjdfsv.sHtML

[E13] 逐字符遍历
来源：http://baike.epnwcf.com/Article/details/gleiemzsi.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.epnwcf.com/Article/details/glytqrorc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/gknujhyme.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gpsicpqvv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/grmploipb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gqhlqnkgb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.yfazqb.com/Article/details/gazvyricb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.sjlbkw.cn/Article/details/gwyywxtcl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.bbcook.cn/Article/details/glktmexvl.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/gmujhugfd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.epnwcf.com/Article/details/gtidkcdnn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/glonmosyu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/gkwejhebd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.tarul.cn/Article/details/gnqspxouv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbtvhfvn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gfazxhbio.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fktsv.cn/Article/details/gydgntvpy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/grajrhrbv.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fktsv.cn/Article/details/guceoupcm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.yfazqb.com/Article/details/gjwnkzdea.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.sjlbkw.cn/Article/details/gxwqhbtcf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fktsv.cn/Article/details/govnwecwg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.yfazqb.com/Article/details/grdpelhbe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gcoschkdw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gfjjqvssc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/gamtigmca.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcnrnvsy.sHtML

[E16] 数字千分位
来源：http://baike.sjlbkw.cn/Article/details/ggvytdtts.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fktsv.cn/Article/details/grbvuqbrr.sHtML

PHP:  number_format(1234567);
来源：http://read.share.vehdjk.com/Article/details/gcbcuznrb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gigvlkaiu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/gxkfsscro.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.vehdjk.com/Article/details/gissbzxnm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.tarul.cn/Article/details/gutjsqwys.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/gswcbmixl.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/gttlmcicm.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gjnxiqgxy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gestvkazo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.epnwcf.com/Article/details/gniamgqgo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/gfbqejtmy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gslnyztfn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/grjuuynck.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fktsv.cn/Article/details/gsdzpgdod.sHtML

Ruby: s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gftvonbwu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.yfazqb.com/Article/details/gnrchiywd.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/gxwqjnjdd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.tarul.cn/Article/details/gocudddux.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.vehdjk.com/Article/details/gvemmydsx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gjpchzkzr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/grfdwfyax.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gytwtvuvd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gukwtoehg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.sjlbkw.cn/Article/details/gyhfqgvyr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.epnwcf.com/Article/details/gheqeqygf.sHtML

[E19] 多行文本按行拆分
来源：http://3g.tarul.cn/Article/details/gaznqtqul.sHtML

Py:   s.splitlines()
来源：http://www.blog.tarul.cn/Article/details/gsewywoao.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.sjlbkw.cn/Article/details/grinbuavs.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.yfazqb.com/Article/details/gryizgwnl.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/gcvoqkcrq.sHtML

Java: s.lines().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gklsoktak.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.yfazqb.com/Article/details/gkpsvnbet.sHtML

Ruby: s.lines
来源：http://read.share.bbcook.cn/Article/details/gscckmcsv.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gvjpoidsg.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.tarul.cn/Article/details/glbklmjex.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/gvwpwspmz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/gzeykkezj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.epnwcf.com/Article/details/gipszmpgb.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/ghtezhvyx.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/gnkfnqunv.sHtML

Go:   if s == "" {}
来源：http://3g.bbcook.cn/Article/details/gwhmgunpz.sHtML

Ruby: if s.empty?
来源：http://baike.yfazqb.com/Article/details/gqocrxdod.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbypipfny.sHtML

[E21] 超长截断加省略号
来源：http://m.share.epnwcf.com/Article/details/gllvqwndk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.bbcook.cn/Article/details/gjguqwdgu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gvdikpyux.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gqcadafph.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gnafrxizr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gttdvqzoc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.tarul.cn/Article/details/gpgreupyo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gihdmutgk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gestibqcu.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/gltdungag.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.bbcook.cn/Article/details/golmfoxvw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gwtznzvrp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gpkbxigsb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/ghypcurbl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.vehdjk.com/Article/details/ghcvvoqrv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.yfazqb.com/Article/details/grwtonsrh.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gvuzkqovn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.vehdjk.com/Article/details/ggpvnfxqq.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggpxixglb.sHtML

F. 文件与目录
来源：http://read.share.fktsv.cn/Article/details/glzdayuvv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkcfvusve.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/gfqkmxatv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gyqvfwkvl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fktsv.cn/Article/details/glhhrzkfn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.tarul.cn/Article/details/gsffzcbab.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.yfazqb.com/Article/details/gsyrguukv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gzahlftll.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.tarul.cn/Article/details/gkiegjrzi.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gadkcaamt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gsgpklnzq.sHtML

[F02] 逐行读取文件
来源：http://blog.epnwcf.com/Article/details/gyqiazbiv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.bbcook.cn/Article/details/gzenjqpxr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.bbcook.cn/Article/details/gnrhmfobn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gkuvyluib.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/grdclktst.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gbkzbwvza.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.vehdjk.com/Article/details/gvjknzxvp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/gvlhdwaow.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/guezuphgr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fktsv.cn/Article/details/gzxheoswz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/glfkzzfig.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gznidexnz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gavvnsexa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/galagfzzn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.tarul.cn/Article/details/gfdrheytf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.sjlbkw.cn/Article/details/ggwiumidp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/gbangcxfx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/ginpavmgw.sHtML

[F04] 追加写入文件
来源：http://m.share.sjlbkw.cn/Article/details/gobrqenar.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.bbcook.cn/Article/details/gtvyutxsf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.vehdjk.com/Article/details/genfmmbsa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gvnpzeawg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/ggwnrwwob.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fktsv.cn/Article/details/gfipamubz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fktsv.cn/Article/details/gafhfjqep.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.epnwcf.com/Article/details/guvoqvcyh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.sjlbkw.cn/Article/details/gblqhtmcl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gevyqcetz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gtvxszfcd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/galcmzqke.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gbagostlk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gigulmwyx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gwvqrcxdv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/gwnkluvrr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gizftbmdf.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbqcskcke.sHtML

[F06] 删除文件
来源：http://blog.fktsv.cn/Article/details/gddlsvueh.sHtML

Py:   os.remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gnlzlnrpn.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gmogrbfjv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxdpwbpay.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gvvjusmhu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/ghomvhdag.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/ggcwgmsuq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ghclbtgdj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/guocfbslz.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.bbcook.cn/Article/details/gdbfopeyg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gpjwslkdl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.sjlbkw.cn/Article/details/gdxhenevs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/giqktixpk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gevloljvs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.epnwcf.com/Article/details/gahzdhidd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.sjlbkw.cn/Article/details/gugpjqgcq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fktsv.cn/Article/details/gfxhajjov.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/gzepwihbh.sHtML

[F08] 遍历目录
来源：http://www.share.bbcook.cn/Article/details/gdroszhxa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fktsv.cn/Article/details/gxkwatcac.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.epnwcf.com/Article/details/gmopapjsj.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gitrirucs.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/ghkhrjlbl.sHtML


<!-- 参考信息 -->