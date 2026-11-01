代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fktsv.cn/Article/details/glvcjjwtf.sHtML

TS:   [...a, ...b];
来源：http://baike.sjlbkw.cn/Article/details/gsvafsioi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.vehdjk.com/Article/details/gbnbvfpuj.sHtML

Go:   append(a, b...)
来源：http://mobile.tarul.cn/Article/details/gquakhuxv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.tarul.cn/Article/details/gdaetdpqo.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.yfazqb.com/Article/details/gfznmejvi.sHtML

[D09] 排序（升序）
来源：http://blog.sjlbkw.cn/Article/details/gcdwljyxr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gbiptcqed.sHtML

PHP:  sort($arr);
来源：http://www.share.epnwcf.com/Article/details/gtbjezjqr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.yfazqb.com/Article/details/genrrcvcj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.vehdjk.com/Article/details/gshbazopg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.bbcook.cn/Article/details/gdtymqhmu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gszgugkfy.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/grprjakuq.sHtML

C#:   list.Sort();
来源：http://www.m.share.vehdjk.com/Article/details/gjsuifxgp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.tarul.cn/Article/details/geuuqzygy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fktsv.cn/Article/details/gaursbpsz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gtpcvsnsa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gdykbjxtw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gmzxxmntm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.tarul.cn/Article/details/gwljyjycm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fktsv.cn/Article/details/gtcukdxcj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/gzelpsppe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.tarul.cn/Article/details/gnubnfxpb.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/gwxivckdk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.epnwcf.com/Article/details/gpsuhhslj.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.vehdjk.com/Article/details/gqhfzxnij.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.sjlbkw.cn/Article/details/gvqegrusp.sHtML

TS:   [...arr].reverse();
来源：http://baike.epnwcf.com/Article/details/gkdzhilvi.sHtML

Java: Collections.reverse(list);
来源：http://m.share.sjlbkw.cn/Article/details/ggeykbooy.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.epnwcf.com/Article/details/goyvlcvcv.sHtML

Ruby: arr.reverse
来源：http://blog.fktsv.cn/Article/details/gfqxmvnzu.sHtML

C#:   list.Reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gmshucerr.sHtML

[D12] 查找元素下标
来源：http://m.share.vehdjk.com/Article/details/gumzsvnya.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fktsv.cn/Article/details/guzbaecoe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gtsuubsve.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gijpqvwkz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gtttjfkwk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.tarul.cn/Article/details/gqzpuzkbc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gpytrsjgo.sHtML

Ruby: arr.index(x)
来源：http://www.blog.bbcook.cn/Article/details/gyldgttnw.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/gcwrsayqf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gzmdsljvj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fktsv.cn/Article/details/gavxvhxxc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.sjlbkw.cn/Article/details/glfcfskjm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.tarul.cn/Article/details/gbcraounz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gcqajihfi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/ghcammxmh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gcnwyajdo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/gmmkhgwjq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.bbcook.cn/Article/details/gnalxayvs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.yfazqb.com/Article/details/gyenlypwg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gcidgmfcf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.tarul.cn/Article/details/gyeasixzf.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/ghwawarqx.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gigjjucpt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.epnwcf.com/Article/details/gvpzxqayj.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqpnqhuz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.bbcook.cn/Article/details/grhpvpgop.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.tarul.cn/Article/details/gjffocghp.sHtML

[D15] 去重
来源：http://read.share.vehdjk.com/Article/details/gfhjqxxhp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gjnstbvue.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gauywcoba.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gqccerlui.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gbbhpfxow.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/gavykfybq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/gomyechlj.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/gnbrugjax.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gcqcorniy.sHtML

[D16] 求和与平均值
来源：http://baike.sjlbkw.cn/Article/details/geqthhiwd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gkvszjyyj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.vehdjk.com/Article/details/ggopmsllz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gfxiebfxs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gvxxiyvgc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.sjlbkw.cn/Article/details/gxebyzpqa.sHtML

Go:   // 手写循环累加
来源：http://baike.vehdjk.com/Article/details/gagfogvjj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/gpaskfugh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fktsv.cn/Article/details/ghweuncwg.sHtML

[D17] 最大值与最小值
来源：http://wap.yfazqb.com/Article/details/gycmehaiw.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.epnwcf.com/Article/details/gpisjcswt.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.epnwcf.com/Article/details/glybybwdn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.vehdjk.com/Article/details/gzbsftuyd.sHtML

TS:   Math.max(...arr);
来源：http://wap.yfazqb.com/Article/details/gkzymfxjc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.tarul.cn/Article/details/gnonesrcr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.yfazqb.com/Article/details/gtwehgyyf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.bbcook.cn/Article/details/gvakwpgfu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/gnmqozvny.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.tarul.cn/Article/details/gyecfwemv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.sjlbkw.cn/Article/details/gpnthnozk.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/gaujqnwvs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.sjlbkw.cn/Article/details/gdihxrutb.sHtML

TS:   nested.flat();
来源：http://blog.yfazqb.com/Article/details/gwyfaablp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjvpjyjc.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/gpyydjnzv.sHtML

Ruby: nested.flatten
来源：http://www.blog.epnwcf.com/Article/details/gvvunwedi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.epnwcf.com/Article/details/gjdwhryhe.sHtML

[D19] 按字段分组
来源：http://www.m.share.vehdjk.com/Article/details/gdabejqjw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fktsv.cn/Article/details/gjvafrxvl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.tarul.cn/Article/details/gkzgcrwfl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/grwdyfvbs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.vehdjk.com/Article/details/gcjcrlngg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.vehdjk.com/Article/details/gpjdrowbj.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.yfazqb.com/Article/details/gvojqdgbg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.tarul.cn/Article/details/ggxigfpjz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.tarul.cn/Article/details/gmsibtaud.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fktsv.cn/Article/details/gpolkvdgr.sHtML

Py:   Counter(arr)
来源：http://read.share.bbcook.cn/Article/details/gomyxlckq.sHtML

PHP:  array_count_values($arr);
来源：http://wap.bbcook.cn/Article/details/gbrvxrser.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.bbcook.cn/Article/details/gntpxqqcf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/grghusojx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.tarul.cn/Article/details/gqjeojsfy.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.sjlbkw.cn/Article/details/gorrljsqf.sHtML

Ruby: arr.tally
来源：http://baike.yfazqb.com/Article/details/gxmtjahpr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.yfazqb.com/Article/details/gusuqjfrt.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fktsv.cn/Article/details/grkagkkuy.sHtML

Py:   x in arr
来源：http://baike.tarul.cn/Article/details/gvoeeqgmc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.epnwcf.com/Article/details/ggbokjcvq.sHtML

JS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gfgfuilbb.sHtML

TS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gywnzmbyd.sHtML

Java: list.contains(x)
来源：http://baike.fktsv.cn/Article/details/gcbunudwa.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.vehdjk.com/Article/details/gfeioovds.sHtML

Ruby: arr.include?(x)
来源：http://blog.fktsv.cn/Article/details/gmzodzicf.sHtML

C#:   list.Contains(x)
来源：http://blog.bbcook.cn/Article/details/grspvjgzh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/gdbirfnbk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.bbcook.cn/Article/details/gusxcxzgz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.vehdjk.com/Article/details/gjxqshtht.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.yfazqb.com/Article/details/gtxrnjjxd.sHtML

TS:   [...arr];
来源：http://baike.vehdjk.com/Article/details/glganlbwa.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.sjlbkw.cn/Article/details/gpillxrnb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fktsv.cn/Article/details/gtbycvkml.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.epnwcf.com/Article/details/ghkxjfcov.sHtML

C#:   new List<int>(list);
来源：http://read.share.bbcook.cn/Article/details/gmamvctob.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/gvnzepxaq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.bbcook.cn/Article/details/gsehlqncd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.yfazqb.com/Article/details/gnoxhjaiy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gobdnrsoa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gmtahapxx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.vehdjk.com/Article/details/gsuhrgqnn.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/ggultmcgp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fktsv.cn/Article/details/gtdnvpqvp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/gmhvlwxwn.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.epnwcf.com/Article/details/grzlkxick.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.yfazqb.com/Article/details/glybyycek.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fktsv.cn/Article/details/gjqsddftx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.yfazqb.com/Article/details/gelfemrgr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.tarul.cn/Article/details/glqirjlrc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/ggkxhvucb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/gatbrvqdv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/gwjihyura.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.vehdjk.com/Article/details/gofnssnqd.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/ggsmvbhwv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fktsv.cn/Article/details/gqqsqqtnr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.epnwcf.com/Article/details/ggnugruhb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.tarul.cn/Article/details/ggnojnkpu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.vehdjk.com/Article/details/gvagithox.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/gnwdpsqei.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.yfazqb.com/Article/details/gxrmadmrq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.yfazqb.com/Article/details/gsnpyuwnk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/glgaxzsmj.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gpqstrodg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.tarul.cn/Article/details/geyofbvob.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/gcbjthamx.sHtML

JS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/ggzspyvtw.sHtML

TS:   arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gqzqmmmza.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gffjpzgli.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.bbcook.cn/Article/details/gwmsgnjst.sHtML

Ruby: arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gqxwjbjiv.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gguxcplzv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxvuwihxn.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/giedeahwd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghtvxaafc.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gksfdsini.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.epnwcf.com/Article/details/goggqbzqe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.tarul.cn/Article/details/gwubsirgi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gdncmsvnt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/glyvwlsto.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.bbcook.cn/Article/details/grascmphr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/glwvxyxes.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.sjlbkw.cn/Article/details/gkywomlsw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gyxziwumu.sHtML

[E02] 重复字符串
来源：http://www.blog.bbcook.cn/Article/details/gvrlsgnpm.sHtML

Py:   "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gknwgrqqi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fktsv.cn/Article/details/gedubqpde.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gfocbhrxx.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gyeexcvgt.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gggcdzzih.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/gfkkbehvo.sHtML

Ruby: "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gcwolvdyv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.vehdjk.com/Article/details/gluvnfxlb.sHtML

[E03] 截取子串
来源：http://mobile.epnwcf.com/Article/details/glonidcbi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.sjlbkw.cn/Article/details/guhaopowy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gxfrwosjy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gsfymebsx.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gldlumawb.sHtML

Java: s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/gxxnbadtd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gibmlwehp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/gqayqqtcb.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.tarul.cn/Article/details/gifngmisx.sHtML

[E04] 查找子串位置
来源：http://www.blog.vehdjk.com/Article/details/gasgwwxxm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gomdxcjiu.sHtML

PHP:  strpos($s, "x");
来源：http://blog.epnwcf.com/Article/details/gmjbdfblf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.bbcook.cn/Article/details/gtugfnmoc.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gegvqlrro.sHtML

Java: s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gtzlmuwha.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fktsv.cn/Article/details/gfnbcikvo.sHtML

Ruby: s.index("x")
来源：http://wap.vehdjk.com/Article/details/guvzeokwi.sHtML

C#:   s.IndexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gvjyrhsyn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.vehdjk.com/Article/details/gtkmlyhlr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.bbcook.cn/Article/details/gpiatczsl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.epnwcf.com/Article/details/gvgysvcvp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gcaxsvxgf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.tarul.cn/Article/details/gdxhrktro.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gtfpszase.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.vehdjk.com/Article/details/gpahskate.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fktsv.cn/Article/details/gclwakebm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gxjjqyhnf.sHtML

[E06] 替换子串
来源：http://3g.yfazqb.com/Article/details/gjhprcjpq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/glxpnyxvp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/gikixdzzx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/ghmrneerc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gqgqyowjw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gehjvevzp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fktsv.cn/Article/details/grgwmqxdg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gwaudpmes.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.yfazqb.com/Article/details/gimfaawyk.sHtML

[E07] 按分隔符拆分
来源：http://baike.sjlbkw.cn/Article/details/gunvbpxqq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fktsv.cn/Article/details/gemfhxspi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gdgtcpink.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.vehdjk.com/Article/details/grbemcwyn.sHtML

TS:   s.split(",")
来源：http://www.m.share.bbcook.cn/Article/details/goxilbpzc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.tarul.cn/Article/details/gdiqtqwrf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fktsv.cn/Article/details/gpdsowivz.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fktsv.cn/Article/details/gvsqsqqlh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpciutuyu.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.epnwcf.com/Article/details/gersoxwcd.sHtML

Py:   ",".join(items)
来源：http://www.share.epnwcf.com/Article/details/gjvxmzvpo.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.vehdjk.com/Article/details/gdeoasgii.sHtML

JS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gupvswcbw.sHtML

TS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gzpaigtfi.sHtML

Java: String.join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gnpqlqegv.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.tarul.cn/Article/details/gphliaunr.sHtML

Ruby: items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/ggqxwlldw.sHtML

C#:   string.Join(",", items)
来源：http://blog.tarul.cn/Article/details/gvhlfqmjk.sHtML

[E09] 去除所有空白字符
来源：http://m.share.sjlbkw.cn/Article/details/gkchzpegy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/guhaodmbk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.sjlbkw.cn/Article/details/goumivvrc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gxpedmahr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gvxluiopp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fktsv.cn/Article/details/garqbxqfc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.bbcook.cn/Article/details/gstjbnzyb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.sjlbkw.cn/Article/details/gpkzuuijw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.epnwcf.com/Article/details/gueowljuu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.vehdjk.com/Article/details/ghepqrtsh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/ggarckqwn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.tarul.cn/Article/details/gevtvizsd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gvqxspegi.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gfxrdznbq.sHtML

Java: String.format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/glmrjqbcw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/ggpkjsxei.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gwxjtzcej.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.bbcook.cn/Article/details/gpfzutpfh.sHtML

[E11] 反转字符串
来源：http://www.share.fktsv.cn/Article/details/gqnzytxhl.sHtML

Py:   s[::-1]
来源：http://read.share.fktsv.cn/Article/details/gzkofrsqk.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gniyatsfb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gcorcijbe.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/goyvxneid.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.tarul.cn/Article/details/gviapsdgw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gqbqdchhw.sHtML

Ruby: s.reverse
来源：http://www.share.fktsv.cn/Article/details/gvkdmfsbv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/ghkyayvoy.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fktsv.cn/Article/details/gvxrioxmh.sHtML

Py:   s.count("a")
来源：http://baike.epnwcf.com/Article/details/gsinfmmyl.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.yfazqb.com/Article/details/ghsizfzhk.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fktsv.cn/Article/details/ghkdsyxog.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gzizbzeih.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/gbbvgfzjc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/grrimuldc.sHtML

Ruby: s.count("a")
来源：http://baike.yfazqb.com/Article/details/gcpquiqfy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.epnwcf.com/Article/details/gqgqffpdp.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.epnwcf.com/Article/details/guaealrze.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.tarul.cn/Article/details/gqvckoigv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.sjlbkw.cn/Article/details/guicatclk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gpsxkjbkg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.epnwcf.com/Article/details/gniyqnimt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.tarul.cn/Article/details/glueweqfu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.tarul.cn/Article/details/gtzxqotmm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.vehdjk.com/Article/details/gydxmzspz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjtupxld.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.epnwcf.com/Article/details/gpevmogdh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.tarul.cn/Article/details/gljuksafq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.bbcook.cn/Article/details/gyeliwpll.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.sjlbkw.cn/Article/details/gfgdadvcu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.epnwcf.com/Article/details/glkjoexyz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.yfazqb.com/Article/details/goorwjtdr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.vehdjk.com/Article/details/gzkyqrezk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.epnwcf.com/Article/details/goetvdcvu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.vehdjk.com/Article/details/gmnucrnsx.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.tarul.cn/Article/details/gaxvnzogp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fktsv.cn/Article/details/gokoaxlgv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.tarul.cn/Article/details/glgugfinb.sHtML


<!-- 参考信息 -->