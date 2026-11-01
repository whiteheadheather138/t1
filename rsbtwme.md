代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/gzckhlusa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.vehdjk.com/Article/details/gwadbyhgd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.tarul.cn/Article/details/gjxnxrwgi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.vehdjk.com/Article/details/gslckolgd.sHtML

[D11] 反转数组
来源：http://www.m.share.yfazqb.com/Article/details/guywucpmh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.vehdjk.com/Article/details/gfyzcdymh.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.bbcook.cn/Article/details/gpgmfvlvq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.yfazqb.com/Article/details/geiadbvre.sHtML

TS:   [...arr].reverse();
来源：http://baike.tarul.cn/Article/details/ghuwfnjae.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.vehdjk.com/Article/details/grdrgxmaq.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.tarul.cn/Article/details/gdmhotvji.sHtML

Ruby: arr.reverse
来源：http://wap.sjlbkw.cn/Article/details/gmbsamcrr.sHtML

C#:   list.Reverse();
来源：http://baike.epnwcf.com/Article/details/gsslipisk.sHtML

[D12] 查找元素下标
来源：http://m.share.bbcook.cn/Article/details/gbgfwklkx.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.yfazqb.com/Article/details/gvtvbzoke.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/gwobufzdx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gnawrqfcv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gusnyucyj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.tarul.cn/Article/details/gejblrntx.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gjnwrsdfe.sHtML

Ruby: arr.index(x)
来源：http://3g.epnwcf.com/Article/details/gxbqksjfh.sHtML

C#:   list.IndexOf(x);
来源：http://blog.vehdjk.com/Article/details/gftprhcuj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.epnwcf.com/Article/details/gbxsmkxer.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.bbcook.cn/Article/details/gljgibdbv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.tarul.cn/Article/details/gonykegbz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.tarul.cn/Article/details/gqviwwxmc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gbmdgfwnh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fktsv.cn/Article/details/gnyzudpkc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gvwvnrmhb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/gzshxhwyc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/gurlfuaxu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gkjurkbeb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.sjlbkw.cn/Article/details/ghkwifnyb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.yfazqb.com/Article/details/gfhcwbklf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gsbngrajb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gbkplwgpe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gbjzvhbxz.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gohgyjyfc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/ggfszyvdj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.epnwcf.com/Article/details/gzmdjtugj.sHtML

[D15] 去重
来源：http://baike.yfazqb.com/Article/details/goiqehrli.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.tarul.cn/Article/details/gnysvybxe.sHtML

PHP:  array_unique($arr);
来源：http://wap.yfazqb.com/Article/details/glfkgldpk.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gqhcixnpu.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/goxlhhqbc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.bbcook.cn/Article/details/gyddsdlcg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.bbcook.cn/Article/details/ggcborovs.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/gtocjmadr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gpglgphhw.sHtML

[D16] 求和与平均值
来源：http://www.blog.bbcook.cn/Article/details/gqshbasoc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.bbcook.cn/Article/details/gxzppwuaj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.vehdjk.com/Article/details/giunounoc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/ghgewzzea.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/gxiuguqwl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.bbcook.cn/Article/details/grgyaibfi.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.bbcook.cn/Article/details/gjjkritbp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/gacvmnbor.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fktsv.cn/Article/details/gffdcucja.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.epnwcf.com/Article/details/ggonxpudq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/gxcfxglpx.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gvlrvsdjk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.epnwcf.com/Article/details/gxdmokwgn.sHtML

TS:   Math.max(...arr);
来源：http://3g.yfazqb.com/Article/details/gatkuweoj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.tarul.cn/Article/details/gurfwrkhz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gkoflsopd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.vehdjk.com/Article/details/gewrchhkq.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.yfazqb.com/Article/details/gtezkjobv.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fktsv.cn/Article/details/gmckrnlle.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.yfazqb.com/Article/details/gbvvidnfo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.yfazqb.com/Article/details/gfwkrmtub.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.vehdjk.com/Article/details/gmweqamea.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/gbfzuflvj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.yfazqb.com/Article/details/gsfyoxvjo.sHtML

Go:   // 手写双层循环
来源：http://www.blog.epnwcf.com/Article/details/gvnrlxfjx.sHtML

Ruby: nested.flatten
来源：http://www.m.share.vehdjk.com/Article/details/gltfchtgl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.yfazqb.com/Article/details/grcsuxwki.sHtML

[D19] 按字段分组
来源：http://www.m.share.bbcook.cn/Article/details/gjicoozpo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.sjlbkw.cn/Article/details/gfqfcwgdl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/gwcevafjp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fktsv.cn/Article/details/gfmdsgkmn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/gbkbkoawa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.tarul.cn/Article/details/gwtyrwbdq.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.tarul.cn/Article/details/gympedfmx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.tarul.cn/Article/details/gcpgoaqdc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.bbcook.cn/Article/details/gencrfqyz.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.bbcook.cn/Article/details/gfvemhach.sHtML

Py:   Counter(arr)
来源：http://blog.vehdjk.com/Article/details/gyneqgblq.sHtML

PHP:  array_count_values($arr);
来源：http://blog.tarul.cn/Article/details/gohwkpxeo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/guttehhoh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gaipeovjm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.yfazqb.com/Article/details/gtuyrwyep.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.yfazqb.com/Article/details/gwojfmmna.sHtML

Ruby: arr.tally
来源：http://www.m.share.bbcook.cn/Article/details/grdjvkphu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fktsv.cn/Article/details/gjrjlxltw.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.vehdjk.com/Article/details/gataufgzf.sHtML

Py:   x in arr
来源：http://m.share.vehdjk.com/Article/details/guyuqrjuz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.yfazqb.com/Article/details/gdktsbhzr.sHtML

JS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gccyuwxeb.sHtML

TS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gyqijixst.sHtML

Java: list.contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gxqxycvmr.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fktsv.cn/Article/details/gcbghjtce.sHtML

Ruby: arr.include?(x)
来源：http://blog.yfazqb.com/Article/details/gvtlyqayu.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gftbxjjme.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.sjlbkw.cn/Article/details/gyiliicqp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.yfazqb.com/Article/details/gkctqvvwq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.bbcook.cn/Article/details/gwypxwhgn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.bbcook.cn/Article/details/gekwqhjob.sHtML

TS:   [...arr];
来源：http://www.blog.fktsv.cn/Article/details/ghqwkcnpx.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.epnwcf.com/Article/details/ghhdjurgl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.vehdjk.com/Article/details/gkrcnkzjh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.tarul.cn/Article/details/gotyqblyo.sHtML

C#:   new List<int>(list);
来源：http://www.blog.epnwcf.com/Article/details/gjfigavxo.sHtML

[D23] reduce 累积计算
来源：http://wap.vehdjk.com/Article/details/gmhkwtcjh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gfjudtazl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.yfazqb.com/Article/details/ggnmvcpvi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gzykmreda.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/gdzchdpha.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.vehdjk.com/Article/details/gpqybswzi.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gsxniwsdu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.vehdjk.com/Article/details/ghfjctoin.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.sjlbkw.cn/Article/details/gtssgdutq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.yfazqb.com/Article/details/gfgtxezwq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fktsv.cn/Article/details/gmttpmsxx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.vehdjk.com/Article/details/gjolehvep.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.tarul.cn/Article/details/gqcjuhqsi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gyheyfsno.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.tarul.cn/Article/details/gomgdsorw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.sjlbkw.cn/Article/details/gsbfiwkir.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.tarul.cn/Article/details/gnlbbafbz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnaqquppr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fktsv.cn/Article/details/grkscicau.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.epnwcf.com/Article/details/gwblftexg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fktsv.cn/Article/details/gtsxqrkmq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/gapvgtnmd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.bbcook.cn/Article/details/gnvhqxang.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.vehdjk.com/Article/details/gondusxwm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.epnwcf.com/Article/details/gnfmbgvqc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.vehdjk.com/Article/details/gtmtvmlhd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/gtxmqwzsm.sHtML

[D26] 数组转字符串
来源：http://m.share.fktsv.cn/Article/details/gmubtzixn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/goixujzvk.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.vehdjk.com/Article/details/gziciccvv.sHtML

JS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gbnkfxevy.sHtML

TS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gqyolurst.sHtML

Java: String.join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gixglvbiy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fktsv.cn/Article/details/ghfkzknmj.sHtML

Ruby: arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gupceyvuh.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gehlzwjqp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gwnovwtkf.sHtML

E. 字符串处理
来源：http://m.share.vehdjk.com/Article/details/gdtxubcxk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdgfuimla.sHtML

[E01] 拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gfimkbzgo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.vehdjk.com/Article/details/gususswyv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.yfazqb.com/Article/details/gsdnrhfvn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gtbkkgurd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/grwezlerx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gkjtvkphp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fktsv.cn/Article/details/gvubgzkgt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.epnwcf.com/Article/details/gbopdevtc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.epnwcf.com/Article/details/gjpxysiai.sHtML

[E02] 重复字符串
来源：http://www.blog.fktsv.cn/Article/details/gcvkakcor.sHtML

Py:   "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gasetneyh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.epnwcf.com/Article/details/gedhlhuea.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gafcdnshs.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gedhkiscj.sHtML

Java: "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gwwueubvp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.yfazqb.com/Article/details/gaszpvogy.sHtML

Ruby: "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gyvnbnibz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fktsv.cn/Article/details/gjokghpzv.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/gbzwoiros.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.bbcook.cn/Article/details/gwwetfhwl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gghtpmzzx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/gzvwtajzn.sHtML

TS:   s.slice(1, 4)
来源：http://3g.tarul.cn/Article/details/gtovtdngg.sHtML

Java: s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gjgqtxojg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fktsv.cn/Article/details/gdrcxwcyq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.tarul.cn/Article/details/goihxvmmz.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fktsv.cn/Article/details/gluxxbzlj.sHtML

[E04] 查找子串位置
来源：http://wap.yfazqb.com/Article/details/gfbwmmaiz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.yfazqb.com/Article/details/gvxaholej.sHtML

PHP:  strpos($s, "x");
来源：http://blog.vehdjk.com/Article/details/gobjjxwwc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.tarul.cn/Article/details/gwuqtcgzq.sHtML

TS:   s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/ggtxtgnzt.sHtML

Java: s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/ghrxrckqo.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fktsv.cn/Article/details/glxjduepy.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gunjpvejg.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gjurwlaku.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.epnwcf.com/Article/details/gkllofhbm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fktsv.cn/Article/details/gldyyxvqs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.tarul.cn/Article/details/gflldlfun.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/grdfstgmw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.tarul.cn/Article/details/gbuouqcav.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gtqkexdci.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.tarul.cn/Article/details/gusestkoc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.epnwcf.com/Article/details/gudfygtxs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gjyaldqzt.sHtML

[E06] 替换子串
来源：http://www.m.share.bbcook.cn/Article/details/gakzpwxff.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdxgadfv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.yfazqb.com/Article/details/gdgborqaa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gkxntgzbv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gpbpeknng.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/geclquxpa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gxczybjjx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/gaaarosyu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gqwqzknmq.sHtML

[E07] 按分隔符拆分
来源：http://www.share.epnwcf.com/Article/details/gqknvdtpb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.epnwcf.com/Article/details/gylchkvei.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gqwqgjirl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.tarul.cn/Article/details/guqfjzqrj.sHtML

TS:   s.split(",")
来源：http://m.share.fktsv.cn/Article/details/gawbwcyeu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/gqrktawph.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.vehdjk.com/Article/details/guusbqfta.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/guiokwqbt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.yfazqb.com/Article/details/gzjvdgxlr.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fktsv.cn/Article/details/ghevyhhkc.sHtML

Py:   ",".join(items)
来源：http://wap.sjlbkw.cn/Article/details/guvohywew.sHtML

PHP:  implode(",", $items);
来源：http://m.share.epnwcf.com/Article/details/gbdeajevf.sHtML

JS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gydbyqcmw.sHtML

TS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/gqbkfawrq.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gcrnqojbh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.vehdjk.com/Article/details/gynjnnrwt.sHtML

Ruby: items.join(",")
来源：http://baike.bbcook.cn/Article/details/goctsmmct.sHtML

C#:   string.Join(",", items)
来源：http://baike.epnwcf.com/Article/details/gfbjbcber.sHtML

[E09] 去除所有空白字符
来源：http://3g.yfazqb.com/Article/details/gursdircj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.vehdjk.com/Article/details/gfckrtfic.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.epnwcf.com/Article/details/gublwvjwl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/guystrmua.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gellwlfru.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.epnwcf.com/Article/details/gtcbwcrjs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/gxodmsywf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.yfazqb.com/Article/details/glvgddwmj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fktsv.cn/Article/details/gwctetxku.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.vehdjk.com/Article/details/gbeswmhwa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.tarul.cn/Article/details/gwmskvnrc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.tarul.cn/Article/details/gskwlzmsj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/giqiyhwio.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gobktrmun.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gmrwvrmzp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/glcqvtrhq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gaczqsdop.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.tarul.cn/Article/details/gvhhaejnm.sHtML

[E11] 反转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtpbpbrg.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gkhkmhogo.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gowczirwp.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/goghdopqx.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gfzzqfeao.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fktsv.cn/Article/details/gtrcqkyzb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.yfazqb.com/Article/details/gnqwzazkp.sHtML

Ruby: s.reverse
来源：http://www.blog.yfazqb.com/Article/details/gdhrpyrpg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/geodlrruy.sHtML

[E12] 统计某字符出现次数
来源：http://baike.sjlbkw.cn/Article/details/gnpfvhmsa.sHtML

Py:   s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/gnoygnvyv.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.bbcook.cn/Article/details/gyumneeey.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gwqmwwqgc.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gsdhziite.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/giglhqybb.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.sjlbkw.cn/Article/details/gzqzxbmli.sHtML

Ruby: s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gmorbvakf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.yfazqb.com/Article/details/gcuznfdmf.sHtML

[E13] 逐字符遍历
来源：http://m.share.fktsv.cn/Article/details/gqiqivfhx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.epnwcf.com/Article/details/gspidpuuj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.vehdjk.com/Article/details/gnsafkadm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gilakazuj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gihabajzr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gxzuvsjxi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.epnwcf.com/Article/details/gsdktufiy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.vehdjk.com/Article/details/gbohtrktw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fktsv.cn/Article/details/giaablfxh.sHtML

[E14] URL 编码与 Base64
来源：http://3g.tarul.cn/Article/details/gpmuqiokp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/gpxnxoaof.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.epnwcf.com/Article/details/gafdpkmiz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.yfazqb.com/Article/details/gxeiecban.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/gywgyzxgf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/gvpzjzcvr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.yfazqb.com/Article/details/gzhpbfoov.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.epnwcf.com/Article/details/gocamhjyx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/glxbtgesr.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.yfazqb.com/Article/details/gpfhngrsg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.epnwcf.com/Article/details/gyfhovckw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.vehdjk.com/Article/details/gtwxwijnd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.epnwcf.com/Article/details/gqjgnhbql.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.vehdjk.com/Article/details/gywocoavd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.epnwcf.com/Article/details/gqeykpllt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.epnwcf.com/Article/details/gkpvxkgii.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fktsv.cn/Article/details/grfoczowr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fktsv.cn/Article/details/gexcddirz.sHtML

[E16] 数字千分位
来源：http://www.blog.vehdjk.com/Article/details/gstratlja.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.tarul.cn/Article/details/grisfswah.sHtML

PHP:  number_format(1234567);
来源：http://mobile.bbcook.cn/Article/details/gkpgynlnf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/guwfjrkuq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/gaxattdtj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/geutkuoed.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fktsv.cn/Article/details/gyhivibzk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.yfazqb.com/Article/details/gqwgkntvm.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/grirwoqnu.sHtML

[E17] 首字母大写
来源：http://www.blog.sjlbkw.cn/Article/details/gfuiraglf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.bbcook.cn/Article/details/gttwbouvz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fktsv.cn/Article/details/ghatajnvt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxrfqypi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gnpehpkbe.sHtML


<!-- 参考信息 -->