代发 wailian999

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/ghywahhit.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.vehdjk.com/Article/details/gumiiqucd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/glfokmdal.sHtML

C#:   new List<int>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gvlrkxgbw.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/grdiyescp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.vehdjk.com/Article/details/gcqmccjvs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.epnwcf.com/Article/details/gzneviclt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gkgrffurj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gkvloscpt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.sjlbkw.cn/Article/details/gsstqkkxf.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/goqojcwte.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.vehdjk.com/Article/details/gucgdibsu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.sjlbkw.cn/Article/details/grwsktvmh.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.sjlbkw.cn/Article/details/gczicmupy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.bbcook.cn/Article/details/gfdljlvrp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.vehdjk.com/Article/details/grddsdoth.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.epnwcf.com/Article/details/ggvcnwhee.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.epnwcf.com/Article/details/geajidaww.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.epnwcf.com/Article/details/geeaeemye.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.yfazqb.com/Article/details/geikcfngf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.tarul.cn/Article/details/guleghtrg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.vehdjk.com/Article/details/grybqlewf.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.bbcook.cn/Article/details/grvopcdcn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.yfazqb.com/Article/details/glodizgko.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.sjlbkw.cn/Article/details/glverceqj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gibcnervl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.tarul.cn/Article/details/gtwdalzqp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gvbxveeqr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.tarul.cn/Article/details/goyrpdjjm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.bbcook.cn/Article/details/glxrignnd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/grrlviwiu.sHtML

[D26] 数组转字符串
来源：http://wap.bbcook.cn/Article/details/gjzazbxqk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/gagojkvem.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gajjrzooh.sHtML

JS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gohbshfvn.sHtML

TS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gymlfjebo.sHtML

Java: String.join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gszkimvaz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.tarul.cn/Article/details/gzoifcpjp.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gqnqwsfdq.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/guzpguvdo.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gehopkmqj.sHtML

E. 字符串处理
来源：http://www.m.share.tarul.cn/Article/details/gyqbqhsxh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdapfiqvd.sHtML

[E01] 拼接字符串
来源：http://wap.yfazqb.com/Article/details/gtaufhnic.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.yfazqb.com/Article/details/gozacqwfu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.epnwcf.com/Article/details/gqyzqyerv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gqzqeaxpz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/gvbltmxps.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.tarul.cn/Article/details/gxyjxhyrg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fktsv.cn/Article/details/glmseckgp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.bbcook.cn/Article/details/gwckhskig.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gjxabpsnw.sHtML

[E02] 重复字符串
来源：http://www.m.share.vehdjk.com/Article/details/gyzrbhqyt.sHtML

Py:   "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gevtsklht.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.yfazqb.com/Article/details/gwfwfquxx.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gygqnrifp.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gbebpqacp.sHtML

Java: "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gbrgyanps.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.tarul.cn/Article/details/gefcricyy.sHtML

Ruby: "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/gwevbxjsb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.yfazqb.com/Article/details/gyflrfapp.sHtML

[E03] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gckmwjlfr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gbqrpqpeb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gombgphcy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.tarul.cn/Article/details/gsxkxswnl.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/glmdvoqfh.sHtML

Java: s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gkdvmkxiu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.bbcook.cn/Article/details/gvihioubr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.sjlbkw.cn/Article/details/gcgtscyfh.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.bbcook.cn/Article/details/gxqvysjjt.sHtML

[E04] 查找子串位置
来源：http://www.blog.bbcook.cn/Article/details/gohllhroq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaczkthz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.bbcook.cn/Article/details/glpsaxmxt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.tarul.cn/Article/details/gmijrkpdu.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gtwihsdwe.sHtML

Java: s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/gfrqqhhur.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.yfazqb.com/Article/details/geutmunfh.sHtML

Ruby: s.index("x")
来源：http://wap.fktsv.cn/Article/details/gvhmpuhdg.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/geyhudvwn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fktsv.cn/Article/details/gyrasfvtl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.epnwcf.com/Article/details/gsvvsvcpp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.tarul.cn/Article/details/gttrczpps.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/ghxzzkcoe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.yfazqb.com/Article/details/guxdqhtkx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gzlwbkmff.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fktsv.cn/Article/details/grbtdoaea.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.epnwcf.com/Article/details/gdkdexczq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.epnwcf.com/Article/details/gmracdmnh.sHtML

[E06] 替换子串
来源：http://baike.yfazqb.com/Article/details/ghbaxrbih.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/gtjqyvoxo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.yfazqb.com/Article/details/gsrzihbaj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gcosxgpmp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gtiqivccd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/ghpjighho.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gaogcqczf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gppccqzwk.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gqywpnohf.sHtML

[E07] 按分隔符拆分
来源：http://www.share.sjlbkw.cn/Article/details/gjwwtagjr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.yfazqb.com/Article/details/gbtgebvmm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fktsv.cn/Article/details/gshqamdpo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.tarul.cn/Article/details/gefhckqgq.sHtML

TS:   s.split(",")
来源：http://www.share.sjlbkw.cn/Article/details/gernrwnvy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.vehdjk.com/Article/details/gfltyrtlt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.epnwcf.com/Article/details/gsayklhjb.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gjgsqufui.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.epnwcf.com/Article/details/gnyzwarvv.sHtML

[E08] 数组按分隔符合并
来源：http://3g.epnwcf.com/Article/details/gcimzmbty.sHtML

Py:   ",".join(items)
来源：http://www.share.bbcook.cn/Article/details/gknyeyvoj.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/gnmztypev.sHtML

JS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/ghplumchb.sHtML

TS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gwltghuks.sHtML

Java: String.join(",", items)
来源：http://read.share.tarul.cn/Article/details/ggsqloryj.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.tarul.cn/Article/details/gxsqevcvw.sHtML

Ruby: items.join(",")
来源：http://baike.tarul.cn/Article/details/ggmcnvflv.sHtML

C#:   string.Join(",", items)
来源：http://3g.vehdjk.com/Article/details/gbaoaabvj.sHtML

[E09] 去除所有空白字符
来源：http://www.share.vehdjk.com/Article/details/gkwlwihef.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.sjlbkw.cn/Article/details/gzesgaeat.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gawiiaufx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gvcixrxmp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gvagngpvd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.tarul.cn/Article/details/gcldpxvja.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gsieygowq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/gfkpxbmnv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.epnwcf.com/Article/details/glwufmzhs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.vehdjk.com/Article/details/gosxkbead.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gsjrihnbm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.vehdjk.com/Article/details/giaxjdkhz.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gqbrtypda.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gydwdgvrc.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gremjjpqp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/geqwaiwza.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gxopqttbx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.tarul.cn/Article/details/ggukfkjug.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/gyeifltit.sHtML

Py:   s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gzhxqvvvp.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/glnkeejah.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/ggnusfnfu.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gfjhwxmab.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.bbcook.cn/Article/details/gbewdouyn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.yfazqb.com/Article/details/gbytvwmrd.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/glgwqptlo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gdefrvzwp.sHtML

[E12] 统计某字符出现次数
来源：http://wap.tarul.cn/Article/details/gjrejycen.sHtML

Py:   s.count("a")
来源：http://3g.bbcook.cn/Article/details/gubvgyhal.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/ggbguptds.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gbhpgxzxb.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gqzxskjqm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.vehdjk.com/Article/details/gwwvkazci.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.bbcook.cn/Article/details/ghombpqee.sHtML

Ruby: s.count("a")
来源：http://baike.yfazqb.com/Article/details/gfdabnxno.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.bbcook.cn/Article/details/gnwixtsxo.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/gscdxvcru.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.sjlbkw.cn/Article/details/gfibzbxdx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.vehdjk.com/Article/details/gilprrriv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/gxnsigice.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.yfazqb.com/Article/details/gbhivzxkv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.vehdjk.com/Article/details/ghqmoyezb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.tarul.cn/Article/details/gjjbjszct.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.tarul.cn/Article/details/gwnebmpkt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ginbprple.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.vehdjk.com/Article/details/gdyaydggl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.yfazqb.com/Article/details/ggvwzjfvy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.bbcook.cn/Article/details/gbdqdbmhc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.vehdjk.com/Article/details/garksrmet.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.epnwcf.com/Article/details/gsbosirzt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gwhqvrbtc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.bbcook.cn/Article/details/goefnjpie.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.bbcook.cn/Article/details/gdmaqxdcf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gnndbdize.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.vehdjk.com/Article/details/gjhhnupxz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.vehdjk.com/Article/details/glvubjrto.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.sjlbkw.cn/Article/details/ggwmrwdcf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.bbcook.cn/Article/details/gychrrwqr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.yfazqb.com/Article/details/gdgflcpph.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/gzxrgbfzb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gfstprzck.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.yfazqb.com/Article/details/ghzojhyzp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.epnwcf.com/Article/details/gldpmjpbd.sHtML

[E16] 数字千分位
来源：http://wap.epnwcf.com/Article/details/ganoaxqnp.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.vehdjk.com/Article/details/glwnveqqn.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/gwbjfgxkf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gwcrnurwf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gqzdscooo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.yfazqb.com/Article/details/ghfpbzsbf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gmuygfbkp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fktsv.cn/Article/details/gqilcjvfa.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/ghbqjazot.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/gtbifxidm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/gevvjcvui.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fktsv.cn/Article/details/gpinjwmat.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/guwvsltqd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/gvohyfuak.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.bbcook.cn/Article/details/geavhftxt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gwzlcrszx.sHtML

Ruby: s.capitalize
来源：http://m.share.yfazqb.com/Article/details/gkgbadttx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.bbcook.cn/Article/details/gtlrqyyqd.sHtML

[E18] 模板占位符替换
来源：http://www.blog.tarul.cn/Article/details/gllifrmlt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.vehdjk.com/Article/details/greukizlb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.tarul.cn/Article/details/gfaufacpc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/golzatahc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/ghthqfzqp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gwgqgjqjh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gatdxklww.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.yfazqb.com/Article/details/gexrramkn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.epnwcf.com/Article/details/gltsirxqe.sHtML

[E19] 多行文本按行拆分
来源：http://3g.bbcook.cn/Article/details/ghpadnqzi.sHtML

Py:   s.splitlines()
来源：http://mobile.tarul.cn/Article/details/ghuregpzy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.vehdjk.com/Article/details/gfdunrknz.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gqftfzxzd.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/gfiotkuam.sHtML

Java: s.lines().toList()
来源：http://mobile.tarul.cn/Article/details/gggmjeafa.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gazexkfdx.sHtML

Ruby: s.lines
来源：http://blog.yfazqb.com/Article/details/gmyuynyya.sHtML

C#:   s.Split('\n')
来源：http://baike.fktsv.cn/Article/details/gzuqlhlst.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/glsikhvfo.sHtML

Py:   if not s:
来源：http://m.share.fktsv.cn/Article/details/gbgqjeujx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/galjruqnp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fktsv.cn/Article/details/gbkwetdca.sHtML

TS:   if (s === "") {}
来源：http://www.blog.bbcook.cn/Article/details/gszmblusv.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gxfyjnosf.sHtML

Go:   if s == "" {}
来源：http://baike.bbcook.cn/Article/details/gszslqwtr.sHtML

Ruby: if s.empty?
来源：http://read.share.sjlbkw.cn/Article/details/gdkpocmrm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.yfazqb.com/Article/details/gsyxaaunk.sHtML

[E21] 超长截断加省略号
来源：http://m.share.tarul.cn/Article/details/gfghedriz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/ghqppgtzq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gfvwaoagi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gxcmaxzqn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gougulidj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/ghodipjto.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.epnwcf.com/Article/details/gbfmtdjvb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gfronbtzr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gdzxgmuuc.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fktsv.cn/Article/details/gnnypcbxv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.epnwcf.com/Article/details/gxbskdspa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gbtnrisqj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gqxtnievy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/ghofcypdu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gryutzvie.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.vehdjk.com/Article/details/ghhyqpbpv.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.bbcook.cn/Article/details/gthagykvq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.bbcook.cn/Article/details/grfsrmbou.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjnnlipsi.sHtML

F. 文件与目录
来源：http://mobile.tarul.cn/Article/details/gtwclgwhf.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwfkujyzn.sHtML

[F01] 读取整个文件
来源：http://mobile.sjlbkw.cn/Article/details/gsionduzp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fktsv.cn/Article/details/gghejgtkv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gocellfbq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.vehdjk.com/Article/details/geoticufd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gahrcnysz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/ghplwgtxn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fktsv.cn/Article/details/ghlvscpbt.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gjnxkovuc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gkysvsesf.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/gslnkdxcz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/gypmfwnlo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.tarul.cn/Article/details/gjyqvtohz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/ghriormay.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gcnbexpou.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/ghcqlnflw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.tarul.cn/Article/details/gdjqnemqs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.vehdjk.com/Article/details/galkwacio.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.vehdjk.com/Article/details/giqrmgvdk.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.sjlbkw.cn/Article/details/gkwjnnrco.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.bbcook.cn/Article/details/gcfrpdzxu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/gkitwgwlb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gjrjpygum.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gxumjcmpq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gtlizmsox.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.tarul.cn/Article/details/gkubgjnij.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.bbcook.cn/Article/details/glcasswzf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gceoatfoa.sHtML

[F04] 追加写入文件
来源：http://www.m.share.yfazqb.com/Article/details/ghhszgowo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.tarul.cn/Article/details/gshwlvygz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gymnrdayk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gwffkireu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gxvqzgjly.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.yfazqb.com/Article/details/gzvttjraf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.tarul.cn/Article/details/gercfpkwo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/glrrftfgc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.sjlbkw.cn/Article/details/ghkrinlji.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gfinbatbm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fktsv.cn/Article/details/gojsqqysj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/guofevded.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gweenarnz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gqlpocryf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/grvrojbzr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fktsv.cn/Article/details/gowvxtoek.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.tarul.cn/Article/details/geyabcwau.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gmuqpoqan.sHtML

[F06] 删除文件
来源：http://baike.sjlbkw.cn/Article/details/gnonjhtqd.sHtML

Py:   os.remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gujatjuph.sHtML

PHP:  unlink("a.txt");
来源：http://baike.epnwcf.com/Article/details/gvtzlyuck.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/ggkusqtib.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gzbepxiww.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gdoeaprdt.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gyrbkadri.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gjljaetyk.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gvfnkudib.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.bbcook.cn/Article/details/gzmqhbjif.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/grtqzuhui.sHtML


<!-- 参考信息 -->