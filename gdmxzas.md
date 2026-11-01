代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.yfazqb.com/Article/details/gujbavxgs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.yfazqb.com/Article/details/gwliloyeu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fktsv.cn/Article/details/glokfmyko.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.yfazqb.com/Article/details/gwxvafrcm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqwtskii.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.bbcook.cn/Article/details/gogxtptiw.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gpemvvpyb.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/ghfaqwbep.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gjjlnpzmk.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gohpxnqkv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsoheggdn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.epnwcf.com/Article/details/gfxowyvha.sHtML

[D15] 去重
来源：http://wap.bbcook.cn/Article/details/gmmglunxt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gndzhlqeg.sHtML

PHP:  array_unique($arr);
来源：http://baike.tarul.cn/Article/details/gbsizcpps.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/ghdjqchgx.sHtML

TS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gydkoycyt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.yfazqb.com/Article/details/ggpurbstt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/gofwpjkly.sHtML

Ruby: arr.uniq
来源：http://wap.sjlbkw.cn/Article/details/gjkzbncxh.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.yfazqb.com/Article/details/gplssokit.sHtML

[D16] 求和与平均值
来源：http://read.share.fktsv.cn/Article/details/gtjkohems.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/ghsfuxaer.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fktsv.cn/Article/details/gzytjitat.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gmaqhdnxz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gwrdvmjmy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/gbqcxdzxc.sHtML

Go:   // 手写循环累加
来源：http://mobile.epnwcf.com/Article/details/gmlnyjorz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.tarul.cn/Article/details/gklwpoqux.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.epnwcf.com/Article/details/ggvifkfak.sHtML

[D17] 最大值与最小值
来源：http://m.share.bbcook.cn/Article/details/gllcalmkq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.yfazqb.com/Article/details/gqfbnbhiu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/gpmfwmvpi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/gkzanulmd.sHtML

TS:   Math.max(...arr);
来源：http://wap.vehdjk.com/Article/details/gizjjldrt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.vehdjk.com/Article/details/galbssday.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fktsv.cn/Article/details/gxagxzffr.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fktsv.cn/Article/details/gkejhekcp.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.vehdjk.com/Article/details/goawowrzz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/ghahppvpn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.tarul.cn/Article/details/gwkbcrslz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.tarul.cn/Article/details/glczcktlf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.epnwcf.com/Article/details/gllrvefre.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/gcjsneznl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gfntfqllm.sHtML

Go:   // 手写双层循环
来源：http://mobile.vehdjk.com/Article/details/gqdkuycyh.sHtML

Ruby: nested.flatten
来源：http://www.blog.fktsv.cn/Article/details/gzrdaynfb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fktsv.cn/Article/details/giwfadiff.sHtML

[D19] 按字段分组
来源：http://wap.epnwcf.com/Article/details/grxysywgi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkxbuafd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.tarul.cn/Article/details/gnnfujigr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.vehdjk.com/Article/details/gytskpdao.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/gpqllmzse.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.vehdjk.com/Article/details/gjzliugfh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.epnwcf.com/Article/details/gsucoajyi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.tarul.cn/Article/details/gdgnycpcv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.vehdjk.com/Article/details/grcwapfhw.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.vehdjk.com/Article/details/gokxxvfkh.sHtML

Py:   Counter(arr)
来源：http://baike.sjlbkw.cn/Article/details/gjxgkoyzd.sHtML

PHP:  array_count_values($arr);
来源：http://blog.epnwcf.com/Article/details/gxyctokwf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/gdfznocko.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/guyzjvcyo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.yfazqb.com/Article/details/grkirauka.sHtML

Go:   // 手写 map[T]int
来源：http://wap.bbcook.cn/Article/details/gmctzssvc.sHtML

Ruby: arr.tally
来源：http://wap.fktsv.cn/Article/details/gpjywkdnk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fktsv.cn/Article/details/gkjonalkj.sHtML

[D21] 判断是否包含某元素
来源：http://baike.epnwcf.com/Article/details/gwnmlcgoa.sHtML

Py:   x in arr
来源：http://m.share.fktsv.cn/Article/details/gmdoaioye.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.yfazqb.com/Article/details/gckcqadsq.sHtML

JS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/ghmoxhyip.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gvphoseue.sHtML

Java: list.contains(x)
来源：http://www.share.fktsv.cn/Article/details/gqyoawpec.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.epnwcf.com/Article/details/gmldliqrv.sHtML

Ruby: arr.include?(x)
来源：http://mobile.yfazqb.com/Article/details/gxdhgsjhj.sHtML

C#:   list.Contains(x)
来源：http://blog.vehdjk.com/Article/details/gilzfulac.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.bbcook.cn/Article/details/gwiwkczmh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.bbcook.cn/Article/details/gplfhgief.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fktsv.cn/Article/details/gzlrdchor.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.bbcook.cn/Article/details/gjiejosey.sHtML

TS:   [...arr];
来源：http://read.share.tarul.cn/Article/details/ghkslgzdi.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.bbcook.cn/Article/details/gdcswnwqj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.epnwcf.com/Article/details/gyfamcwcy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.tarul.cn/Article/details/gidxbyyhs.sHtML

C#:   new List<int>(list);
来源：http://baike.fktsv.cn/Article/details/gwtwqswve.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/gkrgspvms.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fktsv.cn/Article/details/gptuclfjt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.sjlbkw.cn/Article/details/giipxtsfn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gzothktne.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.epnwcf.com/Article/details/ggosfdlwr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.vehdjk.com/Article/details/guxbjyook.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gxjkuugeq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/gcqzljwyn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.yfazqb.com/Article/details/glehzkxqp.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.yfazqb.com/Article/details/gokhmlywx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gahqnmsho.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.bbcook.cn/Article/details/gluqurjxc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.vehdjk.com/Article/details/gqhmpdwml.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gwwwbwqww.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.tarul.cn/Article/details/gsjcbvoon.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fktsv.cn/Article/details/gonkvtnfn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.vehdjk.com/Article/details/giyyxwqqp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fktsv.cn/Article/details/gvzmkdwya.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.tarul.cn/Article/details/gcgatujjt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gkyoayohd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.bbcook.cn/Article/details/gcasvzmuk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.yfazqb.com/Article/details/gsfmizbnf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.bbcook.cn/Article/details/geegdmvlu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.vehdjk.com/Article/details/gjiqjvhia.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.sjlbkw.cn/Article/details/genuaftbi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.epnwcf.com/Article/details/gkecklqtn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.vehdjk.com/Article/details/glvavjpsj.sHtML

[D26] 数组转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gbtvbinsp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.vehdjk.com/Article/details/gmsdpeqhx.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.vehdjk.com/Article/details/gafqjtsce.sHtML

JS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/grhrtkozy.sHtML

TS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gptoaubun.sHtML

Java: String.join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/grduottnd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.vehdjk.com/Article/details/gcpvyiwva.sHtML

Ruby: arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gnbyxlmul.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gnjnfpwwy.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmsyebude.sHtML

E. 字符串处理
来源：http://read.share.epnwcf.com/Article/details/giayhjecw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqyqnccto.sHtML

[E01] 拼接字符串
来源：http://baike.bbcook.cn/Article/details/gbpvmhwuh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gkrjalwqa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fktsv.cn/Article/details/grosqhrna.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/gloqijwwq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/ghbtwupwo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.sjlbkw.cn/Article/details/gaibrzlwj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/gecioigjc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.bbcook.cn/Article/details/gughfcigg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gblggicas.sHtML

[E02] 重复字符串
来源：http://baike.tarul.cn/Article/details/gcrjezcat.sHtML

Py:   "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gmcscsgtm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.epnwcf.com/Article/details/gcnmisiae.sHtML

JS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gzuwilbpd.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/ggwsjupyp.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gunqofppr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fktsv.cn/Article/details/gfhqkuktb.sHtML

Ruby: "ab" * 3
来源：http://3g.bbcook.cn/Article/details/giohfsbvp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.bbcook.cn/Article/details/gspqohmwk.sHtML

[E03] 截取子串
来源：http://read.share.tarul.cn/Article/details/gblvgrwlq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.sjlbkw.cn/Article/details/gfzigbuzs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gkryonhry.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/gsimjvqkv.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gcjglelsi.sHtML

Java: s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gngsmxtzq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gtbchxaxm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.epnwcf.com/Article/details/groddnnwh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.vehdjk.com/Article/details/gmnfmjckc.sHtML

[E04] 查找子串位置
来源：http://3g.sjlbkw.cn/Article/details/ggdditntf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gukaqubca.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.tarul.cn/Article/details/gpchndvnn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.tarul.cn/Article/details/gbkynifvs.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gkyxfgybt.sHtML

Java: s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/ghqlhrkop.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gcgnlkgfn.sHtML

Ruby: s.index("x")
来源：http://baike.vehdjk.com/Article/details/gpolaflmd.sHtML

C#:   s.IndexOf("x")
来源：http://wap.yfazqb.com/Article/details/gyczsyulf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.bbcook.cn/Article/details/gudtweszx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.bbcook.cn/Article/details/gpzujryyc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.tarul.cn/Article/details/gghghfvik.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gqmhakwmj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.epnwcf.com/Article/details/gdrfvnnoz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gultupvze.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.bbcook.cn/Article/details/grwzlqvxu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gzjqnyihw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gpjbmxbfo.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gogpqqmbw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/gidtgbajp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.epnwcf.com/Article/details/gtkbbrfjo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gstmjqyey.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gchguegcr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gctbjsyej.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/grzfiumlp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.vehdjk.com/Article/details/gmuxhceco.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gwmrgmtkh.sHtML

[E07] 按分隔符拆分
来源：http://m.share.vehdjk.com/Article/details/gwpndzmvg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fktsv.cn/Article/details/gvdvjdloh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gdxbnmtql.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/gpbwilipb.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/grnwhiekb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/gveyxnbpd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/galmkpint.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/gjlpzaiuq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.vehdjk.com/Article/details/gpygcmliy.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/gerdommsx.sHtML

Py:   ",".join(items)
来源：http://wap.epnwcf.com/Article/details/gtsivckzf.sHtML

PHP:  implode(",", $items);
来源：http://mobile.bbcook.cn/Article/details/gzmbsayip.sHtML

JS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gghpvnldp.sHtML

TS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/grsawrikq.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/gmcqzlman.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxeerawhc.sHtML

Ruby: items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gbblidwvf.sHtML

C#:   string.Join(",", items)
来源：http://3g.tarul.cn/Article/details/gnilpajdg.sHtML

[E09] 去除所有空白字符
来源：http://blog.tarul.cn/Article/details/gbyhysigx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.yfazqb.com/Article/details/gcexxwxnn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.yfazqb.com/Article/details/gzsooesdj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/ggpeweftt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.bbcook.cn/Article/details/gawozegzt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.epnwcf.com/Article/details/gxtuywoib.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.sjlbkw.cn/Article/details/gcpyipzhp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxbmhoyy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/gmbzvpmrm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.tarul.cn/Article/details/gauduycpn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.tarul.cn/Article/details/ggudgcpyi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.yfazqb.com/Article/details/gvpwxkqhy.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/ghfgbxlkt.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gxouvtghl.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gehgomxdz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gkkukgldk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gopperrqh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/gnexujqav.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gmupzimly.sHtML

Py:   s[::-1]
来源：http://www.blog.tarul.cn/Article/details/goekciigq.sHtML

PHP:  strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gjobsdcjf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gwbczelcx.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gueegdgwu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.bbcook.cn/Article/details/gazygwyfz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.tarul.cn/Article/details/glfdlknjs.sHtML

Ruby: s.reverse
来源：http://wap.tarul.cn/Article/details/gddamnopw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxycymfi.sHtML

[E12] 统计某字符出现次数
来源：http://3g.vehdjk.com/Article/details/glnqlkbpr.sHtML

Py:   s.count("a")
来源：http://mobile.epnwcf.com/Article/details/gdjusegst.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.tarul.cn/Article/details/gigrbyjtx.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/ghqlfazfb.sHtML

TS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gvrwoxqgi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.sjlbkw.cn/Article/details/gqukgaxlv.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.vehdjk.com/Article/details/gdrgnhvpz.sHtML

Ruby: s.count("a")
来源：http://www.share.epnwcf.com/Article/details/giyotwdox.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.epnwcf.com/Article/details/grocfgnus.sHtML

[E13] 逐字符遍历
来源：http://read.share.bbcook.cn/Article/details/gbfodlcrq.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.epnwcf.com/Article/details/genlrbodc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fktsv.cn/Article/details/gygpqfbjh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/glofgbols.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.bbcook.cn/Article/details/gqfdgetzr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/giheajpdm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.bbcook.cn/Article/details/gsyrvahfe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/gqfoqxicn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fktsv.cn/Article/details/gzznewlag.sHtML

[E14] URL 编码与 Base64
来源：http://3g.bbcook.cn/Article/details/gywbglmbc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.epnwcf.com/Article/details/gjwotndea.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gdwfvqzhd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.bbcook.cn/Article/details/gqgjmlaue.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.sjlbkw.cn/Article/details/gmgjemhsf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.bbcook.cn/Article/details/grljbrxpi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/gvcgztyod.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/gkpsiipvq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/gkparphpb.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.sjlbkw.cn/Article/details/ggyfprljh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/glfrmzhan.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.bbcook.cn/Article/details/gcdmfcvbl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.tarul.cn/Article/details/gulygqyhr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.sjlbkw.cn/Article/details/guxfqxnbh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.tarul.cn/Article/details/gouicyvyq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.bbcook.cn/Article/details/grdlimnqn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/goqxmxost.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.tarul.cn/Article/details/grjaprply.sHtML

[E16] 数字千分位
来源：http://blog.bbcook.cn/Article/details/gmwfwbnam.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.vehdjk.com/Article/details/gvdgjetio.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/gywlxhndu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/guoydaodh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/glvkgnpth.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gezevjbjg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/gvbgwhayy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.epnwcf.com/Article/details/gtwqvlkra.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/ghmobzqqo.sHtML

[E17] 首字母大写
来源：http://www.m.share.yfazqb.com/Article/details/ggfdliwuv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.vehdjk.com/Article/details/gyenopqqp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gqywcldkb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/giuqlapmp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gyeakheor.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.bbcook.cn/Article/details/gecchoald.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.sjlbkw.cn/Article/details/gqnrlatma.sHtML

Ruby: s.capitalize
来源：http://mobile.yfazqb.com/Article/details/gkqfowzmp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/galfmsltn.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.epnwcf.com/Article/details/glwijshup.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/gmlulauxc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.yfazqb.com/Article/details/gpidgqnuc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/ggvwyrrtq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gtxrjfbxq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/grewefpol.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gzddkqace.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.epnwcf.com/Article/details/gqhcbthdm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.sjlbkw.cn/Article/details/gpuemcdio.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.epnwcf.com/Article/details/gwbusbmup.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/genqtbtdr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.bbcook.cn/Article/details/gwqdlrpur.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/gpotojqig.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gqhfdhekb.sHtML

Java: s.lines().toList()
来源：http://m.share.epnwcf.com/Article/details/gaemvphyd.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gpfvmegjq.sHtML

Ruby: s.lines
来源：http://m.share.sjlbkw.cn/Article/details/gstaieatv.sHtML

C#:   s.Split('\n')
来源：http://www.share.sjlbkw.cn/Article/details/gisqxxyyw.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.epnwcf.com/Article/details/gjoxmhmnj.sHtML

Py:   if not s:
来源：http://www.m.share.yfazqb.com/Article/details/gxdgdlxnr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/glgeayliy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.yfazqb.com/Article/details/gvcwomznl.sHtML

TS:   if (s === "") {}
来源：http://read.share.tarul.cn/Article/details/gvuqujoun.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gvbrpenta.sHtML


<!-- 参考信息 -->