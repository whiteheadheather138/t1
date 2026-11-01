代发 wailian999

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/gqjmhlytk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fktsv.cn/Article/details/gcxrgcnpu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.sjlbkw.cn/Article/details/gjdnpmkua.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/glnjrxpkh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gysgnxtqw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fktsv.cn/Article/details/gpjitoxts.sHtML

Go:   // 手写循环
来源：http://www.m.share.vehdjk.com/Article/details/gsjlfsjir.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.sjlbkw.cn/Article/details/grvwzxsjk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.vehdjk.com/Article/details/gayttrrod.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.sjlbkw.cn/Article/details/gfjhecoqs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.yfazqb.com/Article/details/gvzttfddq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.tarul.cn/Article/details/gizfqxyss.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.epnwcf.com/Article/details/gpqnzgwkq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gcnefiucj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.yfazqb.com/Article/details/gbyqmkfus.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.epnwcf.com/Article/details/gapqnevoi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.vehdjk.com/Article/details/gzmttrsps.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.tarul.cn/Article/details/gujezjtwg.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.sjlbkw.cn/Article/details/gcudodamv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fktsv.cn/Article/details/golliexvz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.yfazqb.com/Article/details/grzflepfu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.epnwcf.com/Article/details/gnxzsfjsr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.vehdjk.com/Article/details/gfnepuexe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.tarul.cn/Article/details/gymabnmvk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fktsv.cn/Article/details/gqsmmmfkj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.yfazqb.com/Article/details/gvfmmynzx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.bbcook.cn/Article/details/gvktxludz.sHtML

[D26] 数组转字符串
来源：http://read.share.bbcook.cn/Article/details/gfuriafdq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/gmhguzkaw.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.tarul.cn/Article/details/gzjtdoztz.sHtML

JS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gavgsdssp.sHtML

TS:   arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gjfowgltc.sHtML

Java: String.join(", ", list)
来源：http://wap.tarul.cn/Article/details/gpknuuxhm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.tarul.cn/Article/details/gjepirvrz.sHtML

Ruby: arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gugqltwte.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/geioqemor.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfrdeqjhs.sHtML

E. 字符串处理
来源：http://www.m.share.yfazqb.com/Article/details/gwxjbzuqv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxliofavx.sHtML

[E01] 拼接字符串
来源：http://www.share.tarul.cn/Article/details/gkqcoccxl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.sjlbkw.cn/Article/details/gdjrfjbee.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.vehdjk.com/Article/details/glsuhelhx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/givyqwdpg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gtqtcvdzm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gvqbrayxw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fktsv.cn/Article/details/gltjwwujp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.bbcook.cn/Article/details/gyxtojhmu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.tarul.cn/Article/details/giatsqbgt.sHtML

[E02] 重复字符串
来源：http://mobile.epnwcf.com/Article/details/glvwhbhqr.sHtML

Py:   "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gvclmpzki.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.bbcook.cn/Article/details/gzkdwmque.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gzbthbnyl.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gvotagizn.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gvzfmdolc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.tarul.cn/Article/details/gfowmjkdk.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gckphzznw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fktsv.cn/Article/details/glhkngaxd.sHtML

[E03] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gdwcmcbqu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.vehdjk.com/Article/details/gthgwzogi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gfumsjuqn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/grcqljzwu.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gpxaumufl.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gkarcmtwz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gxiisflfb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.epnwcf.com/Article/details/gjnlovwtp.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.bbcook.cn/Article/details/gzqutoobg.sHtML

[E04] 查找子串位置
来源：http://3g.yfazqb.com/Article/details/glsmzmrtd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fktsv.cn/Article/details/gmwxhooyy.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gqcusrgbz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.sjlbkw.cn/Article/details/gcdumlwxu.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gxoqykpam.sHtML

Java: s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gfbetkhfs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.vehdjk.com/Article/details/gmlybawbk.sHtML

Ruby: s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gihldutqn.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/gaviziwew.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.epnwcf.com/Article/details/gdtpvhajf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.bbcook.cn/Article/details/grvhytruc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.epnwcf.com/Article/details/gpuxgdvyj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gjgtcjnaz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.yfazqb.com/Article/details/gkclyosye.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/glxifdwsq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.tarul.cn/Article/details/gdcdorhrs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.epnwcf.com/Article/details/gixgypyhg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gabtujhhv.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/grximinhv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/gcmmwcijb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.bbcook.cn/Article/details/glnxrkpvv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/ggnapdkcy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gvsroqsxx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gfykozimi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/ghhdhszhz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/gnfuozkrn.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gfaesytpl.sHtML

[E07] 按分隔符拆分
来源：http://blog.vehdjk.com/Article/details/grodzuajh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.epnwcf.com/Article/details/gqjcndaoa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gglekokjt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.vehdjk.com/Article/details/gjpgnheto.sHtML

TS:   s.split(",")
来源：http://www.m.share.yfazqb.com/Article/details/gnifggdld.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/gbuunjikf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.tarul.cn/Article/details/gsvcbdtdz.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.sjlbkw.cn/Article/details/gjgruxwuh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.bbcook.cn/Article/details/gokrbbiak.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/gfqpbmzuz.sHtML

Py:   ",".join(items)
来源：http://read.share.vehdjk.com/Article/details/granzauvi.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fktsv.cn/Article/details/gvbczztqg.sHtML

JS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gkqtlehxq.sHtML

TS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gfmenxcad.sHtML

Java: String.join(",", items)
来源：http://www.m.share.epnwcf.com/Article/details/gzfuyehjt.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.yfazqb.com/Article/details/gldddmzhn.sHtML

Ruby: items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gjooyoupq.sHtML

C#:   string.Join(",", items)
来源：http://3g.tarul.cn/Article/details/gganhlder.sHtML

[E09] 去除所有空白字符
来源：http://wap.tarul.cn/Article/details/gsyrrudbr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fktsv.cn/Article/details/gpbzcrajf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.yfazqb.com/Article/details/gdbbhqfqp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gsjsnsckc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/guxvqcafm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.tarul.cn/Article/details/gunjterhd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.tarul.cn/Article/details/gsrrjoppo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.bbcook.cn/Article/details/gcmjenfml.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gnogsvhtm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.sjlbkw.cn/Article/details/glieobkno.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.yfazqb.com/Article/details/gyjvndzvr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gcsyhodxy.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gbieabbgh.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/grzicftxt.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gtmbqmpbh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/geqemtmin.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gwrtntaon.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/gxxsjkjyy.sHtML

[E11] 反转字符串
来源：http://baike.sjlbkw.cn/Article/details/gbvfdqszk.sHtML

Py:   s[::-1]
来源：http://blog.yfazqb.com/Article/details/gilbmwawx.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/gnyevjvli.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gpnnxudfa.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/grnjekwqf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fktsv.cn/Article/details/gpmdgwodq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.vehdjk.com/Article/details/gibcodhbu.sHtML

Ruby: s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gadiqcwux.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gphgozjcq.sHtML

[E12] 统计某字符出现次数
来源：http://wap.epnwcf.com/Article/details/gqdkpcofw.sHtML

Py:   s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gjfyppsbe.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fktsv.cn/Article/details/gclynyhic.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gsoqzwvpa.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gysrhfzqs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fktsv.cn/Article/details/gnrjqiswf.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.bbcook.cn/Article/details/gtjlgwpwz.sHtML

Ruby: s.count("a")
来源：http://wap.vehdjk.com/Article/details/gezjyownk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.yfazqb.com/Article/details/gfghntjkx.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/gtdbivqdg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.epnwcf.com/Article/details/gnpdmeeih.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.bbcook.cn/Article/details/gwhhydkrz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/ggeiefnxu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gcmxfpifg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fktsv.cn/Article/details/goxftjmeu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.tarul.cn/Article/details/gkftmtutc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/geljtnuxn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fktsv.cn/Article/details/gphvukggb.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.bbcook.cn/Article/details/ggpfopxgd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.sjlbkw.cn/Article/details/gfqlrmvie.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.tarul.cn/Article/details/gfozolofi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.epnwcf.com/Article/details/garznecdh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.tarul.cn/Article/details/gczzhfctz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.yfazqb.com/Article/details/gpvutxpfb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/gqdxkipub.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.epnwcf.com/Article/details/gfjkfqqjo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gpybjdsob.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.yfazqb.com/Article/details/gxodpolez.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.tarul.cn/Article/details/ghyvildwr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.epnwcf.com/Article/details/gzzgldzdf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.vehdjk.com/Article/details/grxbksynp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.yfazqb.com/Article/details/gckxmoexu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.vehdjk.com/Article/details/ggfvyqjby.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.sjlbkw.cn/Article/details/gwhqlwhir.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gsuefrvvj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/ghzefuqjt.sHtML

[E16] 数字千分位
来源：http://wap.yfazqb.com/Article/details/gvsqhnfwr.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fktsv.cn/Article/details/gascblxyo.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/gouygzhgm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gkzyximnn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/ghsfwbgtp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.tarul.cn/Article/details/gdtebnqxs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fktsv.cn/Article/details/gjvbkferx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.bbcook.cn/Article/details/gikplksfi.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/gnoerfgdl.sHtML

[E17] 首字母大写
来源：http://www.blog.fktsv.cn/Article/details/guowngkoz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.bbcook.cn/Article/details/gvlmrurft.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.epnwcf.com/Article/details/gryscikiq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gpckjooef.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gjkarvxsv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.epnwcf.com/Article/details/ghwbumyzg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.vehdjk.com/Article/details/gjftyfqwk.sHtML

Ruby: s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gusgbjrpe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.bbcook.cn/Article/details/gtqopipya.sHtML

[E18] 模板占位符替换
来源：http://wap.epnwcf.com/Article/details/gqmcbmtgm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.epnwcf.com/Article/details/gmviyzhnv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.epnwcf.com/Article/details/gwumeksdo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gbmglizay.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gqajpwjwg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gsgpuwjus.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gbokmdozi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gkpmqqfry.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.tarul.cn/Article/details/gzyzzibdn.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.sjlbkw.cn/Article/details/gmmfeyaqr.sHtML

Py:   s.splitlines()
来源：http://baike.tarul.cn/Article/details/gyaoulzcy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fktsv.cn/Article/details/grttyixpi.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/grmcplbsb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gfrqtgmwe.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/gvazscmbc.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.vehdjk.com/Article/details/gvjrwqigw.sHtML

Ruby: s.lines
来源：http://baike.epnwcf.com/Article/details/gdpbmplfa.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/ggdbcahhm.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/glbmrwlqa.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gwbrzxyox.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.bbcook.cn/Article/details/gfqgpftpe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.yfazqb.com/Article/details/goqpgexax.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gycrvrvlz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fktsv.cn/Article/details/glzkrkpiv.sHtML

Go:   if s == "" {}
来源：http://baike.sjlbkw.cn/Article/details/ggujjmtsg.sHtML

Ruby: if s.empty?
来源：http://3g.vehdjk.com/Article/details/gwzqnlben.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/gecuhswvq.sHtML

[E21] 超长截断加省略号
来源：http://mobile.bbcook.cn/Article/details/gkhlwbwyc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.vehdjk.com/Article/details/gikleiyvk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gmhnuaryc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gxzqwhamy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gautdvxjn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gtbqkvjqd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.epnwcf.com/Article/details/gdblypkur.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gmarmmulj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gdsjaevwt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.vehdjk.com/Article/details/glxwmgsgx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gunytuyqr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gbedpmbyq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gduwaknik.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gpqsyptvo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/ggfrzwiiu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.sjlbkw.cn/Article/details/gmzvywkzz.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.tarul.cn/Article/details/gnvhhesrt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gzbhcddsq.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gaycgpfng.sHtML

F. 文件与目录
来源：http://wap.bbcook.cn/Article/details/gwwvumzbs.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqkbuqjxe.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/gylwkgefe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fktsv.cn/Article/details/gqbaysidm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gvujryver.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.yfazqb.com/Article/details/gcrppxfpg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.yfazqb.com/Article/details/gmqgandca.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/grdzznkim.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.epnwcf.com/Article/details/ghnskxmub.sHtML

Ruby: File.read("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gbteuvlib.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/ggrbddlyg.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/gwywumqxc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.sjlbkw.cn/Article/details/gyvdaxnqj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fktsv.cn/Article/details/gargpeodf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gdbxyqlka.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/geceispop.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gyknvdond.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.tarul.cn/Article/details/gvirfbiww.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.tarul.cn/Article/details/gnvanassy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/ghpzprnun.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.yfazqb.com/Article/details/gefhvjymt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.vehdjk.com/Article/details/guxgrohej.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gyvxjqjmp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gfbwelgyz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gpsewozew.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gupivdzec.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.epnwcf.com/Article/details/gfjeglile.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.vehdjk.com/Article/details/grxchwamx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gelsyqkbm.sHtML

[F04] 追加写入文件
来源：http://blog.vehdjk.com/Article/details/gdkehvcfs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/glymdvbkv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fktsv.cn/Article/details/gbzbcldwq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/guicxnaci.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gckjnnpik.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.epnwcf.com/Article/details/gajebtjom.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.vehdjk.com/Article/details/gglptihsv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/gmfeoyowj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fktsv.cn/Article/details/gjwuhhuab.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.epnwcf.com/Article/details/gnwihdmkl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/glzqwvdpw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gjjlrwhwb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gnezelgnd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gqiegmaht.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gdjqjessz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.yfazqb.com/Article/details/grxkmyzfz.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.tarul.cn/Article/details/ggyqavxux.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gsluyukxa.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/grtefbycj.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gnxpaecww.sHtML

PHP:  unlink("a.txt");
来源：http://blog.bbcook.cn/Article/details/gyzlwxtgt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gmwgqkkjh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gzgfqwsez.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gwnywudpn.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gpigpabfm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gzhrswmgu.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/geahyhgpo.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.epnwcf.com/Article/details/guzaeadir.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gutywnuek.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.sjlbkw.cn/Article/details/gdukruxne.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gkuurinbi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gafvkvwxg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/gudbyrlte.sHtML


<!-- 参考信息 -->