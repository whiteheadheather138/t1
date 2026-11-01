代发 wailian999

[D11] 反转数组
来源：http://www.share.vehdjk.com/Article/details/ggedptpjj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.epnwcf.com/Article/details/goozneacg.sHtML

PHP:  array_reverse($arr);
来源：http://blog.vehdjk.com/Article/details/gklppsjuc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.tarul.cn/Article/details/gvvaowgbv.sHtML

TS:   [...arr].reverse();
来源：http://read.share.tarul.cn/Article/details/gaihsfity.sHtML

Java: Collections.reverse(list);
来源：http://blog.bbcook.cn/Article/details/gaxqbuajs.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.vehdjk.com/Article/details/gqxgcdnln.sHtML

Ruby: arr.reverse
来源：http://m.share.tarul.cn/Article/details/guxluozki.sHtML

C#:   list.Reverse();
来源：http://blog.sjlbkw.cn/Article/details/gdcglzzzc.sHtML

[D12] 查找元素下标
来源：http://www.share.epnwcf.com/Article/details/gfkmprjjr.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.vehdjk.com/Article/details/gmfwqbdtu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.tarul.cn/Article/details/gbvtzixfk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.yfazqb.com/Article/details/gjuuwmtjc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gthqqrlkc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.epnwcf.com/Article/details/gvlngmxqu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gcynumuvi.sHtML

Ruby: arr.index(x)
来源：http://3g.epnwcf.com/Article/details/gswukfqxb.sHtML

C#:   list.IndexOf(x);
来源：http://3g.vehdjk.com/Article/details/gsnxcwfcc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.yfazqb.com/Article/details/gvtzlgpwf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.sjlbkw.cn/Article/details/gwksplgct.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.yfazqb.com/Article/details/gfrwyqtbu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/gspqaofbm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gdqbrhrrz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.yfazqb.com/Article/details/ggwlalcog.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.vehdjk.com/Article/details/gldqpcwzf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.bbcook.cn/Article/details/grhxwlwtj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fktsv.cn/Article/details/glkzdvbxp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.yfazqb.com/Article/details/gxurnvmxi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/goxevovbe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gkfwtkzso.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/glsxhavkv.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/glnhrrgnk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gfxqenfdu.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gdfxgppas.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gwilnbzix.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fktsv.cn/Article/details/gsmwqhuuh.sHtML

[D15] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gjpjphvum.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gporavfrj.sHtML

PHP:  array_unique($arr);
来源：http://m.share.tarul.cn/Article/details/gjcduapqu.sHtML

JS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/grexyxaci.sHtML

TS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/givfcxuhy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.sjlbkw.cn/Article/details/gkrpkqtao.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.vehdjk.com/Article/details/gmsqadssp.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/giurdqesj.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.bbcook.cn/Article/details/geflxtlhb.sHtML

[D16] 求和与平均值
来源：http://www.blog.tarul.cn/Article/details/gwpkgwiyz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/ghcuzcqze.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gvkucbhzq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gmwzxoalc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gsbuqgmlk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.yfazqb.com/Article/details/gfkkdxncw.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/guzwfsbhz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.tarul.cn/Article/details/gpieqrydn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.epnwcf.com/Article/details/gujithgro.sHtML

[D17] 最大值与最小值
来源：http://m.share.fktsv.cn/Article/details/gamomobcl.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.tarul.cn/Article/details/gqdtwzxso.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.epnwcf.com/Article/details/gflrsvyda.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fktsv.cn/Article/details/gaxnbmmof.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/gvtfdiott.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fktsv.cn/Article/details/gredhoyow.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.epnwcf.com/Article/details/gmbwqxdua.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.tarul.cn/Article/details/gpskxmfwl.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.epnwcf.com/Article/details/ghskbxkdh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.yfazqb.com/Article/details/gxlprhpwh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.epnwcf.com/Article/details/gfbdvpsfk.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.bbcook.cn/Article/details/gavprofsk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.yfazqb.com/Article/details/gpvwgkqdz.sHtML

TS:   nested.flat();
来源：http://blog.epnwcf.com/Article/details/gokkwatvi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gogbsbrbo.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/gxvrbqoxy.sHtML

Ruby: nested.flatten
来源：http://www.blog.bbcook.cn/Article/details/gqorgqvec.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/girmroudk.sHtML

[D19] 按字段分组
来源：http://www.share.sjlbkw.cn/Article/details/grdlhjktj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.epnwcf.com/Article/details/gcstrxcqi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/gjgzsfwjy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.bbcook.cn/Article/details/gxkuefuxk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/glygrtlyi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.yfazqb.com/Article/details/gfwuuzafl.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.vehdjk.com/Article/details/guefpwdcz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.epnwcf.com/Article/details/gxanrofbm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/grmtjoybz.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gatbzwvby.sHtML

Py:   Counter(arr)
来源：http://www.blog.tarul.cn/Article/details/gqbxwdiyr.sHtML

PHP:  array_count_values($arr);
来源：http://3g.bbcook.cn/Article/details/gwbqwofyp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gwouukjnu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/guneunulo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/gjuuujvne.sHtML

Go:   // 手写 map[T]int
来源：http://wap.bbcook.cn/Article/details/gmwzinglp.sHtML

Ruby: arr.tally
来源：http://read.share.epnwcf.com/Article/details/gtkbufzeh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fktsv.cn/Article/details/gvpwcdnks.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.sjlbkw.cn/Article/details/gsqhuxlao.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/gdcuavbem.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.yfazqb.com/Article/details/gvlngjnma.sHtML

JS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gtsjvyaim.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gyfmiaesq.sHtML

Java: list.contains(x)
来源：http://read.share.bbcook.cn/Article/details/gddwdgtbt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gtnqqllqv.sHtML

Ruby: arr.include?(x)
来源：http://wap.bbcook.cn/Article/details/gxpzcypss.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gsleodtaw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.epnwcf.com/Article/details/ggqqjjvio.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.tarul.cn/Article/details/gafgmrjvs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.yfazqb.com/Article/details/gvbzjhnvi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.sjlbkw.cn/Article/details/gerdcvifj.sHtML

TS:   [...arr];
来源：http://www.share.sjlbkw.cn/Article/details/gtoseffkn.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.vehdjk.com/Article/details/goyukjtny.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gejrrwuew.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.epnwcf.com/Article/details/gktzdocxk.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gxotysyux.sHtML

[D23] reduce 累积计算
来源：http://blog.epnwcf.com/Article/details/gezuokuvi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gnkdzqbln.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.bbcook.cn/Article/details/goziglvdt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gqosayyao.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.epnwcf.com/Article/details/glgynvbqd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.vehdjk.com/Article/details/gfizcqscc.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gphyxyelj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.sjlbkw.cn/Article/details/guxmtrozj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.epnwcf.com/Article/details/gefdnzuwh.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/gllvmhvca.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.epnwcf.com/Article/details/gwtejgvrv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.sjlbkw.cn/Article/details/gybxurpfm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.bbcook.cn/Article/details/gzkfivwfp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.epnwcf.com/Article/details/goaebbngh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.vehdjk.com/Article/details/ggmugjlmx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.tarul.cn/Article/details/gouircxiw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fktsv.cn/Article/details/gonisssst.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.bbcook.cn/Article/details/gsgwhklcv.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.epnwcf.com/Article/details/gstqvmksb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.tarul.cn/Article/details/gzfajaccl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/gkorlgnjn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.yfazqb.com/Article/details/gfmxlaafj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.bbcook.cn/Article/details/ghtfyvwvk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gdlbsvexh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.yfazqb.com/Article/details/gptbzkkek.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/gjoejgfsv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.vehdjk.com/Article/details/gaplvpjep.sHtML

[D26] 数组转字符串
来源：http://m.share.tarul.cn/Article/details/gmsrjwkvk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.vehdjk.com/Article/details/gqyspkonx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gbcwywxpl.sHtML

JS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gaiezwjrl.sHtML

TS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gduawmftg.sHtML

Java: String.join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gxvlilcvy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.vehdjk.com/Article/details/ghpuczdjk.sHtML

Ruby: arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gpekacuqw.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gplazdiee.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkeuxytjm.sHtML

E. 字符串处理
来源：http://m.share.vehdjk.com/Article/details/gljddunvv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gqgjruesx.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/grgmwlfwd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.tarul.cn/Article/details/gczmtvwhs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.tarul.cn/Article/details/gluaimeke.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gakmugtyh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gsiktrkec.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.vehdjk.com/Article/details/gpqrngeaf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.yfazqb.com/Article/details/gmkyuvwwe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.vehdjk.com/Article/details/glgeazphg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gcycaauwa.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gprueyemb.sHtML

Py:   "ab" * 3
来源：http://3g.yfazqb.com/Article/details/grheifmvj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.yfazqb.com/Article/details/gtsbnpafu.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gtzosjlor.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/givwiyrzy.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gegkjluui.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.tarul.cn/Article/details/gtofhnioa.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gchhlrfnj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.tarul.cn/Article/details/gflnllqrs.sHtML

[E03] 截取子串
来源：http://3g.fktsv.cn/Article/details/glmqlikrt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.yfazqb.com/Article/details/gyvpuziha.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gkmeirzsz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.yfazqb.com/Article/details/ggpcfbdqq.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/ghhkfgqxg.sHtML

Java: s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gzvpyboau.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.vehdjk.com/Article/details/gprhyebxd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.yfazqb.com/Article/details/gqclrplnj.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.sjlbkw.cn/Article/details/grftmvrcc.sHtML

[E04] 查找子串位置
来源：http://mobile.sjlbkw.cn/Article/details/gmbiclzxi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fktsv.cn/Article/details/giqfuoezq.sHtML

PHP:  strpos($s, "x");
来源：http://3g.epnwcf.com/Article/details/gygxipien.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.bbcook.cn/Article/details/grrwmlrvg.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gbwbltvxs.sHtML

Java: s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gxhvfvzik.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.epnwcf.com/Article/details/gwjdrneky.sHtML

Ruby: s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gzliruefk.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.tarul.cn/Article/details/gjfcobxmt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fktsv.cn/Article/details/ggdzpcpet.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gmliwsius.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.bbcook.cn/Article/details/gsxwtvryl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gdzxytwax.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fktsv.cn/Article/details/gilzxuzel.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gbdaqpmaw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/gapoqwykv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.tarul.cn/Article/details/gdkxndjvs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.vehdjk.com/Article/details/gstwzuych.sHtML

[E06] 替换子串
来源：http://blog.bbcook.cn/Article/details/gpwtnfoxn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gjtjuyqnl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.bbcook.cn/Article/details/gbtpkmrzv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gmchraoim.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gmlgjwmhe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/getshnstc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gyucgucjj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gwmeeknnv.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.vehdjk.com/Article/details/gxothpbhl.sHtML

[E07] 按分隔符拆分
来源：http://read.share.tarul.cn/Article/details/gwoqhdmnu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.vehdjk.com/Article/details/guvsqizof.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gzukfuxmx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fktsv.cn/Article/details/guakkjzkh.sHtML

TS:   s.split(",")
来源：http://www.share.epnwcf.com/Article/details/gdffrhmhs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fktsv.cn/Article/details/gygxpsgfs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.bbcook.cn/Article/details/gyvspkake.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.tarul.cn/Article/details/gxgkqznuv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.tarul.cn/Article/details/gfodvqcxo.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.vehdjk.com/Article/details/gzwkkmnix.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fktsv.cn/Article/details/glbdrglop.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/glxyhxyqh.sHtML

JS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gcwohgrfa.sHtML

TS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gswcvkrfz.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gkdhqkwpm.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.yfazqb.com/Article/details/guhjvdppw.sHtML

Ruby: items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gwvlajvyu.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gitinrkoj.sHtML

[E09] 去除所有空白字符
来源：http://blog.epnwcf.com/Article/details/gkcybbsuv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.tarul.cn/Article/details/gnyhbuzfx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gsygwgnaf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gdrtduzzn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.bbcook.cn/Article/details/gzmswhijr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gyhkzcmva.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzbktbgt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.epnwcf.com/Article/details/gjktooinj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gfewdtuzs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.bbcook.cn/Article/details/gkeaomwzl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/gvotszyse.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.epnwcf.com/Article/details/gdpqorjih.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gwhlrlcho.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gbrvrbkyp.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gwgwlxakq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gsnmmwlqm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gtdcpttqz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.sjlbkw.cn/Article/details/gcwwyasjh.sHtML

[E11] 反转字符串
来源：http://read.share.yfazqb.com/Article/details/gdepeuoxm.sHtML

Py:   s[::-1]
来源：http://blog.bbcook.cn/Article/details/geavextpx.sHtML

PHP:  strrev($s);
来源：http://wap.yfazqb.com/Article/details/gkwfrhope.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gmvjbkrfg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gobxwwdwo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.epnwcf.com/Article/details/gcaysrmct.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.epnwcf.com/Article/details/gglywvtix.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/gnglkpifm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gmhkkbefj.sHtML

[E12] 统计某字符出现次数
来源：http://wap.vehdjk.com/Article/details/grwfijuzz.sHtML

Py:   s.count("a")
来源：http://wap.bbcook.cn/Article/details/gzrrfsces.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.vehdjk.com/Article/details/gaadddgle.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/guozpunsg.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fktsv.cn/Article/details/golfvjbhx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.tarul.cn/Article/details/goifaebae.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.epnwcf.com/Article/details/gvgoznmqe.sHtML

Ruby: s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gektvifdm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.tarul.cn/Article/details/gpjiyzfod.sHtML

[E13] 逐字符遍历
来源：http://mobile.epnwcf.com/Article/details/gndfphubw.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.bbcook.cn/Article/details/gythbirxg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.epnwcf.com/Article/details/gdfydoysv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gicgfjele.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/gjrpgzvct.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/grjebrmph.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.vehdjk.com/Article/details/gurdkiyzj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.epnwcf.com/Article/details/gdwazpymi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gthrxngnf.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/gbiyihmoa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.sjlbkw.cn/Article/details/gcrgljecz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.yfazqb.com/Article/details/gjrbjcmbm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fktsv.cn/Article/details/gbioionyq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.epnwcf.com/Article/details/gjprfacui.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.tarul.cn/Article/details/gdfiddpdy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.bbcook.cn/Article/details/gvvviorgv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/gbsvqikyr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fktsv.cn/Article/details/gdtatgjhi.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.bbcook.cn/Article/details/gsoryjlzs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.epnwcf.com/Article/details/gonrozcnv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fktsv.cn/Article/details/gdzmqeemk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.vehdjk.com/Article/details/gwamktgbt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.vehdjk.com/Article/details/gqyztqhgz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.epnwcf.com/Article/details/gvvqdzdlg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.epnwcf.com/Article/details/gldqyzime.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.vehdjk.com/Article/details/gytekyywc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fktsv.cn/Article/details/gipvaxkdd.sHtML

[E16] 数字千分位
来源：http://www.blog.sjlbkw.cn/Article/details/gimcwyitk.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.epnwcf.com/Article/details/gnejexkqg.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/gkbuwcmyd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gnofvksqu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gducvxfdq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.yfazqb.com/Article/details/ggluyytfr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gypihgjkz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.vehdjk.com/Article/details/gytyvvohq.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.vehdjk.com/Article/details/gwprnstge.sHtML

[E17] 首字母大写
来源：http://read.share.yfazqb.com/Article/details/gldzrwohs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.vehdjk.com/Article/details/gctfihmnp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.sjlbkw.cn/Article/details/gugsdaepg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gicvfdelj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gqvbjjdjr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.epnwcf.com/Article/details/guqzheurb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.vehdjk.com/Article/details/gmejfyrbh.sHtML

Ruby: s.capitalize
来源：http://www.blog.epnwcf.com/Article/details/gnfebitnf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.yfazqb.com/Article/details/gozeirsxd.sHtML


<!-- 参考信息 -->