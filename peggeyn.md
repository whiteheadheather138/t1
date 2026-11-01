代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gyoaptiux.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gmgbrkddt.sHtML

C#:   list.Sort();
来源：http://www.share.bbcook.cn/Article/details/gjsdlqkke.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.bbcook.cn/Article/details/glazqzadu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.yfazqb.com/Article/details/gpkvnqqvr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gvwmddzvi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gdnbdsocj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gtqrtganf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fktsv.cn/Article/details/giilqkrhe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.yfazqb.com/Article/details/gxtahmimv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.vehdjk.com/Article/details/gorptomrz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.vehdjk.com/Article/details/gmichumpv.sHtML

[D11] 反转数组
来源：http://baike.fktsv.cn/Article/details/gjcmdrgvm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.vehdjk.com/Article/details/gxehfiljr.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/gfyezxqvk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.vehdjk.com/Article/details/gefmbaryi.sHtML

TS:   [...arr].reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gttvrvcyp.sHtML

Java: Collections.reverse(list);
来源：http://baike.yfazqb.com/Article/details/gidqtfxjx.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.yfazqb.com/Article/details/gzvkmvjcv.sHtML

Ruby: arr.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gelujmsgc.sHtML

C#:   list.Reverse();
来源：http://3g.epnwcf.com/Article/details/gokxairls.sHtML

[D12] 查找元素下标
来源：http://www.m.share.epnwcf.com/Article/details/glwiuamrk.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.yfazqb.com/Article/details/gmtmnxzji.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.yfazqb.com/Article/details/gckgjhwdl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/gdcdejcex.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gpiqqwaca.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.sjlbkw.cn/Article/details/gzhnttsma.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.vehdjk.com/Article/details/goxukrscb.sHtML

Ruby: arr.index(x)
来源：http://blog.tarul.cn/Article/details/gezovjghn.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.yfazqb.com/Article/details/gauydmeby.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fktsv.cn/Article/details/glebpmhjn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.yfazqb.com/Article/details/gfghucbun.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.vehdjk.com/Article/details/gqrrovmev.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gbcwyukob.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gccnfwdiv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gpbcwcjgp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fktsv.cn/Article/details/gdvescpzy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.yfazqb.com/Article/details/gnzrzikox.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gustmdbcl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.epnwcf.com/Article/details/gdzjzldxk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gzisqmegp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.epnwcf.com/Article/details/grexzsbga.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gmqtlwpvg.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gyombywir.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gmseuijmj.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gyjngwnee.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.yfazqb.com/Article/details/gtqzdiguw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fktsv.cn/Article/details/grejiwayp.sHtML

[D15] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gydycwazl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.vehdjk.com/Article/details/gajatvmhk.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gifcdipqq.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/ghstcqrxl.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/ghkzrmlbk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.yfazqb.com/Article/details/gdazhsjro.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.tarul.cn/Article/details/gaxdvdtxa.sHtML

Ruby: arr.uniq
来源：http://baike.fktsv.cn/Article/details/gsqjfeyil.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.epnwcf.com/Article/details/gzomlcvus.sHtML

[D16] 求和与平均值
来源：http://www.share.fktsv.cn/Article/details/gxsotjsjq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.vehdjk.com/Article/details/gxxbhzsbz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.yfazqb.com/Article/details/grbxgyjba.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gnqtnnsoo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/glyorrhwg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.tarul.cn/Article/details/gisqtazlb.sHtML

Go:   // 手写循环累加
来源：http://mobile.yfazqb.com/Article/details/gaflzajzt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.epnwcf.com/Article/details/gsxlaehyq.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fktsv.cn/Article/details/gkzbvrctf.sHtML

[D17] 最大值与最小值
来源：http://read.share.bbcook.cn/Article/details/galknftuc.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gwvhpfbrg.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fktsv.cn/Article/details/gtrmylagj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.epnwcf.com/Article/details/gvimyzckh.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gtpmyolck.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.tarul.cn/Article/details/gbknnoeco.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gzedvautk.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.yfazqb.com/Article/details/gkygszjuq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.vehdjk.com/Article/details/ggajmibnz.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.vehdjk.com/Article/details/gkywowdmf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.sjlbkw.cn/Article/details/ggacmorbc.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.epnwcf.com/Article/details/gqelsylma.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.tarul.cn/Article/details/ghofwdajd.sHtML

TS:   nested.flat();
来源：http://www.m.share.bbcook.cn/Article/details/gpxghltxj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.yfazqb.com/Article/details/gtvmwqxlx.sHtML

Go:   // 手写双层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gxhshgazm.sHtML

Ruby: nested.flatten
来源：http://baike.tarul.cn/Article/details/gdfavkcnf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.vehdjk.com/Article/details/gspdwqfhz.sHtML

[D19] 按字段分组
来源：http://www.m.share.vehdjk.com/Article/details/gweblyjpf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.sjlbkw.cn/Article/details/glzoqwbof.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.sjlbkw.cn/Article/details/gytcfxumk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/grgjfrcnx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.sjlbkw.cn/Article/details/gqaljydwe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.epnwcf.com/Article/details/gfrtmmrnz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.bbcook.cn/Article/details/gahqsbzau.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fktsv.cn/Article/details/geomrxgvb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fktsv.cn/Article/details/gtcjskbjy.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.bbcook.cn/Article/details/gfjngvngi.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gdhmjovyv.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fktsv.cn/Article/details/grwsyhtcw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/grrpdioth.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/ggqlbmwze.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.epnwcf.com/Article/details/gitztlwcb.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/gsqwbxyvg.sHtML

Ruby: arr.tally
来源：http://read.share.tarul.cn/Article/details/gkunvkbqc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.vehdjk.com/Article/details/gusbbqgkt.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fktsv.cn/Article/details/goljzsoxw.sHtML

Py:   x in arr
来源：http://mobile.sjlbkw.cn/Article/details/gswyorpln.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwccmzdx.sHtML

JS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gdmbdqdvo.sHtML

TS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/gyzrorkqg.sHtML

Java: list.contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gtiibsrsl.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.epnwcf.com/Article/details/gyufrcbmz.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/gtrdsjlmz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/grasvqeei.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.tarul.cn/Article/details/gxrkozagm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.yfazqb.com/Article/details/gzoaqjslw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fktsv.cn/Article/details/gdqzrqmjn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/gagkccnom.sHtML

TS:   [...arr];
来源：http://blog.fktsv.cn/Article/details/gbnqosoju.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/gxelpvloc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.yfazqb.com/Article/details/gauvatong.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.vehdjk.com/Article/details/gowzcakkm.sHtML

C#:   new List<int>(list);
来源：http://wap.tarul.cn/Article/details/gmfbksrss.sHtML

[D23] reduce 累积计算
来源：http://blog.tarul.cn/Article/details/gbghvpyej.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gsfewqxzh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.sjlbkw.cn/Article/details/gamxhcumg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gbcoaoeer.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gzzshgrnt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.tarul.cn/Article/details/gslzzueqw.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gbpndbuak.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.tarul.cn/Article/details/glienvxck.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.epnwcf.com/Article/details/gaiztymvc.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.bbcook.cn/Article/details/gwoureupj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.yfazqb.com/Article/details/gtobmrrpl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.tarul.cn/Article/details/gsvhyjrhq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/gtmbqphhg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gouwbfvlq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/goroomzzn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.tarul.cn/Article/details/gpbyupfym.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fktsv.cn/Article/details/geldrodjk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.bbcook.cn/Article/details/gwdzqoyfa.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.epnwcf.com/Article/details/gwoahifqq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.yfazqb.com/Article/details/glocyrzgc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.yfazqb.com/Article/details/gfuntegux.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/glznghfbj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.tarul.cn/Article/details/geseoazfa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fktsv.cn/Article/details/gdalhvqay.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.vehdjk.com/Article/details/gdhjxemjr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/ggwzkethq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gsxgxlqfv.sHtML

[D26] 数组转字符串
来源：http://3g.tarul.cn/Article/details/gjocgjmbv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fktsv.cn/Article/details/ghwuxtcmx.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/ghygrescc.sHtML

JS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gvdnrycpx.sHtML

TS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gikzmdryh.sHtML

Java: String.join(", ", list)
来源：http://mobile.tarul.cn/Article/details/grqsqhedq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.tarul.cn/Article/details/gkpkdwpgd.sHtML

Ruby: arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gzhmthyfc.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fktsv.cn/Article/details/goypyhbud.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/geahgjgqx.sHtML

E. 字符串处理
来源：http://www.m.share.tarul.cn/Article/details/grapoeaah.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqmtngnmf.sHtML

[E01] 拼接字符串
来源：http://blog.bbcook.cn/Article/details/gqeszkilb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.epnwcf.com/Article/details/gzwxygrlz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.sjlbkw.cn/Article/details/gpnunxjqx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/gbccrpenl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/gvcdzdixz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.tarul.cn/Article/details/gtpgqaeaf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.sjlbkw.cn/Article/details/gsmznqjxl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.yfazqb.com/Article/details/gxkqoiuoi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/goybsvwaq.sHtML

[E02] 重复字符串
来源：http://www.share.yfazqb.com/Article/details/gyfvxhhqx.sHtML

Py:   "ab" * 3
来源：http://blog.yfazqb.com/Article/details/gpbhfjmiq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.yfazqb.com/Article/details/grnqrrfxr.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gotmdlfjf.sHtML

TS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gpqyutffs.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gdzhywrii.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.sjlbkw.cn/Article/details/gwmfhbyvo.sHtML

Ruby: "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gmhmcvbag.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.epnwcf.com/Article/details/ggvecbomm.sHtML

[E03] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gafysirxy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.epnwcf.com/Article/details/gmjqmjtiz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gicnsnrxh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gxcdnxmhs.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fktsv.cn/Article/details/gkvtoqqts.sHtML

Java: s.substring(1, 4)
来源：http://www.share.vehdjk.com/Article/details/ggzuomrzb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.yfazqb.com/Article/details/gkjxlijvs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.vehdjk.com/Article/details/gmrftuweu.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.bbcook.cn/Article/details/gngvqaqax.sHtML

[E04] 查找子串位置
来源：http://blog.yfazqb.com/Article/details/gdiavhwjl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.tarul.cn/Article/details/gmqjqghqm.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.bbcook.cn/Article/details/gffxubwfy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.epnwcf.com/Article/details/gzthgzboq.sHtML

TS:   s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/gijirglmw.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gikdxmxpk.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.yfazqb.com/Article/details/gctjhcvdp.sHtML

Ruby: s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/gaqnkfrqi.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/goxflglwp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fktsv.cn/Article/details/gxmhvdokk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.tarul.cn/Article/details/gwmdmdpmr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.sjlbkw.cn/Article/details/gglfajxor.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/giwttxfhl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.bbcook.cn/Article/details/gxguegvyy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gyrdlahrd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.tarul.cn/Article/details/gkwaibmpu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.bbcook.cn/Article/details/ghcnebcmz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.epnwcf.com/Article/details/ghznjujkr.sHtML

[E06] 替换子串
来源：http://m.share.vehdjk.com/Article/details/gbohfdnna.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/glyhbamuz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/gyfoofatj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gkpuoriqb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gihgbejmd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/ghuswfimx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gftrjnmsu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gjbyagwtu.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gurgohleb.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gswzybrxw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fktsv.cn/Article/details/gggpivmfb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gpkbeobej.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.yfazqb.com/Article/details/gbyrkgrwh.sHtML

TS:   s.split(",")
来源：http://blog.yfazqb.com/Article/details/gudlkvhth.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.bbcook.cn/Article/details/gpnrmuzuy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fktsv.cn/Article/details/gkqlvpnei.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.bbcook.cn/Article/details/gtnlxzppd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.bbcook.cn/Article/details/gexhdmxjp.sHtML

[E08] 数组按分隔符合并
来源：http://baike.sjlbkw.cn/Article/details/ggxxcsekb.sHtML

Py:   ",".join(items)
来源：http://www.blog.sjlbkw.cn/Article/details/gdwtazvok.sHtML

PHP:  implode(",", $items);
来源：http://3g.tarul.cn/Article/details/gbsrrifrd.sHtML

JS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gadkdwtee.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gahaduqki.sHtML

Java: String.join(",", items)
来源：http://baike.bbcook.cn/Article/details/gmkgxdsni.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/gvtftvkly.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/gvpqjmjxa.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/gvqsxmpch.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fktsv.cn/Article/details/gzdvotyfh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.sjlbkw.cn/Article/details/gofgmaylk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.tarul.cn/Article/details/gwqhpvkqu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gaoujzrsx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/ggszkkdbt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gisqupkvd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.yfazqb.com/Article/details/gpocebyaz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.bbcook.cn/Article/details/gixtjrwlr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gmtjrhmkw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.sjlbkw.cn/Article/details/gevxrknqa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/ghvgnthex.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.epnwcf.com/Article/details/gkperhmzs.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gmgqbzfbe.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gskhxzabh.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/grtwkbkbw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gpvmtujdz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/guuprvdbg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.yfazqb.com/Article/details/gzoeliyde.sHtML

[E11] 反转字符串
来源：http://www.blog.tarul.cn/Article/details/ghkjbhbhl.sHtML

Py:   s[::-1]
来源：http://baike.tarul.cn/Article/details/gvakoerlr.sHtML

PHP:  strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gdjluykzd.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gtztiqyxi.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gorwvdsmj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gqejwjobq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.vehdjk.com/Article/details/ghsmrhmkb.sHtML

Ruby: s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/grwrzchtl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/gdqkmfynn.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gsryustgv.sHtML

Py:   s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gawlbdkwj.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.vehdjk.com/Article/details/gdeodtfjd.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/ggbljocru.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gwdrqqnfl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.sjlbkw.cn/Article/details/gnscxovrm.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.tarul.cn/Article/details/ghchkxsry.sHtML

Ruby: s.count("a")
来源：http://wap.vehdjk.com/Article/details/gbjtzkbre.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gerlursjh.sHtML

[E13] 逐字符遍历
来源：http://blog.tarul.cn/Article/details/gdybcykvw.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.sjlbkw.cn/Article/details/gcsbbrqrh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.sjlbkw.cn/Article/details/ggfyiypld.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gdxsjlpzv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gyeeepuuo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gjlkphkot.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.sjlbkw.cn/Article/details/gulrpuqbp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.sjlbkw.cn/Article/details/gshtccxtk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/gahbmsyfo.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/guoxadkfm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.epnwcf.com/Article/details/gpbxgjgnn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gnxzmnlfs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.bbcook.cn/Article/details/ghtewgiph.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.bbcook.cn/Article/details/guvgrrlxe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.epnwcf.com/Article/details/gheveaihc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/guruxcuqt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.epnwcf.com/Article/details/gbcndixok.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gbytaqaal.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.bbcook.cn/Article/details/gkmcgxqjv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.epnwcf.com/Article/details/gmywltgkx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.yfazqb.com/Article/details/gqyqwcbcn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.sjlbkw.cn/Article/details/geudrjkho.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fktsv.cn/Article/details/gatdtllgk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.yfazqb.com/Article/details/gvmlxldzk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.tarul.cn/Article/details/grlimqmxu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.yfazqb.com/Article/details/gtmobbldy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.vehdjk.com/Article/details/gbqcfvfhm.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/germaewde.sHtML

Py:   f"{1234567:,}"
来源：http://blog.bbcook.cn/Article/details/glyzfopcu.sHtML

PHP:  number_format(1234567);
来源：http://mobile.tarul.cn/Article/details/gxaegtvmo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gxprlmesn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gkadtekwr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/glcpgpqsu.sHtML


<!-- 参考信息 -->