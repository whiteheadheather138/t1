代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gdwgwltkq.sHtML

Java: list.subList(1, 4);
来源：http://3g.fktsv.cn/Article/details/gtjtnwigb.sHtML

Go:   arr[1:4]
来源：http://3g.epnwcf.com/Article/details/ggpnxfqtl.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.tarul.cn/Article/details/gmssbpaaz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/ghmwqxbmh.sHtML

[D08] 合并两个数组
来源：http://read.share.yfazqb.com/Article/details/gofjlshzy.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.sjlbkw.cn/Article/details/gsugwlapa.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.bbcook.cn/Article/details/gviiezsrv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fktsv.cn/Article/details/gggmlgzec.sHtML

TS:   [...a, ...b];
来源：http://blog.bbcook.cn/Article/details/gqegngizz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.tarul.cn/Article/details/ggmqsqcnl.sHtML

Go:   append(a, b...)
来源：http://m.share.vehdjk.com/Article/details/gaxvujcyj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.vehdjk.com/Article/details/gpuqjwkle.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.bbcook.cn/Article/details/gbkvrrtkk.sHtML

[D09] 排序（升序）
来源：http://read.share.tarul.cn/Article/details/gaodelgue.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gqhvkalon.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/gdmcphlbw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.bbcook.cn/Article/details/gojnkwdxs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.vehdjk.com/Article/details/gngglofgr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.tarul.cn/Article/details/gpkivqnau.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/ggewstmtr.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gbsekasdc.sHtML

C#:   list.Sort();
来源：http://www.m.share.epnwcf.com/Article/details/gqbpwhgen.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.tarul.cn/Article/details/gepqbtymq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/gvtqdexti.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/gajtasrpj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.yfazqb.com/Article/details/gcrwtnfkg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/guweqgduo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.yfazqb.com/Article/details/gsoyvoymk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fktsv.cn/Article/details/gnvqkhhbm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.vehdjk.com/Article/details/ghzxoifuz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.bbcook.cn/Article/details/gvcpcqopn.sHtML

[D11] 反转数组
来源：http://wap.yfazqb.com/Article/details/gzjkwofxn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.bbcook.cn/Article/details/ggdzgiuzy.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.vehdjk.com/Article/details/gdlftduzq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.epnwcf.com/Article/details/gaqpeculk.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gzpuefyfk.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.vehdjk.com/Article/details/grhoybnxl.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fktsv.cn/Article/details/gqngvvlbg.sHtML

Ruby: arr.reverse
来源：http://baike.tarul.cn/Article/details/ghsqccbzz.sHtML

C#:   list.Reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gvlrnlilu.sHtML

[D12] 查找元素下标
来源：http://www.share.tarul.cn/Article/details/gnteurkgt.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.bbcook.cn/Article/details/gxyxrgkfe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gobdbadqx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/gdkbjgmzr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gljuyxkud.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.sjlbkw.cn/Article/details/glglbjxlg.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.tarul.cn/Article/details/ghlltnvmq.sHtML

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/ghlznhkrs.sHtML

C#:   list.IndexOf(x);
来源：http://blog.epnwcf.com/Article/details/gpemljkvh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.epnwcf.com/Article/details/gvgxgargv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.bbcook.cn/Article/details/gufybipsm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fktsv.cn/Article/details/gpujxkomv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fktsv.cn/Article/details/ggwphxqoh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.sjlbkw.cn/Article/details/gxavdcfyg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.yfazqb.com/Article/details/ggrfhtwdm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.yfazqb.com/Article/details/gxeqkddly.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.yfazqb.com/Article/details/geurpgtyz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/grqntewdr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.yfazqb.com/Article/details/gzfgjdkda.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.vehdjk.com/Article/details/gqcwbglrs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gswseqdxk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gugzbxbip.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.yfazqb.com/Article/details/gwgfecphp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.vehdjk.com/Article/details/gqefzuyya.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gckykxjis.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gsrfbtcrn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.bbcook.cn/Article/details/gqxvcsjdh.sHtML

[D15] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gldhogrbh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gsknpwvln.sHtML

PHP:  array_unique($arr);
来源：http://3g.bbcook.cn/Article/details/gzrkldras.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gdlizlwrj.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gmibdzydr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.bbcook.cn/Article/details/geqasyrlz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.bbcook.cn/Article/details/glglpksrm.sHtML

Ruby: arr.uniq
来源：http://baike.epnwcf.com/Article/details/gjylupkfe.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.sjlbkw.cn/Article/details/ggpwfsvbb.sHtML

[D16] 求和与平均值
来源：http://read.share.yfazqb.com/Article/details/gzcunwtiy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.vehdjk.com/Article/details/gelsojdkh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fktsv.cn/Article/details/giiptzygc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gkihjqnwa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/ggtxuifus.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/gkfkqrgjl.sHtML

Go:   // 手写循环累加
来源：http://blog.tarul.cn/Article/details/gbdzliloe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.epnwcf.com/Article/details/gnjodsrtr.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.epnwcf.com/Article/details/gahjmibnm.sHtML

[D17] 最大值与最小值
来源：http://wap.sjlbkw.cn/Article/details/gxukiwsbb.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.tarul.cn/Article/details/gxwgrddeg.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gexovgbpn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.tarul.cn/Article/details/gqzmtirng.sHtML

TS:   Math.max(...arr);
来源：http://mobile.tarul.cn/Article/details/guagpsfkv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.epnwcf.com/Article/details/ggycjhmdr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.bbcook.cn/Article/details/ghhyytqxv.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.epnwcf.com/Article/details/gzpuzboxp.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.sjlbkw.cn/Article/details/gslbgddqg.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.yfazqb.com/Article/details/gzzppvjif.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.epnwcf.com/Article/details/gytqetski.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/gjsmqewih.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.bbcook.cn/Article/details/gdbyvhcrt.sHtML

TS:   nested.flat();
来源：http://blog.tarul.cn/Article/details/gefoeczgk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.vehdjk.com/Article/details/gawzawmzo.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/gdvhxfgop.sHtML

Ruby: nested.flatten
来源：http://www.share.yfazqb.com/Article/details/ggxdskhmp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fktsv.cn/Article/details/ghkwkqgdh.sHtML

[D19] 按字段分组
来源：http://www.share.vehdjk.com/Article/details/gisedtsoz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gfpnsulhv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.yfazqb.com/Article/details/glgbpuuzz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.yfazqb.com/Article/details/gchmnxmlx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/gmhjkdqrx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.bbcook.cn/Article/details/gshnsmkyu.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.tarul.cn/Article/details/gfryctqtp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.tarul.cn/Article/details/guuaxwrms.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/ggemqjzup.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.tarul.cn/Article/details/gukjqmgod.sHtML

Py:   Counter(arr)
来源：http://mobile.sjlbkw.cn/Article/details/grjxkhrtk.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.bbcook.cn/Article/details/ggrxveipc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gseelukqn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.yfazqb.com/Article/details/gcnzbxmcg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.bbcook.cn/Article/details/ggwcnoeqz.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.sjlbkw.cn/Article/details/gvbtrykbs.sHtML

Ruby: arr.tally
来源：http://wap.tarul.cn/Article/details/gyjrlzxbv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.tarul.cn/Article/details/gcgraitcp.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.bbcook.cn/Article/details/gpgdjhpbx.sHtML

Py:   x in arr
来源：http://www.blog.yfazqb.com/Article/details/greagevwu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.vehdjk.com/Article/details/gzfztqyxd.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/giiekwzuf.sHtML

TS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/gdcmqjobk.sHtML

Java: list.contains(x)
来源：http://mobile.bbcook.cn/Article/details/gxctnrydn.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gwcbpjviu.sHtML

Ruby: arr.include?(x)
来源：http://3g.vehdjk.com/Article/details/gtmfwyytp.sHtML

C#:   list.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gthxtpday.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.sjlbkw.cn/Article/details/gdlzcajtu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.epnwcf.com/Article/details/glpynyzyq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.tarul.cn/Article/details/gilsbihwa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.epnwcf.com/Article/details/ggprmbnjp.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/gtqsvirqc.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.bbcook.cn/Article/details/ghgrkymfw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gnonxrmgc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.tarul.cn/Article/details/ggggvcuha.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/gxrwmhjri.sHtML

[D23] reduce 累积计算
来源：http://3g.tarul.cn/Article/details/ghxgjtfbg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.epnwcf.com/Article/details/gbvkazurt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.vehdjk.com/Article/details/gbwcfnjza.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gyyghyepg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gjkqmvjed.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.vehdjk.com/Article/details/gkvhvukra.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gdtxefogb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.bbcook.cn/Article/details/gdzfcfmvu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.vehdjk.com/Article/details/gmiqulnnz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/grxpbkhpc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.yfazqb.com/Article/details/ghcjovejh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.bbcook.cn/Article/details/gyteuvrbt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gjckuxtvk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.epnwcf.com/Article/details/gmslzfxwb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fktsv.cn/Article/details/ghwebufag.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.vehdjk.com/Article/details/ghxhmdeii.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.sjlbkw.cn/Article/details/gqhqwxryy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.yfazqb.com/Article/details/gvfvqsxvc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.yfazqb.com/Article/details/gamvqrgwx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.sjlbkw.cn/Article/details/gneaxowvg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gtzblhego.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.epnwcf.com/Article/details/gagomzqhk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.bbcook.cn/Article/details/geztubmpq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gxnpkektd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.yfazqb.com/Article/details/gfwantbtv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.vehdjk.com/Article/details/gxxnvgtdb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gmuqobfkd.sHtML

[D26] 数组转字符串
来源：http://read.share.fktsv.cn/Article/details/gjdchricx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.yfazqb.com/Article/details/grphwlqot.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.yfazqb.com/Article/details/glhilgcxs.sHtML

JS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/giwpjvnwu.sHtML

TS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/grqqsorlt.sHtML

Java: String.join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/gbgduaoac.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/grrizwwge.sHtML

Ruby: arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gxgvscpwk.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gokjgrzft.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcrbccyhk.sHtML

E. 字符串处理
来源：http://blog.sjlbkw.cn/Article/details/gmcmiseel.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grxqwbjni.sHtML

[E01] 拼接字符串
来源：http://3g.fktsv.cn/Article/details/gklizxfrf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/gaocvlbta.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/glfjggelg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gbnprnnzm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/gdogvtqjm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/gyuiavzet.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.bbcook.cn/Article/details/gqzuuxbgw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/gozxbempz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gqwedlqzy.sHtML

[E02] 重复字符串
来源：http://baike.fktsv.cn/Article/details/giumcombq.sHtML

Py:   "ab" * 3
来源：http://3g.bbcook.cn/Article/details/gwyhbpqkh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.sjlbkw.cn/Article/details/gkleeliaw.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/grzedsldm.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/geuhebiyh.sHtML

Java: "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gdtnqdkfx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fktsv.cn/Article/details/glzimhfyr.sHtML

Ruby: "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gckfvmnla.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fktsv.cn/Article/details/geemohyeb.sHtML

[E03] 截取子串
来源：http://baike.fktsv.cn/Article/details/grhziowdp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.tarul.cn/Article/details/gwgqtnurb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gvpjwamtl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gkzcnjcqf.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gxznwyrse.sHtML

Java: s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gkfrayvfs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.tarul.cn/Article/details/gatccpctn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.yfazqb.com/Article/details/gnipmdbtj.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.vehdjk.com/Article/details/gvldofkcj.sHtML

[E04] 查找子串位置
来源：http://wap.yfazqb.com/Article/details/gyqhavrwx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.bbcook.cn/Article/details/gecokqyeg.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.yfazqb.com/Article/details/grpehsjww.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.yfazqb.com/Article/details/gvlxoiuir.sHtML

TS:   s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/galdlyucn.sHtML

Java: s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gpnmrtlzg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.bbcook.cn/Article/details/gkkxgdbat.sHtML

Ruby: s.index("x")
来源：http://mobile.vehdjk.com/Article/details/gtxlbaukf.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gibsdqpsp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.sjlbkw.cn/Article/details/gnyntrbyb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.sjlbkw.cn/Article/details/ggtyeufdv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.epnwcf.com/Article/details/gwubwvpwk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gqxfoqhbx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.tarul.cn/Article/details/ghhmlujze.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gutjsaqwx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.epnwcf.com/Article/details/gyqqckiyp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.tarul.cn/Article/details/gbaxmhcsu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gszzipsdg.sHtML

[E06] 替换子串
来源：http://www.blog.fktsv.cn/Article/details/ggulewxuv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gibxuwtoq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/gcjazecti.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gvbmrieuc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/geaykbvsz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gowdumahx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/gxmafchcw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/ghvxzevxq.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/gljakmlwl.sHtML

[E07] 按分隔符拆分
来源：http://wap.yfazqb.com/Article/details/gefvusndw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/gvsnhqtfa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fktsv.cn/Article/details/grwqsffdd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.sjlbkw.cn/Article/details/gckdlffnr.sHtML

TS:   s.split(",")
来源：http://mobile.fktsv.cn/Article/details/goreuidwd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.sjlbkw.cn/Article/details/gkzfdnreb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/gjadnxhea.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gfnloptkc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.yfazqb.com/Article/details/gspgmbqbt.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.tarul.cn/Article/details/ggukygrxm.sHtML

Py:   ",".join(items)
来源：http://www.blog.epnwcf.com/Article/details/gyywjsgfn.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.tarul.cn/Article/details/ghflywlqh.sHtML

JS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gneixgrna.sHtML

TS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gtoadwkdi.sHtML

Java: String.join(",", items)
来源：http://baike.tarul.cn/Article/details/gjfdrxryo.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.epnwcf.com/Article/details/gqebgwkxx.sHtML

Ruby: items.join(",")
来源：http://mobile.tarul.cn/Article/details/gyuzbfdyw.sHtML

C#:   string.Join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/goqdtddet.sHtML

[E09] 去除所有空白字符
来源：http://3g.vehdjk.com/Article/details/gsdxavplc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fktsv.cn/Article/details/golxbdxps.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.sjlbkw.cn/Article/details/geqiaagmy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/ghsridjub.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gehavxkyf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.bbcook.cn/Article/details/gjzpfqmmd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.vehdjk.com/Article/details/gyjzyxahz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.vehdjk.com/Article/details/gyeotmmgw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/gccgdfdsg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.tarul.cn/Article/details/gwmdubfkz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/geedhzwun.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/gxleqntrh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/getdapmba.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gfhvcaiwl.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gilsnhxoq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/ghpqnjpgv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/ghsallaus.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.bbcook.cn/Article/details/gzhibtkey.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gwejrqddc.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gurargpdw.sHtML

PHP:  strrev($s);
来源：http://3g.tarul.cn/Article/details/gsqkzifkw.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gqjwoafat.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gphbpgqpu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.sjlbkw.cn/Article/details/gtyumeulu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gwisfmcma.sHtML

Ruby: s.reverse
来源：http://blog.vehdjk.com/Article/details/gmterbnip.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.yfazqb.com/Article/details/gprnyzipv.sHtML

[E12] 统计某字符出现次数
来源：http://blog.epnwcf.com/Article/details/gzqfxepnh.sHtML

Py:   s.count("a")
来源：http://blog.bbcook.cn/Article/details/gaypdnvgz.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gljpefimd.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.epnwcf.com/Article/details/gtsnlcara.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/gtghkxjcu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.epnwcf.com/Article/details/gbjfaoter.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.tarul.cn/Article/details/ghbnockcb.sHtML

Ruby: s.count("a")
来源：http://www.share.tarul.cn/Article/details/gxwghuawa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.bbcook.cn/Article/details/grfoxkqbq.sHtML

[E13] 逐字符遍历
来源：http://baike.bbcook.cn/Article/details/gakndorfy.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gcsbojxpn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fktsv.cn/Article/details/grwbltorq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gtoycpejt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gqdyvnfgc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.tarul.cn/Article/details/gqqujhbak.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmghpszh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.bbcook.cn/Article/details/grvbabqfz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.bbcook.cn/Article/details/gwtovrcic.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.sjlbkw.cn/Article/details/gqkrpxeqt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.yfazqb.com/Article/details/gshwzbhov.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.yfazqb.com/Article/details/gcjjakbip.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.vehdjk.com/Article/details/gtlhkfxjz.sHtML


<!-- 参考信息 -->