代发 wailian999

[D15] 去重
来源：http://read.share.fktsv.cn/Article/details/gyczewbzc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fktsv.cn/Article/details/gzqwleoet.sHtML

PHP:  array_unique($arr);
来源：http://www.share.epnwcf.com/Article/details/guxyfvpoz.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gfimuhqax.sHtML

TS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gprybeeym.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.bbcook.cn/Article/details/gslbdhary.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fktsv.cn/Article/details/gswchewpy.sHtML

Ruby: arr.uniq
来源：http://mobile.epnwcf.com/Article/details/grimhojpf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.vehdjk.com/Article/details/gbfcaewns.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gpmolnsur.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.epnwcf.com/Article/details/gkkhtkuyx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.epnwcf.com/Article/details/gakijijjk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/glkyrjept.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/gihcdykld.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fktsv.cn/Article/details/guanpxvcw.sHtML

Go:   // 手写循环累加
来源：http://3g.epnwcf.com/Article/details/goqukjjhe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.sjlbkw.cn/Article/details/gytunshix.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fktsv.cn/Article/details/gymvlltdu.sHtML

[D17] 最大值与最小值
来源：http://blog.vehdjk.com/Article/details/gpjolqior.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gyljeivgx.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fktsv.cn/Article/details/gpqdxzydd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.sjlbkw.cn/Article/details/gomvhiddd.sHtML

TS:   Math.max(...arr);
来源：http://www.share.epnwcf.com/Article/details/gmdzyxcwx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fktsv.cn/Article/details/gzshakdhs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.vehdjk.com/Article/details/grzhopubo.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fktsv.cn/Article/details/glnlhihmb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/geyeouyfe.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.bbcook.cn/Article/details/gnmpvhmjz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.yfazqb.com/Article/details/gllskutoz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.sjlbkw.cn/Article/details/gezifjfqn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.sjlbkw.cn/Article/details/gtlozhowm.sHtML

TS:   nested.flat();
来源：http://www.m.share.yfazqb.com/Article/details/gkapzsqxv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.sjlbkw.cn/Article/details/gxhdqxkzb.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/garkyapsa.sHtML

Ruby: nested.flatten
来源：http://baike.sjlbkw.cn/Article/details/gwzddtyrp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.yfazqb.com/Article/details/gndhfftqv.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/gfyrsqjaw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gvdvdssbi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.vehdjk.com/Article/details/geqfzcaib.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.bbcook.cn/Article/details/gtdmsrxtx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/gzkzyhfdq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.sjlbkw.cn/Article/details/gwuerqljo.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.yfazqb.com/Article/details/giporvvgm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fktsv.cn/Article/details/gqqdgxsup.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.tarul.cn/Article/details/ghhfyiaut.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.sjlbkw.cn/Article/details/gdykzmgpm.sHtML

Py:   Counter(arr)
来源：http://read.share.bbcook.cn/Article/details/grqpytuva.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.bbcook.cn/Article/details/gxvcyqpgi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/gwnjoaiue.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/goqcczlwz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.bbcook.cn/Article/details/gnlinfdcv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/gecppyoyf.sHtML

Ruby: arr.tally
来源：http://m.share.tarul.cn/Article/details/gzdwnuwbm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.vehdjk.com/Article/details/grbhpluzh.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fktsv.cn/Article/details/glihabeou.sHtML

Py:   x in arr
来源：http://3g.tarul.cn/Article/details/gcffkwsvk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.bbcook.cn/Article/details/gmcyhjnzm.sHtML

JS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gcszfhajv.sHtML

TS:   arr.includes(x)
来源：http://read.share.fktsv.cn/Article/details/gcnqwushh.sHtML

Java: list.contains(x)
来源：http://baike.fktsv.cn/Article/details/gfketsanv.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gggmadubm.sHtML

Ruby: arr.include?(x)
来源：http://mobile.bbcook.cn/Article/details/grnjpwibc.sHtML

C#:   list.Contains(x)
来源：http://baike.bbcook.cn/Article/details/gvbzrppuu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.vehdjk.com/Article/details/glmwfgfni.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.bbcook.cn/Article/details/gjaurkarl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.sjlbkw.cn/Article/details/gtgrqlgnn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.yfazqb.com/Article/details/gpsumradj.sHtML

TS:   [...arr];
来源：http://mobile.yfazqb.com/Article/details/gnzdnnfba.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.bbcook.cn/Article/details/guhpmuuqb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.tarul.cn/Article/details/gsfwebqan.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.yfazqb.com/Article/details/gskibnumy.sHtML

C#:   new List<int>(list);
来源：http://mobile.vehdjk.com/Article/details/gpdfogxau.sHtML

[D23] reduce 累积计算
来源：http://m.share.tarul.cn/Article/details/gnntxivux.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gscziiwho.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.yfazqb.com/Article/details/garukzfpo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gcqayegob.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/gyaypwzom.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fktsv.cn/Article/details/ggzgkwxqd.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gwhiktccb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.sjlbkw.cn/Article/details/gtxbvbnei.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.epnwcf.com/Article/details/gxoxxcrkw.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/gmcttnyhw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.bbcook.cn/Article/details/gtknlkpbv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.sjlbkw.cn/Article/details/gowwelbpn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.vehdjk.com/Article/details/ghuoqfyck.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gxwgnmzfv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.yfazqb.com/Article/details/ggaeqxzjw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fktsv.cn/Article/details/gfhepjsgb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.bbcook.cn/Article/details/gboryhhwj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.bbcook.cn/Article/details/gsojehakr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.vehdjk.com/Article/details/gikufdtfc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.epnwcf.com/Article/details/gwnpxwdyr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.sjlbkw.cn/Article/details/ggqtswfsa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/gdcjpaluf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.yfazqb.com/Article/details/gutgqhiac.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fktsv.cn/Article/details/glifeevcl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.yfazqb.com/Article/details/gpwsitvaf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.tarul.cn/Article/details/gifyqrabr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.yfazqb.com/Article/details/gztnkdvxh.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gzgxomjok.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gohyrgxzb.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.sjlbkw.cn/Article/details/geeeehpon.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/grewqerfs.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gpfsbkqrx.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gxkdmfhuq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.sjlbkw.cn/Article/details/gzwzurfav.sHtML

Ruby: arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/ghoggbema.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gomszvwcm.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/geonkgmtx.sHtML

E. 字符串处理
来源：http://www.blog.yfazqb.com/Article/details/gfmaodgcu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcykzrnyu.sHtML

[E01] 拼接字符串
来源：http://read.share.epnwcf.com/Article/details/genwinjgt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.sjlbkw.cn/Article/details/gohmirpff.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.bbcook.cn/Article/details/gwjdixppi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/gftlzoixl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gxkejnuhk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.tarul.cn/Article/details/gjdrgjejv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fktsv.cn/Article/details/gmtqiunyf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.bbcook.cn/Article/details/gcaziljxw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gphhlqdfl.sHtML

[E02] 重复字符串
来源：http://www.blog.vehdjk.com/Article/details/gnjtmovbc.sHtML

Py:   "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gpcjgasou.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/ggctheapn.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gbqovmjgb.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gmlqjmajj.sHtML

Java: "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gpybqxxtk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.sjlbkw.cn/Article/details/gpvcuhbmj.sHtML

Ruby: "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gyyazkfer.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gfbkwnyrb.sHtML

[E03] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gwkquthwx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.bbcook.cn/Article/details/gtyphiysc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gqqddrdkp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gjxrmcrny.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gyftsdfmc.sHtML

Java: s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gsjvshybf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.bbcook.cn/Article/details/gpovhnppw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.yfazqb.com/Article/details/gxpcewnly.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.epnwcf.com/Article/details/gfovssggb.sHtML

[E04] 查找子串位置
来源：http://www.share.yfazqb.com/Article/details/gurbzxbrn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gsbuvgfyv.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.bbcook.cn/Article/details/gsujjmqmf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.epnwcf.com/Article/details/guuqjeoph.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gxtuqxlqd.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gjtbiqchu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.tarul.cn/Article/details/glnetylfv.sHtML

Ruby: s.index("x")
来源：http://wap.tarul.cn/Article/details/gsjixtmry.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gxnmfpqgk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.bbcook.cn/Article/details/gziocftgj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.epnwcf.com/Article/details/gmjgzgkqx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.tarul.cn/Article/details/gjtkjrcve.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gtggrfhhw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.yfazqb.com/Article/details/gfscgwkki.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gexjbvglr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.yfazqb.com/Article/details/gxfihgcpv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.vehdjk.com/Article/details/gyiyntofv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.yfazqb.com/Article/details/gsonzlvlj.sHtML

[E06] 替换子串
来源：http://www.m.share.tarul.cn/Article/details/gpnjgjkfh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/ghdyqlynv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fktsv.cn/Article/details/gtqxmtcuu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gghpesjej.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gbqmqrelw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gpdwqnriv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gdrlwzuye.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gxffetabd.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.vehdjk.com/Article/details/gtoepxrly.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/gyfqbetwp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.vehdjk.com/Article/details/gmyjpfpdy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gtvqdrxyh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/gmcusixnl.sHtML

TS:   s.split(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gedwqnnul.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/gtqqdwdln.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/gjsovkcfk.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.epnwcf.com/Article/details/gpoljxwml.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.yfazqb.com/Article/details/gelimfwfb.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.yfazqb.com/Article/details/gbibprrnk.sHtML

Py:   ",".join(items)
来源：http://www.blog.tarul.cn/Article/details/gikgkicey.sHtML

PHP:  implode(",", $items);
来源：http://www.share.vehdjk.com/Article/details/gqkowwaox.sHtML

JS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gmrhuzant.sHtML

TS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gazfkruyk.sHtML

Java: String.join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gvxntpqjt.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/gekusmnrj.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gwijqhent.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gcuqurwgk.sHtML

[E09] 去除所有空白字符
来源：http://mobile.bbcook.cn/Article/details/gcjyminfi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.sjlbkw.cn/Article/details/gxgscaxbi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.tarul.cn/Article/details/gsflfmtlx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/geeomfuol.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/gsqjsbmln.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gebodjxpg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.yfazqb.com/Article/details/ghxlwhlue.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.bbcook.cn/Article/details/gmagzwcgr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.yfazqb.com/Article/details/ghpzzqtvp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.sjlbkw.cn/Article/details/gnckbzuan.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fktsv.cn/Article/details/gmqhjuptm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.vehdjk.com/Article/details/ghncrisus.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gcjuwnkks.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gbyigjkei.sHtML

Java: String.format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gqnjdcyvk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gwtvyexzo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gvjqcucko.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/gyflwagve.sHtML

[E11] 反转字符串
来源：http://baike.bbcook.cn/Article/details/gptowsxhb.sHtML

Py:   s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gsrkcgyoy.sHtML

PHP:  strrev($s);
来源：http://3g.vehdjk.com/Article/details/gsikvmuuk.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/goonwunhp.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gerrkciht.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.tarul.cn/Article/details/gpeuprykv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.yfazqb.com/Article/details/gzgmbfcox.sHtML

Ruby: s.reverse
来源：http://wap.vehdjk.com/Article/details/gvtlrxoio.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/ggxqxuuvq.sHtML

[E12] 统计某字符出现次数
来源：http://wap.sjlbkw.cn/Article/details/gltujehco.sHtML

Py:   s.count("a")
来源：http://wap.yfazqb.com/Article/details/grczxyljk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.vehdjk.com/Article/details/gebctifmd.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gydvfkwkp.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gsaltprmy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxayqwccv.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.epnwcf.com/Article/details/ghlmnwale.sHtML

Ruby: s.count("a")
来源：http://baike.yfazqb.com/Article/details/gcgzfxvvd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.bbcook.cn/Article/details/githkkibh.sHtML

[E13] 逐字符遍历
来源：http://baike.bbcook.cn/Article/details/gjvnfjbjv.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.vehdjk.com/Article/details/gqcppvtbn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.sjlbkw.cn/Article/details/gqaakqooi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.vehdjk.com/Article/details/gmhyyamgo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/guhcnmyxz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gvgtydemb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.vehdjk.com/Article/details/gnhqixefp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.bbcook.cn/Article/details/giuooscrp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.epnwcf.com/Article/details/ghixelgbb.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/gbibqmetq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.epnwcf.com/Article/details/gslsvvqou.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.tarul.cn/Article/details/gkxbqwcix.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.vehdjk.com/Article/details/gdpevgfvl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.tarul.cn/Article/details/gbinlouej.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrpwdqsx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.bbcook.cn/Article/details/gxjoivhku.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.bbcook.cn/Article/details/guvhawiei.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/goidaoxxx.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.yfazqb.com/Article/details/gmrpvmpyg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fktsv.cn/Article/details/gzdkcbmjc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/gxhpjemao.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gyjxmeqts.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.yfazqb.com/Article/details/gisdxlxer.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.vehdjk.com/Article/details/gyfdpuejj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.vehdjk.com/Article/details/gszdcwhcg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.vehdjk.com/Article/details/gcsqjueeu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fktsv.cn/Article/details/gzsptpyut.sHtML

[E16] 数字千分位
来源：http://www.blog.tarul.cn/Article/details/gclrlrknl.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.bbcook.cn/Article/details/gzzaffeai.sHtML

PHP:  number_format(1234567);
来源：http://www.share.yfazqb.com/Article/details/gpzcusijx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gkaiukdza.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gplltcyfd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.vehdjk.com/Article/details/gokkimnsy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.tarul.cn/Article/details/gwcxgujkn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.vehdjk.com/Article/details/gfufvrwxo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.tarul.cn/Article/details/goyrlldzj.sHtML

[E17] 首字母大写
来源：http://read.share.epnwcf.com/Article/details/getmoezom.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gioonyiae.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.tarul.cn/Article/details/gzediljkt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gxjwudish.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gitcgvewg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.bbcook.cn/Article/details/gmvaslany.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.yfazqb.com/Article/details/gymwqtqmn.sHtML

Ruby: s.capitalize
来源：http://www.share.bbcook.cn/Article/details/gxwmozcmd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.yfazqb.com/Article/details/gpbcktlhw.sHtML

[E18] 模板占位符替换
来源：http://mobile.fktsv.cn/Article/details/gcvbzssgx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.bbcook.cn/Article/details/gxxjjyflv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.sjlbkw.cn/Article/details/gmzjvjjjl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gbbnyaekh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gjdmbsomt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/ghpykuuga.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gxoqhwkkk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/griyxammi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.vehdjk.com/Article/details/gjrowuroi.sHtML

[E19] 多行文本按行拆分
来源：http://wap.sjlbkw.cn/Article/details/gpdckinwu.sHtML

Py:   s.splitlines()
来源：http://m.share.epnwcf.com/Article/details/gbemrxcjw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gluwsbtok.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gbfrziopz.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gkdgbijmc.sHtML

Java: s.lines().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gbtbkytbg.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.epnwcf.com/Article/details/ggvkhamxf.sHtML

Ruby: s.lines
来源：http://www.m.share.tarul.cn/Article/details/gnmapmspk.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/gmotnjxoo.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fktsv.cn/Article/details/gbclihnyf.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gvsdkoboc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.bbcook.cn/Article/details/gdvwntqsi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.bbcook.cn/Article/details/glbibnftk.sHtML

TS:   if (s === "") {}
来源：http://3g.tarul.cn/Article/details/gxkobcliu.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/gxodvhhmp.sHtML

Go:   if s == "" {}
来源：http://www.m.share.tarul.cn/Article/details/gbvesrmkz.sHtML

Ruby: if s.empty?
来源：http://www.m.share.tarul.cn/Article/details/goxzaiezt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gypincujb.sHtML

[E21] 超长截断加省略号
来源：http://wap.tarul.cn/Article/details/gvvryasre.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.sjlbkw.cn/Article/details/gafetmhwt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gwekshhvi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gictwssij.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/ggolxrzqk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/ghxbqfyic.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.vehdjk.com/Article/details/goveetcyd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gwwglzzui.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gpnwiujmm.sHtML


<!-- 参考信息 -->