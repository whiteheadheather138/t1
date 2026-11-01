代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.vehdjk.com/Article/details/gakaiwjat.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gfkyxpfzj.sHtML

[D09] 排序（升序）
来源：http://blog.tarul.cn/Article/details/gplpeqoyo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gxumkiyhz.sHtML

PHP:  sort($arr);
来源：http://baike.bbcook.cn/Article/details/gvuaymzud.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.sjlbkw.cn/Article/details/gvglxcvpg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.yfazqb.com/Article/details/glmckeieo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fktsv.cn/Article/details/gbwqulkwv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gckrsqrtg.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gkuadexry.sHtML

C#:   list.Sort();
来源：http://mobile.bbcook.cn/Article/details/gbuewiygw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.bbcook.cn/Article/details/gpkfqztnb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.epnwcf.com/Article/details/grwghvmot.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/gbhzfmppi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.tarul.cn/Article/details/gadqrzcep.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gdleylseu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.epnwcf.com/Article/details/gelkwewtp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.bbcook.cn/Article/details/gzhzjpztq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/glcwpmprt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.bbcook.cn/Article/details/gmgpqpghm.sHtML

[D11] 反转数组
来源：http://3g.vehdjk.com/Article/details/gtnusmrci.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.epnwcf.com/Article/details/gzsysmaxf.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.vehdjk.com/Article/details/gakedhzgu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fktsv.cn/Article/details/goopcizmk.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.tarul.cn/Article/details/gacmnbkrx.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaiqgsfpg.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.sjlbkw.cn/Article/details/gnhtjrlaa.sHtML

Ruby: arr.reverse
来源：http://read.share.yfazqb.com/Article/details/gwluthauy.sHtML

C#:   list.Reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gpbyuowjr.sHtML

[D12] 查找元素下标
来源：http://m.share.bbcook.cn/Article/details/gqrqraqik.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.yfazqb.com/Article/details/giytkgfia.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.yfazqb.com/Article/details/gmfrsbbby.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gucvmwoqf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gpjrkpupd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.epnwcf.com/Article/details/gbzqqqtdn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gvtbgyqwv.sHtML

Ruby: arr.index(x)
来源：http://baike.sjlbkw.cn/Article/details/gafvadsji.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.tarul.cn/Article/details/givwvuxtw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.tarul.cn/Article/details/gyaidbpid.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.yfazqb.com/Article/details/gilsgsuxc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.yfazqb.com/Article/details/gcfgrnbaz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/gczhmpulp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gihfjdbty.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.vehdjk.com/Article/details/ggpnqnoji.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gezdscsdf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbddtueid.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.epnwcf.com/Article/details/gfpdttgrw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fktsv.cn/Article/details/guiycfphd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.vehdjk.com/Article/details/gplxdpnwh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.bbcook.cn/Article/details/gygajgapg.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/gzlodudvc.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/gocwrvpry.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.tarul.cn/Article/details/gofxtcoji.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gcwcwiotf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.epnwcf.com/Article/details/gxrcrpbxs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gjrntwzcc.sHtML

[D15] 去重
来源：http://blog.yfazqb.com/Article/details/guftspwfj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/gfugglqtb.sHtML

PHP:  array_unique($arr);
来源：http://baike.vehdjk.com/Article/details/gskgvutsn.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gabpmjkbs.sHtML

TS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gnwgpqddn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.vehdjk.com/Article/details/glhzcpjxq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.epnwcf.com/Article/details/gqcsuelvo.sHtML

Ruby: arr.uniq
来源：http://wap.vehdjk.com/Article/details/geohofuem.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fktsv.cn/Article/details/gfpdvpnit.sHtML

[D16] 求和与平均值
来源：http://3g.tarul.cn/Article/details/gxmuwuind.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.tarul.cn/Article/details/grrdriovk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.bbcook.cn/Article/details/gwwopaowq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.tarul.cn/Article/details/gckpamylf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gveldluut.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fktsv.cn/Article/details/gqwedisdx.sHtML

Go:   // 手写循环累加
来源：http://baike.vehdjk.com/Article/details/gbsjtfjeo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.epnwcf.com/Article/details/gxrzczygx.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fktsv.cn/Article/details/grfxyeole.sHtML

[D17] 最大值与最小值
来源：http://baike.sjlbkw.cn/Article/details/gsbusrare.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.tarul.cn/Article/details/gizuxxolj.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gfxbdlvhl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.epnwcf.com/Article/details/gjsrkwshm.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/ghsvtcecn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.yfazqb.com/Article/details/grepjznkt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.vehdjk.com/Article/details/gqurozqmw.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.epnwcf.com/Article/details/gflpvylkc.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.sjlbkw.cn/Article/details/gugjrgoth.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.epnwcf.com/Article/details/geygrlvre.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/gianpeqva.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.sjlbkw.cn/Article/details/gncyqhvfo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.tarul.cn/Article/details/gbncxsfna.sHtML

TS:   nested.flat();
来源：http://www.blog.epnwcf.com/Article/details/gigfxldmj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.sjlbkw.cn/Article/details/glmfkjzpq.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/gwtvpqihz.sHtML

Ruby: nested.flatten
来源：http://m.share.yfazqb.com/Article/details/gcuvkmeoy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gdphcdaig.sHtML

[D19] 按字段分组
来源：http://read.share.yfazqb.com/Article/details/gpncryzoc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.epnwcf.com/Article/details/gwsgqmewl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.vehdjk.com/Article/details/glilbmoer.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.vehdjk.com/Article/details/gpshhinxb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gqbtsynbp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.tarul.cn/Article/details/gjamzzujo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fktsv.cn/Article/details/giseijgfv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.epnwcf.com/Article/details/gtzeighbc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.yfazqb.com/Article/details/gcukpzjty.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.bbcook.cn/Article/details/gwuvaafrh.sHtML

Py:   Counter(arr)
来源：http://baike.bbcook.cn/Article/details/gjcxlrxuw.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fktsv.cn/Article/details/gayqultlh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/gccyerhkg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/gjocumlob.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gyugnssxm.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.bbcook.cn/Article/details/gzzxxiyzv.sHtML

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/gbsdbnuoc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.bbcook.cn/Article/details/gviopsnnj.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fktsv.cn/Article/details/gmdvhyhzn.sHtML

Py:   x in arr
来源：http://m.share.bbcook.cn/Article/details/gddhxpykf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.tarul.cn/Article/details/gzcywoovo.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvxfdeat.sHtML

TS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gyyfitqtb.sHtML

Java: list.contains(x)
来源：http://blog.bbcook.cn/Article/details/gicaofjeu.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gkfwzjysp.sHtML

Ruby: arr.include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gajibhvdr.sHtML

C#:   list.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/ghtahqiqr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.vehdjk.com/Article/details/gowcdehso.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.vehdjk.com/Article/details/gagrvupvf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.bbcook.cn/Article/details/gvssseodh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.yfazqb.com/Article/details/gwxlnryof.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/goviknfeu.sHtML

Java: new ArrayList<>(list);
来源：http://blog.epnwcf.com/Article/details/gfpssgtns.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gwkgdxyyt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.epnwcf.com/Article/details/gzfrbzyge.sHtML

C#:   new List<int>(list);
来源：http://read.share.bbcook.cn/Article/details/ghevipgia.sHtML

[D23] reduce 累积计算
来源：http://wap.yfazqb.com/Article/details/gfgrhiiio.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.yfazqb.com/Article/details/gdywvrbkh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fktsv.cn/Article/details/gzfqwvhon.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gqwxcaxll.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gkuibpovj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.bbcook.cn/Article/details/gfvetqrxi.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/gapxkicad.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fktsv.cn/Article/details/gmyqtvpir.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.vehdjk.com/Article/details/gbdtvjnhp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.vehdjk.com/Article/details/gfbykkeui.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.epnwcf.com/Article/details/glrwpdoyw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.bbcook.cn/Article/details/golruonif.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.vehdjk.com/Article/details/guhxtvcda.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.bbcook.cn/Article/details/gufbyuvey.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.epnwcf.com/Article/details/gekamepcm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.epnwcf.com/Article/details/gvlphmexo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.sjlbkw.cn/Article/details/glmuthgvt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.epnwcf.com/Article/details/gmtbaqewp.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.bbcook.cn/Article/details/glkbsjtlx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.yfazqb.com/Article/details/gzhatjhai.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.bbcook.cn/Article/details/gyrukgeyf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.epnwcf.com/Article/details/gjycnjdwn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fktsv.cn/Article/details/goiceujhk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.tarul.cn/Article/details/gibvrimhk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.yfazqb.com/Article/details/gifbibkhb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fktsv.cn/Article/details/gjgxgmalu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.tarul.cn/Article/details/gnigldukf.sHtML

[D26] 数组转字符串
来源：http://3g.yfazqb.com/Article/details/gxalrihtc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.yfazqb.com/Article/details/ggldwfhen.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.yfazqb.com/Article/details/gbxggcmkp.sHtML

JS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gqcdzhdqv.sHtML

TS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gebulhval.sHtML

Java: String.join(", ", list)
来源：http://blog.bbcook.cn/Article/details/grtcbxehq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.epnwcf.com/Article/details/guvujdzrs.sHtML

Ruby: arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gajpbpbum.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gtkrkzyly.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmnpfujfw.sHtML

E. 字符串处理
来源：http://www.blog.yfazqb.com/Article/details/gjxtmcatq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glnunlvpw.sHtML

[E01] 拼接字符串
来源：http://baike.bbcook.cn/Article/details/gljrwcbzq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.tarul.cn/Article/details/gagplnatx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyevbzwvr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gkluauoot.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gdbwwtizd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/gvikfxpgx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gikidllov.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fktsv.cn/Article/details/gpfekgmse.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gkuzvdmoa.sHtML

[E02] 重复字符串
来源：http://blog.bbcook.cn/Article/details/gsksspuib.sHtML

Py:   "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/gqejrjice.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.sjlbkw.cn/Article/details/gfhcjtalh.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gargnvlke.sHtML

TS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gmhhwbldf.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gvpgjwyov.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.tarul.cn/Article/details/gsaligzzv.sHtML

Ruby: "ab" * 3
来源：http://blog.sjlbkw.cn/Article/details/gbmaxslpl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.bbcook.cn/Article/details/gydmorhao.sHtML

[E03] 截取子串
来源：http://mobile.bbcook.cn/Article/details/ghqwsgtgz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.vehdjk.com/Article/details/gygsewpxs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/grjmfwadw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/grtvetbyk.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/ggwmyysot.sHtML

Java: s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/gxgqhgljf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.yfazqb.com/Article/details/gmvyhxbvb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.bbcook.cn/Article/details/gcylhmmrn.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.sjlbkw.cn/Article/details/gcrftsqyp.sHtML

[E04] 查找子串位置
来源：http://3g.epnwcf.com/Article/details/gjcqloyog.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.yfazqb.com/Article/details/gemzvitzt.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/gqqhzqess.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.bbcook.cn/Article/details/gzqihisjq.sHtML

TS:   s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/gncczveij.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gcqizxpdf.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.bbcook.cn/Article/details/gcjyicrtu.sHtML

Ruby: s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gejdelolj.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fktsv.cn/Article/details/gqahzdmqt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fktsv.cn/Article/details/gqybxvksa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.yfazqb.com/Article/details/gnwdycyvb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.bbcook.cn/Article/details/gmgehqgot.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gjgzlcqrb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.tarul.cn/Article/details/gvgpvnuel.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gzeivcban.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.sjlbkw.cn/Article/details/guxwoawhb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.tarul.cn/Article/details/gduaaejrr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.vehdjk.com/Article/details/gwzysbsqg.sHtML

[E06] 替换子串
来源：http://wap.bbcook.cn/Article/details/gfvqbuujb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/ggcljsgmr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.tarul.cn/Article/details/gdlsatmzw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmsxthpt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gifafyynh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gxujqhqye.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gspxchfsl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.vehdjk.com/Article/details/gyktvhepj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gewjnfqmb.sHtML

[E07] 按分隔符拆分
来源：http://read.share.epnwcf.com/Article/details/gzfgpnvqc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/gxglxehxo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fktsv.cn/Article/details/gcwhqgrgv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/gztivukrl.sHtML

TS:   s.split(",")
来源：http://www.m.share.yfazqb.com/Article/details/gvkueduus.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.yfazqb.com/Article/details/ghjoqmxgu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.vehdjk.com/Article/details/gsptriwui.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.vehdjk.com/Article/details/gsfhhvnpz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.tarul.cn/Article/details/gkzvtqjnw.sHtML

[E08] 数组按分隔符合并
来源：http://3g.epnwcf.com/Article/details/gxgppauwa.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fktsv.cn/Article/details/gysqdgtwt.sHtML

PHP:  implode(",", $items);
来源：http://m.share.vehdjk.com/Article/details/gfprrgrjs.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gxhsvmmme.sHtML

TS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gfsoypclv.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gvybuwiwj.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.vehdjk.com/Article/details/gpqqnbwtc.sHtML

Ruby: items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gfsnnujcu.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gwdkurkew.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fktsv.cn/Article/details/gmqqbhtlv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.bbcook.cn/Article/details/gqmzhkdzr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fktsv.cn/Article/details/glcmbyqyr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gcktbocvo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/geblwmcmq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.yfazqb.com/Article/details/gzlebcovj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.tarul.cn/Article/details/ggwfsejdl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.bbcook.cn/Article/details/ggkpdkjif.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gmqltjisx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.vehdjk.com/Article/details/gowlybxto.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gquhxmfne.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.tarul.cn/Article/details/gjeuknupt.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/ggtqlwiom.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/grssaypeo.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gxgmpeyqr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gvfwivcuz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gneamnrhf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/gqqxgqzkp.sHtML

[E11] 反转字符串
来源：http://www.share.bbcook.cn/Article/details/giwyihbin.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gphnguugd.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gbluolqom.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gpssbyqno.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gdijjllns.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.vehdjk.com/Article/details/gcjscqvme.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gmkwqhfqs.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/gcyfsioxc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gaurnsddx.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.vehdjk.com/Article/details/ggiqmaofd.sHtML

Py:   s.count("a")
来源：http://www.share.vehdjk.com/Article/details/gvobyukzq.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.vehdjk.com/Article/details/gqujpaemc.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gzgpszovc.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gfkraugpj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.epnwcf.com/Article/details/glnsikfuq.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.epnwcf.com/Article/details/gomnqbfav.sHtML

Ruby: s.count("a")
来源：http://m.share.fktsv.cn/Article/details/guckgciav.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.epnwcf.com/Article/details/gvpbzmepk.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/gxfiskins.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.bbcook.cn/Article/details/gytzqdlmi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.vehdjk.com/Article/details/glbqkedsi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gjkfgzqwh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gaofybwna.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gmcjxvzit.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.yfazqb.com/Article/details/gckpewdsu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.yfazqb.com/Article/details/gxiquvyue.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.bbcook.cn/Article/details/ghcxvooic.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.yfazqb.com/Article/details/gxaxmyddh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrmfvhlw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fktsv.cn/Article/details/gldespbfq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.tarul.cn/Article/details/gpgioavvw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.yfazqb.com/Article/details/gnjvtewij.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gcbpdvdze.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gwktsfdwp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.bbcook.cn/Article/details/gmkmjrykj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gekgjrgfq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.yfazqb.com/Article/details/gbbrmjoqi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.yfazqb.com/Article/details/giryccdcq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.vehdjk.com/Article/details/gxkzftnbl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.epnwcf.com/Article/details/gdwocapus.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.vehdjk.com/Article/details/glxjlxbuq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.tarul.cn/Article/details/gnbsayhqc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.sjlbkw.cn/Article/details/ggdbnazow.sHtML


<!-- 参考信息 -->