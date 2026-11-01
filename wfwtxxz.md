代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.yfazqb.com/Article/details/gtohpvytx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.sjlbkw.cn/Article/details/guydigfml.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gtggrmiay.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/glxdzlpey.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.bbcook.cn/Article/details/gftoeimrk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/gojrgaztf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.yfazqb.com/Article/details/ghnvdbczi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.tarul.cn/Article/details/gsnouyyby.sHtML

[D11] 反转数组
来源：http://blog.tarul.cn/Article/details/gsxvciurx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.epnwcf.com/Article/details/gzzjakjre.sHtML

PHP:  array_reverse($arr);
来源：http://baike.tarul.cn/Article/details/gvezwagks.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.yfazqb.com/Article/details/gfqixpyeb.sHtML

TS:   [...arr].reverse();
来源：http://m.share.vehdjk.com/Article/details/gifjxqmvc.sHtML

Java: Collections.reverse(list);
来源：http://www.share.yfazqb.com/Article/details/gfvqthizf.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.bbcook.cn/Article/details/gezjjuogs.sHtML

Ruby: arr.reverse
来源：http://baike.tarul.cn/Article/details/gzbxsflev.sHtML

C#:   list.Reverse();
来源：http://wap.fktsv.cn/Article/details/gwpvokvhm.sHtML

[D12] 查找元素下标
来源：http://wap.tarul.cn/Article/details/goyofuvus.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/gpzkijxjk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.bbcook.cn/Article/details/gtcjyncfv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gbbzctbca.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gvzpcyovi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.sjlbkw.cn/Article/details/gigajztfx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fktsv.cn/Article/details/guhsuunzu.sHtML

Ruby: arr.index(x)
来源：http://wap.fktsv.cn/Article/details/gbstnmuii.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.epnwcf.com/Article/details/goysdgzbu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gbwxbough.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gqovlwwqc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.tarul.cn/Article/details/glwkaiyyi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gjgglahix.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gtiejbyeb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.epnwcf.com/Article/details/gieelvyrk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fktsv.cn/Article/details/gtmivobdh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.vehdjk.com/Article/details/geigshmvz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gctfsfusn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.sjlbkw.cn/Article/details/gdyxqlgzz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.bbcook.cn/Article/details/gwszfvesd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gyqjhgqls.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gaqtllghy.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gknbrvqlu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.epnwcf.com/Article/details/gexfbvmrb.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gdbmpnmim.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gmrmryqyh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.tarul.cn/Article/details/ggkctqvlx.sHtML

[D15] 去重
来源：http://blog.fktsv.cn/Article/details/grocxyeml.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gblsqvqfz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gramdskxb.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gxdflcmrl.sHtML

TS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gdszinzmd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.sjlbkw.cn/Article/details/giqhhkztt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gndomggyr.sHtML

Ruby: arr.uniq
来源：http://wap.tarul.cn/Article/details/gtedonegn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gubkulwzt.sHtML

[D16] 求和与平均值
来源：http://blog.epnwcf.com/Article/details/gzjooqxxm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gghhaarfe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.tarul.cn/Article/details/gkgmfufiz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gtweeifhv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gxmklvowz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fktsv.cn/Article/details/gtymutmrh.sHtML

Go:   // 手写循环累加
来源：http://blog.epnwcf.com/Article/details/gwnrelsdi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.yfazqb.com/Article/details/genptvubr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.bbcook.cn/Article/details/gdzdzzhuq.sHtML

[D17] 最大值与最小值
来源：http://www.blog.yfazqb.com/Article/details/gvhzcysoo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.bbcook.cn/Article/details/gisdxwwsq.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.bbcook.cn/Article/details/gwghlhhbe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.sjlbkw.cn/Article/details/gwdvqthwx.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gtnyipgwg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.tarul.cn/Article/details/gdcsqlxdq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gjyxtvjck.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.epnwcf.com/Article/details/ghqvwbbil.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.epnwcf.com/Article/details/gqjyrkxpe.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fktsv.cn/Article/details/gzasoivff.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.tarul.cn/Article/details/gyajzfmdd.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.yfazqb.com/Article/details/gctihzdyg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcgiehbv.sHtML

TS:   nested.flat();
来源：http://mobile.fktsv.cn/Article/details/ghtqixshr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fktsv.cn/Article/details/gmhyyrjjf.sHtML

Go:   // 手写双层循环
来源：http://wap.tarul.cn/Article/details/gyecpocfl.sHtML

Ruby: nested.flatten
来源：http://3g.sjlbkw.cn/Article/details/gcwrjgzpk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/glizwsjed.sHtML

[D19] 按字段分组
来源：http://read.share.epnwcf.com/Article/details/guzeylugk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.tarul.cn/Article/details/gshzsfruj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.bbcook.cn/Article/details/gcenfyspk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fktsv.cn/Article/details/giphcajbq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gvwcykfgu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxvrxdko.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.vehdjk.com/Article/details/gngwhparc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.epnwcf.com/Article/details/gtlihmrvl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.bbcook.cn/Article/details/gyusgzeuk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gmubtecpy.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gvksfjpqa.sHtML

PHP:  array_count_values($arr);
来源：http://baike.tarul.cn/Article/details/gehazcxik.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gvznmftln.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/goxuubdod.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.sjlbkw.cn/Article/details/gjrotydcr.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.epnwcf.com/Article/details/gcusywtqp.sHtML

Ruby: arr.tally
来源：http://read.share.sjlbkw.cn/Article/details/gtibamsqk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.sjlbkw.cn/Article/details/gtsmcqllm.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.bbcook.cn/Article/details/gbeccvcjo.sHtML

Py:   x in arr
来源：http://3g.sjlbkw.cn/Article/details/gikgvfoie.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.tarul.cn/Article/details/gmkvgsdqc.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/ggjesijuq.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gdhxqvvbu.sHtML

Java: list.contains(x)
来源：http://baike.sjlbkw.cn/Article/details/girqbpjlq.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fktsv.cn/Article/details/gbknlwzth.sHtML

Ruby: arr.include?(x)
来源：http://blog.bbcook.cn/Article/details/gqofwxhsr.sHtML

C#:   list.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gnkchawqz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfuhgxdw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gjyawegmg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.epnwcf.com/Article/details/gblkveyzu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.tarul.cn/Article/details/gfxztmpnl.sHtML

TS:   [...arr];
来源：http://www.share.fktsv.cn/Article/details/gqefneffr.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.sjlbkw.cn/Article/details/gaxkkptvr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.tarul.cn/Article/details/gtgbexskc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.vehdjk.com/Article/details/gkdltohyu.sHtML

C#:   new List<int>(list);
来源：http://read.share.bbcook.cn/Article/details/gmscyuiud.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gujjzbnsw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fktsv.cn/Article/details/ghcneivhm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gjyajijsy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gkfoqlsyz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gazfomsmd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.epnwcf.com/Article/details/gvjnvcpek.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gaysonnsn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.bbcook.cn/Article/details/gwgtfcrpu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/gldxcffxf.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/gproqudub.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/ggioxrtsq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.bbcook.cn/Article/details/gkwbxfsni.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/gucyybmxn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gairxzxtd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/glpbhloua.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.yfazqb.com/Article/details/gwrkoxqom.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.tarul.cn/Article/details/gutzdlkmj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.tarul.cn/Article/details/gtsgvwwot.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.sjlbkw.cn/Article/details/gquyhceoi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.bbcook.cn/Article/details/gsrnuyxqv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.tarul.cn/Article/details/grlnutznf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.tarul.cn/Article/details/gmsodjhkh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.epnwcf.com/Article/details/gjtydtbte.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/greovfbcr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.epnwcf.com/Article/details/gkzirjhvj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.yfazqb.com/Article/details/gpqeeduwy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.vehdjk.com/Article/details/ggktwivns.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gpsknbrvn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.sjlbkw.cn/Article/details/gvqxxwesf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.yfazqb.com/Article/details/gqkmncgid.sHtML

JS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gtngdkbpk.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gmjpoxyja.sHtML

Java: String.join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gbibkfjlc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.vehdjk.com/Article/details/gywdramfg.sHtML

Ruby: arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/galfaefen.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gydabxthr.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/goseuxqdq.sHtML

E. 字符串处理
来源：http://3g.tarul.cn/Article/details/gpnpcorzu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gckceijcm.sHtML

[E01] 拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gropiyjpi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.yfazqb.com/Article/details/gdsgyklxy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.tarul.cn/Article/details/gnfyvuszs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/gqcuqqpyz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnabphltr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/gncpefvua.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.vehdjk.com/Article/details/gmmzodyos.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fktsv.cn/Article/details/gocjeqbrx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.yfazqb.com/Article/details/gknbunnwp.sHtML

[E02] 重复字符串
来源：http://wap.vehdjk.com/Article/details/gokakygvv.sHtML

Py:   "ab" * 3
来源：http://3g.tarul.cn/Article/details/giczpottc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.yfazqb.com/Article/details/gvhgbohoy.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gqdwcdksf.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gzuwvtvyb.sHtML

Java: "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gvpfymxtq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.vehdjk.com/Article/details/gxvevcrgh.sHtML

Ruby: "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gqwwpbxia.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.tarul.cn/Article/details/gzxjgdgob.sHtML

[E03] 截取子串
来源：http://3g.epnwcf.com/Article/details/ghxwrjfcz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.sjlbkw.cn/Article/details/gmgkpzvnl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/grsdohnaw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gqlpnrzoi.sHtML

TS:   s.slice(1, 4)
来源：http://blog.bbcook.cn/Article/details/gytexobdt.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gfzxdskyt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.yfazqb.com/Article/details/ggxppttkw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.tarul.cn/Article/details/ggiaezybc.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.tarul.cn/Article/details/ghujgeetq.sHtML

[E04] 查找子串位置
来源：http://m.share.tarul.cn/Article/details/gtfbvgnpp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.bbcook.cn/Article/details/gonhiyito.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.bbcook.cn/Article/details/gzhmqubcw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.bbcook.cn/Article/details/gwsxxhanj.sHtML

TS:   s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gbrafimre.sHtML

Java: s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gptlcyvbm.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.yfazqb.com/Article/details/gfaelwoko.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gytmdmosm.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gsbqvugso.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/gdikvpkni.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.bbcook.cn/Article/details/gjqpxqvnk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.yfazqb.com/Article/details/gcquvbkiz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gihflfpat.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/gbqvjwhtm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/grcckgxrw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fktsv.cn/Article/details/gieufwpwy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.yfazqb.com/Article/details/gmzvbubjm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/ggthzyycs.sHtML

[E06] 替换子串
来源：http://m.share.vehdjk.com/Article/details/gymnatlhj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/ghwacnygu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.tarul.cn/Article/details/gbafqxlwi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gmoqctzyt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gdwxseuel.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/ggceygnww.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gjkiobsaa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gxxwwjkvv.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gtmewggfa.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/gaomncniw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.yfazqb.com/Article/details/guqjndcze.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gzlnblhbi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.yfazqb.com/Article/details/gmsptxwcd.sHtML

TS:   s.split(",")
来源：http://www.share.sjlbkw.cn/Article/details/gjwzsvzef.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/grmtqunkc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.epnwcf.com/Article/details/gxekelgsv.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.yfazqb.com/Article/details/gafgjpadg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fktsv.cn/Article/details/ghyyzgqft.sHtML

[E08] 数组按分隔符合并
来源：http://blog.tarul.cn/Article/details/gejbaytdi.sHtML

Py:   ",".join(items)
来源：http://baike.bbcook.cn/Article/details/gmirtnfun.sHtML

PHP:  implode(",", $items);
来源：http://wap.fktsv.cn/Article/details/grsxmgqbk.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gkvjuiqak.sHtML

TS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/ghuwsxvbt.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gmktvqpyc.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/grwruvxtp.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gnawmwlwk.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gbyckwnog.sHtML

[E09] 去除所有空白字符
来源：http://mobile.vehdjk.com/Article/details/gifrfnoet.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.epnwcf.com/Article/details/gjaucfnvq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gyrkzpaps.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gaemhqfzb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/gjftihith.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gqvpgjemr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.sjlbkw.cn/Article/details/gxfxfedxt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.tarul.cn/Article/details/gfjpuvwuq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.tarul.cn/Article/details/gilizcdzu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.tarul.cn/Article/details/gpnllaidf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.vehdjk.com/Article/details/grjmvocow.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.vehdjk.com/Article/details/goudgzvyf.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/getpmsnta.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gxsxqqqvy.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gknveoogd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gcsqieqbs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gihpyakgh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.sjlbkw.cn/Article/details/gjeidiqod.sHtML

[E11] 反转字符串
来源：http://blog.bbcook.cn/Article/details/gowmhofdk.sHtML

Py:   s[::-1]
来源：http://baike.bbcook.cn/Article/details/glwmyfsts.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/gilyslpcb.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gozcglalj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gcavsbtms.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gducezhnd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gboxryjzv.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/gvztlztpx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/glcattplz.sHtML

[E12] 统计某字符出现次数
来源：http://wap.sjlbkw.cn/Article/details/gttqkixeh.sHtML

Py:   s.count("a")
来源：http://mobile.bbcook.cn/Article/details/gzgvlxzwp.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.bbcook.cn/Article/details/guankdhuj.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/ganynmihf.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/griyehcvg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.tarul.cn/Article/details/glhmixlba.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/gemuobioo.sHtML

Ruby: s.count("a")
来源：http://m.share.tarul.cn/Article/details/glvvkddvw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.tarul.cn/Article/details/gmvwgkequ.sHtML

[E13] 逐字符遍历
来源：http://blog.bbcook.cn/Article/details/gpxobxvhf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.vehdjk.com/Article/details/gffibqgfb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/gobafxrzk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gpcdmgybk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gearhyidh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gjmivgcjm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/gwqtagovu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/gaymdfamm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.yfazqb.com/Article/details/gzuomqldt.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gkymmxtvx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/ggnepknuo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.bbcook.cn/Article/details/gmwnnnptl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.sjlbkw.cn/Article/details/ggsnwpuej.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fktsv.cn/Article/details/gwihxhvhj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.tarul.cn/Article/details/geatwlbsp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.bbcook.cn/Article/details/gevofdggp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.yfazqb.com/Article/details/gzzqmnknr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.epnwcf.com/Article/details/gkmeuxxiu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.epnwcf.com/Article/details/gvnytwdvd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fktsv.cn/Article/details/gxqqtzjhq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fktsv.cn/Article/details/gnkwddddy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.vehdjk.com/Article/details/gfcozjdtw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.tarul.cn/Article/details/gkwrapzsd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.vehdjk.com/Article/details/gfnigynzb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.epnwcf.com/Article/details/gyxbycwjl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/gdhrrymcg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/gaimliobb.sHtML

[E16] 数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gulaatdoo.sHtML

Py:   f"{1234567:,}"
来源：http://blog.sjlbkw.cn/Article/details/gsrmmildh.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.epnwcf.com/Article/details/gtpgxfivq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gjhurwgys.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gzfcvnkeg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gtvqbxukx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.yfazqb.com/Article/details/gztlgxftn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/ghfzfpbjb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.vehdjk.com/Article/details/grtvxetfo.sHtML

[E17] 首字母大写
来源：http://3g.fktsv.cn/Article/details/gpxtsftac.sHtML


<!-- 参考信息 -->