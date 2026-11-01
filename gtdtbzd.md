代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fktsv.cn/Article/details/gjcrvhgca.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fktsv.cn/Article/details/giejhlygy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.vehdjk.com/Article/details/gobrilinb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.tarul.cn/Article/details/giswsjdug.sHtML

[D11] 反转数组
来源：http://www.m.share.yfazqb.com/Article/details/gknwpepbo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gceufiifx.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gddquwnlo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.vehdjk.com/Article/details/gmofbboqc.sHtML

TS:   [...arr].reverse();
来源：http://read.share.epnwcf.com/Article/details/gkwmgdyaf.sHtML

Java: Collections.reverse(list);
来源：http://www.share.tarul.cn/Article/details/gyqacgcvx.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.sjlbkw.cn/Article/details/ganjfpdkw.sHtML

Ruby: arr.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gfgfmxvtp.sHtML

C#:   list.Reverse();
来源：http://baike.sjlbkw.cn/Article/details/gklvnphwo.sHtML

[D12] 查找元素下标
来源：http://read.share.tarul.cn/Article/details/gyelfrgxy.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.sjlbkw.cn/Article/details/gtjobghgt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fktsv.cn/Article/details/gosppmthz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gkzoovozt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.sjlbkw.cn/Article/details/gglqdilcg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/grnpsbosy.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fktsv.cn/Article/details/gfivllfzw.sHtML

Ruby: arr.index(x)
来源：http://baike.fktsv.cn/Article/details/gmakzsykg.sHtML

C#:   list.IndexOf(x);
来源：http://baike.tarul.cn/Article/details/grtcodnjt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.sjlbkw.cn/Article/details/gwnhstxlf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.tarul.cn/Article/details/glpbxordz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.vehdjk.com/Article/details/ggbtsrbaq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/gcehhzjak.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/gmdpqpgfv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.tarul.cn/Article/details/gyxhvebrx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.vehdjk.com/Article/details/gawjbomlf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.vehdjk.com/Article/details/gqdupcmck.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fktsv.cn/Article/details/geknecrur.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.epnwcf.com/Article/details/gupmuxdpo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gfjyryenk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/glexqnchv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gwxlaaxxx.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/glhrnnqjz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gjzmxexju.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/glfcbrmuq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.sjlbkw.cn/Article/details/glnvjucyv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fktsv.cn/Article/details/geqjkfxvc.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/ghqmjslro.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/gfpqfltuz.sHtML

PHP:  array_unique($arr);
来源：http://wap.tarul.cn/Article/details/gymmfgopx.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gvmcxkmhx.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gfmhvttos.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.bbcook.cn/Article/details/ghgnfjgzl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.tarul.cn/Article/details/gqsonutkr.sHtML

Ruby: arr.uniq
来源：http://mobile.fktsv.cn/Article/details/gvvhtunch.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/gvhuezrfk.sHtML

[D16] 求和与平均值
来源：http://mobile.bbcook.cn/Article/details/grcffdkim.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.yfazqb.com/Article/details/giaklamnp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gfdlzsmsh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/goecleudo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.bbcook.cn/Article/details/gbhrvjwav.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.sjlbkw.cn/Article/details/gqpqkggzf.sHtML

Go:   // 手写循环累加
来源：http://blog.bbcook.cn/Article/details/ghtbnnhzu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.bbcook.cn/Article/details/gpcllxxut.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.epnwcf.com/Article/details/genpnuace.sHtML

[D17] 最大值与最小值
来源：http://baike.epnwcf.com/Article/details/gsvlxmoon.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fktsv.cn/Article/details/gbzxtemzf.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gfcomdqrz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fktsv.cn/Article/details/gfpiyfywl.sHtML

TS:   Math.max(...arr);
来源：http://wap.sjlbkw.cn/Article/details/glyytmbht.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.bbcook.cn/Article/details/gnlxhutoc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fktsv.cn/Article/details/gejvtotgy.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gtogyhnwc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.tarul.cn/Article/details/gijkgimyl.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.bbcook.cn/Article/details/gtkbqhdqp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.sjlbkw.cn/Article/details/gshwzgzny.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gfrqfajml.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.sjlbkw.cn/Article/details/gujptqnfv.sHtML

TS:   nested.flat();
来源：http://3g.yfazqb.com/Article/details/glyglltxt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fktsv.cn/Article/details/gsfmubdrx.sHtML

Go:   // 手写双层循环
来源：http://wap.bbcook.cn/Article/details/gugcsajaw.sHtML

Ruby: nested.flatten
来源：http://blog.sjlbkw.cn/Article/details/gipdbsgxg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fktsv.cn/Article/details/gdflbuqdc.sHtML

[D19] 按字段分组
来源：http://baike.bbcook.cn/Article/details/gtdpvdiyh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.tarul.cn/Article/details/gxrjwhhtt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fktsv.cn/Article/details/gvjpsqsqg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.vehdjk.com/Article/details/gmkeatsfm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fktsv.cn/Article/details/gufcqvmih.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.bbcook.cn/Article/details/garvwvlqq.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.yfazqb.com/Article/details/gruzcuvox.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/glutukblv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.bbcook.cn/Article/details/gwbdfymsb.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fktsv.cn/Article/details/gsttjqnrp.sHtML

Py:   Counter(arr)
来源：http://read.share.vehdjk.com/Article/details/giuxphxvn.sHtML

PHP:  array_count_values($arr);
来源：http://3g.bbcook.cn/Article/details/gycbmfcrk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/ghpgwmvot.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gbkgstfer.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fktsv.cn/Article/details/ggnnxevmm.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.sjlbkw.cn/Article/details/gkoeoirwe.sHtML

Ruby: arr.tally
来源：http://3g.epnwcf.com/Article/details/gzzrfdsdg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.yfazqb.com/Article/details/gxgwszubz.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.epnwcf.com/Article/details/gkvauxzhn.sHtML

Py:   x in arr
来源：http://read.share.tarul.cn/Article/details/glllfciaw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.tarul.cn/Article/details/ghcowuyem.sHtML

JS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/gqkklffbx.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gmrsdssip.sHtML

Java: list.contains(x)
来源：http://m.share.bbcook.cn/Article/details/gnxxmfgwc.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.bbcook.cn/Article/details/gqtwvozxq.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/ghcqthvpy.sHtML

C#:   list.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/ggbqcatvw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.sjlbkw.cn/Article/details/gqphswpfq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.bbcook.cn/Article/details/gboacmirk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.sjlbkw.cn/Article/details/gnlfwpmal.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.yfazqb.com/Article/details/gzkvwmgxj.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/gdvwbyzko.sHtML

Java: new ArrayList<>(list);
来源：http://3g.vehdjk.com/Article/details/gavxrnfku.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.sjlbkw.cn/Article/details/grbocmywk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fktsv.cn/Article/details/ghuwrcych.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gmskbbbis.sHtML

[D23] reduce 累积计算
来源：http://3g.sjlbkw.cn/Article/details/gbezqnkbq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.yfazqb.com/Article/details/gyrabpwwe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.yfazqb.com/Article/details/gsqvaglcd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/gyjgzyuvj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gmhmpxpqw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.vehdjk.com/Article/details/goyvbceeo.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gtccblfev.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.yfazqb.com/Article/details/govjstntl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.bbcook.cn/Article/details/gxnqhafii.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/gbvmhooio.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.sjlbkw.cn/Article/details/goystuydo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.vehdjk.com/Article/details/gatxqouqq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.yfazqb.com/Article/details/gjdpmdevc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.vehdjk.com/Article/details/gusiuzroh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.vehdjk.com/Article/details/gpkansvpe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/gcafepaly.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.tarul.cn/Article/details/gmeuzzmju.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.bbcook.cn/Article/details/gsvxbcdyx.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.bbcook.cn/Article/details/gxwuhnyhq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.yfazqb.com/Article/details/guctdgdqj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.epnwcf.com/Article/details/gicpbkjlu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.vehdjk.com/Article/details/gwewoebnt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.bbcook.cn/Article/details/gqnlrpedy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.vehdjk.com/Article/details/gvxamvwvf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.tarul.cn/Article/details/gmufmbcms.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.tarul.cn/Article/details/giodgoxnt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.vehdjk.com/Article/details/gymbugbaq.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gfettcvgv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.tarul.cn/Article/details/giihqazno.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gmmzfwubf.sHtML

JS:   arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gqbsapsdh.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gqklgcbry.sHtML

Java: String.join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/gyhtemhvd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.epnwcf.com/Article/details/gzjpitvkl.sHtML

Ruby: arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gdojncprf.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/ghiyflxof.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gearprqeu.sHtML

E. 字符串处理
来源：http://read.share.bbcook.cn/Article/details/gtvoquhgv.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfmcxrkzo.sHtML

[E01] 拼接字符串
来源：http://m.share.tarul.cn/Article/details/ghvqtxpem.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/ggzxsygni.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fktsv.cn/Article/details/gscusipns.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gxohleoqs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gebdiijld.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.yfazqb.com/Article/details/gdjkdzdns.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.epnwcf.com/Article/details/gaswwouuh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.yfazqb.com/Article/details/gsqodykcn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gljvcqhkl.sHtML

[E02] 重复字符串
来源：http://mobile.tarul.cn/Article/details/gzxpbxrls.sHtML

Py:   "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/gduwlfmae.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.epnwcf.com/Article/details/gdhhzctlc.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/grithsngh.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gcpjdcauq.sHtML

Java: "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gzprlgoxz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.yfazqb.com/Article/details/gwvzgxztu.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gibgxzpmv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.epnwcf.com/Article/details/gjhsjeqpw.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/grkmpvdhq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.sjlbkw.cn/Article/details/gxygwxlxi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gvqsaahcj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.tarul.cn/Article/details/ggpzkgvno.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gffbcewyo.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gtiwtuxmk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.bbcook.cn/Article/details/glsllapyu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.tarul.cn/Article/details/ghzhahalq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.yfazqb.com/Article/details/gdxkfdbxu.sHtML

[E04] 查找子串位置
来源：http://baike.fktsv.cn/Article/details/gfymzbngq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/gchsfpkdb.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/grldzkhlf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.bbcook.cn/Article/details/gnsfeayoq.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gfnlgaebi.sHtML

Java: s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gaadyjwpm.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fktsv.cn/Article/details/gotfrakyj.sHtML

Ruby: s.index("x")
来源：http://baike.epnwcf.com/Article/details/gmjndrlde.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gmllfhhor.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.epnwcf.com/Article/details/ghhdvthar.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.vehdjk.com/Article/details/gfzbneohx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fktsv.cn/Article/details/gotwkiqqi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gmkebeurh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fktsv.cn/Article/details/gwhkkohzv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gbudwmoij.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/gjaerigqe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.yfazqb.com/Article/details/gfvieyrqj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gzuxmtkwq.sHtML

[E06] 替换子串
来源：http://www.m.share.yfazqb.com/Article/details/gkquzdmqk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gmrmzatfi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.epnwcf.com/Article/details/gcnwvyaxg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gxmwxbqml.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gcbawsobi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/ggocygomc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gmolkolud.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.bbcook.cn/Article/details/ghjbkyagm.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fktsv.cn/Article/details/gpfnyqgpg.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fktsv.cn/Article/details/gjsgncqrd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.tarul.cn/Article/details/gjzpgpnfz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gynxrfcwj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.sjlbkw.cn/Article/details/ggiyhdhvp.sHtML

TS:   s.split(",")
来源：http://read.share.bbcook.cn/Article/details/gbwnfvaat.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/gqnvltavm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fktsv.cn/Article/details/gulrqimqk.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.yfazqb.com/Article/details/gxycbtwoj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.epnwcf.com/Article/details/ghmjytcsp.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.tarul.cn/Article/details/gzgakdjjo.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/glhorngzw.sHtML

PHP:  implode(",", $items);
来源：http://blog.yfazqb.com/Article/details/gnkugbvnz.sHtML

JS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gdhuhnkbd.sHtML

TS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gacugybex.sHtML

Java: String.join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/gzazlucbz.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.tarul.cn/Article/details/galualnsy.sHtML

Ruby: items.join(",")
来源：http://baike.tarul.cn/Article/details/gsiuntjrf.sHtML

C#:   string.Join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gpcggxkyc.sHtML

[E09] 去除所有空白字符
来源：http://m.share.sjlbkw.cn/Article/details/gqekfzfev.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.epnwcf.com/Article/details/gziaymrlv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/gyafeuypl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gwbirgxey.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gkwqjnqgj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gvckwewhj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gpuqmdwfb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.epnwcf.com/Article/details/gkgbadpul.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.tarul.cn/Article/details/gyzgeisyt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/gdqiigbor.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.vehdjk.com/Article/details/gwzztdvzw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.bbcook.cn/Article/details/gdhsrlodw.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gljrsjkjs.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gvgfoozkv.sHtML

Java: String.format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gsabytmfs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gfhilconm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gfdawiknu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.sjlbkw.cn/Article/details/gsendvumk.sHtML

[E11] 反转字符串
来源：http://m.share.tarul.cn/Article/details/gqbgtixra.sHtML

Py:   s[::-1]
来源：http://read.share.tarul.cn/Article/details/grpoqbzhi.sHtML

PHP:  strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gfdqjumuz.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/ghtdurcmq.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gyroaspdf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.tarul.cn/Article/details/gtxunloup.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.bbcook.cn/Article/details/gmzeibkpv.sHtML

Ruby: s.reverse
来源：http://read.share.epnwcf.com/Article/details/gkxazkqdh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gqraacnfk.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.vehdjk.com/Article/details/gqvuiieah.sHtML

Py:   s.count("a")
来源：http://3g.fktsv.cn/Article/details/gelcoleel.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.tarul.cn/Article/details/ghwncsznt.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gpshzfrye.sHtML

TS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gojeptptm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.yfazqb.com/Article/details/gxljtwcox.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.vehdjk.com/Article/details/gnoczkzmd.sHtML

Ruby: s.count("a")
来源：http://read.share.epnwcf.com/Article/details/geitkfkvk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.tarul.cn/Article/details/guxsgbraw.sHtML

[E13] 逐字符遍历
来源：http://wap.epnwcf.com/Article/details/ggiodgdow.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.yfazqb.com/Article/details/gvlklouzv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.yfazqb.com/Article/details/gpmlsmfpt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gsmxbnval.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gevsnznvy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/gntematec.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.bbcook.cn/Article/details/gtodonfgt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.epnwcf.com/Article/details/gikymyzfl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gubycqrkn.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gzxjjxrzq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.vehdjk.com/Article/details/gxavfbpvx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.sjlbkw.cn/Article/details/gwjohenjk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gdpenrrsv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsybzxsne.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/galuniuab.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gpnlqnfym.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.tarul.cn/Article/details/gzopvxtfq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.yfazqb.com/Article/details/gdbdtvpfx.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.sjlbkw.cn/Article/details/gtsussnbr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.bbcook.cn/Article/details/gwyaeiymc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.vehdjk.com/Article/details/ggjltciol.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/gmrajjmpa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.epnwcf.com/Article/details/gfxlpfqly.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fktsv.cn/Article/details/gaivvhppv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.bbcook.cn/Article/details/gzbmvcowf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/geyyjntna.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.epnwcf.com/Article/details/glewcnbgt.sHtML

[E16] 数字千分位
来源：http://mobile.vehdjk.com/Article/details/gejjnhuvg.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.yfazqb.com/Article/details/ggpgqaivh.sHtML

PHP:  number_format(1234567);
来源：http://3g.tarul.cn/Article/details/gyfjtmosz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gkslxhzzr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/grvxbhmah.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gxcywsfdr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.yfazqb.com/Article/details/gqtknimjl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fktsv.cn/Article/details/gyyqldjnn.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.vehdjk.com/Article/details/gzqlwokms.sHtML

[E17] 首字母大写
来源：http://www.blog.fktsv.cn/Article/details/gxyeecpvy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.tarul.cn/Article/details/gkuyetvcu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/gnuqgkcny.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gpgrxnfnf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gfazjtqoo.sHtML


<!-- 参考信息 -->