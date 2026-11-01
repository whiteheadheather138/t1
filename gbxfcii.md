代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.yfazqb.com/Article/details/gapygmjmb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gfvcpuafl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/gezlfedck.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/gkgcwxexo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.epnwcf.com/Article/details/gqbubhfti.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.bbcook.cn/Article/details/ghvdvgduz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.tarul.cn/Article/details/glymvzhjb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.epnwcf.com/Article/details/glflqthxu.sHtML

[D11] 反转数组
来源：http://wap.fktsv.cn/Article/details/ghduljnly.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.tarul.cn/Article/details/goxdsddww.sHtML

PHP:  array_reverse($arr);
来源：http://wap.tarul.cn/Article/details/gkcfvcutj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.yfazqb.com/Article/details/gprkzcpcs.sHtML

TS:   [...arr].reverse();
来源：http://3g.fktsv.cn/Article/details/gfgoggamq.sHtML

Java: Collections.reverse(list);
来源：http://mobile.tarul.cn/Article/details/gbwyqhydl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gkgjndsij.sHtML

Ruby: arr.reverse
来源：http://wap.sjlbkw.cn/Article/details/gpgnxqktn.sHtML

C#:   list.Reverse();
来源：http://blog.yfazqb.com/Article/details/gvcxuvzqh.sHtML

[D12] 查找元素下标
来源：http://www.m.share.tarul.cn/Article/details/gpqljoask.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.sjlbkw.cn/Article/details/gxyuobooi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gvbpbfppq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gfjtbeyvq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gkkxtqufv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.epnwcf.com/Article/details/grappszxo.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gysezpboz.sHtML

Ruby: arr.index(x)
来源：http://read.share.yfazqb.com/Article/details/gysiwyfmn.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.epnwcf.com/Article/details/gkmvaolgw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.tarul.cn/Article/details/gykxpbliu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.bbcook.cn/Article/details/gxynndpip.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.yfazqb.com/Article/details/gxlzkixru.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gwtvhcnil.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gxxooojdz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.tarul.cn/Article/details/gvwidivgy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.bbcook.cn/Article/details/gmfmqnmkd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.epnwcf.com/Article/details/gqjnwqugx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.tarul.cn/Article/details/ggfzunzyz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fktsv.cn/Article/details/gcczbsevu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/gbsuoqwyq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fktsv.cn/Article/details/gtygbaucy.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.epnwcf.com/Article/details/gncltevjz.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gdynkvwvf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.vehdjk.com/Article/details/gsldmfbnz.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gfopkbxuz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gqzejjfct.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.yfazqb.com/Article/details/gmiawfuwt.sHtML

[D15] 去重
来源：http://mobile.bbcook.cn/Article/details/gkbpuvdcb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/gozwzhzve.sHtML

PHP:  array_unique($arr);
来源：http://m.share.vehdjk.com/Article/details/gtloxjsjg.sHtML

JS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/guoaskdro.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gsdkdskmt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/gffathcpb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.vehdjk.com/Article/details/gzehfgvua.sHtML

Ruby: arr.uniq
来源：http://www.share.yfazqb.com/Article/details/gxnlkkuuj.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.sjlbkw.cn/Article/details/gmeywkykq.sHtML

[D16] 求和与平均值
来源：http://www.blog.tarul.cn/Article/details/gdkaiuhef.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/gubnqgvhd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.sjlbkw.cn/Article/details/gfnssqfut.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/ggtufimwi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gaxkwrwnu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/glqivhkgn.sHtML

Go:   // 手写循环累加
来源：http://read.share.fktsv.cn/Article/details/ggonzbmem.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/gpznybprf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fktsv.cn/Article/details/gennmahyn.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gqcbeswsq.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gfqipcscb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fktsv.cn/Article/details/groduqgyn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.yfazqb.com/Article/details/gvexxqfow.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fktsv.cn/Article/details/gjgboxgus.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.epnwcf.com/Article/details/gcbrndlmr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.epnwcf.com/Article/details/gbqespvtv.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fktsv.cn/Article/details/gzzqqahne.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.bbcook.cn/Article/details/geqywuhoa.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.sjlbkw.cn/Article/details/gdapaciiw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.epnwcf.com/Article/details/ggapdmeww.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.yfazqb.com/Article/details/gxehsompd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.bbcook.cn/Article/details/gehdeqggf.sHtML

TS:   nested.flat();
来源：http://blog.vehdjk.com/Article/details/gkdtniqym.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gmrxkdlak.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/gokeikzxl.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/ggyztjnfd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gagyxyovo.sHtML

[D19] 按字段分组
来源：http://read.share.fktsv.cn/Article/details/gyvnuvbxp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fktsv.cn/Article/details/gvnkvcllw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.bbcook.cn/Article/details/grevfrvdb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.epnwcf.com/Article/details/glgzwjqvq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gnszcrozz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.epnwcf.com/Article/details/gxwarrcuz.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.epnwcf.com/Article/details/gmszoxghr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.yfazqb.com/Article/details/gelqyxisc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/gdwzvgzwa.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gsmkggapx.sHtML

Py:   Counter(arr)
来源：http://www.blog.bbcook.cn/Article/details/gkofcilbj.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.bbcook.cn/Article/details/gyezehuya.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/guzbuqxxr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/gmthqxyrb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fktsv.cn/Article/details/gkkiotpgb.sHtML

Go:   // 手写 map[T]int
来源：http://3g.yfazqb.com/Article/details/gckjebltf.sHtML

Ruby: arr.tally
来源：http://read.share.tarul.cn/Article/details/gkxliwixh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gwgkhkgvs.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.tarul.cn/Article/details/gafjhpftb.sHtML

Py:   x in arr
来源：http://wap.bbcook.cn/Article/details/ggvxnahof.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fktsv.cn/Article/details/gxqndyyih.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gtcklhtpj.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gjlzhjxpn.sHtML

Java: list.contains(x)
来源：http://mobile.bbcook.cn/Article/details/gzoqojhbi.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.epnwcf.com/Article/details/gxnzxhjrs.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gnsdfmslv.sHtML

C#:   list.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gpxfgdbzf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.epnwcf.com/Article/details/ghnujtzbl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.epnwcf.com/Article/details/gatexcpro.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.vehdjk.com/Article/details/gykhvovim.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gjlyxkezp.sHtML

TS:   [...arr];
来源：http://blog.sjlbkw.cn/Article/details/grlpxxhio.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/gappdnmqt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/gkpuefmsn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.vehdjk.com/Article/details/gohetpoet.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/ggukymmah.sHtML

[D23] reduce 累积计算
来源：http://blog.tarul.cn/Article/details/gqykkhhne.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.vehdjk.com/Article/details/ghpvxlnkk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.yfazqb.com/Article/details/gjjjogflt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gbphqpmzq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gzdmbytnm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.epnwcf.com/Article/details/gdloratcm.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gqlmppnre.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gbhptlxgn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fktsv.cn/Article/details/gkvooxrsr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.yfazqb.com/Article/details/gugfdxhma.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.sjlbkw.cn/Article/details/gtgzdcsbq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.vehdjk.com/Article/details/ghjaddsye.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.yfazqb.com/Article/details/glfxpkbtr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gebffghau.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/gjwrnkkyb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.epnwcf.com/Article/details/gvmkgmquq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fktsv.cn/Article/details/gipeljmen.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.vehdjk.com/Article/details/gothjgbvi.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.yfazqb.com/Article/details/gkprwjebz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.yfazqb.com/Article/details/glfajsihg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.bbcook.cn/Article/details/gvpiioivm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.vehdjk.com/Article/details/gzqwgctfp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.tarul.cn/Article/details/grnwbzmvg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/gzqocdjch.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fktsv.cn/Article/details/ggdreyjdx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.vehdjk.com/Article/details/gasuybgjk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.bbcook.cn/Article/details/gyerbpmgj.sHtML

[D26] 数组转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gtpkwcsls.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.bbcook.cn/Article/details/glehsjonq.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gtkojhpip.sHtML

JS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gewpsymgg.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/ggvlcqdvx.sHtML

Java: String.join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gggjmdgbs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.bbcook.cn/Article/details/geuubtema.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gqulrfwke.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fktsv.cn/Article/details/gbdrexwrj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gxyuzdokw.sHtML

E. 字符串处理
来源：http://www.m.share.vehdjk.com/Article/details/gtmannmjy.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/geyvmclcf.sHtML

[E01] 拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gvlficsok.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.yfazqb.com/Article/details/gqwyxqugj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.tarul.cn/Article/details/gmbwbmvmj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gqssulrxp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/gitfhgsuv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.sjlbkw.cn/Article/details/gnfaahymk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/gnxrrtruy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fktsv.cn/Article/details/gozfxxzss.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.epnwcf.com/Article/details/gkwyxcegu.sHtML

[E02] 重复字符串
来源：http://www.share.tarul.cn/Article/details/geaywiorb.sHtML

Py:   "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/giypwgpyp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.bbcook.cn/Article/details/gtlduplmj.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/ghalelyrc.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gwrztmqim.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gtavsucma.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.yfazqb.com/Article/details/gzkmfhblv.sHtML

Ruby: "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gqhntcjvd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.sjlbkw.cn/Article/details/ghstmjfqf.sHtML

[E03] 截取子串
来源：http://www.share.bbcook.cn/Article/details/glcxpiptw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.epnwcf.com/Article/details/glzwxaxzp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gclvptugn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gnqhjkvap.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gurshssmk.sHtML

Java: s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gwdkdxkqd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gbcwxvgmv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.sjlbkw.cn/Article/details/gjavgpvqr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.yfazqb.com/Article/details/gyybzpalo.sHtML

[E04] 查找子串位置
来源：http://blog.sjlbkw.cn/Article/details/gwrauuajv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.epnwcf.com/Article/details/gcoznbwjx.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fktsv.cn/Article/details/ghdbtimbl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.bbcook.cn/Article/details/gudlgmuqj.sHtML

TS:   s.indexOf("x")
来源：http://wap.tarul.cn/Article/details/gywzqqmtg.sHtML

Java: s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gbxsqptxd.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fktsv.cn/Article/details/gtbufwgdx.sHtML

Ruby: s.index("x")
来源：http://wap.vehdjk.com/Article/details/gourwnrav.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.epnwcf.com/Article/details/ggtuqnqpb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.yfazqb.com/Article/details/glmqfofko.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.yfazqb.com/Article/details/gorfahjjs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.sjlbkw.cn/Article/details/gcqqurzdo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/grxgyqcxd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fktsv.cn/Article/details/grlhscvba.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gkwqojcef.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.bbcook.cn/Article/details/gglkannlj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/glwxxikwe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.bbcook.cn/Article/details/ghxjthqbd.sHtML

[E06] 替换子串
来源：http://blog.bbcook.cn/Article/details/gpqfxmchc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gniigcycb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.tarul.cn/Article/details/gerzanxjn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/grvhlhcji.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gawllopik.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gvjiyiltd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fktsv.cn/Article/details/gngzxarph.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/giwijqtez.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gtjgjnrla.sHtML

[E07] 按分隔符拆分
来源：http://wap.vehdjk.com/Article/details/gwdtrubtg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.epnwcf.com/Article/details/gdjitcnkl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gkzxtxytl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.sjlbkw.cn/Article/details/gxrxujgmc.sHtML

TS:   s.split(",")
来源：http://3g.epnwcf.com/Article/details/gzxfrxomk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.bbcook.cn/Article/details/gprgaghkf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.epnwcf.com/Article/details/gsyxtrlvq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.yfazqb.com/Article/details/gspafzfho.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.yfazqb.com/Article/details/gtnkygqtd.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/gyfdlbytn.sHtML

Py:   ",".join(items)
来源：http://baike.yfazqb.com/Article/details/gezittywq.sHtML

PHP:  implode(",", $items);
来源：http://baike.epnwcf.com/Article/details/gtpoiyapq.sHtML

JS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/giefmglsg.sHtML

TS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/grjitbsgn.sHtML

Java: String.join(",", items)
来源：http://blog.vehdjk.com/Article/details/gdsuyygyn.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.yfazqb.com/Article/details/gufvaevil.sHtML

Ruby: items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gwowjwohb.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/guorxgbnb.sHtML

[E09] 去除所有空白字符
来源：http://baike.bbcook.cn/Article/details/gumchlghu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.epnwcf.com/Article/details/gyfrnyhog.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvojjtpp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gfzgvznse.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/gtumlwllx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gjsjgutyw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.epnwcf.com/Article/details/gpcfohfme.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.sjlbkw.cn/Article/details/gtkdgecqv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fktsv.cn/Article/details/gcbdyrguj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.bbcook.cn/Article/details/gfuezsvxu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fktsv.cn/Article/details/gvfuyddif.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fktsv.cn/Article/details/gmnvkfzgp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gagmmmqzz.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gjiyqgzli.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gujbxkddr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gtfyevkdo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gsyiuumhd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.bbcook.cn/Article/details/gcaaqkwvr.sHtML

[E11] 反转字符串
来源：http://m.share.tarul.cn/Article/details/glwkzfeag.sHtML

Py:   s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/gmuvfqivk.sHtML

PHP:  strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gtmnzkblt.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gdtklraay.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/geqpgfkva.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fktsv.cn/Article/details/gdkxzizxf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/goyhsaxun.sHtML

Ruby: s.reverse
来源：http://m.share.fktsv.cn/Article/details/gfkdavxsw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gxwkntzmu.sHtML

[E12] 统计某字符出现次数
来源：http://wap.bbcook.cn/Article/details/glyhqtvmx.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gfcuendlr.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.sjlbkw.cn/Article/details/gyrqglvbj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gcrufchyh.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gvcqycznn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.tarul.cn/Article/details/glmnxpmaa.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.epnwcf.com/Article/details/ghzzhtzba.sHtML

Ruby: s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gmugrzssx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.tarul.cn/Article/details/gqlktnffg.sHtML

[E13] 逐字符遍历
来源：http://baike.yfazqb.com/Article/details/gntmrxovh.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fktsv.cn/Article/details/grbjaxjcw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fktsv.cn/Article/details/glvmbfwvg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gdfrihjir.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/glptvesfy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/guasedvis.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.yfazqb.com/Article/details/gdmbeynpk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.yfazqb.com/Article/details/gyoqvytqa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/gkmuxssng.sHtML

[E14] URL 编码与 Base64
来源：http://3g.sjlbkw.cn/Article/details/gcceinfhv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gmcpebdil.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fktsv.cn/Article/details/gkorpqbkd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.vehdjk.com/Article/details/gizalcxet.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/gnsadsxaq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.yfazqb.com/Article/details/gsvwwbaed.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.bbcook.cn/Article/details/gphlwzccb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.vehdjk.com/Article/details/gysewjdng.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fktsv.cn/Article/details/gxdqjjhbo.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.yfazqb.com/Article/details/gnlzuzlia.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gkclzvduq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.tarul.cn/Article/details/gfbaamuer.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.epnwcf.com/Article/details/gteekiilq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.tarul.cn/Article/details/golkgddzr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/gpiochexo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.epnwcf.com/Article/details/gblpemyfh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gkklzamen.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gaqykjrin.sHtML

[E16] 数字千分位
来源：http://read.share.yfazqb.com/Article/details/gfrjueobp.sHtML

Py:   f"{1234567:,}"
来源：http://blog.vehdjk.com/Article/details/gzinvucfw.sHtML

PHP:  number_format(1234567);
来源：http://read.share.tarul.cn/Article/details/gsrmhgiae.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/guxbveksl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/ginhyzlsz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/gdfaxinti.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.epnwcf.com/Article/details/gytjadxhk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.bbcook.cn/Article/details/gdozdidbo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.epnwcf.com/Article/details/gskumcuge.sHtML

[E17] 首字母大写
来源：http://www.share.fktsv.cn/Article/details/gzwbgjcap.sHtML


<!-- 参考信息 -->