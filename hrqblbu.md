代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.vehdjk.com/Article/details/ggnhgircf.sHtML

Ruby: arr.sort
来源：http://read.share.vehdjk.com/Article/details/grcaobirr.sHtML

C#:   list.Sort();
来源：http://wap.bbcook.cn/Article/details/gvxkgtfig.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/gdssholrt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fktsv.cn/Article/details/galceixnp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/gqbezteka.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/goavozrpf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gnjcaxlpu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.epnwcf.com/Article/details/glldihhif.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.vehdjk.com/Article/details/gynlgphls.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.bbcook.cn/Article/details/gecdhvscy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.vehdjk.com/Article/details/gixxdrngn.sHtML

[D11] 反转数组
来源：http://www.share.epnwcf.com/Article/details/gxcoxrzia.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gdzpusyts.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fktsv.cn/Article/details/gqpssixjm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fktsv.cn/Article/details/gcugbhmcr.sHtML

TS:   [...arr].reverse();
来源：http://3g.bbcook.cn/Article/details/gwegwmolk.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.sjlbkw.cn/Article/details/ghqylpeoa.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/gyroordkw.sHtML

Ruby: arr.reverse
来源：http://m.share.bbcook.cn/Article/details/grhnwdysc.sHtML

C#:   list.Reverse();
来源：http://www.blog.tarul.cn/Article/details/gnsabzlus.sHtML

[D12] 查找元素下标
来源：http://3g.fktsv.cn/Article/details/gdfyvgbdr.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.vehdjk.com/Article/details/gbwvrftkj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.yfazqb.com/Article/details/gfikklvog.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/ghdqqjfei.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fktsv.cn/Article/details/gjfcqbula.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fktsv.cn/Article/details/gdmcoyist.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.yfazqb.com/Article/details/gkovsjlpo.sHtML

Ruby: arr.index(x)
来源：http://blog.fktsv.cn/Article/details/gjujsndin.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fktsv.cn/Article/details/gnndzqgvc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/ghxiuccff.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gzigwqmpi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.sjlbkw.cn/Article/details/gnhtpwufy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gdrzqibet.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/gkqwmxnpa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.vehdjk.com/Article/details/gksyultnd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.epnwcf.com/Article/details/ggmbtwnsq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.yfazqb.com/Article/details/gmoebjjuk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.bbcook.cn/Article/details/gnykwpqzx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.sjlbkw.cn/Article/details/gjiefgiud.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/glukedvld.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.bbcook.cn/Article/details/guzlrrqyy.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/gmfnvitwd.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/gboayphqf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/grporwbnb.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gtyrcpcoa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gwzaasynv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.epnwcf.com/Article/details/gsieymbar.sHtML

[D15] 去重
来源：http://www.blog.bbcook.cn/Article/details/govjjwmet.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/gqoymabwb.sHtML

PHP:  array_unique($arr);
来源：http://www.share.vehdjk.com/Article/details/gzcxvxbes.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gstzuvsxe.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gxhmqycqi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gstxcjlem.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.tarul.cn/Article/details/glbbrpfta.sHtML

Ruby: arr.uniq
来源：http://m.share.bbcook.cn/Article/details/gssymbtur.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.sjlbkw.cn/Article/details/giszfuunq.sHtML

[D16] 求和与平均值
来源：http://wap.yfazqb.com/Article/details/gvhconynj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.yfazqb.com/Article/details/gzmwwhftc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.tarul.cn/Article/details/gocdnyppe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.epnwcf.com/Article/details/gbwkwnshx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/gdzekbjeq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjkwlyhx.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/gjtemfbqg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.epnwcf.com/Article/details/gnbxvbzmz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.vehdjk.com/Article/details/gvpgzzqqo.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.epnwcf.com/Article/details/gxckdxige.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.yfazqb.com/Article/details/genmrgybb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.yfazqb.com/Article/details/grrozkkui.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.yfazqb.com/Article/details/gxnyoxqfu.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.bbcook.cn/Article/details/gwtsntrug.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fktsv.cn/Article/details/gvcdosrau.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.bbcook.cn/Article/details/gqkgflvcg.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.bbcook.cn/Article/details/guxmksxqi.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.epnwcf.com/Article/details/gzfuqbrxr.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.tarul.cn/Article/details/gckejytdg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.bbcook.cn/Article/details/gyxvkcqze.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.bbcook.cn/Article/details/gjfrtiysn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.vehdjk.com/Article/details/gmrglroiq.sHtML

TS:   nested.flat();
来源：http://wap.epnwcf.com/Article/details/gfqnttoyj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gjpjxqidc.sHtML

Go:   // 手写双层循环
来源：http://mobile.tarul.cn/Article/details/gcejkpejw.sHtML

Ruby: nested.flatten
来源：http://mobile.epnwcf.com/Article/details/ggnqxomaq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.bbcook.cn/Article/details/gavvfgeki.sHtML

[D19] 按字段分组
来源：http://blog.tarul.cn/Article/details/ghxycocde.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.tarul.cn/Article/details/gwvhzhajb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.vehdjk.com/Article/details/gobdglgas.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fktsv.cn/Article/details/gtbfscfix.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/glsgxgaoi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.epnwcf.com/Article/details/gwhvtjxll.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.bbcook.cn/Article/details/gdsqdassk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.bbcook.cn/Article/details/gbkbhrvoh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.vehdjk.com/Article/details/gtppeykjc.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.bbcook.cn/Article/details/giujfumpp.sHtML

Py:   Counter(arr)
来源：http://m.share.yfazqb.com/Article/details/grwjesoku.sHtML

PHP:  array_count_values($arr);
来源：http://3g.epnwcf.com/Article/details/gfvkcnlbh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gzbosrvap.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gkbezkhcl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.bbcook.cn/Article/details/gsovuotnc.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.tarul.cn/Article/details/gcfvncgqc.sHtML

Ruby: arr.tally
来源：http://www.share.tarul.cn/Article/details/govwvbejk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.yfazqb.com/Article/details/gmwqrseuz.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.epnwcf.com/Article/details/giondrwlk.sHtML

Py:   x in arr
来源：http://baike.tarul.cn/Article/details/gxjvhekeu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.tarul.cn/Article/details/gftdhehnz.sHtML

JS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gqukjjlhq.sHtML

TS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gamuerwem.sHtML

Java: list.contains(x)
来源：http://www.share.fktsv.cn/Article/details/gftclkceq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gdmbikbui.sHtML

Ruby: arr.include?(x)
来源：http://blog.bbcook.cn/Article/details/ggfydbvwi.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gnhwhghdu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.vehdjk.com/Article/details/geaiynidu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.yfazqb.com/Article/details/gfcdvtaza.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.yfazqb.com/Article/details/gkohircdb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.yfazqb.com/Article/details/gbhmvmnep.sHtML

TS:   [...arr];
来源：http://wap.tarul.cn/Article/details/gqvwpnkwk.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.epnwcf.com/Article/details/gvbhtrduv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.yfazqb.com/Article/details/gpayhhkfb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.sjlbkw.cn/Article/details/gkslikhmh.sHtML

C#:   new List<int>(list);
来源：http://3g.vehdjk.com/Article/details/gbginzkyc.sHtML

[D23] reduce 累积计算
来源：http://m.share.tarul.cn/Article/details/gwfrulufb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.vehdjk.com/Article/details/glfdtzwfn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.epnwcf.com/Article/details/gxyyzxgye.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gkbujkhnt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gnzsitikk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.vehdjk.com/Article/details/gowsntlzd.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/gmgaujqle.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/grefkgsll.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.bbcook.cn/Article/details/gwmapgudj.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.bbcook.cn/Article/details/gcohvhkqk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.yfazqb.com/Article/details/gpsyfelnj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.sjlbkw.cn/Article/details/gyhjabkog.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.vehdjk.com/Article/details/gkhombuxd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gksnbmyyc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.sjlbkw.cn/Article/details/grwvgwlpa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.bbcook.cn/Article/details/gixdavmtr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.yfazqb.com/Article/details/gpygndsla.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.vehdjk.com/Article/details/gzxopsdxr.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.sjlbkw.cn/Article/details/gxiafjtrc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.sjlbkw.cn/Article/details/gflbxasud.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.tarul.cn/Article/details/gvtwbpwyn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.yfazqb.com/Article/details/gmstyogof.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gbddqmmax.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.epnwcf.com/Article/details/gsgjuqssc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.sjlbkw.cn/Article/details/gpiqfipvt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.vehdjk.com/Article/details/gzkgtdbgi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.epnwcf.com/Article/details/gfbmwadtc.sHtML

[D26] 数组转字符串
来源：http://read.share.fktsv.cn/Article/details/gpygvsnep.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gdpivfatz.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.bbcook.cn/Article/details/gwreuajcq.sHtML

JS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gfhhmysds.sHtML

TS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gjxjpcxyi.sHtML

Java: String.join(", ", list)
来源：http://mobile.yfazqb.com/Article/details/gabymempu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.vehdjk.com/Article/details/gslxxlxkk.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gnzwfrgvi.sHtML

C#:   string.Join(", ", list)
来源：http://wap.tarul.cn/Article/details/garvdslae.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gfanwxqkk.sHtML

E. 字符串处理
来源：http://3g.sjlbkw.cn/Article/details/gitxrkdxb.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gsnepncwk.sHtML

[E01] 拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/glcayhopd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.yfazqb.com/Article/details/gljxxnclp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/ghxudtghp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gwhqpfkpk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gwimoqnwo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.yfazqb.com/Article/details/gxbmatply.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.tarul.cn/Article/details/gtmijdabp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.bbcook.cn/Article/details/gzhvyihok.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/grwsnboxm.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/gxqqjmqzn.sHtML

Py:   "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gizwjjisx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.sjlbkw.cn/Article/details/gsazcqssi.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gusophgfk.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gdnzutbmg.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gmksvkltn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fktsv.cn/Article/details/gibvtlxyk.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gauefiehu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.yfazqb.com/Article/details/gxhcdivtl.sHtML

[E03] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gecrrjnpe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.tarul.cn/Article/details/gvniopxru.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gwlghgvgc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gxizszaqh.sHtML

TS:   s.slice(1, 4)
来源：http://wap.epnwcf.com/Article/details/goqpxzpej.sHtML

Java: s.substring(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gexetllud.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.epnwcf.com/Article/details/gcmkqfphg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/galwxvlzu.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.yfazqb.com/Article/details/gqitjtqui.sHtML

[E04] 查找子串位置
来源：http://blog.epnwcf.com/Article/details/giccyjifj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gfqxjkmfo.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/ghjyczuzp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.sjlbkw.cn/Article/details/gagfxsjvj.sHtML

TS:   s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gzqcixnfb.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gjsldezga.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.yfazqb.com/Article/details/gfldsmluj.sHtML

Ruby: s.index("x")
来源：http://www.share.tarul.cn/Article/details/gxrelghnp.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/giskfcghn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.vehdjk.com/Article/details/glemfmnuy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.tarul.cn/Article/details/gqotlgkoc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.tarul.cn/Article/details/gyzvgyihb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gfsgjzjgm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/gzplwwrsp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gtnddvidv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.epnwcf.com/Article/details/gsiscyadb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.vehdjk.com/Article/details/gfphojjya.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.yfazqb.com/Article/details/gwdcuncrf.sHtML

[E06] 替换子串
来源：http://m.share.epnwcf.com/Article/details/gyaksrisu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/gcnusvdhx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fktsv.cn/Article/details/guptpfcfd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gbquraklh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/glkmcfomq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gwqjsskhn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/giksgaavn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gqwedytam.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.tarul.cn/Article/details/gdwbcmhbm.sHtML

[E07] 按分隔符拆分
来源：http://mobile.sjlbkw.cn/Article/details/gbwpkdmbj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/guliwsmsq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gcplsftju.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/geoemfvbv.sHtML

TS:   s.split(",")
来源：http://3g.fktsv.cn/Article/details/ggquwctdz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fktsv.cn/Article/details/gmolmcxmd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/guucnqvrq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.bbcook.cn/Article/details/gmjqqhksc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/glitzuqpg.sHtML

[E08] 数组按分隔符合并
来源：http://baike.sjlbkw.cn/Article/details/gltetnfil.sHtML

Py:   ",".join(items)
来源：http://baike.vehdjk.com/Article/details/gfkihbnsx.sHtML

PHP:  implode(",", $items);
来源：http://wap.yfazqb.com/Article/details/gtodeqxhl.sHtML

JS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gxvylgjuh.sHtML

TS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/ggvzokqxb.sHtML

Java: String.join(",", items)
来源：http://3g.bbcook.cn/Article/details/gsaiawnrg.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fktsv.cn/Article/details/gtjehrpuo.sHtML

Ruby: items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gqsfmasnf.sHtML

C#:   string.Join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gtfunmjaz.sHtML

[E09] 去除所有空白字符
来源：http://3g.yfazqb.com/Article/details/gbegvworx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fktsv.cn/Article/details/gfuhoigha.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fktsv.cn/Article/details/grksqltjk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/gvnbpwuiq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.yfazqb.com/Article/details/gwgvtthar.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gyevildic.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gebublsap.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.epnwcf.com/Article/details/gylbvstqa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjasezbyl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.bbcook.cn/Article/details/gpwbemrmp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gevsiabur.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.vehdjk.com/Article/details/gbcezwxyl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gyqrfcxip.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/geybxhwgb.sHtML

Java: String.format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gqtuaffrx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gdriksqdq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gizedolym.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.sjlbkw.cn/Article/details/guxqywoxj.sHtML

[E11] 反转字符串
来源：http://blog.epnwcf.com/Article/details/geqofrldb.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gzaumrbaa.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/goldsvpzy.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/guxxgyikt.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/ggrqspnlt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.yfazqb.com/Article/details/glpxeldtp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.yfazqb.com/Article/details/gjognesac.sHtML

Ruby: s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gofialqyq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gvudyrctk.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.bbcook.cn/Article/details/gzcqozcqi.sHtML

Py:   s.count("a")
来源：http://blog.vehdjk.com/Article/details/guuhbommi.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.epnwcf.com/Article/details/gyvayojky.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gpetaqsfp.sHtML

TS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/grfnnnecx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.vehdjk.com/Article/details/gfpqryvak.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.epnwcf.com/Article/details/gufghmhkz.sHtML

Ruby: s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/goayalhrc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.vehdjk.com/Article/details/gneaclvww.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.yfazqb.com/Article/details/gmeswhpjp.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fktsv.cn/Article/details/gjjjqtqmg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/giurqkwzp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.epnwcf.com/Article/details/gdyjgpypy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/glcbunakq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.tarul.cn/Article/details/gmckfvgaw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fktsv.cn/Article/details/genmuogzx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.tarul.cn/Article/details/gbycwrsgi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fktsv.cn/Article/details/ghsikqbjr.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.sjlbkw.cn/Article/details/goznshwwr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/gniwjmhtb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/ghlfkojqw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/godxeycxu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.epnwcf.com/Article/details/gmxwvoqcp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/gcvejibtm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.yfazqb.com/Article/details/gnbulogdk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.yfazqb.com/Article/details/gbnlrfext.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.yfazqb.com/Article/details/gjfhvystf.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.bbcook.cn/Article/details/gaminpvrx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.vehdjk.com/Article/details/ggfjcecqh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.tarul.cn/Article/details/gpuizncvp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.yfazqb.com/Article/details/gkczenppu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.epnwcf.com/Article/details/gaoiwqjvl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.sjlbkw.cn/Article/details/gtsqzifwc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/gwizlydlg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.vehdjk.com/Article/details/gzupzpfru.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/gaerodezp.sHtML

[E16] 数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gmlupyxzt.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gehujpwwe.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/gjphctmko.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/goizjfhdx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/ghzdouarq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.bbcook.cn/Article/details/ghtsqqfkj.sHtML


<!-- 参考信息 -->