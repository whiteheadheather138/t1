代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gqdvtinxm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gzwkzkjlv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.sjlbkw.cn/Article/details/goqbnactn.sHtML

Go:   // 手写循环累加
来源：http://m.share.yfazqb.com/Article/details/gugyweytp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.yfazqb.com/Article/details/ghcqqrdjj.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.sjlbkw.cn/Article/details/gmmeeubub.sHtML

[D17] 最大值与最小值
来源：http://blog.vehdjk.com/Article/details/ggswerrbd.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fktsv.cn/Article/details/grxpxodrq.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/gexfvuqbf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.tarul.cn/Article/details/gotrkhryl.sHtML

TS:   Math.max(...arr);
来源：http://baike.yfazqb.com/Article/details/gthkpgafe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.epnwcf.com/Article/details/geunyqxva.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.tarul.cn/Article/details/gvxpqjxzj.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.sjlbkw.cn/Article/details/gktemxkka.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.sjlbkw.cn/Article/details/gnlxmvpke.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.tarul.cn/Article/details/gpolkbazi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fktsv.cn/Article/details/gejmdkful.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.tarul.cn/Article/details/gwiaygwjb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.epnwcf.com/Article/details/griguhtre.sHtML

TS:   nested.flat();
来源：http://3g.bbcook.cn/Article/details/gbwjjfcpq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fktsv.cn/Article/details/gtyeparyk.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.vehdjk.com/Article/details/gawmaruxx.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gyxzoglbt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fktsv.cn/Article/details/gozlyyaip.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/gpmwfgxjj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fktsv.cn/Article/details/gvmqyeaed.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.vehdjk.com/Article/details/gqaczjovv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.sjlbkw.cn/Article/details/gngswjueh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gyuwafmki.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.yfazqb.com/Article/details/ggubeecba.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fktsv.cn/Article/details/gpaulqpdx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.vehdjk.com/Article/details/gzrjbnjpg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.sjlbkw.cn/Article/details/glhpfuhto.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.bbcook.cn/Article/details/gtryhyvsj.sHtML

Py:   Counter(arr)
来源：http://mobile.yfazqb.com/Article/details/gudnwqqwg.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gkepayafv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gxplngtkc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/goninixab.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.vehdjk.com/Article/details/goifcippw.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.epnwcf.com/Article/details/gfsmuvtoj.sHtML

Ruby: arr.tally
来源：http://read.share.tarul.cn/Article/details/gwouyyond.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.sjlbkw.cn/Article/details/giyzrtier.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/gaccijttb.sHtML

Py:   x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/gslwgngbm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.sjlbkw.cn/Article/details/guhbeeehv.sHtML

JS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/ggjrvyzpe.sHtML

TS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gnlziiffq.sHtML

Java: list.contains(x)
来源：http://wap.tarul.cn/Article/details/gjxtmqrkt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gidfzwuju.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gjsxlarkq.sHtML

C#:   list.Contains(x)
来源：http://3g.yfazqb.com/Article/details/gngjobufz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/glyhszchv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.yfazqb.com/Article/details/gnrpzuuqg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.epnwcf.com/Article/details/gqmlylrbq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.vehdjk.com/Article/details/gouyjownn.sHtML

TS:   [...arr];
来源：http://baike.epnwcf.com/Article/details/gwgdcvagu.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.yfazqb.com/Article/details/grnqgwcna.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fktsv.cn/Article/details/gtqocgwli.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.vehdjk.com/Article/details/girazvwan.sHtML

C#:   new List<int>(list);
来源：http://wap.fktsv.cn/Article/details/grkdtqkga.sHtML

[D23] reduce 累积计算
来源：http://blog.bbcook.cn/Article/details/gecjswhqs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.yfazqb.com/Article/details/gvtbuvtli.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fktsv.cn/Article/details/gdrscsrvy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gnqzqknzb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gfhorqsnb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.bbcook.cn/Article/details/gbpzdstdi.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gutgsufgx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fktsv.cn/Article/details/gmlzedzeo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.tarul.cn/Article/details/gccbdifgh.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.tarul.cn/Article/details/gfyvykocd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.yfazqb.com/Article/details/grhcxfyrw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.tarul.cn/Article/details/gprewkkkv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.epnwcf.com/Article/details/ghgfbsxyv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gpcvopkce.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.sjlbkw.cn/Article/details/giqfdxqnw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.vehdjk.com/Article/details/gaokegzrc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gowgvtquh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fktsv.cn/Article/details/gosmuxyli.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.epnwcf.com/Article/details/gslbculci.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.bbcook.cn/Article/details/gvfieyceb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fktsv.cn/Article/details/grdbmsztz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.vehdjk.com/Article/details/grbjbhnkq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.sjlbkw.cn/Article/details/gcjkyernd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.epnwcf.com/Article/details/gdyqjxggg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.bbcook.cn/Article/details/gstwrjszv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.tarul.cn/Article/details/gswbwygbj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.epnwcf.com/Article/details/gvougcuzx.sHtML

[D26] 数组转字符串
来源：http://baike.sjlbkw.cn/Article/details/gkgdcjvwy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gklgolgvc.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.tarul.cn/Article/details/gcldhpdly.sHtML

JS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gokwsjupw.sHtML

TS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gqhrxdwlb.sHtML

Java: String.join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gzlxrixnh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.vehdjk.com/Article/details/gocylhxwp.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gcdzmsfkh.sHtML

C#:   string.Join(", ", list)
来源：http://3g.yfazqb.com/Article/details/grcgybsno.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdsfrkeew.sHtML

E. 字符串处理
来源：http://read.share.yfazqb.com/Article/details/geshuuyfa.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghmjqrffu.sHtML

[E01] 拼接字符串
来源：http://3g.yfazqb.com/Article/details/gpidiwiqn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.tarul.cn/Article/details/gpuianoev.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.vehdjk.com/Article/details/gfyxfupas.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gmihvotfd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/ghoslnxeu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fktsv.cn/Article/details/gfrnewapf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fktsv.cn/Article/details/gmlzvuajv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.sjlbkw.cn/Article/details/glldcqevr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gbhxaumfo.sHtML

[E02] 重复字符串
来源：http://mobile.bbcook.cn/Article/details/gfxtqyyxu.sHtML

Py:   "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/ggpvdpota.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.bbcook.cn/Article/details/gjladxxpp.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/getcvhwyh.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gyjljxfrq.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gyrjjuxwc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.vehdjk.com/Article/details/gmqhlpwuo.sHtML

Ruby: "ab" * 3
来源：http://blog.tarul.cn/Article/details/gachgpycw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.yfazqb.com/Article/details/ggvmgpved.sHtML

[E03] 截取子串
来源：http://read.share.fktsv.cn/Article/details/ggwcdkgzd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.bbcook.cn/Article/details/gsuckwpmg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/grnmxlbeq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/goybgnvwa.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.vehdjk.com/Article/details/guaosnqew.sHtML

Java: s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gxdgwudjt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gxxhveqis.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/gglnehchs.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.tarul.cn/Article/details/gmzvuicxl.sHtML

[E04] 查找子串位置
来源：http://wap.bbcook.cn/Article/details/gdzdwhupj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gixkbuiog.sHtML

PHP:  strpos($s, "x");
来源：http://wap.tarul.cn/Article/details/gslohxctc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.vehdjk.com/Article/details/gsxlckuve.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/guutxvuth.sHtML

Java: s.indexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gfdbhpcap.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.yfazqb.com/Article/details/gkbxerxzb.sHtML

Ruby: s.index("x")
来源：http://wap.epnwcf.com/Article/details/gfdvssmnc.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fktsv.cn/Article/details/giwtcjcon.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.bbcook.cn/Article/details/gglndwjeo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.tarul.cn/Article/details/gtpqrmnay.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.vehdjk.com/Article/details/gaahugqog.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/glepbdssg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.vehdjk.com/Article/details/gxfjoujij.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/gwkrpfklo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.bbcook.cn/Article/details/gtfbdsnig.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gqcyfyjkq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gdmyxxjuy.sHtML

[E06] 替换子串
来源：http://3g.vehdjk.com/Article/details/gcvbgnepe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/ghztgoevl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.sjlbkw.cn/Article/details/gfaghvyfn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gisycpssa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gmazkbsto.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/grhjqazar.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gzaxkyxni.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.epnwcf.com/Article/details/grfulsxsp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gcbpnparc.sHtML

[E07] 按分隔符拆分
来源：http://mobile.tarul.cn/Article/details/gywsnznso.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/gcadmwank.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gjasnczmv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.epnwcf.com/Article/details/gvptcsyhm.sHtML

TS:   s.split(",")
来源：http://read.share.yfazqb.com/Article/details/grwdigijb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.bbcook.cn/Article/details/gnlbybjsr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.bbcook.cn/Article/details/gixrvixzv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.bbcook.cn/Article/details/gmyhxnbcr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.tarul.cn/Article/details/gqtdtdydw.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fktsv.cn/Article/details/gwgildlnx.sHtML

Py:   ",".join(items)
来源：http://3g.yfazqb.com/Article/details/gcetydgrz.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/gnjfsfulp.sHtML

JS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gcotpenss.sHtML

TS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gozubigfs.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gauyouqon.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.bbcook.cn/Article/details/grdszirke.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gefwhgywi.sHtML

C#:   string.Join(",", items)
来源：http://baike.epnwcf.com/Article/details/gthrvffjv.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.vehdjk.com/Article/details/geiryurfr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/grkaclmge.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.yfazqb.com/Article/details/gykmhzqpj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gtiznxfgi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gijyaaier.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/gvhcwzjen.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/gkeewynli.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/ghugimvxv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gzpwannwt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.sjlbkw.cn/Article/details/gnznhprsy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gjwexanoo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.sjlbkw.cn/Article/details/gnlzbthyy.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gsrenfkjw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gugaqbtoe.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gxcveozfr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/ggkciioxn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gjufcuxdj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/gaszdnvvg.sHtML

[E11] 反转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gnidhhtpe.sHtML

Py:   s[::-1]
来源：http://wap.tarul.cn/Article/details/gnvalfdav.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gdhdsmyef.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gmgydodxa.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gwiagjnwv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fktsv.cn/Article/details/gnrxiiryv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.yfazqb.com/Article/details/gnxbkoray.sHtML

Ruby: s.reverse
来源：http://m.share.vehdjk.com/Article/details/gtjkpeffr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.epnwcf.com/Article/details/gpcheozpe.sHtML

[E12] 统计某字符出现次数
来源：http://blog.tarul.cn/Article/details/gszkjkfhl.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gpdfrbgir.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/glibcznza.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gxvshinxs.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.sjlbkw.cn/Article/details/gvyhnwpmg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.sjlbkw.cn/Article/details/gggkyofnh.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/gwrwssibx.sHtML

Ruby: s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/glgnuenkt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gxiachnka.sHtML

[E13] 逐字符遍历
来源：http://3g.fktsv.cn/Article/details/guqgzqqim.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fktsv.cn/Article/details/gmmcwokbi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.sjlbkw.cn/Article/details/gibfhdbjn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.epnwcf.com/Article/details/glvlrdvgc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/geyucckjm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fktsv.cn/Article/details/gedabysvc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.bbcook.cn/Article/details/gohvdzqaq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.vehdjk.com/Article/details/gsqdyrfwj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.yfazqb.com/Article/details/gsscqzcyl.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.sjlbkw.cn/Article/details/gqkbxzjsv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.yfazqb.com/Article/details/gwpvvvosa.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.tarul.cn/Article/details/gvqpsxmad.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.bbcook.cn/Article/details/getjcagox.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/gzrynkhci.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.epnwcf.com/Article/details/geueouwiv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gyftrnnld.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.bbcook.cn/Article/details/globthnaw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.epnwcf.com/Article/details/gwlzzjugx.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.sjlbkw.cn/Article/details/glvvtiowa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggofyggco.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.epnwcf.com/Article/details/gridtixsb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/gurmelfwf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fktsv.cn/Article/details/ggmszmbuq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/gcpqqajvf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.sjlbkw.cn/Article/details/ghdlkmefm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/gjiflxtiv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gwtpclhmz.sHtML

[E16] 数字千分位
来源：http://mobile.yfazqb.com/Article/details/gegpiirsu.sHtML

Py:   f"{1234567:,}"
来源：http://wap.epnwcf.com/Article/details/gthshcanx.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzinqooep.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/ghtltaayb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/grfyfshez.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gyzsaslxv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.bbcook.cn/Article/details/gksrbldtl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fktsv.cn/Article/details/gdblstmkv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.vehdjk.com/Article/details/gimmzxgjd.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/geptlzsaw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.bbcook.cn/Article/details/gboclynds.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.tarul.cn/Article/details/giwpeoutv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gvxlfvnkp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/gdeybpcwm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.tarul.cn/Article/details/gwuqhkhgu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/gzqzfzhxv.sHtML

Ruby: s.capitalize
来源：http://mobile.epnwcf.com/Article/details/gvobsxcyw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.sjlbkw.cn/Article/details/ghpbjhffl.sHtML

[E18] 模板占位符替换
来源：http://read.share.yfazqb.com/Article/details/gcbsjmzby.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.yfazqb.com/Article/details/giwgofuhi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.bbcook.cn/Article/details/gesixpqrp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gwbxyngmy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/goeakoqkb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gtnsrhvqc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.epnwcf.com/Article/details/ghfsmijda.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.vehdjk.com/Article/details/gzkizbjos.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.epnwcf.com/Article/details/ghlciwmnm.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/gegpfpugp.sHtML

Py:   s.splitlines()
来源：http://baike.bbcook.cn/Article/details/gezsecenq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gtdmkjonw.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gnfaenauk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gcepdwtho.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gelcfelto.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.yfazqb.com/Article/details/gxlyyhgvd.sHtML

Ruby: s.lines
来源：http://m.share.tarul.cn/Article/details/gamyparyh.sHtML

C#:   s.Split('\n')
来源：http://read.share.tarul.cn/Article/details/goxwumjpo.sHtML

[E20] 判断字符串是否为空
来源：http://blog.sjlbkw.cn/Article/details/gwiwynnkd.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/gradcfadf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.tarul.cn/Article/details/gxkipchwq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.sjlbkw.cn/Article/details/gupfkmcgv.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.vehdjk.com/Article/details/gnrbmgfdo.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/glyiexcuw.sHtML

Go:   if s == "" {}
来源：http://www.blog.epnwcf.com/Article/details/gxznpdspc.sHtML

Ruby: if s.empty?
来源：http://3g.fktsv.cn/Article/details/gqxqrfnpe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.tarul.cn/Article/details/gdtgpwfpw.sHtML

[E21] 超长截断加省略号
来源：http://read.share.yfazqb.com/Article/details/ggjsokjol.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.epnwcf.com/Article/details/garckyobi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.tarul.cn/Article/details/gpvtocqih.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gkxkhbnja.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gntmibptw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gopzbzikh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.sjlbkw.cn/Article/details/ggcqgpqzy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gtxjelkld.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gusmpktxd.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.sjlbkw.cn/Article/details/govcqywwz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.vehdjk.com/Article/details/gjanykrdk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gyngmtvuw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/ghsjaeurs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/gjrwwxdbx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gfnwgtddt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.sjlbkw.cn/Article/details/gwasgvfwu.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.tarul.cn/Article/details/goarhfrys.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gllzzcmes.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvwykpbcm.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gneomwnbg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghoemyuxu.sHtML


<!-- 参考信息 -->