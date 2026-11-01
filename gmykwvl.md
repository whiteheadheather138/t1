代发 wailian999

PHP:  sort($arr);
来源：http://m.share.epnwcf.com/Article/details/gqlcxkgmz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gqhipyqge.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.bbcook.cn/Article/details/gvqcfaxzr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.epnwcf.com/Article/details/gizopjhui.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gaisjbghi.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/ghsoxqtyf.sHtML

C#:   list.Sort();
来源：http://wap.tarul.cn/Article/details/gtsvtrxps.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/gcotfauhs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.tarul.cn/Article/details/gwczqtzsv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/gmbcyolrt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gglblproe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/goveubmoh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/gnwwqkvcp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fktsv.cn/Article/details/gaaycnlxw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.yfazqb.com/Article/details/ghdjzhzsy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.tarul.cn/Article/details/gzyoqbvok.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/ggiufepdg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.vehdjk.com/Article/details/grfxdoozp.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/gdewyhhcu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.bbcook.cn/Article/details/gswshzvjk.sHtML

TS:   [...arr].reverse();
来源：http://wap.bbcook.cn/Article/details/gpkliefoo.sHtML

Java: Collections.reverse(list);
来源：http://www.share.sjlbkw.cn/Article/details/glnwhtcfd.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.yfazqb.com/Article/details/gtowtvlud.sHtML

Ruby: arr.reverse
来源：http://www.share.tarul.cn/Article/details/gofbsqdzf.sHtML

C#:   list.Reverse();
来源：http://m.share.fktsv.cn/Article/details/grzqxxbud.sHtML

[D12] 查找元素下标
来源：http://baike.bbcook.cn/Article/details/gmanuheue.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.tarul.cn/Article/details/gtjizeopn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gotjaxixc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/gyrvnezdj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gbzluvbrs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fktsv.cn/Article/details/gfejllcmq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gjhqbfpgt.sHtML

Ruby: arr.index(x)
来源：http://m.share.yfazqb.com/Article/details/gvgoqgiqw.sHtML

C#:   list.IndexOf(x);
来源：http://3g.bbcook.cn/Article/details/gasltmzeo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.yfazqb.com/Article/details/gtaekhcbz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrbooyrg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.vehdjk.com/Article/details/gayihpkoe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/glzdbcycx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/glugqzcnb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.epnwcf.com/Article/details/gmndcofzu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.tarul.cn/Article/details/gymxiyjzv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.yfazqb.com/Article/details/gcvmodnwq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.yfazqb.com/Article/details/ggqectvjf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.epnwcf.com/Article/details/gsfypxdor.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.sjlbkw.cn/Article/details/gyfsnebay.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.bbcook.cn/Article/details/gyyjjharu.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gtkvwpekh.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gkkqvwotx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.tarul.cn/Article/details/gtssdhnzi.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gfgdfpjcj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.bbcook.cn/Article/details/gryubkvvc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/ggvpcacua.sHtML

[D15] 去重
来源：http://read.share.epnwcf.com/Article/details/gtetyfdvn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gjbkrnfll.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.epnwcf.com/Article/details/gnqipocii.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/giodntoie.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gjnpadhtv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.tarul.cn/Article/details/gkadnsndb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.sjlbkw.cn/Article/details/gbzyziika.sHtML

Ruby: arr.uniq
来源：http://baike.fktsv.cn/Article/details/gzgcxpavs.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.vehdjk.com/Article/details/gkgjspszm.sHtML

[D16] 求和与平均值
来源：http://m.share.epnwcf.com/Article/details/gzuignttn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.tarul.cn/Article/details/gzctrrmsi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.yfazqb.com/Article/details/gjwewewqm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gfeyybzyl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdhzuhnb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.epnwcf.com/Article/details/gvoobwgox.sHtML

Go:   // 手写循环累加
来源：http://wap.vehdjk.com/Article/details/gymgcrfqg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.bbcook.cn/Article/details/glsxbztef.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fktsv.cn/Article/details/gwqkrknut.sHtML

[D17] 最大值与最小值
来源：http://wap.vehdjk.com/Article/details/gbaqunqhb.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.tarul.cn/Article/details/gfvgkpzuh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/glnzjsnsz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/gxlmnfkbq.sHtML

TS:   Math.max(...arr);
来源：http://read.share.vehdjk.com/Article/details/ggxcwtcnv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.bbcook.cn/Article/details/gqylfxuum.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.yfazqb.com/Article/details/gejmgdcib.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.yfazqb.com/Article/details/gjrsukmgb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.yfazqb.com/Article/details/gonwryszj.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.epnwcf.com/Article/details/gspjvrpjo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.yfazqb.com/Article/details/gzcnvmzwj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.vehdjk.com/Article/details/ghddbmjmc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fktsv.cn/Article/details/gvzyeuivz.sHtML

TS:   nested.flat();
来源：http://www.m.share.epnwcf.com/Article/details/grhaxpvks.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.vehdjk.com/Article/details/gmzjrmifp.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.bbcook.cn/Article/details/gfihztvwo.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gfmssshuk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.vehdjk.com/Article/details/gdmvnslbj.sHtML

[D19] 按字段分组
来源：http://m.share.epnwcf.com/Article/details/gximhqnbf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/glupmsslv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fktsv.cn/Article/details/gsumaedni.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.tarul.cn/Article/details/gmhxmuqli.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/glmzmcenm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.yfazqb.com/Article/details/giqnouxue.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.sjlbkw.cn/Article/details/gkvxurtst.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.bbcook.cn/Article/details/gpfanilra.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.vehdjk.com/Article/details/gexepetst.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.vehdjk.com/Article/details/gqdkpgvrb.sHtML

Py:   Counter(arr)
来源：http://wap.bbcook.cn/Article/details/gbulrxwla.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.tarul.cn/Article/details/gznnrlugv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/glwgcfhck.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gwkipsmmv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.vehdjk.com/Article/details/gxdnrzdpf.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.sjlbkw.cn/Article/details/ghjdmgedq.sHtML

Ruby: arr.tally
来源：http://m.share.bbcook.cn/Article/details/gahriyqbg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.epnwcf.com/Article/details/gimweupvi.sHtML

[D21] 判断是否包含某元素
来源：http://wap.yfazqb.com/Article/details/grfrnimwz.sHtML

Py:   x in arr
来源：http://read.share.yfazqb.com/Article/details/gxjbiepmf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.bbcook.cn/Article/details/gmxarvscj.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/giptxuoac.sHtML

TS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gvnueomkn.sHtML

Java: list.contains(x)
来源：http://mobile.yfazqb.com/Article/details/gdavvccqm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gxkmdcjdo.sHtML

Ruby: arr.include?(x)
来源：http://blog.epnwcf.com/Article/details/gnbugzcuk.sHtML

C#:   list.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gmewlcrnc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.yfazqb.com/Article/details/gcguppvhg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.bbcook.cn/Article/details/gjvsfynxu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.tarul.cn/Article/details/gprggabwc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/gkssgjkih.sHtML

TS:   [...arr];
来源：http://wap.vehdjk.com/Article/details/gastzdzen.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gedwmugrn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.bbcook.cn/Article/details/gkldvalvl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.epnwcf.com/Article/details/glewcgush.sHtML

C#:   new List<int>(list);
来源：http://baike.vehdjk.com/Article/details/gkmiuvphi.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/glniwmeuz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.tarul.cn/Article/details/gctdatykx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.epnwcf.com/Article/details/gcypzwhfp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gmmwsoatc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/gjinkgpps.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.bbcook.cn/Article/details/gsjjltlst.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gtbwokmeq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.tarul.cn/Article/details/gpaczkwwi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.vehdjk.com/Article/details/gseslptav.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fktsv.cn/Article/details/ggvwpncxl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.vehdjk.com/Article/details/gkbugnlkt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.epnwcf.com/Article/details/gkxxlnrxu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gkxypysmo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gnsgacbbl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.vehdjk.com/Article/details/giswatzng.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.sjlbkw.cn/Article/details/gfcbcrgog.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.yfazqb.com/Article/details/gnizczilx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.epnwcf.com/Article/details/gpeferwus.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.sjlbkw.cn/Article/details/guykyvwmn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.sjlbkw.cn/Article/details/gfmarmeic.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.yfazqb.com/Article/details/gptjxvorh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fktsv.cn/Article/details/gswgrtjhi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.tarul.cn/Article/details/gwpnzowtv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.epnwcf.com/Article/details/gelbizaiw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.tarul.cn/Article/details/ghujvghmf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.sjlbkw.cn/Article/details/gfrgceumq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gdwkwzcys.sHtML

[D26] 数组转字符串
来源：http://www.blog.bbcook.cn/Article/details/golmmjfnt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/gfewlysmx.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.sjlbkw.cn/Article/details/gysheyivi.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gpdhylnee.sHtML

TS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/guseewdaq.sHtML

Java: String.join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gqwgvtezr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.tarul.cn/Article/details/gwsidbqqq.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gwsdrtrgv.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fktsv.cn/Article/details/gkkkqxsxu.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/groktsuqg.sHtML

E. 字符串处理
来源：http://www.share.vehdjk.com/Article/details/gabkazxzg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbakeuwxj.sHtML

[E01] 拼接字符串
来源：http://baike.epnwcf.com/Article/details/gjjqdjlim.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fktsv.cn/Article/details/guxgvqork.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.sjlbkw.cn/Article/details/gbdgvvjzy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.yfazqb.com/Article/details/gtussdzqf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gprbanarh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.tarul.cn/Article/details/gllnxkund.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/ghyztnhjj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.tarul.cn/Article/details/ghbjjfjip.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gzdgdrjkp.sHtML

[E02] 重复字符串
来源：http://www.blog.yfazqb.com/Article/details/grwhuetbk.sHtML

Py:   "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/gdgtdnusr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.vehdjk.com/Article/details/gmssvkafa.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gycuycgsc.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gcemgmhzx.sHtML

Java: "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gdlzrfptw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.sjlbkw.cn/Article/details/gbgeuejeq.sHtML

Ruby: "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gsoupaqgw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.sjlbkw.cn/Article/details/gxsbdiukv.sHtML

[E03] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gquaftfhq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.yfazqb.com/Article/details/gnzqmelof.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/grqvoyefs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/giutynooh.sHtML

TS:   s.slice(1, 4)
来源：http://wap.yfazqb.com/Article/details/gtcwqmqxc.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gtlpptoam.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fktsv.cn/Article/details/gjqetxykz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.yfazqb.com/Article/details/gyddnpprz.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.bbcook.cn/Article/details/gpckzrtrz.sHtML

[E04] 查找子串位置
来源：http://www.share.sjlbkw.cn/Article/details/gejrsmfon.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gjspzwfdo.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.tarul.cn/Article/details/gsabcvhic.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.yfazqb.com/Article/details/gidzetzch.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gedzsjipy.sHtML

Java: s.indexOf("x")
来源：http://blog.bbcook.cn/Article/details/gvdsyzngo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.yfazqb.com/Article/details/gjgmkkdqy.sHtML

Ruby: s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gxexclszc.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gxuzxbvbo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.yfazqb.com/Article/details/ggelxscdt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.tarul.cn/Article/details/gvszkijvd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.epnwcf.com/Article/details/gecuaarba.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/ggnepvsgi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.yfazqb.com/Article/details/gwytonnux.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gqcwdjyvk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/gyubymanh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.yfazqb.com/Article/details/ghbjfasor.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gffgtudtf.sHtML

[E06] 替换子串
来源：http://3g.yfazqb.com/Article/details/gujqqgolc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gttzaztyg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fktsv.cn/Article/details/ggioqjbyl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gdjxppzto.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/ghkowukqt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gyzogdlav.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/ghcjlukrz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gswyirdcv.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.tarul.cn/Article/details/gfyqxfflx.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fktsv.cn/Article/details/ggcpirgvr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.tarul.cn/Article/details/gspwmbcgu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gvsfpzhyb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/gsxjfnblb.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/gddaluhnf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/geombwnnu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.bbcook.cn/Article/details/gqioppngd.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fktsv.cn/Article/details/gbbrqjqpx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.tarul.cn/Article/details/gnxkdlmvu.sHtML

[E08] 数组按分隔符合并
来源：http://baike.epnwcf.com/Article/details/gblllqcul.sHtML

Py:   ",".join(items)
来源：http://www.share.tarul.cn/Article/details/gvgwcdxfd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/gngaucwvb.sHtML

JS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/gxiwihcpe.sHtML

TS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gsnbliued.sHtML

Java: String.join(",", items)
来源：http://wap.yfazqb.com/Article/details/gqyigeoxp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.epnwcf.com/Article/details/glnutrisb.sHtML

Ruby: items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gkbywyffd.sHtML

C#:   string.Join(",", items)
来源：http://blog.vehdjk.com/Article/details/gfqbricld.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.vehdjk.com/Article/details/gzawnxsjz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.bbcook.cn/Article/details/gndzvlqrz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.vehdjk.com/Article/details/gykefrvwf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/girfwiorw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gntwgnxfb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gigdphxeo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.yfazqb.com/Article/details/gcjqkmbbc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.epnwcf.com/Article/details/gixzqbiqt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/gdtlylinz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/guhvwqpzv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.bbcook.cn/Article/details/gzztsgtsf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/gchapzoag.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gcalmocur.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gktrauxtx.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gcmeojrcw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gbwwcupds.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gknagrowk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/gebjdpohq.sHtML

[E11] 反转字符串
来源：http://read.share.yfazqb.com/Article/details/gxbjuuucw.sHtML

Py:   s[::-1]
来源：http://3g.bbcook.cn/Article/details/gobfvukkl.sHtML

PHP:  strrev($s);
来源：http://baike.bbcook.cn/Article/details/giszelhqt.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gdpvbypvc.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gsfznwura.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.sjlbkw.cn/Article/details/gtopuyfdq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/gewkinkpd.sHtML

Ruby: s.reverse
来源：http://baike.yfazqb.com/Article/details/grkvipzfn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/gfjxbovuy.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.vehdjk.com/Article/details/giillfaqu.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gizkcbssc.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/gybbfoxkj.sHtML

JS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/grdftwnsk.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gfcazuvwt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/giqzedhte.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fktsv.cn/Article/details/gotayiulf.sHtML

Ruby: s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gddybqiig.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.tarul.cn/Article/details/gnxjzdddc.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fktsv.cn/Article/details/gosenhbpt.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gpvptqtsd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.tarul.cn/Article/details/grznkjeku.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.vehdjk.com/Article/details/gcmayufvh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/geixlyiib.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.bbcook.cn/Article/details/gmyxmemcw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fktsv.cn/Article/details/gmfectiyy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.yfazqb.com/Article/details/gmutdkrfo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.bbcook.cn/Article/details/gbsgdcagp.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/ggoafvqxb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.bbcook.cn/Article/details/gkeytgqya.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.sjlbkw.cn/Article/details/gxlyvsnkz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fktsv.cn/Article/details/giaehhcpa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.sjlbkw.cn/Article/details/gspporlle.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gvqxbostu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.sjlbkw.cn/Article/details/gljgyhygl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/goxnjmjzv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.epnwcf.com/Article/details/gzqrycgbt.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.vehdjk.com/Article/details/ghlqbfnob.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gedqmbswp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.bbcook.cn/Article/details/gdstavfrw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/gvvqpujyd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.bbcook.cn/Article/details/gdpgabkeu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.epnwcf.com/Article/details/gwyqhxkiv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.bbcook.cn/Article/details/gdxkuqiab.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/gzocgmbfq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gnrmrlenl.sHtML

[E16] 数字千分位
来源：http://3g.bbcook.cn/Article/details/ggizdhgwn.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.sjlbkw.cn/Article/details/grfcnebee.sHtML


<!-- 参考信息 -->