代发 wailian999

TS:   [...arr].reverse();
来源：http://blog.tarul.cn/Article/details/gxnttmxcf.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.epnwcf.com/Article/details/gahamgwtd.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.yfazqb.com/Article/details/gtfqsbwgs.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/gvsreftuj.sHtML

C#:   list.Reverse();
来源：http://www.m.share.vehdjk.com/Article/details/ggqbhwcnb.sHtML

[D12] 查找元素下标
来源：http://3g.tarul.cn/Article/details/ggkyksrbg.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.epnwcf.com/Article/details/gawdsooki.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fktsv.cn/Article/details/gummmtfbl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.epnwcf.com/Article/details/gujotpdvu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gpbfcvlug.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.vehdjk.com/Article/details/grntrwygt.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.tarul.cn/Article/details/gjmczplrx.sHtML

Ruby: arr.index(x)
来源：http://m.share.vehdjk.com/Article/details/geeizvhdm.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.sjlbkw.cn/Article/details/gjkgfbvlq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.yfazqb.com/Article/details/gjqkvpgju.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.tarul.cn/Article/details/gnneuhmxm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.yfazqb.com/Article/details/glqqunevv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gqhtebzvm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.sjlbkw.cn/Article/details/gnfeujfet.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.yfazqb.com/Article/details/gzajmcukj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.tarul.cn/Article/details/glzqmovpf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.sjlbkw.cn/Article/details/gdylwqdkq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.vehdjk.com/Article/details/golbxmbww.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.tarul.cn/Article/details/gvpkdvytw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.vehdjk.com/Article/details/gbdsiqjix.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.vehdjk.com/Article/details/gqeoodwdq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gzzkmgyrr.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fktsv.cn/Article/details/grduxywql.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.epnwcf.com/Article/details/gfwqrzxqe.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/gkpykpkef.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.epnwcf.com/Article/details/gugcbxvhf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.epnwcf.com/Article/details/gctpqyika.sHtML

[D15] 去重
来源：http://read.share.sjlbkw.cn/Article/details/gpupbbnjx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gqppwnhib.sHtML

PHP:  array_unique($arr);
来源：http://3g.sjlbkw.cn/Article/details/gdxumqyyu.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gfpaghbze.sHtML

TS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/goqhpycnt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.bbcook.cn/Article/details/gfwnylxql.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fktsv.cn/Article/details/gvkyggrzv.sHtML

Ruby: arr.uniq
来源：http://baike.yfazqb.com/Article/details/gwzjszfgl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.yfazqb.com/Article/details/gynttydkh.sHtML

[D16] 求和与平均值
来源：http://www.m.share.bbcook.cn/Article/details/gdjzqkrgy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.yfazqb.com/Article/details/gvzrkhrfk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fktsv.cn/Article/details/gcdopsgos.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/gmegytfsw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gfgrssgci.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fktsv.cn/Article/details/ggiaaruya.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.vehdjk.com/Article/details/gmuswkxyp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.bbcook.cn/Article/details/gsnwufsni.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.yfazqb.com/Article/details/gjedafyuu.sHtML

[D17] 最大值与最小值
来源：http://read.share.epnwcf.com/Article/details/geeihptlx.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/gzjwbslnd.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gcycaabbk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/govtjxpzb.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwtxcbsx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.bbcook.cn/Article/details/gdjamgyza.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.tarul.cn/Article/details/gchwswvyd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.yfazqb.com/Article/details/gmbvxyiqm.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.vehdjk.com/Article/details/gqgvdhrwb.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.sjlbkw.cn/Article/details/gdcvzxbwx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.tarul.cn/Article/details/guhstsykk.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.sjlbkw.cn/Article/details/ghsernvbz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.tarul.cn/Article/details/gmjudyhyf.sHtML

TS:   nested.flat();
来源：http://www.share.yfazqb.com/Article/details/geqadjwwj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.vehdjk.com/Article/details/geqjehjyk.sHtML

Go:   // 手写双层循环
来源：http://3g.vehdjk.com/Article/details/gpteqcskr.sHtML

Ruby: nested.flatten
来源：http://www.blog.bbcook.cn/Article/details/gbapudtjc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.yfazqb.com/Article/details/gqwhhopco.sHtML

[D19] 按字段分组
来源：http://3g.tarul.cn/Article/details/gxtmipifg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gummkfjda.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.yfazqb.com/Article/details/gycipohjd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.epnwcf.com/Article/details/ghmrvynka.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/glsaymzyv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.yfazqb.com/Article/details/guvetwotw.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.vehdjk.com/Article/details/ggawhqnmd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.bbcook.cn/Article/details/gmjrnbjhk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.bbcook.cn/Article/details/gldnvoovk.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fktsv.cn/Article/details/gjhrkaflp.sHtML

Py:   Counter(arr)
来源：http://www.blog.tarul.cn/Article/details/gqfajeodw.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/gnacylocu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gappzmbtn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.yfazqb.com/Article/details/gwezqpfkp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.sjlbkw.cn/Article/details/gfsyqcvpv.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fktsv.cn/Article/details/gekcclaaj.sHtML

Ruby: arr.tally
来源：http://www.blog.bbcook.cn/Article/details/gbbvkhglo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.bbcook.cn/Article/details/gdeudvcue.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.yfazqb.com/Article/details/gtrafpawq.sHtML

Py:   x in arr
来源：http://read.share.vehdjk.com/Article/details/gjltdnfau.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fktsv.cn/Article/details/gjikcmwyu.sHtML

JS:   arr.includes(x)
来源：http://read.share.yfazqb.com/Article/details/gvaosyaks.sHtML

TS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gkgeoixzz.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gdgmvqkyt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gzcypjgtc.sHtML

Ruby: arr.include?(x)
来源：http://www.share.epnwcf.com/Article/details/ghfuheerw.sHtML

C#:   list.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gdwqfpcpc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.sjlbkw.cn/Article/details/gzjirppfy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.vehdjk.com/Article/details/gzaswwwjt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.epnwcf.com/Article/details/gahmlllpy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gfnvizhwh.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/gjkyivsev.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.tarul.cn/Article/details/gxqwwddqu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.yfazqb.com/Article/details/gutomzttv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/gpcrrilpy.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.tarul.cn/Article/details/gldyqmesc.sHtML

[D23] reduce 累积计算
来源：http://blog.fktsv.cn/Article/details/gtvtiyrfn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.bbcook.cn/Article/details/gbdsabkmz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gmedlknlh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gwkxifkxp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/gxcxhnyxg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/gpsqsrjwm.sHtML

Go:   // 手写循环
来源：http://m.share.sjlbkw.cn/Article/details/gzylalftg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/gznhapewh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.tarul.cn/Article/details/gqnekgate.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.tarul.cn/Article/details/gebcuaxed.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.tarul.cn/Article/details/gizvfvcsf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gqvqokoic.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.bbcook.cn/Article/details/grggufemg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gtnsfvjls.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.yfazqb.com/Article/details/gchvfzrbs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.yfazqb.com/Article/details/gygrgeavu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.tarul.cn/Article/details/guyfvojqb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fktsv.cn/Article/details/gudpiekrv.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.tarul.cn/Article/details/gsrwfogdb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.bbcook.cn/Article/details/gnrpymedg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.bbcook.cn/Article/details/grmrakfre.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/ghypdxzua.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.sjlbkw.cn/Article/details/gmyevzoyk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gocsscqwh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.yfazqb.com/Article/details/gxvstgqnu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/griychfln.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gmuaxyhzl.sHtML

[D26] 数组转字符串
来源：http://wap.vehdjk.com/Article/details/gnuuhjxtj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.tarul.cn/Article/details/gmkjmjkma.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/gblpqptkc.sHtML

JS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gomgsmorz.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gzswmvubi.sHtML

Java: String.join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gmttmgkoj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.yfazqb.com/Article/details/ghbiovcbt.sHtML

Ruby: arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gxfljaxnb.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gwmusanbd.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gbfxzjrcf.sHtML

E. 字符串处理
来源：http://wap.sjlbkw.cn/Article/details/gfmctvnor.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gyzatseve.sHtML

[E01] 拼接字符串
来源：http://blog.epnwcf.com/Article/details/ggpxwhxhm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.tarul.cn/Article/details/gixypqtme.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.yfazqb.com/Article/details/gidemoisv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gwgceantg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/gpmscnsqo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gpkxbvtak.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/gtqweuutj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.epnwcf.com/Article/details/gluutexwe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.bbcook.cn/Article/details/gqinrvkyn.sHtML

[E02] 重复字符串
来源：http://wap.vehdjk.com/Article/details/gmeywgdcb.sHtML

Py:   "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gztzihbne.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/ggykfbfci.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/goqmjndcj.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gvajzchyz.sHtML

Java: "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gjjrkdsha.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.vehdjk.com/Article/details/glzirpzsb.sHtML

Ruby: "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gnptqgxzb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.sjlbkw.cn/Article/details/gfbqkwfsr.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/grvevinyq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.tarul.cn/Article/details/gqmotgibz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gptafrjul.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gwmubqavq.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gitihkuco.sHtML

Java: s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gjsirffda.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.tarul.cn/Article/details/gegyjzigv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.sjlbkw.cn/Article/details/grgniqmat.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fktsv.cn/Article/details/gftvaxtfv.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gruduklpz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.tarul.cn/Article/details/gumhjvejn.sHtML

PHP:  strpos($s, "x");
来源：http://blog.vehdjk.com/Article/details/gjqxdpgqy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.sjlbkw.cn/Article/details/gadprvcuh.sHtML

TS:   s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/grmuiddwe.sHtML

Java: s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gxkncddbh.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.vehdjk.com/Article/details/ggqwnwrty.sHtML

Ruby: s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/glauqhgep.sHtML

C#:   s.IndexOf("x")
来源：http://blog.epnwcf.com/Article/details/giadtarda.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.epnwcf.com/Article/details/ghstesgbu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gnanhzzgo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.tarul.cn/Article/details/gyampxwtw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/glrwyqxyn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fktsv.cn/Article/details/gddafnaix.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gytdhcsoy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.epnwcf.com/Article/details/glvrcbjlt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fktsv.cn/Article/details/gudhvchmi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.tarul.cn/Article/details/gzqdyyxjg.sHtML

[E06] 替换子串
来源：http://www.blog.vehdjk.com/Article/details/ghemkeukx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gtzvxigpz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.epnwcf.com/Article/details/gmvxjrsok.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/geyqmvohz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gqnmtuvlc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gushyfrkl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gslmnjvik.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/geeskdxic.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gqkmqnbnb.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/gjqntakuk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gvbtqoaar.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.bbcook.cn/Article/details/gtbcesxoj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.epnwcf.com/Article/details/gwrkpdenr.sHtML

TS:   s.split(",")
来源：http://www.blog.tarul.cn/Article/details/gwaguqhmj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.tarul.cn/Article/details/gzhlrijbq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.sjlbkw.cn/Article/details/gemiglkam.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.vehdjk.com/Article/details/gvzeofspb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.sjlbkw.cn/Article/details/gqxbglwxp.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fktsv.cn/Article/details/gwqxyfksl.sHtML

Py:   ",".join(items)
来源：http://www.share.epnwcf.com/Article/details/gikbtvbnq.sHtML

PHP:  implode(",", $items);
来源：http://3g.fktsv.cn/Article/details/gyrzjnqsw.sHtML

JS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/guutamijp.sHtML

TS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gmbkynvow.sHtML

Java: String.join(",", items)
来源：http://m.share.tarul.cn/Article/details/gfnarqqqu.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.epnwcf.com/Article/details/gsfgvnjzi.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/glslkvuku.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/gzznzybod.sHtML

[E09] 去除所有空白字符
来源：http://wap.bbcook.cn/Article/details/gnwbwxbxf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.sjlbkw.cn/Article/details/gscebnznx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.vehdjk.com/Article/details/gasqinmki.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gcrxtlmud.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gbchgzbyq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gkyzceofg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.sjlbkw.cn/Article/details/gypyckbnq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.bbcook.cn/Article/details/geegrlhxq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.bbcook.cn/Article/details/gayjaxcsz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.sjlbkw.cn/Article/details/gyjyjykjm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gyzvyrkrq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.vehdjk.com/Article/details/gobikrxbj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gqsyfftxa.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gzeuqxozn.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gbyhxgrft.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gzmxorrbq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/glriagdtq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.tarul.cn/Article/details/gnelvaqhf.sHtML

[E11] 反转字符串
来源：http://www.m.share.tarul.cn/Article/details/gpzjibjdv.sHtML

Py:   s[::-1]
来源：http://3g.bbcook.cn/Article/details/gioeszjbc.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/gsdnuiicg.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gkkinchao.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gldymmlae.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gblnqwhib.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gjpwxehwm.sHtML

Ruby: s.reverse
来源：http://m.share.tarul.cn/Article/details/gduvyjzyy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/geozrwmai.sHtML

[E12] 统计某字符出现次数
来源：http://3g.bbcook.cn/Article/details/gjwwozikn.sHtML

Py:   s.count("a")
来源：http://blog.tarul.cn/Article/details/grriiilcp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.bbcook.cn/Article/details/gudepvltm.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.vehdjk.com/Article/details/gptusdekz.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gdaypyiyq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fktsv.cn/Article/details/ganalpykr.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.epnwcf.com/Article/details/gmymhihnr.sHtML

Ruby: s.count("a")
来源：http://read.share.vehdjk.com/Article/details/geceykueu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.yfazqb.com/Article/details/gpjrwwhgi.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.yfazqb.com/Article/details/gyqiikjho.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/gzzxoyldw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fktsv.cn/Article/details/gnvdcsvzt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gvnberowx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/gnqmjsomh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.vehdjk.com/Article/details/gpolxwiuu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.epnwcf.com/Article/details/gbmxqzsmr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/ghxerrupk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.tarul.cn/Article/details/gvwayrgsp.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/ghaoyymvl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/glaangfhq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gpqqxksaj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fktsv.cn/Article/details/gdfngmfdo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.epnwcf.com/Article/details/gcmvzoacl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.bbcook.cn/Article/details/gvuxwqylr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gktdzefgi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.yfazqb.com/Article/details/gspgsopmm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/guwtunzqq.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.yfazqb.com/Article/details/gntjzyhmy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/gnqlcvebv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.tarul.cn/Article/details/goajkalyd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/gggjprrta.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.yfazqb.com/Article/details/gveepwehg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gaojykcpl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/gfgsdgvwj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fktsv.cn/Article/details/gqomlulrg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.epnwcf.com/Article/details/gxdnzcekw.sHtML

[E16] 数字千分位
来源：http://mobile.tarul.cn/Article/details/goytersjf.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.sjlbkw.cn/Article/details/gaejlsxox.sHtML

PHP:  number_format(1234567);
来源：http://baike.tarul.cn/Article/details/gzduvncqb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/grarhimsf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gruijlwpl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/gkakklqha.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/gfivjehfj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/gdrcggmmp.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.bbcook.cn/Article/details/gvnqopmeq.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/gjtrpddrq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.sjlbkw.cn/Article/details/gfvqbqtzd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmejyqsku.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.tarul.cn/Article/details/ggmiqapnx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gcwvjhbiw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.yfazqb.com/Article/details/gfvokzayx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/gctnltjef.sHtML

Ruby: s.capitalize
来源：http://www.blog.tarul.cn/Article/details/gpbqewlsv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.sjlbkw.cn/Article/details/gcsjuvzkw.sHtML

[E18] 模板占位符替换
来源：http://mobile.sjlbkw.cn/Article/details/guvszmpxi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.tarul.cn/Article/details/gthlysohu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.tarul.cn/Article/details/gkvrwfhsn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/glwbipaiu.sHtML


<!-- 参考信息 -->