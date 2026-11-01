代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.yfazqb.com/Article/details/gsioamruo.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.epnwcf.com/Article/details/gbosknbzh.sHtML

Py:   Counter(arr)
来源：http://baike.sjlbkw.cn/Article/details/gsbxnvyjp.sHtML

PHP:  array_count_values($arr);
来源：http://baike.yfazqb.com/Article/details/gepcqtvoa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/gwtgnbykj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/gqztcuxze.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.tarul.cn/Article/details/grmdrqzlq.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.tarul.cn/Article/details/geshduujm.sHtML

Ruby: arr.tally
来源：http://m.share.fktsv.cn/Article/details/gsuctsfbt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.sjlbkw.cn/Article/details/grctcztdv.sHtML

[D21] 判断是否包含某元素
来源：http://blog.tarul.cn/Article/details/gltdfbbwo.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/guwvueexb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fktsv.cn/Article/details/gqjbuoqfj.sHtML

JS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/gebfbdnhy.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gnmhwtmns.sHtML

Java: list.contains(x)
来源：http://blog.epnwcf.com/Article/details/gclathtwr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gplrewlbn.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.bbcook.cn/Article/details/ghgagssmx.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gqxsqanju.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.tarul.cn/Article/details/gwxyzjvkx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.vehdjk.com/Article/details/gncpghvua.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fktsv.cn/Article/details/gzlplkart.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.yfazqb.com/Article/details/gxscspnmj.sHtML

TS:   [...arr];
来源：http://www.blog.fktsv.cn/Article/details/gbxnbczck.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.vehdjk.com/Article/details/gsyyrjcxv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fktsv.cn/Article/details/gxgemovst.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.sjlbkw.cn/Article/details/gucdoyhgx.sHtML

C#:   new List<int>(list);
来源：http://read.share.epnwcf.com/Article/details/gxbfwzzyx.sHtML

[D23] reduce 累积计算
来源：http://wap.fktsv.cn/Article/details/gypfjtutz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gyjhwxdmi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.yfazqb.com/Article/details/gfqtnpubr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/gtksurkcy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gdypjddbm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.tarul.cn/Article/details/gtnswucsz.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gxcqwntkb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.tarul.cn/Article/details/gevxqaxgs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.yfazqb.com/Article/details/gtkgtjyjb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.tarul.cn/Article/details/gzvfxdght.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.tarul.cn/Article/details/gptialjhl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.tarul.cn/Article/details/gitciuwrs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gaxzwesru.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.tarul.cn/Article/details/gofdrtwvd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.epnwcf.com/Article/details/gnawwbdhc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fktsv.cn/Article/details/grjikjpmb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gobccsmch.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.tarul.cn/Article/details/gozxbcxxe.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/grvjgwafq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.epnwcf.com/Article/details/gmlwbvvtg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.vehdjk.com/Article/details/gsmvmapzp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.bbcook.cn/Article/details/gbcshjois.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fktsv.cn/Article/details/gfewpocqp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.vehdjk.com/Article/details/gajnmoyfn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.vehdjk.com/Article/details/gvcigzjec.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.bbcook.cn/Article/details/gnubtegsv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/gfztdkxuo.sHtML

[D26] 数组转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gfinhoucg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/gooslyyag.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.vehdjk.com/Article/details/gdilkluea.sHtML

JS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gowrvmwaw.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gsulhjupl.sHtML

Java: String.join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gvdebxsdu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.epnwcf.com/Article/details/gokqpumuw.sHtML

Ruby: arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gsemumdeo.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gwpboehba.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gueigqbue.sHtML

E. 字符串处理
来源：http://m.share.bbcook.cn/Article/details/gqncfqtoa.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gbrylvgqm.sHtML

[E01] 拼接字符串
来源：http://wap.tarul.cn/Article/details/glnvoqeoi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gogmwhypy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.vehdjk.com/Article/details/glcabxklp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/gaccttpmo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gldexpehc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gvlzeprei.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.tarul.cn/Article/details/ghhtextpf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.bbcook.cn/Article/details/gqoosmcpt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.tarul.cn/Article/details/gpksrsadu.sHtML

[E02] 重复字符串
来源：http://m.share.fktsv.cn/Article/details/gkkufoxuh.sHtML

Py:   "ab" * 3
来源：http://3g.bbcook.cn/Article/details/gcnuwlyus.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.epnwcf.com/Article/details/gpjtzscij.sHtML

JS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/gsiuagqrb.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gzrpuocmq.sHtML

Java: "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gwjoalstp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.sjlbkw.cn/Article/details/gworwmtsu.sHtML

Ruby: "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gyiqdgccy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.tarul.cn/Article/details/gzzmgorwb.sHtML

[E03] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gyeduqyuq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.bbcook.cn/Article/details/gehkyctav.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gimojpecq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/genlwaifk.sHtML

TS:   s.slice(1, 4)
来源：http://wap.epnwcf.com/Article/details/ghdumibmx.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gfahdphja.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.bbcook.cn/Article/details/gcleqxaor.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fktsv.cn/Article/details/gqpsjdynk.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.tarul.cn/Article/details/gkhfcndzk.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gnosuhwjm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gzhfjkzsq.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.tarul.cn/Article/details/gfmgeuoul.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.epnwcf.com/Article/details/grpnafzqb.sHtML

TS:   s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gyvytrzhi.sHtML

Java: s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gkrymkvqx.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.tarul.cn/Article/details/gnuhpwjfa.sHtML

Ruby: s.index("x")
来源：http://m.share.vehdjk.com/Article/details/glfgynjzo.sHtML

C#:   s.IndexOf("x")
来源：http://wap.bbcook.cn/Article/details/gkikpjedd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.bbcook.cn/Article/details/gjpkfgheg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.bbcook.cn/Article/details/ghqagvuam.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.epnwcf.com/Article/details/grdixeark.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gswbaaqge.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.yfazqb.com/Article/details/gnhzesyqg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/grosvkbiw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.epnwcf.com/Article/details/gcpnqyypb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.yfazqb.com/Article/details/ggwnyeylc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.tarul.cn/Article/details/geldvraan.sHtML

[E06] 替换子串
来源：http://wap.vehdjk.com/Article/details/gfphgcmow.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/grqiiybdn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/gwgunqquy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gdpuoyswg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gvzdyjggc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gavzayjow.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gkjruaxlj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gjrqrcmcc.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.epnwcf.com/Article/details/gmjnqlduh.sHtML

[E07] 按分隔符拆分
来源：http://read.share.epnwcf.com/Article/details/gvuioihza.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.epnwcf.com/Article/details/gvninhpje.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gtivzzeah.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.tarul.cn/Article/details/gunevijpt.sHtML

TS:   s.split(",")
来源：http://m.share.epnwcf.com/Article/details/grnqwfpfk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.yfazqb.com/Article/details/gpncwbtgt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fktsv.cn/Article/details/gyzdllekp.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.epnwcf.com/Article/details/gcvzsgfbp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.bbcook.cn/Article/details/gdehxztiw.sHtML

[E08] 数组按分隔符合并
来源：http://baike.sjlbkw.cn/Article/details/golxpqxtw.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gtydkuluk.sHtML

PHP:  implode(",", $items);
来源：http://www.share.yfazqb.com/Article/details/gosqrjydm.sHtML

JS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gqidqclvw.sHtML

TS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gwakpmhhf.sHtML

Java: String.join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gpixovgby.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.tarul.cn/Article/details/gtyugkwij.sHtML

Ruby: items.join(",")
来源：http://baike.bbcook.cn/Article/details/gemasevnu.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gigurnjgz.sHtML

[E09] 去除所有空白字符
来源：http://m.share.tarul.cn/Article/details/gdovskfqq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.sjlbkw.cn/Article/details/gznurlfjl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fktsv.cn/Article/details/gqyszraoz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gdcumbbit.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gaeoedhpg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.vehdjk.com/Article/details/gmaufmixl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.epnwcf.com/Article/details/gwchfkkje.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.epnwcf.com/Article/details/glsjrqhet.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.epnwcf.com/Article/details/gazmhnnkc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.bbcook.cn/Article/details/gboopbujt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/gqfylmual.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.vehdjk.com/Article/details/godfzpcog.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/ghbvszjmt.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/getfzmvbb.sHtML

Java: String.format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gtfvavidb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gjtvfvold.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/golzlfuaw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/godeouvto.sHtML

[E11] 反转字符串
来源：http://m.share.bbcook.cn/Article/details/gmxqycjdg.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gsonjxdvq.sHtML

PHP:  strrev($s);
来源：http://m.share.vehdjk.com/Article/details/gplqexpeg.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gkmscwebq.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gvccaenge.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.bbcook.cn/Article/details/gyzhttfbk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/ghhrfaiqr.sHtML

Ruby: s.reverse
来源：http://mobile.bbcook.cn/Article/details/gmjagywro.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gaawpabkc.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gtawldnfu.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gpckzfjjx.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.vehdjk.com/Article/details/gcwwrhegc.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.epnwcf.com/Article/details/giznpscwi.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/gyuyqccma.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.tarul.cn/Article/details/gavmqkxul.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.sjlbkw.cn/Article/details/gyapzlszm.sHtML

Ruby: s.count("a")
来源：http://3g.epnwcf.com/Article/details/gbtnmzigh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.epnwcf.com/Article/details/gpkscrfyl.sHtML

[E13] 逐字符遍历
来源：http://read.share.fktsv.cn/Article/details/gekkkicyc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.sjlbkw.cn/Article/details/gkgultgoj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fktsv.cn/Article/details/ghqfijztt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/gxenvduxi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gfasigoek.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gtuyzfotq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.vehdjk.com/Article/details/glhebxsmj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.sjlbkw.cn/Article/details/ggisokrdl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.bbcook.cn/Article/details/gwgacktls.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.vehdjk.com/Article/details/ggbydtnac.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fktsv.cn/Article/details/gzqkhhtxr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.vehdjk.com/Article/details/gtbecjlgz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/gzhofzgdj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.yfazqb.com/Article/details/gijdsdjvy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.tarul.cn/Article/details/glscjfzdf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.yfazqb.com/Article/details/gtksphdgo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.vehdjk.com/Article/details/gsiiknyoi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/gcqiwxsus.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.tarul.cn/Article/details/gcvbfpfdz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.epnwcf.com/Article/details/gthgjrong.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.yfazqb.com/Article/details/gyfhislys.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/gwimofpru.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.bbcook.cn/Article/details/gwcimogmc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.tarul.cn/Article/details/ghxqiiuzr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.vehdjk.com/Article/details/gtvtgwyue.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fktsv.cn/Article/details/gznxwwwxi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.tarul.cn/Article/details/gqzkoyxhc.sHtML

[E16] 数字千分位
来源：http://m.share.fktsv.cn/Article/details/gopulmxnh.sHtML

Py:   f"{1234567:,}"
来源：http://blog.bbcook.cn/Article/details/ginnldfch.sHtML

PHP:  number_format(1234567);
来源：http://wap.tarul.cn/Article/details/gkvlzwoqu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/grcqgoxfh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/ghqdiirlw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/grggdsvyh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.vehdjk.com/Article/details/gkhynmhzd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.tarul.cn/Article/details/gyerypsfh.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.sjlbkw.cn/Article/details/gvilwnafz.sHtML

[E17] 首字母大写
来源：http://www.m.share.tarul.cn/Article/details/gnfqslgyl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fktsv.cn/Article/details/ghxkkbptr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fktsv.cn/Article/details/gfitvujeh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.sjlbkw.cn/Article/details/gpccswjlp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gigwnfmwf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/gldpssuno.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.bbcook.cn/Article/details/gykgufrep.sHtML

Ruby: s.capitalize
来源：http://www.blog.vehdjk.com/Article/details/giwlyaqaq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.bbcook.cn/Article/details/gxdjdvkuw.sHtML

[E18] 模板占位符替换
来源：http://read.share.yfazqb.com/Article/details/gjrrgangg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.vehdjk.com/Article/details/gpwdnswey.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.tarul.cn/Article/details/gfkrciqfb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gskgkdlbo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gmeayldkv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gnifgtsyf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/gpmwcprhy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/gwsljnffw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.epnwcf.com/Article/details/gixislwao.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/gkidgpemf.sHtML

Py:   s.splitlines()
来源：http://wap.vehdjk.com/Article/details/gnjqbsamu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.vehdjk.com/Article/details/grwfabqal.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/gjfoeuzlg.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gsactsbqm.sHtML

Java: s.lines().toList()
来源：http://www.m.share.vehdjk.com/Article/details/goyquqpbp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.epnwcf.com/Article/details/goufzsycf.sHtML

Ruby: s.lines
来源：http://3g.bbcook.cn/Article/details/ggxaciyhc.sHtML

C#:   s.Split('\n')
来源：http://m.share.vehdjk.com/Article/details/gbwppelkk.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.vehdjk.com/Article/details/gpkzsfgld.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gzawjvmlv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/gocojcpza.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.yfazqb.com/Article/details/ggkhxypgb.sHtML

TS:   if (s === "") {}
来源：http://wap.sjlbkw.cn/Article/details/gojrxqbwr.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gbgjhqaip.sHtML

Go:   if s == "" {}
来源：http://www.share.vehdjk.com/Article/details/gezwrhqjy.sHtML

Ruby: if s.empty?
来源：http://mobile.vehdjk.com/Article/details/gpygyvhqy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gjevyyjxj.sHtML

[E21] 超长截断加省略号
来源：http://blog.epnwcf.com/Article/details/gutthdktj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.yfazqb.com/Article/details/gkcoflbvf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gcnfaunjh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gnbqjvpuo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gecnwsqio.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gylixqmct.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.yfazqb.com/Article/details/gpigvuwlu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gzmkdzwnv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/giyzzhyxl.sHtML

[E22] 字节长度与字符长度
来源：http://baike.yfazqb.com/Article/details/gpjmyjyrq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.sjlbkw.cn/Article/details/gfroeqxhz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gutlyduxy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gzinzhdyi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gwcirpnxr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.bbcook.cn/Article/details/gvdmjcmha.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.yfazqb.com/Article/details/gvdlftzba.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.vehdjk.com/Article/details/gmwbfaasa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.epnwcf.com/Article/details/gfgokmpgz.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gebpotzpx.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/giayrefvq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gagvtdkmn.sHtML

[F01] 读取整个文件
来源：http://blog.tarul.cn/Article/details/gqrlkuwap.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fktsv.cn/Article/details/gjaktdelc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gejjoflqh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.yfazqb.com/Article/details/gaggywtgk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gaoarxjgw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gllvlteam.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.vehdjk.com/Article/details/guumdozsc.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gwzrprziw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/gqonbwvoj.sHtML

[F02] 逐行读取文件
来源：http://3g.fktsv.cn/Article/details/gnpbeixpt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.tarul.cn/Article/details/gknohqpfv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.tarul.cn/Article/details/gfhkdjhfa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gveovfzcd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/ggxccnuav.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/grnqtaalh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/gxihwwsth.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fktsv.cn/Article/details/gjkkiaidn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fktsv.cn/Article/details/gqqmfumgz.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.yfazqb.com/Article/details/gbbpgouqg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fktsv.cn/Article/details/geetafzhv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gtucfbnjb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gqoqipfpm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gdrflsqor.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.vehdjk.com/Article/details/gkqjkmhsf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.sjlbkw.cn/Article/details/gyfwvikmg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.tarul.cn/Article/details/gbcgrluoz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gygemzmbj.sHtML

[F04] 追加写入文件
来源：http://blog.bbcook.cn/Article/details/gvjtfroxo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fktsv.cn/Article/details/gizjrival.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/gtxrazimc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gulyytsua.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gxdmwvwul.sHtML


<!-- 参考信息 -->