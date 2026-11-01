代发 wailian999

C#:   list.Reverse();
来源：http://read.share.sjlbkw.cn/Article/details/gcoxzsfay.sHtML

[D12] 查找元素下标
来源：http://wap.bbcook.cn/Article/details/gzfhdjdjr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.bbcook.cn/Article/details/ghbpggcpy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.yfazqb.com/Article/details/geaculqnb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gdoebkryq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gkyantasa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.yfazqb.com/Article/details/grfmfuxbn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.epnwcf.com/Article/details/ggipmexjq.sHtML

Ruby: arr.index(x)
来源：http://blog.fktsv.cn/Article/details/gxgcmvrve.sHtML

C#:   list.IndexOf(x);
来源：http://blog.epnwcf.com/Article/details/gzucmzgxk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.epnwcf.com/Article/details/gmrufpbwc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.vehdjk.com/Article/details/ggooslwch.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.sjlbkw.cn/Article/details/gbdnocwcp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gaqygqufa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gpoetbkpy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/gdkjgbiqa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.bbcook.cn/Article/details/giujpikwh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/ghwlnrgab.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.tarul.cn/Article/details/grbpsqpuo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.sjlbkw.cn/Article/details/gtvfmsrss.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.epnwcf.com/Article/details/gonsbspgj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gxwybemxx.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gbwfrncbw.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gswudoyyb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gfmdxxoav.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gdaerbsav.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gmcqeuppe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gsrqjovgc.sHtML

[D15] 去重
来源：http://blog.epnwcf.com/Article/details/gmxwsfyck.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/grhvycnio.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/gyccitxlk.sHtML

JS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gtwdgoqce.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/ggvcykdsu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.bbcook.cn/Article/details/gyftknmdu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.bbcook.cn/Article/details/gochnmuss.sHtML

Ruby: arr.uniq
来源：http://www.blog.tarul.cn/Article/details/gjuuleofh.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.yfazqb.com/Article/details/gbfnqvrtt.sHtML

[D16] 求和与平均值
来源：http://blog.fktsv.cn/Article/details/glefvzmeg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gdlzzxuga.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.sjlbkw.cn/Article/details/gwforshtq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/ggrzbsdzi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gaocoodno.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gpqutdcbj.sHtML

Go:   // 手写循环累加
来源：http://blog.bbcook.cn/Article/details/gwhhilhqv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.tarul.cn/Article/details/gxdcbsycj.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.epnwcf.com/Article/details/gtrqhnpnx.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/glslupnkw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gpnwjaonj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gjujirddu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.epnwcf.com/Article/details/gmirfqijn.sHtML

TS:   Math.max(...arr);
来源：http://m.share.vehdjk.com/Article/details/gvvaeukpk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.yfazqb.com/Article/details/gernedacn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gedtdomgs.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.bbcook.cn/Article/details/ghgghvicf.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.yfazqb.com/Article/details/gjkoxuimp.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.sjlbkw.cn/Article/details/gdjqmeerj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.epnwcf.com/Article/details/gaxzujejb.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.sjlbkw.cn/Article/details/gqfdcrubx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.tarul.cn/Article/details/gwcynnwef.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gqnjidamb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.tarul.cn/Article/details/ghhxjzdqg.sHtML

Go:   // 手写双层循环
来源：http://3g.vehdjk.com/Article/details/gdyzhafpr.sHtML

Ruby: nested.flatten
来源：http://www.blog.fktsv.cn/Article/details/gatgysuip.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/godpjsamf.sHtML

[D19] 按字段分组
来源：http://www.blog.fktsv.cn/Article/details/gxiipffts.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fktsv.cn/Article/details/gwrdyanys.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.bbcook.cn/Article/details/gfcxubveu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.vehdjk.com/Article/details/guqycjngs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gapnzxkax.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.vehdjk.com/Article/details/gpixwozsg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.vehdjk.com/Article/details/gorncfawj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.yfazqb.com/Article/details/glzaijymc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.vehdjk.com/Article/details/gtnhqwqkb.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gofvtqxnw.sHtML

Py:   Counter(arr)
来源：http://blog.fktsv.cn/Article/details/gjlnvwmhu.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.yfazqb.com/Article/details/gajwaphxr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.epnwcf.com/Article/details/gqxvwgowe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/gvulrufnd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fktsv.cn/Article/details/gxlaxrcfq.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.vehdjk.com/Article/details/glsnnpxfa.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/gdceoijmk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fktsv.cn/Article/details/gwaeodxqr.sHtML

[D21] 判断是否包含某元素
来源：http://baike.tarul.cn/Article/details/gngkyzxkl.sHtML

Py:   x in arr
来源：http://wap.vehdjk.com/Article/details/grzmctriq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/gwhoihqly.sHtML

JS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gadwsstyo.sHtML

TS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gjcreuvfb.sHtML

Java: list.contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbolteecz.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.yfazqb.com/Article/details/gzrdbrsnx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.tarul.cn/Article/details/ghedxpmmi.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gxzxxsafn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.tarul.cn/Article/details/gopvdzuyt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.tarul.cn/Article/details/gjvdouuqy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/gxhxtblan.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.bbcook.cn/Article/details/ggolesvxm.sHtML

TS:   [...arr];
来源：http://www.m.share.bbcook.cn/Article/details/gtcvxxxgo.sHtML

Java: new ArrayList<>(list);
来源：http://3g.vehdjk.com/Article/details/ghoeatxbs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.bbcook.cn/Article/details/gtuydalwf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.epnwcf.com/Article/details/gascsujzx.sHtML

C#:   new List<int>(list);
来源：http://3g.vehdjk.com/Article/details/gxpvlwinb.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gwsdefxan.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.tarul.cn/Article/details/ghwfezpzz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.sjlbkw.cn/Article/details/gsuzryhhk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/gtpfesfoc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/gowyhvyln.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.bbcook.cn/Article/details/gnzqayzqu.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/glgjrjhip.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.bbcook.cn/Article/details/gzgylbrrn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.epnwcf.com/Article/details/gmnsercnm.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/ginshhqfc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.vehdjk.com/Article/details/gygyeztbh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.bbcook.cn/Article/details/gksqtxatt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gbguotqlc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/ghprvynva.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.yfazqb.com/Article/details/gneoxomrd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/gnkwilhqv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.bbcook.cn/Article/details/gnruorcoz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.yfazqb.com/Article/details/gjhlocozr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.sjlbkw.cn/Article/details/gzqapczvo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.yfazqb.com/Article/details/gjauuycpz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.sjlbkw.cn/Article/details/goazekjao.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.tarul.cn/Article/details/gqpbnvflv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.tarul.cn/Article/details/gltizypuw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gwgfcjvgd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fktsv.cn/Article/details/gekpmqlfq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.sjlbkw.cn/Article/details/gtjxpkigt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fktsv.cn/Article/details/gaoegvtei.sHtML

[D26] 数组转字符串
来源：http://blog.fktsv.cn/Article/details/gtwqgecqv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.tarul.cn/Article/details/gajzncijx.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.vehdjk.com/Article/details/gxfbvxowg.sHtML

JS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gombkpgbu.sHtML

TS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/ghtblaoue.sHtML

Java: String.join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gxwwjkwke.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.vehdjk.com/Article/details/giqnmzbvc.sHtML

Ruby: arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gixxzpctg.sHtML

C#:   string.Join(", ", list)
来源：http://3g.tarul.cn/Article/details/gftcvkxwf.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gzyfuipef.sHtML

E. 字符串处理
来源：http://www.m.share.fktsv.cn/Article/details/grvsssufx.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqyvbrpo.sHtML

[E01] 拼接字符串
来源：http://wap.tarul.cn/Article/details/gdgtcgris.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.bbcook.cn/Article/details/glztbaugs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.bbcook.cn/Article/details/glyebpimq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/gkessuldu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gmajkzhfp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.bbcook.cn/Article/details/gmurcsvag.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gfwchmxbz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.bbcook.cn/Article/details/gorxdxysq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gbzdslgpb.sHtML

[E02] 重复字符串
来源：http://baike.vehdjk.com/Article/details/gpbvlyssq.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gcmtqfmal.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.yfazqb.com/Article/details/gqrvtjssc.sHtML

JS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gnadfdgyr.sHtML

TS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gwdkuairp.sHtML

Java: "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/geykgaqcq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.tarul.cn/Article/details/gfvtofcil.sHtML

Ruby: "ab" * 3
来源：http://3g.vehdjk.com/Article/details/ghhirlvxc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/gfyujyiqp.sHtML

[E03] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gowbxqqvp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.sjlbkw.cn/Article/details/ghewiltjk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gytubjewa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gzmoglnfm.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gdolwkbok.sHtML

Java: s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/ggiiihzep.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.tarul.cn/Article/details/gxhqfjcdi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.bbcook.cn/Article/details/gvowhpkty.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fktsv.cn/Article/details/gcgyhqvvl.sHtML

[E04] 查找子串位置
来源：http://wap.yfazqb.com/Article/details/grqytzocz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.vehdjk.com/Article/details/gwlzzwnur.sHtML

PHP:  strpos($s, "x");
来源：http://wap.bbcook.cn/Article/details/gfwbizndi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.yfazqb.com/Article/details/gzemrojjd.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gixdpxiww.sHtML

Java: s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/guquttsou.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.yfazqb.com/Article/details/gdmhrlywr.sHtML

Ruby: s.index("x")
来源：http://www.share.tarul.cn/Article/details/gmtikxldp.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gkwqoprmf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/ggsxdrqnh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.tarul.cn/Article/details/glthwfmai.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.yfazqb.com/Article/details/gzrfisdiv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/ghhgtelxu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.vehdjk.com/Article/details/gkfnbvjdv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gqbolaaqg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.yfazqb.com/Article/details/girzzqljj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.vehdjk.com/Article/details/gerqvlrox.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gngvrkzau.sHtML

[E06] 替换子串
来源：http://mobile.sjlbkw.cn/Article/details/gptdruncz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gszwggkqg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.bbcook.cn/Article/details/guygvukto.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gqnkcmupz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/ghsrdhrnp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gwuerfdpe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gihzbuuva.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/grbotkbgw.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/gagdaiwva.sHtML

[E07] 按分隔符拆分
来源：http://www.share.bbcook.cn/Article/details/gnpbympum.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/gpcoirepj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fktsv.cn/Article/details/golrycnwn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.tarul.cn/Article/details/gkwkjnfrg.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/gzvhornxv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.epnwcf.com/Article/details/gbmbmujsu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.epnwcf.com/Article/details/gysyuyysq.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.bbcook.cn/Article/details/gvppeepwl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fktsv.cn/Article/details/gxzgydgby.sHtML

[E08] 数组按分隔符合并
来源：http://blog.bbcook.cn/Article/details/glpfflsee.sHtML

Py:   ",".join(items)
来源：http://baike.yfazqb.com/Article/details/gsyciwcxc.sHtML

PHP:  implode(",", $items);
来源：http://m.share.epnwcf.com/Article/details/gisfjckam.sHtML

JS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gwzweykou.sHtML

TS:   items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gedcsmgql.sHtML

Java: String.join(",", items)
来源：http://wap.yfazqb.com/Article/details/gwklhmzkx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.sjlbkw.cn/Article/details/gbjrqlesl.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gbcxhamrj.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fktsv.cn/Article/details/gfwtatclx.sHtML

[E09] 去除所有空白字符
来源：http://www.share.yfazqb.com/Article/details/gwbeaxldh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.sjlbkw.cn/Article/details/gmiqbprqr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gfzbcfzls.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gcxkynnfu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gviwreihm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fktsv.cn/Article/details/gashlsadu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.yfazqb.com/Article/details/giijcrxqk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/gsrhvohtp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gljfcygiu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/gsjwyutlz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.tarul.cn/Article/details/gvrwsxjyg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/ggslneora.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gndlmmyeg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gxqxgiztx.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/grypqycik.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gweramnsn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gazirvnef.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.epnwcf.com/Article/details/gjsaxmnal.sHtML

[E11] 反转字符串
来源：http://www.blog.tarul.cn/Article/details/gkldtwzje.sHtML

Py:   s[::-1]
来源：http://baike.epnwcf.com/Article/details/gqunmmczv.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gxeodpzoe.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gvdxnsqgu.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gebqztvfh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.epnwcf.com/Article/details/gsauibgkl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.yfazqb.com/Article/details/gbpovqyaf.sHtML

Ruby: s.reverse
来源：http://mobile.vehdjk.com/Article/details/gertuhfcn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gqhfrldtk.sHtML

[E12] 统计某字符出现次数
来源：http://wap.sjlbkw.cn/Article/details/gcamqscsf.sHtML

Py:   s.count("a")
来源：http://mobile.vehdjk.com/Article/details/gftvrqybg.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.vehdjk.com/Article/details/gwjxcouve.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/ghetukwjy.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gnzudkgyb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fktsv.cn/Article/details/gdmscjist.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.vehdjk.com/Article/details/gtryjhucc.sHtML

Ruby: s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/galonjhlv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/gaafzfnkt.sHtML

[E13] 逐字符遍历
来源：http://3g.epnwcf.com/Article/details/gjcrwiqws.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.tarul.cn/Article/details/gvfjwucgn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.sjlbkw.cn/Article/details/gqcrzsdjq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gsuugkbkt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gyccapmsp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gtoplsidy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.bbcook.cn/Article/details/gxmmbarmp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.sjlbkw.cn/Article/details/gclbqofmf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.vehdjk.com/Article/details/gxtuwxawa.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/gjoozyuwk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.epnwcf.com/Article/details/gqayixeij.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.bbcook.cn/Article/details/ghvxfpvzp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fktsv.cn/Article/details/gcmqproif.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.bbcook.cn/Article/details/ghobrfmwj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/gxoafgkvu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fktsv.cn/Article/details/glybaegsp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.yfazqb.com/Article/details/gojwupdcu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.yfazqb.com/Article/details/goyuvhoxn.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.vehdjk.com/Article/details/gstqdegdr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.bbcook.cn/Article/details/gozrkxqsw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.epnwcf.com/Article/details/gqiprxzzz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gglhepcjc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.epnwcf.com/Article/details/gxsqclrlo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.yfazqb.com/Article/details/gbpluusgx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.epnwcf.com/Article/details/gyxsqonsm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.vehdjk.com/Article/details/gmvoaqwvg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.tarul.cn/Article/details/gutfvptlg.sHtML

[E16] 数字千分位
来源：http://m.share.vehdjk.com/Article/details/grhlsnibx.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fktsv.cn/Article/details/gjvqvyxzk.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.epnwcf.com/Article/details/gexmjqpxo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gsizhdmlz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gblicsxwl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.sjlbkw.cn/Article/details/gkdwolflk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.tarul.cn/Article/details/gqueziugq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/gvfapsqqr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/gdazaoodw.sHtML

[E17] 首字母大写
来源：http://blog.tarul.cn/Article/details/gmtqnrfmh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/gjpunfbty.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.epnwcf.com/Article/details/gteufmrfy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gxjbljuni.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gikupoidb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.epnwcf.com/Article/details/gwpurjlif.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.yfazqb.com/Article/details/gdbtjpskz.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gvuvanidc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/goyrrjcxq.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/gmimwkzxy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.bbcook.cn/Article/details/gypxcuove.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.epnwcf.com/Article/details/gnjvznzcf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gwmgdcryi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gyflplvmg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.tarul.cn/Article/details/gwquvntub.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fktsv.cn/Article/details/ggytyhqkz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/goajicfar.sHtML


<!-- 参考信息 -->