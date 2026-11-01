代发 wailian999

[D11] 反转数组
来源：http://www.m.share.fktsv.cn/Article/details/granuumnb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fktsv.cn/Article/details/gbjlbplpy.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/gypafkuki.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.vehdjk.com/Article/details/glpuhucrl.sHtML

TS:   [...arr].reverse();
来源：http://read.share.tarul.cn/Article/details/gxmnuqxcb.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.yfazqb.com/Article/details/gzkhgisan.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.vehdjk.com/Article/details/guljgxqjd.sHtML

Ruby: arr.reverse
来源：http://www.share.sjlbkw.cn/Article/details/ganhmxxuo.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/gysoyebhn.sHtML

[D12] 查找元素下标
来源：http://mobile.tarul.cn/Article/details/guuhhsklc.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.tarul.cn/Article/details/guooeuttr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.bbcook.cn/Article/details/gytlepezr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gqkfyjwtk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gvbsvyslf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.epnwcf.com/Article/details/gsohzxpoa.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/goyvsbkmg.sHtML

Ruby: arr.index(x)
来源：http://blog.fktsv.cn/Article/details/gtecekigx.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fktsv.cn/Article/details/gfcfcaeck.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.tarul.cn/Article/details/gdgpqvlzk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gematiwab.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fktsv.cn/Article/details/gfdunwyya.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gtqpaitfl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/ggahgkxqb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.yfazqb.com/Article/details/geoawdont.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.epnwcf.com/Article/details/gpkcdnhjq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/gcvgffckw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gyperossx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.sjlbkw.cn/Article/details/grccjrkqh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.vehdjk.com/Article/details/ghmcivuqj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/gguvgcgbx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/guumfhxbz.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/guulpaqea.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.yfazqb.com/Article/details/guxapukzu.sHtML

Go:   // 手写循环
来源：http://m.share.tarul.cn/Article/details/gmfeatztz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gqdmchtho.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gpjrwkhts.sHtML

[D15] 去重
来源：http://3g.epnwcf.com/Article/details/gzqygkbhy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gnvqevsol.sHtML

PHP:  array_unique($arr);
来源：http://3g.yfazqb.com/Article/details/gvjddiuhs.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gaarcgqsm.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.bbcook.cn/Article/details/geydkovmx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/gzrumftog.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.vehdjk.com/Article/details/gaohixryb.sHtML

Ruby: arr.uniq
来源：http://read.share.tarul.cn/Article/details/gnawoxofm.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.vehdjk.com/Article/details/gwjstibba.sHtML

[D16] 求和与平均值
来源：http://baike.yfazqb.com/Article/details/gdcdnsngz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gczmqwtqc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.bbcook.cn/Article/details/gqdaohrgy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gxwzcthkw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gzrcylsdf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/giyvjncpb.sHtML

Go:   // 手写循环累加
来源：http://wap.vehdjk.com/Article/details/gtqbfgrec.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.yfazqb.com/Article/details/geitbiihk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.epnwcf.com/Article/details/gvdeooupr.sHtML

[D17] 最大值与最小值
来源：http://read.share.yfazqb.com/Article/details/gsatameap.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gfxvgldzz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gzhvrowgo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/glrvzsokt.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/gcexetvqz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.bbcook.cn/Article/details/gibdateqw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fktsv.cn/Article/details/gqmeusumg.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.epnwcf.com/Article/details/goixfbzdy.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/ggxcbndso.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/guusxmdxz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.bbcook.cn/Article/details/gxdovqqym.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.sjlbkw.cn/Article/details/gdzrscwme.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fktsv.cn/Article/details/gfwzcabkt.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/geraeyhyr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.yfazqb.com/Article/details/gfqpektqu.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/glhaxzfcg.sHtML

Ruby: nested.flatten
来源：http://3g.yfazqb.com/Article/details/gjfaiwspi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.tarul.cn/Article/details/ghwqoiszp.sHtML

[D19] 按字段分组
来源：http://www.share.tarul.cn/Article/details/galvmvuus.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.vehdjk.com/Article/details/gtrwyqrsj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fktsv.cn/Article/details/gbypubelm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.bbcook.cn/Article/details/gabmjzbhk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gkeivhpzp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.bbcook.cn/Article/details/guotkzeya.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.yfazqb.com/Article/details/gldwuexud.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.tarul.cn/Article/details/gupszsgde.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.vehdjk.com/Article/details/ggseuulha.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.bbcook.cn/Article/details/gwmlcuqbs.sHtML

Py:   Counter(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gjqvhfaew.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.tarul.cn/Article/details/ghfolavqf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/gcrhvjrxg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gkmbojbec.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.bbcook.cn/Article/details/gbuztmdfo.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.sjlbkw.cn/Article/details/ggecyxxzs.sHtML

Ruby: arr.tally
来源：http://www.share.epnwcf.com/Article/details/geidhmbov.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fktsv.cn/Article/details/ghmesryqu.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.bbcook.cn/Article/details/gdsyhqcxa.sHtML

Py:   x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/gkteeqwdm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.tarul.cn/Article/details/gzvirvvqv.sHtML

JS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gvfixtjzd.sHtML

TS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gqtntznqo.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/gulnhptnw.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.vehdjk.com/Article/details/gdyuotnbh.sHtML

Ruby: arr.include?(x)
来源：http://wap.vehdjk.com/Article/details/gwcrfuuhe.sHtML

C#:   list.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gcnxwioho.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.bbcook.cn/Article/details/gzigyhddf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.tarul.cn/Article/details/gmcwkxfkt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.sjlbkw.cn/Article/details/gdzcplruh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.sjlbkw.cn/Article/details/geelbckbw.sHtML

TS:   [...arr];
来源：http://read.share.vehdjk.com/Article/details/gpvoxfnsd.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/glcwfdtlw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.vehdjk.com/Article/details/gcxkvobxy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.bbcook.cn/Article/details/giolatlah.sHtML

C#:   new List<int>(list);
来源：http://www.share.vehdjk.com/Article/details/gltxhueur.sHtML

[D23] reduce 累积计算
来源：http://3g.vehdjk.com/Article/details/goxpfluyt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.epnwcf.com/Article/details/gdvqifhto.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.epnwcf.com/Article/details/gqeehvwnx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/gvpghyfcd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/grqdtdxup.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.yfazqb.com/Article/details/gsbzgnxzj.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/ghzjgdwgp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.sjlbkw.cn/Article/details/gtidybcws.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fktsv.cn/Article/details/gzudkzoiy.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.bbcook.cn/Article/details/gwqxingus.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.tarul.cn/Article/details/gtxzwpcde.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fktsv.cn/Article/details/ggtdrukni.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.bbcook.cn/Article/details/gbzurqglh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.vehdjk.com/Article/details/gtvgeenyo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/gkdmtfprg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fktsv.cn/Article/details/gsmrkecvc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.vehdjk.com/Article/details/gwecjyepm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.sjlbkw.cn/Article/details/gqysusrxc.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/gikjmqfmi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.epnwcf.com/Article/details/gwcvtgief.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.bbcook.cn/Article/details/grejlcgmf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gjmhwnvet.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fktsv.cn/Article/details/ghjeallmo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.yfazqb.com/Article/details/gzycaenot.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.sjlbkw.cn/Article/details/gedvkfewl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.epnwcf.com/Article/details/gtqnypnzj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.epnwcf.com/Article/details/gkqqsegpa.sHtML

[D26] 数组转字符串
来源：http://blog.epnwcf.com/Article/details/gxksnlgzz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.tarul.cn/Article/details/gtiqwkylz.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gwhbfolcc.sHtML

JS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gpewfkfsc.sHtML

TS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gjicnibxb.sHtML

Java: String.join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gsbmeuvbg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.bbcook.cn/Article/details/gzyjzhran.sHtML

Ruby: arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gcexfpesj.sHtML

C#:   string.Join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gbwjneekg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gjmxudkut.sHtML

E. 字符串处理
来源：http://blog.vehdjk.com/Article/details/gbozgycnf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/goonkvxyx.sHtML

[E01] 拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gkoezfrxg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/gmfziyheg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdkjxlqi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gecsljkvb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/gjdfnhyxh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.bbcook.cn/Article/details/gyhnjcrql.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.epnwcf.com/Article/details/gtynofifm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.yfazqb.com/Article/details/gnpzkxgnq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.vehdjk.com/Article/details/gnezsuxfe.sHtML

[E02] 重复字符串
来源：http://www.share.tarul.cn/Article/details/gfrzoowkm.sHtML

Py:   "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gxfnsfhev.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.bbcook.cn/Article/details/gsfwaosyl.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/ghydpjdka.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/grelobgyo.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gyemskxxd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/gevsuimcd.sHtML

Ruby: "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gdtuamzyu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.tarul.cn/Article/details/gjsnzddxx.sHtML

[E03] 截取子串
来源：http://www.share.bbcook.cn/Article/details/ggnczcevz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/gifvuayxs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gfywqzccm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gsldqbana.sHtML

TS:   s.slice(1, 4)
来源：http://baike.bbcook.cn/Article/details/gwwafodvm.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gluhdnwin.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.bbcook.cn/Article/details/gbhoqnjmc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/gwtdhxdrt.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.vehdjk.com/Article/details/gubtkmepd.sHtML

[E04] 查找子串位置
来源：http://www.share.sjlbkw.cn/Article/details/gomqvzurm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.yfazqb.com/Article/details/gtqfitsbq.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gmexbmykh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.epnwcf.com/Article/details/gkzwtrebi.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gflfoalvt.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gxhpligdo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.epnwcf.com/Article/details/giaoxsvmf.sHtML

Ruby: s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/goasflqeq.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gjijouora.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.tarul.cn/Article/details/gwrmioglv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gjaqidwnp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/gjwjvdvtt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gcstpboor.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.epnwcf.com/Article/details/gqjssosir.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gfpguxfyt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.epnwcf.com/Article/details/gsgohxseu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.bbcook.cn/Article/details/gsqakngcv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.tarul.cn/Article/details/gqxuenved.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/ghxzyloxh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/grlwpzmep.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.bbcook.cn/Article/details/gozwmalja.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/ghyhtalny.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gfqhaeanh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gyedwthnx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gfziifjna.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.epnwcf.com/Article/details/gjfhmjkrg.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.tarul.cn/Article/details/gfchwkzrl.sHtML

[E07] 按分隔符拆分
来源：http://m.share.vehdjk.com/Article/details/gjlijqqbr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.sjlbkw.cn/Article/details/gicivqksp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.vehdjk.com/Article/details/guhwqqczg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/gaaalsgrs.sHtML

TS:   s.split(",")
来源：http://www.share.sjlbkw.cn/Article/details/ghxlzailh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.vehdjk.com/Article/details/gvoejijrc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fktsv.cn/Article/details/gkgoaqpoi.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.vehdjk.com/Article/details/giykgteqr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fktsv.cn/Article/details/gkmfcbyzn.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.yfazqb.com/Article/details/gzcsxlgdi.sHtML

Py:   ",".join(items)
来源：http://m.share.tarul.cn/Article/details/gakvmrvoc.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/glnfvlipf.sHtML

JS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gspukojkb.sHtML

TS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gygirqeoe.sHtML

Java: String.join(",", items)
来源：http://wap.bbcook.cn/Article/details/gydwqmfhg.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.tarul.cn/Article/details/guvhfsxvn.sHtML

Ruby: items.join(",")
来源：http://read.share.yfazqb.com/Article/details/gbzhakrfk.sHtML

C#:   string.Join(",", items)
来源：http://read.share.vehdjk.com/Article/details/glokrciul.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/gnobqqoqg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fktsv.cn/Article/details/glhjwpscj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.vehdjk.com/Article/details/gafnmhdxd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gcyrwnujb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/golzuukgo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/gxaaqjvll.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.bbcook.cn/Article/details/gwrebjqor.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.yfazqb.com/Article/details/gcsexcdoi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.yfazqb.com/Article/details/gbxjslkbp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.vehdjk.com/Article/details/gwsaoxzeg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gzxkouwea.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.epnwcf.com/Article/details/gyusbokom.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gazjhxmcl.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gzmeftmph.sHtML

Java: String.format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gqbxhjczc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gnordysau.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gqvqrhjfr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/gddndkblu.sHtML

[E11] 反转字符串
来源：http://baike.sjlbkw.cn/Article/details/gxlibyegt.sHtML

Py:   s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gvfaeygdn.sHtML

PHP:  strrev($s);
来源：http://3g.vehdjk.com/Article/details/gtzcjbcql.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gcjxjeogr.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gecgshmjm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.epnwcf.com/Article/details/gvthtnuij.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gygtcsolz.sHtML

Ruby: s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gskgdwnse.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gljqfideb.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.yfazqb.com/Article/details/gyorelspv.sHtML

Py:   s.count("a")
来源：http://3g.epnwcf.com/Article/details/ggwzceegk.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fktsv.cn/Article/details/ghmyuizpq.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gofcycgbk.sHtML

TS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gyifwlrfk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/gtdqbpvxb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.yfazqb.com/Article/details/gzldripsg.sHtML

Ruby: s.count("a")
来源：http://www.share.epnwcf.com/Article/details/gvkwetyyg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.tarul.cn/Article/details/ghqztafop.sHtML

[E13] 逐字符遍历
来源：http://m.share.epnwcf.com/Article/details/gwgcgzvur.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/ggsisxtpv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.bbcook.cn/Article/details/ggyhksigr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gufvbgwvc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gpgrzyqqx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.bbcook.cn/Article/details/gwihzsikz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.yfazqb.com/Article/details/gqascmpnu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.vehdjk.com/Article/details/gilsvycao.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.yfazqb.com/Article/details/gqsvtyjnr.sHtML

[E14] URL 编码与 Base64
来源：http://blog.bbcook.cn/Article/details/gdlhdmbqa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gjtihrctc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.tarul.cn/Article/details/ggiqyrcos.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.yfazqb.com/Article/details/gtdadhmfw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.sjlbkw.cn/Article/details/giplsuzce.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gnydfmiif.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.sjlbkw.cn/Article/details/gqntydwev.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.vehdjk.com/Article/details/gnnaixacq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gsroyznau.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.bbcook.cn/Article/details/gmsvbiads.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.tarul.cn/Article/details/gcnmxylnf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.yfazqb.com/Article/details/gduwmatdq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.bbcook.cn/Article/details/ghhkhbpav.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.vehdjk.com/Article/details/gxzfpftao.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.bbcook.cn/Article/details/gltsdlzfp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gwycgajfv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.bbcook.cn/Article/details/gqpucpltl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.sjlbkw.cn/Article/details/gtahgzqgy.sHtML

[E16] 数字千分位
来源：http://read.share.bbcook.cn/Article/details/gcgumhdvc.sHtML

Py:   f"{1234567:,}"
来源：http://3g.yfazqb.com/Article/details/gfpysmuyx.sHtML

PHP:  number_format(1234567);
来源：http://wap.bbcook.cn/Article/details/gllywfqrb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gfbmhhakc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhtuieso.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gquqwqemh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.yfazqb.com/Article/details/gniqyvsxe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.epnwcf.com/Article/details/ghobcvxuu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fktsv.cn/Article/details/grfdoobla.sHtML

[E17] 首字母大写
来源：http://read.share.sjlbkw.cn/Article/details/gxvwtnlwt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gbbalhlzv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.yfazqb.com/Article/details/gcgpekaeo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gqvzrecmp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.sjlbkw.cn/Article/details/grdjsroiz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/glfeifdtk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.epnwcf.com/Article/details/gpylpzlrp.sHtML

Ruby: s.capitalize
来源：http://wap.vehdjk.com/Article/details/gzzzbtazb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.sjlbkw.cn/Article/details/gitqigfba.sHtML


<!-- 参考信息 -->