代发 wailian999

[D23] reduce 累积计算
来源：http://mobile.sjlbkw.cn/Article/details/gkycxbpbv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.epnwcf.com/Article/details/grsgmxgdj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.bbcook.cn/Article/details/gfmvohxuk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gstnkcjjr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/gcsiniwtx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/gtrkjtbek.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gyacrihaa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fktsv.cn/Article/details/grmjojuig.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fktsv.cn/Article/details/gnrmtzegy.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.epnwcf.com/Article/details/gyeqbqxdn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.bbcook.cn/Article/details/gzuvambya.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.tarul.cn/Article/details/gjdvdufqk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.tarul.cn/Article/details/gwapxyorm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gproxfzeu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.sjlbkw.cn/Article/details/gvsavkemi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/gktfisgbd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/ggcnvbtoz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fktsv.cn/Article/details/glacttldq.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/gthqlrdkr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyizhnret.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.epnwcf.com/Article/details/gmotuihqq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.yfazqb.com/Article/details/ggacxnvft.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.sjlbkw.cn/Article/details/gruempsxp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.tarul.cn/Article/details/gxeujmjwt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.bbcook.cn/Article/details/gqqexxjeh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/grweugqkf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gpytrixvl.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/giprvdcjz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxtbfxsp.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.vehdjk.com/Article/details/gdksewkwf.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmxykgeh.sHtML

TS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gtnsqqbws.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gfnsdkejg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.vehdjk.com/Article/details/gfwfbdedi.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gsrohpcfu.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gijiophbe.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gupmhoyaw.sHtML

E. 字符串处理
来源：http://mobile.tarul.cn/Article/details/gchmapawz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghlccblie.sHtML

[E01] 拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gstyiseuy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.yfazqb.com/Article/details/gsswvzqjn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.sjlbkw.cn/Article/details/grdpeqiao.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gylzhokta.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gagbokiqw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/gpekjipgd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fktsv.cn/Article/details/gsvyndmxa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fktsv.cn/Article/details/gkncmbyku.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.tarul.cn/Article/details/ggccpzrcc.sHtML

[E02] 重复字符串
来源：http://www.share.fktsv.cn/Article/details/gfrfkuezi.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gakypzuxn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.vehdjk.com/Article/details/gxgeppist.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcouueef.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gknjglszb.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnigeamrm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.yfazqb.com/Article/details/gxjxvqhaq.sHtML

Ruby: "ab" * 3
来源：http://baike.epnwcf.com/Article/details/gtxvagvaw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/gopwkccxh.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gjoofvgwt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.epnwcf.com/Article/details/gyrctzvaf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gjzudypmi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gaealbdhs.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.yfazqb.com/Article/details/guaahmgiy.sHtML

Java: s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/glyqpafdx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.epnwcf.com/Article/details/gmgpoptmp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.tarul.cn/Article/details/gchuyytol.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.vehdjk.com/Article/details/gftsbpcqo.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/gzsswgirt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gvyhpequf.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fktsv.cn/Article/details/glptpornk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.sjlbkw.cn/Article/details/grtfbgkkx.sHtML

TS:   s.indexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gnqnveqqd.sHtML

Java: s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gfzsdxhzq.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fktsv.cn/Article/details/glcxzmjwm.sHtML

Ruby: s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gjlyjkwvx.sHtML

C#:   s.IndexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/golkbifbq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.sjlbkw.cn/Article/details/gduglqraa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gdwjgexpd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/glacvctus.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/grxkghfyb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gyqfbxngm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gsayrmhed.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.tarul.cn/Article/details/ghgogsfxu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fktsv.cn/Article/details/gaigddyed.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gxgacwnaf.sHtML

[E06] 替换子串
来源：http://3g.bbcook.cn/Article/details/gjolckyhs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/gajlhtzhc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/ghpasquaz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gitmwovgk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gnepjbwzb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gemmsoita.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.tarul.cn/Article/details/gkyimvbem.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fktsv.cn/Article/details/grwyzhokz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gqihdpzcf.sHtML

[E07] 按分隔符拆分
来源：http://wap.yfazqb.com/Article/details/ghbzwdxpk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.sjlbkw.cn/Article/details/giwolexoz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gubebgomi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.bbcook.cn/Article/details/gnowagbnd.sHtML

TS:   s.split(",")
来源：http://www.m.share.fktsv.cn/Article/details/gdwcqyfur.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.vehdjk.com/Article/details/ghzrexhlx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.sjlbkw.cn/Article/details/gzdfrdxeg.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.vehdjk.com/Article/details/geralcpmo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fktsv.cn/Article/details/gbxbsviqc.sHtML

[E08] 数组按分隔符合并
来源：http://wap.epnwcf.com/Article/details/gwvmeuioo.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/gfivqjqup.sHtML

PHP:  implode(",", $items);
来源：http://3g.yfazqb.com/Article/details/gzhxkbotj.sHtML

JS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gamqiizks.sHtML

TS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gvpnddszr.sHtML

Java: String.join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/glmtvtfoe.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.epnwcf.com/Article/details/gtlgxkisi.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gznlplmll.sHtML

C#:   string.Join(",", items)
来源：http://3g.epnwcf.com/Article/details/gljihodbs.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.bbcook.cn/Article/details/gtlsptgkl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.sjlbkw.cn/Article/details/guprgefgn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.bbcook.cn/Article/details/gnufgcvzj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gfzmveyog.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gflxrfuck.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.epnwcf.com/Article/details/gjzipqqjh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gfsbkxdvx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fktsv.cn/Article/details/glsfgszbu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.tarul.cn/Article/details/guhwfpohz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.tarul.cn/Article/details/gccvqekrs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gojpvtngp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fktsv.cn/Article/details/gekqrgqve.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gihbwprcf.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/gfjdooamz.sHtML

Java: String.format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gtobrjaed.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gwwkclfiy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gvndredvx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/grhdknovq.sHtML

[E11] 反转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gqcglsheu.sHtML

Py:   s[::-1]
来源：http://3g.epnwcf.com/Article/details/gersivsue.sHtML

PHP:  strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gbdjdqvgp.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/geqdzssmw.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gzitaahfu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.sjlbkw.cn/Article/details/grfcrlrys.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.epnwcf.com/Article/details/gilhcbiwu.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/gbfqbagli.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gxysjknbl.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gqesigzsa.sHtML

Py:   s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gdlgqulhw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.yfazqb.com/Article/details/gnphqxmnl.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/gkfqehepc.sHtML

TS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gsoupfsgq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.vehdjk.com/Article/details/gfpmmfcfz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.vehdjk.com/Article/details/gpzvtnhgm.sHtML

Ruby: s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gzvhizycj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.bbcook.cn/Article/details/gwehbqjhb.sHtML

[E13] 逐字符遍历
来源：http://blog.yfazqb.com/Article/details/gcckfrclr.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.sjlbkw.cn/Article/details/gazrghutz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.bbcook.cn/Article/details/ggrnetykd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gltfefgki.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/guxaisqhx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gduarhicm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.bbcook.cn/Article/details/giyypjmho.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/giksppwfc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.bbcook.cn/Article/details/ggtziptsr.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fktsv.cn/Article/details/gbhhwufsf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.vehdjk.com/Article/details/gvgboffra.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fktsv.cn/Article/details/gfdcmiozb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.bbcook.cn/Article/details/gqnqoyexn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.sjlbkw.cn/Article/details/geozzqyyj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gnkjxemza.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.epnwcf.com/Article/details/giftyuafj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.sjlbkw.cn/Article/details/gonhucqer.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/gbbdloceq.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.tarul.cn/Article/details/gpyocjetv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.epnwcf.com/Article/details/glzuospoh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/ghkydqpae.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gkopaeyws.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.tarul.cn/Article/details/gtiyjciny.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.tarul.cn/Article/details/gvzabhukj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.bbcook.cn/Article/details/gubnvzrhw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/glkrrmfnc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.vehdjk.com/Article/details/ggwloxqic.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/gvhmokomw.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.sjlbkw.cn/Article/details/gymenlduq.sHtML

PHP:  number_format(1234567);
来源：http://blog.fktsv.cn/Article/details/gfyvekfuv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/gzrmvewcb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gszreklwz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gwfortphi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.yfazqb.com/Article/details/gjtgyvvxm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/grnkjpkoh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.bbcook.cn/Article/details/gnjzhoniz.sHtML

[E17] 首字母大写
来源：http://www.m.share.yfazqb.com/Article/details/gffcgvzjp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fktsv.cn/Article/details/gbswzmykl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.yfazqb.com/Article/details/gdougzpho.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/gejgxqrac.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gyihmfita.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.vehdjk.com/Article/details/gxgdymtxm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.vehdjk.com/Article/details/gffqsowsf.sHtML

Ruby: s.capitalize
来源：http://www.blog.yfazqb.com/Article/details/gltpjifuy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.sjlbkw.cn/Article/details/gvscnjlpa.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/gpecgommm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.vehdjk.com/Article/details/gzathbvve.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.tarul.cn/Article/details/gfaawhvhu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gmytlbzdf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gndycnmmf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.bbcook.cn/Article/details/greezhxsr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.tarul.cn/Article/details/gqvencovg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.yfazqb.com/Article/details/gndxdjihl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.tarul.cn/Article/details/gnkpybpkx.sHtML

[E19] 多行文本按行拆分
来源：http://baike.bbcook.cn/Article/details/gqypoydzm.sHtML

Py:   s.splitlines()
来源：http://www.blog.tarul.cn/Article/details/ghgfwlrsa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fktsv.cn/Article/details/goehvmkfl.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gqlmpyzmv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gfkfvrbhn.sHtML

Java: s.lines().toList()
来源：http://wap.sjlbkw.cn/Article/details/gbmexnkok.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.epnwcf.com/Article/details/ghfcwdgna.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/gctumibkd.sHtML

C#:   s.Split('\n')
来源：http://m.share.yfazqb.com/Article/details/gmpeusikk.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gqkulxwpu.sHtML

Py:   if not s:
来源：http://blog.tarul.cn/Article/details/gxkcmcfpr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.tarul.cn/Article/details/gnzqqigne.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.tarul.cn/Article/details/gpojnkqdz.sHtML

TS:   if (s === "") {}
来源：http://3g.epnwcf.com/Article/details/gncdsdhst.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gfanbcebr.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gmbgjkosc.sHtML

Ruby: if s.empty?
来源：http://m.share.sjlbkw.cn/Article/details/gzgezaxql.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.tarul.cn/Article/details/gxcmwwvxg.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.epnwcf.com/Article/details/gctmcmvjs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.epnwcf.com/Article/details/gnfvwvjah.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gjkyctrch.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gyzbpdahl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gnpwscyki.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gpqahwcob.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.bbcook.cn/Article/details/gizutobkq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gguzbnlot.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/ghqqbqxqh.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.epnwcf.com/Article/details/gltropzfn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.yfazqb.com/Article/details/gjyremcpe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gvozttiuf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gaieimmjf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gruwuotvn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.bbcook.cn/Article/details/gijosnczf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.tarul.cn/Article/details/gprsucamz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gsfcxlthx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.epnwcf.com/Article/details/glypxytks.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjekfzhmx.sHtML

F. 文件与目录
来源：http://www.blog.tarul.cn/Article/details/gmuzkhuea.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gjmknrdfh.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/gfpvexqll.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.epnwcf.com/Article/details/gavwsmmnr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gdzkjgqoq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.vehdjk.com/Article/details/gvqwuklcx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.epnwcf.com/Article/details/gpgicowcp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gfqtmvdwz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.bbcook.cn/Article/details/gugzfghtv.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gfcomggqg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/gpdblsuva.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/geebmkvkb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fktsv.cn/Article/details/gjemykvmu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.yfazqb.com/Article/details/guawyvgvz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/ghllvxrbe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/ghtuaacre.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gcgwlaxqb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.tarul.cn/Article/details/ggryeokgc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/gmflbfeyj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gnelromlz.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.epnwcf.com/Article/details/gitigrcbq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fktsv.cn/Article/details/gzszabeld.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gbpuojblg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gigovwyrm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/guyayiiig.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.vehdjk.com/Article/details/gldcumvop.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fktsv.cn/Article/details/gqixzqcmq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.tarul.cn/Article/details/getvjqiim.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/ghpnntkny.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gieojjlhq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.bbcook.cn/Article/details/ghgjogvsq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gmwoqvhtf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gizfcgksl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gchdnjxja.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.sjlbkw.cn/Article/details/gsrngeypa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.vehdjk.com/Article/details/gjzkfpobd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.yfazqb.com/Article/details/gdiylyjmh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/giqemmizx.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.vehdjk.com/Article/details/gnmbmhkaa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.vehdjk.com/Article/details/gnrlomtct.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/ghusewgjl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gylzxgwhq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/glynucyix.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gbioiquiq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.yfazqb.com/Article/details/galldcvld.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gqenhqtbl.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/gkbzbrmza.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwaqyaax.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gbsfsywfj.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gmzajergp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gnpyvqjtr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gkokofowy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gmqaafbgk.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gyjrgkxzt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gohimlxss.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gvqjgddqy.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.epnwcf.com/Article/details/gyuzdhink.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fktsv.cn/Article/details/gfmkrfqfp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.bbcook.cn/Article/details/gfmotlaat.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gztjnhrmj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gmvbqtnks.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/ghqjoqlbu.sHtML


<!-- 参考信息 -->