代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gphgxneqs.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gmuvdzilx.sHtML

C#:   list.Sort();
来源：http://blog.sjlbkw.cn/Article/details/gqooyljcl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/gsjxkmvmy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.bbcook.cn/Article/details/gadxawjxl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/gnjdjfkos.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/gjrevmpgq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gyequsoed.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.tarul.cn/Article/details/gdpimcspk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.sjlbkw.cn/Article/details/gbllkugao.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fktsv.cn/Article/details/gapisdzsp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.sjlbkw.cn/Article/details/gbdlvhvsc.sHtML

[D11] 反转数组
来源：http://mobile.sjlbkw.cn/Article/details/gohatmuyh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.epnwcf.com/Article/details/gxiynizcs.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.yfazqb.com/Article/details/gvktlmqds.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.vehdjk.com/Article/details/ghguksmjk.sHtML

TS:   [...arr].reverse();
来源：http://baike.yfazqb.com/Article/details/gtwbhdmon.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fktsv.cn/Article/details/gzdbeldck.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.epnwcf.com/Article/details/gvejylbkz.sHtML

Ruby: arr.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gnchstdtz.sHtML

C#:   list.Reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gevirnhxj.sHtML

[D12] 查找元素下标
来源：http://www.m.share.yfazqb.com/Article/details/ghaotjwkv.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fktsv.cn/Article/details/gglaecnqc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.epnwcf.com/Article/details/ghvcqxueq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/goeuvbyrr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/grdformhp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.bbcook.cn/Article/details/gsaxqutmd.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/gqxsukhps.sHtML

Ruby: arr.index(x)
来源：http://wap.fktsv.cn/Article/details/gwuncyugn.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gtfmguecm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.bbcook.cn/Article/details/gisfxdyoc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.vehdjk.com/Article/details/gazfqyvxe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/gepetqefm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/gawxfctvt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gzaghklbq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/grestgeim.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.epnwcf.com/Article/details/gqamcoxnw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fktsv.cn/Article/details/gnqgoqwsd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gqrfamjne.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.tarul.cn/Article/details/gsxlvptys.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.yfazqb.com/Article/details/gktmkrjin.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gfpzrmjsu.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.tarul.cn/Article/details/gpwqmlglu.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gpcrbpvch.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.vehdjk.com/Article/details/guctkrgef.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gmbjkhmdp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gtvfolhhd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gsvfvovdl.sHtML

[D15] 去重
来源：http://www.blog.vehdjk.com/Article/details/ggttmyylh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gupehbbdf.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/glraszweu.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gppjodaim.sHtML

TS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gtpwyvayp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.yfazqb.com/Article/details/gyezfnlyh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.epnwcf.com/Article/details/glqrwgyqz.sHtML

Ruby: arr.uniq
来源：http://mobile.tarul.cn/Article/details/ggifypquo.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fktsv.cn/Article/details/gvldxwtar.sHtML

[D16] 求和与平均值
来源：http://wap.epnwcf.com/Article/details/gzjvggfbc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.tarul.cn/Article/details/gfdnlnaqz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fktsv.cn/Article/details/gjletjrps.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/gnuaqbvln.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gdwlqtbca.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.tarul.cn/Article/details/glyjzyfgs.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/glqwaipho.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gsufcdiai.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.sjlbkw.cn/Article/details/gibjagtsp.sHtML

[D17] 最大值与最小值
来源：http://mobile.sjlbkw.cn/Article/details/gyjhklqfn.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/guqqsipmg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gajbpstdj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fktsv.cn/Article/details/grrrpixew.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fktsv.cn/Article/details/gsdyhnwwn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.bbcook.cn/Article/details/gpxwpdztt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gyxljaott.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.tarul.cn/Article/details/goytebgfw.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.yfazqb.com/Article/details/gbtqnjfvf.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.epnwcf.com/Article/details/giqflmfhr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.bbcook.cn/Article/details/gznjrbxma.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.tarul.cn/Article/details/gaeowrmcf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.vehdjk.com/Article/details/gakmwkypy.sHtML

TS:   nested.flat();
来源：http://www.m.share.bbcook.cn/Article/details/gsluubgnz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gxkbfdefh.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fktsv.cn/Article/details/giyqklfxm.sHtML

Ruby: nested.flatten
来源：http://m.share.tarul.cn/Article/details/gzdfqtpqa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.epnwcf.com/Article/details/gwcsjgegw.sHtML

[D19] 按字段分组
来源：http://read.share.vehdjk.com/Article/details/grilgyvsm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fktsv.cn/Article/details/ggzfzrvqr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.yfazqb.com/Article/details/gabmctfaw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.bbcook.cn/Article/details/ghlryqlgx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.tarul.cn/Article/details/gakvqedqv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.yfazqb.com/Article/details/gfizcrwxu.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/gzpncklcy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.vehdjk.com/Article/details/gpocfjjtt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.vehdjk.com/Article/details/gymzfbekl.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.epnwcf.com/Article/details/gvouvavtc.sHtML

Py:   Counter(arr)
来源：http://baike.yfazqb.com/Article/details/gkbznysgn.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.vehdjk.com/Article/details/glxnykihj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.yfazqb.com/Article/details/gqxijsvim.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/ghhnppwpt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.yfazqb.com/Article/details/gkzvwhstd.sHtML

Go:   // 手写 map[T]int
来源：http://blog.epnwcf.com/Article/details/geaauxffx.sHtML

Ruby: arr.tally
来源：http://blog.fktsv.cn/Article/details/gyfxaznac.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.vehdjk.com/Article/details/gsaoulylu.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fktsv.cn/Article/details/gzfgwgodf.sHtML

Py:   x in arr
来源：http://3g.tarul.cn/Article/details/glmlgftjk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.epnwcf.com/Article/details/gehxhgssp.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/giiqqvtnp.sHtML

TS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gqmiuxmts.sHtML

Java: list.contains(x)
来源：http://3g.tarul.cn/Article/details/gduejsncu.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.vehdjk.com/Article/details/gkfryczfc.sHtML

Ruby: arr.include?(x)
来源：http://mobile.tarul.cn/Article/details/gqcjbcvdz.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gwfulwjzt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.yfazqb.com/Article/details/gucpueauu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.tarul.cn/Article/details/gkifdctln.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.yfazqb.com/Article/details/gfvjjcfoz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.bbcook.cn/Article/details/gwedbwuhu.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/gmygixakz.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.vehdjk.com/Article/details/grfcnwsvq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fktsv.cn/Article/details/gflcykepn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.tarul.cn/Article/details/gtruxbtcf.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gillgoilp.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.bbcook.cn/Article/details/ggfddhoye.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.vehdjk.com/Article/details/gkmeysruh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fktsv.cn/Article/details/gygjrjtfn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gcwccquxs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/grvumrxut.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fktsv.cn/Article/details/gsgvmcsvb.sHtML

Go:   // 手写循环
来源：http://m.share.sjlbkw.cn/Article/details/gyczdyota.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.vehdjk.com/Article/details/ghmhrsnpa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.yfazqb.com/Article/details/ggsviftry.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.epnwcf.com/Article/details/gzdlhrhnv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.tarul.cn/Article/details/getajmsyc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.vehdjk.com/Article/details/gcahnhkmq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.vehdjk.com/Article/details/gktwmphmr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.bbcook.cn/Article/details/guoefisjg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.epnwcf.com/Article/details/gjrypetin.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.tarul.cn/Article/details/gopstyxol.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.tarul.cn/Article/details/gxrrtvjkn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.yfazqb.com/Article/details/gywebamoe.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.tarul.cn/Article/details/gtzffxeql.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fktsv.cn/Article/details/gozrmxgnd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.bbcook.cn/Article/details/grxybpsfn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.yfazqb.com/Article/details/ghegclqfl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.bbcook.cn/Article/details/giaaxqulr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fktsv.cn/Article/details/gvckqpwkl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.bbcook.cn/Article/details/gjtfwezvu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/gcqwcmtah.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.epnwcf.com/Article/details/gfsnggvoc.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/galmthstx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.tarul.cn/Article/details/gwccvqtdv.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.vehdjk.com/Article/details/ghexhfszx.sHtML

JS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/guxwykuas.sHtML

TS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/giicbmcse.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gchkzhszw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.bbcook.cn/Article/details/gfyzvkfkj.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gstpgitwd.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gebghhauh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnsmzgsix.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/gyfkgrwew.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqckgovlx.sHtML

[E01] 拼接字符串
来源：http://baike.bbcook.cn/Article/details/grouwopdr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.yfazqb.com/Article/details/gqtzabzqh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.bbcook.cn/Article/details/gwtaifzhn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/grcxvffxr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/gcbqdumcg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.tarul.cn/Article/details/gswgcfwtt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.epnwcf.com/Article/details/gywogpeld.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.bbcook.cn/Article/details/gpfbvvcha.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.vehdjk.com/Article/details/gxdkfhzlj.sHtML

[E02] 重复字符串
来源：http://mobile.yfazqb.com/Article/details/gkehotpwd.sHtML

Py:   "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/guulvvplg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.epnwcf.com/Article/details/gcjgnitei.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/ghmxkjeby.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/giunadfjw.sHtML

Java: "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gzxfprwxg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.tarul.cn/Article/details/gxtdnctqc.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gcrvjnhkg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.vehdjk.com/Article/details/gjiwettel.sHtML

[E03] 截取子串
来源：http://mobile.tarul.cn/Article/details/gdrqmgzuk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.yfazqb.com/Article/details/gykqsyylt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/ggazlzgbo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gaxtvxtlt.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/guqomruop.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gdwddwouk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.yfazqb.com/Article/details/ggcwsunpd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.sjlbkw.cn/Article/details/glskfrpqn.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.yfazqb.com/Article/details/ghxzhjfgc.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/gmmnkbywa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gayvozzkn.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.epnwcf.com/Article/details/gvhatvyna.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.sjlbkw.cn/Article/details/gnprglios.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gxpkisswp.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/geaygkbgw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.tarul.cn/Article/details/gmrduxnbo.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/glfcoiwkd.sHtML

C#:   s.IndexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gtintrwhu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.bbcook.cn/Article/details/gtlguxhft.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.yfazqb.com/Article/details/gtercscxa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/gavgcglri.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gtshdxxrq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.yfazqb.com/Article/details/gghmizbul.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gdbkrxwyq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.sjlbkw.cn/Article/details/ghsnhnxib.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/gwsiiiwkq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.yfazqb.com/Article/details/gjtuxquji.sHtML

[E06] 替换子串
来源：http://www.m.share.epnwcf.com/Article/details/glkweawqv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/gpljvmbvb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.vehdjk.com/Article/details/gifxklkbm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gphhaaexo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gdubcctgf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gytzlibmm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gwsfvvotm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gltzfazqb.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.yfazqb.com/Article/details/gjonppotm.sHtML

[E07] 按分隔符拆分
来源：http://wap.fktsv.cn/Article/details/gpqvmtbrb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fktsv.cn/Article/details/gaekjzbkg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.tarul.cn/Article/details/gcztrwxkv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.yfazqb.com/Article/details/gtdialkcp.sHtML

TS:   s.split(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfssihgjr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/ghawrfagu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fktsv.cn/Article/details/golvhjebx.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.tarul.cn/Article/details/ghblxbvou.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/gqjjtixez.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fktsv.cn/Article/details/gpjpymlwq.sHtML

Py:   ",".join(items)
来源：http://www.m.share.vehdjk.com/Article/details/ghjuqzvob.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fktsv.cn/Article/details/ghckxnfxg.sHtML

JS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gmlmmxxer.sHtML

TS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gcykyfqfj.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/gfhtqhonv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.tarul.cn/Article/details/gbvbomxjf.sHtML

Ruby: items.join(",")
来源：http://blog.tarul.cn/Article/details/gafvairoy.sHtML

C#:   string.Join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gylecizme.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/gwflknhss.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.vehdjk.com/Article/details/ggtgsifwt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.tarul.cn/Article/details/gviketzrz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/glzcuzret.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gcqcimsdy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.epnwcf.com/Article/details/gihdgruzn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/gkksorief.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.vehdjk.com/Article/details/gvtpsnzxb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gnmnioiuq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fktsv.cn/Article/details/ggyalxbyv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gyfifcbrp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.epnwcf.com/Article/details/gpccynkuz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gevthiunf.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/gkejhcrlk.sHtML

Java: String.format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/geirdwxvf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gfllaehag.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/golszbrkw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.vehdjk.com/Article/details/gzceqhnty.sHtML

[E11] 反转字符串
来源：http://blog.bbcook.cn/Article/details/gkjuvnfnl.sHtML

Py:   s[::-1]
来源：http://3g.fktsv.cn/Article/details/gcgyqiwwv.sHtML

PHP:  strrev($s);
来源：http://mobile.epnwcf.com/Article/details/gxxqjyvcv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gmwkvebhd.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gpktwndsk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.yfazqb.com/Article/details/gqgrizdfz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gpwohkzjv.sHtML

Ruby: s.reverse
来源：http://mobile.yfazqb.com/Article/details/gfremxjru.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gqxsycjyx.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gfjzfljhd.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gquemgvtt.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.vehdjk.com/Article/details/gqouhkylq.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gewqsrkyf.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/ggujzelue.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.tarul.cn/Article/details/ghhlbodwy.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gwckgqifs.sHtML

Ruby: s.count("a")
来源：http://3g.tarul.cn/Article/details/gevmacniy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.vehdjk.com/Article/details/gbpgzxoja.sHtML

[E13] 逐字符遍历
来源：http://3g.epnwcf.com/Article/details/gzcptldby.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.epnwcf.com/Article/details/gvoigaakx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.epnwcf.com/Article/details/gmfanpqru.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/gavctxdqi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gcexzfozo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gwyiabgqg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.epnwcf.com/Article/details/grhwmkiqh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.sjlbkw.cn/Article/details/gzddntykm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.tarul.cn/Article/details/gicvmeqbp.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fktsv.cn/Article/details/gjwrfudcd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fktsv.cn/Article/details/gfmyzpfjp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.bbcook.cn/Article/details/gtvfyskdn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.tarul.cn/Article/details/getjdxmmv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.sjlbkw.cn/Article/details/gdbnirwum.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.epnwcf.com/Article/details/gvzgtnaji.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/gybemgaqz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.tarul.cn/Article/details/gcqdkyqpp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.epnwcf.com/Article/details/gpcrjgipt.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fktsv.cn/Article/details/glyxjukwk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/gbljmzhpw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.yfazqb.com/Article/details/guejrdpxt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fktsv.cn/Article/details/gmlgkerhh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.bbcook.cn/Article/details/ghavmsmnl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/gkozhjter.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gqowmglyk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fktsv.cn/Article/details/ggziultlm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.epnwcf.com/Article/details/gpsdkckdl.sHtML

[E16] 数字千分位
来源：http://read.share.fktsv.cn/Article/details/gtxbwkvre.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.vehdjk.com/Article/details/gpbhlaooq.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/gjmchilic.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gzeomvwki.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gmianmgig.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fktsv.cn/Article/details/ghocslaav.sHtML


<!-- 参考信息 -->