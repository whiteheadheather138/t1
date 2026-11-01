代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gnhqwvcqc.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/ghbbkbfzr.sHtML

C#:   list.Sort();
来源：http://mobile.fktsv.cn/Article/details/goplatgnx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/gvblwqvlh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.yfazqb.com/Article/details/gxieszktg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gmnjiywee.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.epnwcf.com/Article/details/gtsiczrze.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gzipeprrw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.tarul.cn/Article/details/gihgdzlko.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fktsv.cn/Article/details/gebirkqih.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.tarul.cn/Article/details/gwfqbmgur.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.vehdjk.com/Article/details/gblrqfvuf.sHtML

[D11] 反转数组
来源：http://baike.tarul.cn/Article/details/gigmoogcp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.tarul.cn/Article/details/gjbzfjcxy.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gthfosmal.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.epnwcf.com/Article/details/gierrytvl.sHtML

TS:   [...arr].reverse();
来源：http://3g.bbcook.cn/Article/details/gyhutvouw.sHtML

Java: Collections.reverse(list);
来源：http://blog.epnwcf.com/Article/details/gzxoyolmf.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.yfazqb.com/Article/details/gnywwchqf.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fktsv.cn/Article/details/goopmzzkq.sHtML

C#:   list.Reverse();
来源：http://mobile.bbcook.cn/Article/details/gczvugxyi.sHtML

[D12] 查找元素下标
来源：http://baike.vehdjk.com/Article/details/glgithucu.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.tarul.cn/Article/details/gbzqrwjgm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.epnwcf.com/Article/details/gbruncrlx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gjuhqobmf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/gcebbzksq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.sjlbkw.cn/Article/details/gjgqgazrk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gnicdqktm.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.tarul.cn/Article/details/gavjgzeju.sHtML

C#:   list.IndexOf(x);
来源：http://baike.yfazqb.com/Article/details/guqiwebos.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.epnwcf.com/Article/details/gmvswgbpi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fktsv.cn/Article/details/grmzafxbt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fktsv.cn/Article/details/gpcgbajwv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fktsv.cn/Article/details/grorypfvg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/ghstadici.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.epnwcf.com/Article/details/ghboqmqto.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.tarul.cn/Article/details/gzmembxgd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.yfazqb.com/Article/details/gnxyxzjcg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gwxwpcpkr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.sjlbkw.cn/Article/details/gyblxydqw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.tarul.cn/Article/details/gvnbxwlxa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.epnwcf.com/Article/details/gkyhixwex.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fktsv.cn/Article/details/gjcobngoo.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gjgfujfug.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gducfycql.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/gssykimfp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.yfazqb.com/Article/details/gssczhfmg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.vehdjk.com/Article/details/gncdepsvt.sHtML

[D15] 去重
来源：http://www.share.bbcook.cn/Article/details/gcrhfmntl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gbpmymtte.sHtML

PHP:  array_unique($arr);
来源：http://read.share.bbcook.cn/Article/details/gvzevunve.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gfccmmpqv.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/glbuhyvcp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.vehdjk.com/Article/details/gaiujbfxb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.sjlbkw.cn/Article/details/gnwvosifw.sHtML

Ruby: arr.uniq
来源：http://www.blog.vehdjk.com/Article/details/guqragzaf.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.epnwcf.com/Article/details/gbkpjbrzr.sHtML

[D16] 求和与平均值
来源：http://3g.bbcook.cn/Article/details/gljyyzpxx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.vehdjk.com/Article/details/geaewbxdr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.epnwcf.com/Article/details/grckgsfan.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.vehdjk.com/Article/details/gmkyggfdb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gubdqjorv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gbrpkgmjt.sHtML

Go:   // 手写循环累加
来源：http://blog.yfazqb.com/Article/details/gtdnaawxr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/gowlbbpgo.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.yfazqb.com/Article/details/gdmtxvgst.sHtML

[D17] 最大值与最小值
来源：http://3g.vehdjk.com/Article/details/geytfvwft.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.tarul.cn/Article/details/ggbepblid.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.yfazqb.com/Article/details/gfhtrcupj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fktsv.cn/Article/details/gtytidnpe.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gaqsileby.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/gecjsyjqh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.epnwcf.com/Article/details/gpaobszib.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.epnwcf.com/Article/details/gkkirchbk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.bbcook.cn/Article/details/gqmcmcacp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.sjlbkw.cn/Article/details/gpicdqnjm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/gqegltjiu.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fktsv.cn/Article/details/gvktwixag.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.epnwcf.com/Article/details/gpppisjxa.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gdsybpazo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.vehdjk.com/Article/details/giypauftu.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/gkjwyosny.sHtML

Ruby: nested.flatten
来源：http://3g.yfazqb.com/Article/details/gzainhfrp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.yfazqb.com/Article/details/gnbhfdwat.sHtML

[D19] 按字段分组
来源：http://blog.bbcook.cn/Article/details/gvodegyoe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.sjlbkw.cn/Article/details/gckbbschr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fktsv.cn/Article/details/gedgnatfi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fktsv.cn/Article/details/ghtbtxorz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gicrbjode.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fktsv.cn/Article/details/gdgqsjsqv.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.epnwcf.com/Article/details/gwdsxyihl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.sjlbkw.cn/Article/details/gvbniriwm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.epnwcf.com/Article/details/gpzfsvayn.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/glacbznmv.sHtML

Py:   Counter(arr)
来源：http://read.share.vehdjk.com/Article/details/gnsjgxuna.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/gtsagxpxp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gikqfqoqu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gzmqokjqa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.epnwcf.com/Article/details/grbfhlxjn.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/gfblmjdfx.sHtML

Ruby: arr.tally
来源：http://blog.vehdjk.com/Article/details/goagpeatk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gruouvtfi.sHtML

[D21] 判断是否包含某元素
来源：http://baike.yfazqb.com/Article/details/gkenznbhx.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/gpxwczszt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.bbcook.cn/Article/details/gyuyyccgp.sHtML

JS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gyapygife.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gjyojamtd.sHtML

Java: list.contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuxqlfze.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.vehdjk.com/Article/details/gqevkzudo.sHtML

Ruby: arr.include?(x)
来源：http://read.share.epnwcf.com/Article/details/gjtxiwlwh.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/grfggdnmy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.sjlbkw.cn/Article/details/gybyyubjy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.vehdjk.com/Article/details/gtgdrmjyd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/gqbukxfmb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gdglthfuc.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/gqkkeowgf.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/gladgdufz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/gbtdkqzyr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.yfazqb.com/Article/details/gviixgoer.sHtML

C#:   new List<int>(list);
来源：http://www.blog.yfazqb.com/Article/details/gnbycjzyd.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/gglsfdoef.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fktsv.cn/Article/details/gspsgdygl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gazkgzsmr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/grviizphg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gzdhyiwwz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fktsv.cn/Article/details/ghdfzuqco.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gjggfdbha.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.sjlbkw.cn/Article/details/gqjbokumr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/gjvhahcgl.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.yfazqb.com/Article/details/grltasksa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fktsv.cn/Article/details/gxnfsywkk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.yfazqb.com/Article/details/gcgrmvkxh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.vehdjk.com/Article/details/gcgmgsapu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gjvrtbjwe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.tarul.cn/Article/details/gyknoxuqo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.yfazqb.com/Article/details/gsmpsmwmt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.yfazqb.com/Article/details/grsvvxtgv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.bbcook.cn/Article/details/gmqiidgxy.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.tarul.cn/Article/details/goxwcbnbh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.bbcook.cn/Article/details/gqmgscttw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.vehdjk.com/Article/details/gegcauxkx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.bbcook.cn/Article/details/grhuefjsx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.bbcook.cn/Article/details/gcrtbrjen.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gvcveexqh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.vehdjk.com/Article/details/gmadvvptq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fktsv.cn/Article/details/gbcqqwzef.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.vehdjk.com/Article/details/gvrnulmee.sHtML

[D26] 数组转字符串
来源：http://m.share.yfazqb.com/Article/details/gmgjxasff.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.bbcook.cn/Article/details/gxeqhppve.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.yfazqb.com/Article/details/gheyexadb.sHtML

JS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gydbscizm.sHtML

TS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gtvapdbsd.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/gsllhmocs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.yfazqb.com/Article/details/giexvlffn.sHtML

Ruby: arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gqpunjitb.sHtML

C#:   string.Join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gtvdrkqjc.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtfssctmt.sHtML

E. 字符串处理
来源：http://baike.sjlbkw.cn/Article/details/ghtbndhdo.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gsgxblhyk.sHtML

[E01] 拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/grrlncdmb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.tarul.cn/Article/details/grcekcknj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.sjlbkw.cn/Article/details/gosrmwavi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gkadnubgh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gegpyojcc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fktsv.cn/Article/details/gdnpsvieb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.vehdjk.com/Article/details/gysuxhjpg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fktsv.cn/Article/details/gdiqdvwel.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.tarul.cn/Article/details/gqzwllufy.sHtML

[E02] 重复字符串
来源：http://www.blog.vehdjk.com/Article/details/geiabzmhf.sHtML

Py:   "ab" * 3
来源：http://blog.sjlbkw.cn/Article/details/gulyiqyvm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/grtpmisiu.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gfptapihf.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyoktbym.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gkogowywu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/gggehowvi.sHtML

Ruby: "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/gonfbgmib.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fktsv.cn/Article/details/gyjfqrghs.sHtML

[E03] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gjwjnnadn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fktsv.cn/Article/details/gtqgwwfdd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gwwezrrlm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/grqdphdel.sHtML

TS:   s.slice(1, 4)
来源：http://baike.yfazqb.com/Article/details/gsdqcomcd.sHtML

Java: s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/gbgmvhmwq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.yfazqb.com/Article/details/geoafnsfo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.sjlbkw.cn/Article/details/gxltlztvd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fktsv.cn/Article/details/gymfcwgxc.sHtML

[E04] 查找子串位置
来源：http://blog.bbcook.cn/Article/details/grllgsdtb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.epnwcf.com/Article/details/gpqcnrtzu.sHtML

PHP:  strpos($s, "x");
来源：http://baike.vehdjk.com/Article/details/gjobishqf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.sjlbkw.cn/Article/details/glwgenuoh.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/grqvduhcy.sHtML

Java: s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/glpmtlnia.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fktsv.cn/Article/details/gbzmswgnl.sHtML

Ruby: s.index("x")
来源：http://read.share.fktsv.cn/Article/details/gitzibqvh.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gffvwawye.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.yfazqb.com/Article/details/gwyofuhdt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.bbcook.cn/Article/details/geaovbrie.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.sjlbkw.cn/Article/details/goiuphmwt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gclxybwxd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.tarul.cn/Article/details/gvrcsxpso.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gwlbrzzdw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.tarul.cn/Article/details/gaqmjlciv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/grkowhegb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gmsjhbmhe.sHtML

[E06] 替换子串
来源：http://read.share.fktsv.cn/Article/details/gsqsukeul.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/gtzyisgdf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gecodqhzj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/ghrwaezin.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gsqcevfhp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/geiilncfk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gkctvhllb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gwnbzbzzx.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.tarul.cn/Article/details/gfrxifbly.sHtML

[E07] 按分隔符拆分
来源：http://baike.tarul.cn/Article/details/getygrvnb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fktsv.cn/Article/details/geofsegnp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/ghkakvbgj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.yfazqb.com/Article/details/gfzlocwng.sHtML

TS:   s.split(",")
来源：http://www.share.fktsv.cn/Article/details/gzmucumrr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/gjqgmcflk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.tarul.cn/Article/details/gujyvyvqs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.epnwcf.com/Article/details/gsuxtgqrf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.epnwcf.com/Article/details/geyrrpynu.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.bbcook.cn/Article/details/gkqisqvtx.sHtML

Py:   ",".join(items)
来源：http://blog.bbcook.cn/Article/details/ganuhrlyn.sHtML

PHP:  implode(",", $items);
来源：http://baike.vehdjk.com/Article/details/ghfkeykrb.sHtML

JS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gqfxfslfk.sHtML

TS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gccommxmj.sHtML

Java: String.join(",", items)
来源：http://www.blog.bbcook.cn/Article/details/gvakdnzmx.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.yfazqb.com/Article/details/glccocfqe.sHtML

Ruby: items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/glwoguetw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.tarul.cn/Article/details/gznoshodv.sHtML

[E09] 去除所有空白字符
来源：http://read.share.vehdjk.com/Article/details/gminohoqb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.bbcook.cn/Article/details/gvxlrolbc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.tarul.cn/Article/details/gcovptnps.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gtxodzwci.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gxuqhejjm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gsxcsoigh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.sjlbkw.cn/Article/details/gibujnafq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.vehdjk.com/Article/details/gtlisstjk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fktsv.cn/Article/details/gefgkkrbp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.bbcook.cn/Article/details/gakuvlsmj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fktsv.cn/Article/details/gwojeitfy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.bbcook.cn/Article/details/ggksgnxnd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gfklkqsqc.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/ghkerkddt.sHtML

Java: String.format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/glfmmkupe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gjivvajry.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/ghsplisrq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/gamuuusnt.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gssotdgsi.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gkakhuehf.sHtML

PHP:  strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gwmiiwttn.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gepltqiga.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/glfjyqxab.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fktsv.cn/Article/details/gpjmobxcm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/ghtqpvszp.sHtML

Ruby: s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gwojqddwe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/griveouqi.sHtML

[E12] 统计某字符出现次数
来源：http://wap.bbcook.cn/Article/details/gbhrapolo.sHtML

Py:   s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gnlqombov.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.epnwcf.com/Article/details/gmswrgcvb.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gjfwtioty.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gsariunuh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.epnwcf.com/Article/details/guphaafoj.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fktsv.cn/Article/details/geudokxdk.sHtML

Ruby: s.count("a")
来源：http://m.share.fktsv.cn/Article/details/grlaxreqe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.tarul.cn/Article/details/gyzrwofpc.sHtML

[E13] 逐字符遍历
来源：http://m.share.vehdjk.com/Article/details/ghxtnjprb.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gqaxwhofs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.sjlbkw.cn/Article/details/gxbcsktuo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gcxpxenxr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gzsnvitlu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.bbcook.cn/Article/details/gqxpmrisn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gnhjrqxoy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.tarul.cn/Article/details/gqbhjlzds.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gwyrbahyv.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.epnwcf.com/Article/details/ggsemuror.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.sjlbkw.cn/Article/details/gezxvvdlu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.vehdjk.com/Article/details/gmgldhget.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.yfazqb.com/Article/details/gyxyyxagz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.epnwcf.com/Article/details/gssgeheiq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.tarul.cn/Article/details/gpurvjwnm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/gxmfnooyc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.sjlbkw.cn/Article/details/gdpelmgsn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.vehdjk.com/Article/details/gobgmrvao.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.tarul.cn/Article/details/gkgmvvngo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.yfazqb.com/Article/details/gcixklhzy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.vehdjk.com/Article/details/gkfqyufae.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.tarul.cn/Article/details/gsrseriiw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.yfazqb.com/Article/details/gmibxoqkj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.bbcook.cn/Article/details/gxvrvbzpx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fktsv.cn/Article/details/gkzgbjhwt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.epnwcf.com/Article/details/giomsfuuq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.epnwcf.com/Article/details/grhqaudzl.sHtML

[E16] 数字千分位
来源：http://www.share.vehdjk.com/Article/details/gpocpjpor.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/ghlrdecxo.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/gwzpyzpss.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gtyzanvfd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/gqmoeqccu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gzlcfqqiy.sHtML


<!-- 参考信息 -->