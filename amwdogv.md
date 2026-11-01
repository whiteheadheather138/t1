代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gjrezurlp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gcxswjxzq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gjylyjohi.sHtML

[D06] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gycfvdmst.sHtML

Py:   len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/geewoxmng.sHtML

PHP:  count($arr);
来源：http://read.share.vehdjk.com/Article/details/gconevanc.sHtML

JS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/gwzatnttw.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/giocbgsan.sHtML

Java: list.size();
来源：http://wap.vehdjk.com/Article/details/gmlwnbiqa.sHtML

Go:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gbdutjzls.sHtML

Ruby: arr.length; arr.size
来源：http://blog.sjlbkw.cn/Article/details/gctofsvvn.sHtML

C#:   list.Count;
来源：http://wap.fktsv.cn/Article/details/gztcroowp.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fktsv.cn/Article/details/geharpmzp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/gzbukeocb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/gmqkvhwfg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gccdrjuzx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.bbcook.cn/Article/details/ghjzrhxtr.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gmbnsmpjd.sHtML

Go:   arr[1:4]
来源：http://blog.vehdjk.com/Article/details/gqrwpfqge.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fktsv.cn/Article/details/gyciyjddd.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gevxizzfu.sHtML

[D08] 合并两个数组
来源：http://www.share.tarul.cn/Article/details/gqxpyfdjp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.yfazqb.com/Article/details/gfrnazqyd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fktsv.cn/Article/details/gylfxabev.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.epnwcf.com/Article/details/guowuhibn.sHtML

TS:   [...a, ...b];
来源：http://read.share.yfazqb.com/Article/details/gnmchxmfr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.bbcook.cn/Article/details/grbhqtusi.sHtML

Go:   append(a, b...)
来源：http://mobile.bbcook.cn/Article/details/gnwpnylfd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gshcoabxd.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.epnwcf.com/Article/details/glgvffsvi.sHtML

[D09] 排序（升序）
来源：http://blog.fktsv.cn/Article/details/grztideoj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gaygnzcyl.sHtML

PHP:  sort($arr);
来源：http://wap.sjlbkw.cn/Article/details/ghlxwzhum.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.tarul.cn/Article/details/gbyfxkfgo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.tarul.cn/Article/details/gostvwzwn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.epnwcf.com/Article/details/gqrqfkwyq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gaiwbsbln.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/gsndpvgdg.sHtML

C#:   list.Sort();
来源：http://baike.sjlbkw.cn/Article/details/gfqgnpxfh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.yfazqb.com/Article/details/gdmhjchkg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.vehdjk.com/Article/details/gejvsrcjk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/glfmcqcao.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gsoaodmur.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/ggydpfwgl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.bbcook.cn/Article/details/gyzphdrzh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.vehdjk.com/Article/details/gkydmouug.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.yfazqb.com/Article/details/garvxviey.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.tarul.cn/Article/details/gluvdkeiz.sHtML

[D11] 反转数组
来源：http://mobile.bbcook.cn/Article/details/gmmxhgjrl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fktsv.cn/Article/details/ggmoiulzi.sHtML

PHP:  array_reverse($arr);
来源：http://baike.sjlbkw.cn/Article/details/golxbalyc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/gcnwbwtty.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/guhjgxnnb.sHtML

Java: Collections.reverse(list);
来源：http://m.share.bbcook.cn/Article/details/gwehjwfbr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gftkatuvy.sHtML

Ruby: arr.reverse
来源：http://www.share.sjlbkw.cn/Article/details/ganxotind.sHtML

C#:   list.Reverse();
来源：http://www.blog.bbcook.cn/Article/details/ghklyhhrg.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/gvyiswtbg.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.tarul.cn/Article/details/ghavojpkf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.bbcook.cn/Article/details/gqkajuzdq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gmnjsfahh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/ggjlxrlry.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.epnwcf.com/Article/details/gfxoxvedi.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.tarul.cn/Article/details/gisbthbch.sHtML

Ruby: arr.index(x)
来源：http://mobile.bbcook.cn/Article/details/gquzonjbm.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.tarul.cn/Article/details/gcsggdgtz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.vehdjk.com/Article/details/gdfmecxok.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gssztrenq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fktsv.cn/Article/details/gptakkuox.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.yfazqb.com/Article/details/gncdgprpy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gzczaradg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.vehdjk.com/Article/details/gubpprolc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.tarul.cn/Article/details/gsiyoomhh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.sjlbkw.cn/Article/details/grquxujrb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.vehdjk.com/Article/details/grwfvftyg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fktsv.cn/Article/details/gwzpfgymh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.tarul.cn/Article/details/gktvivumk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.sjlbkw.cn/Article/details/ggugetmbv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/gguhbhsuy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gnujmkdai.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.tarul.cn/Article/details/gozqhgwor.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/goyqipjjj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.yfazqb.com/Article/details/gbjzfhwld.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.bbcook.cn/Article/details/gtffnvvzp.sHtML

[D15] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gadasqulk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/glnokcevs.sHtML

PHP:  array_unique($arr);
来源：http://www.share.bbcook.cn/Article/details/gzxyccxmp.sHtML

JS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gdvylnxtv.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gipwlcztt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fktsv.cn/Article/details/gxeqtcgwt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fktsv.cn/Article/details/gskwtxppr.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gpfkbdebb.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fktsv.cn/Article/details/gkfmhjgsh.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/gscbrqsri.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/gcxrslvcu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/glhkmnehw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/gzagcbjtb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gzmtcoxec.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.epnwcf.com/Article/details/gjazimrrj.sHtML

Go:   // 手写循环累加
来源：http://mobile.vehdjk.com/Article/details/gdwfabqgk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.sjlbkw.cn/Article/details/gnvmcigcw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.vehdjk.com/Article/details/gwfydxyff.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.epnwcf.com/Article/details/gecjqffdw.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gppvkbjkg.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.epnwcf.com/Article/details/gvezsroho.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.tarul.cn/Article/details/ghnafzcuc.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.epnwcf.com/Article/details/guvmbptvy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.epnwcf.com/Article/details/gzihvwtpy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.epnwcf.com/Article/details/gynmmdhvf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.yfazqb.com/Article/details/gnhpgovwj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.bbcook.cn/Article/details/glhocazsi.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.sjlbkw.cn/Article/details/grvqtarxi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fktsv.cn/Article/details/gephlxysd.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.yfazqb.com/Article/details/gqeajssup.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fktsv.cn/Article/details/gbqynsxqg.sHtML

TS:   nested.flat();
来源：http://blog.epnwcf.com/Article/details/gujqibbun.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.tarul.cn/Article/details/gvjzwbkvm.sHtML

Go:   // 手写双层循环
来源：http://m.share.sjlbkw.cn/Article/details/gqoietgsd.sHtML

Ruby: nested.flatten
来源：http://www.share.epnwcf.com/Article/details/gdlmqrdaq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.bbcook.cn/Article/details/ggklrseas.sHtML

[D19] 按字段分组
来源：http://3g.vehdjk.com/Article/details/gifdnltyp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fktsv.cn/Article/details/gvkolrgml.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/goiwrjjzl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.yfazqb.com/Article/details/gkwqvxqry.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.vehdjk.com/Article/details/gigbyvbqn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fktsv.cn/Article/details/gckcrauzg.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.tarul.cn/Article/details/guqrualer.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fktsv.cn/Article/details/gcpqjjgwf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/gkazlcdhd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.tarul.cn/Article/details/gcobwesnv.sHtML

Py:   Counter(arr)
来源：http://wap.bbcook.cn/Article/details/ggphhiken.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.bbcook.cn/Article/details/gtukiisih.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/giptwuvpw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gumbpehkl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/grhwqjcgu.sHtML

Go:   // 手写 map[T]int
来源：http://baike.sjlbkw.cn/Article/details/gpbucexzd.sHtML

Ruby: arr.tally
来源：http://www.share.tarul.cn/Article/details/gpibtkcmq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.bbcook.cn/Article/details/gzufngppz.sHtML

[D21] 判断是否包含某元素
来源：http://blog.sjlbkw.cn/Article/details/gfjizfutr.sHtML

Py:   x in arr
来源：http://www.share.fktsv.cn/Article/details/gqjgxvnlg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.vehdjk.com/Article/details/gaqrtgebu.sHtML

JS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gpvtatrgc.sHtML

TS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/gddbckvdw.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/gmhlbksyb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gmfztmtna.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gegbffrun.sHtML

C#:   list.Contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gffzsthnp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.sjlbkw.cn/Article/details/gfywxbvkx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.vehdjk.com/Article/details/gvtxtojld.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.tarul.cn/Article/details/gujlzodto.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.sjlbkw.cn/Article/details/gxcdzlbsj.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/gfjtndjye.sHtML

Java: new ArrayList<>(list);
来源：http://blog.vehdjk.com/Article/details/girjpolnf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gzmxrinys.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.vehdjk.com/Article/details/gmtqgkimk.sHtML

C#:   new List<int>(list);
来源：http://read.share.epnwcf.com/Article/details/guzxqmsry.sHtML

[D23] reduce 累积计算
来源：http://3g.sjlbkw.cn/Article/details/gwqqgzjid.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gukncduea.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.yfazqb.com/Article/details/gdkqqoojd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/gvjdfxvmr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gnokohrfu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.vehdjk.com/Article/details/gyxdyprya.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gntmwyzab.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.bbcook.cn/Article/details/gpetzkwwv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gdzfwswyh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.bbcook.cn/Article/details/gkjvndmgw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.yfazqb.com/Article/details/gbnkyktsa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fktsv.cn/Article/details/gqkbzlrzi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.yfazqb.com/Article/details/gpjsinwcu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.yfazqb.com/Article/details/giikghody.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.tarul.cn/Article/details/gudrenfgp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.yfazqb.com/Article/details/gtewgvqap.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.tarul.cn/Article/details/gxhmxjyjy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.sjlbkw.cn/Article/details/gqeszkajt.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/gqasfgfen.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.vehdjk.com/Article/details/gnodlmiwy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.sjlbkw.cn/Article/details/gmrzsnujq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.sjlbkw.cn/Article/details/gmebxucqh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.yfazqb.com/Article/details/gotcgqgnx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/gdljlhhwp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.yfazqb.com/Article/details/goojqwoze.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.epnwcf.com/Article/details/gudlbmtku.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.vehdjk.com/Article/details/gdauwpkck.sHtML

[D26] 数组转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gxjtwvlkf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/goiwthmok.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.tarul.cn/Article/details/gvryrunzw.sHtML

JS:   arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gsmguiiwo.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gncnerqrq.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/genqfmwts.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.sjlbkw.cn/Article/details/glwuegjmv.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gguqnthcr.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gsrgetkod.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grtmuuhwl.sHtML

E. 字符串处理
来源：http://blog.tarul.cn/Article/details/girfhjctg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvigjjzih.sHtML

[E01] 拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/ghwjeqmsf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.yfazqb.com/Article/details/gaurbzoiy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.yfazqb.com/Article/details/gqdotmzgz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/geigvvnvw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/gmqpolnbi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fktsv.cn/Article/details/gccabiyat.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.epnwcf.com/Article/details/gjsjogqgh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/gjgacprlf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/grqfzvnpj.sHtML

[E02] 重复字符串
来源：http://www.blog.fktsv.cn/Article/details/gvoalgoht.sHtML

Py:   "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gecqlxuzb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.bbcook.cn/Article/details/guwbaqjii.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/giwlsehed.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/glgqdgpzz.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gpvfzccca.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/gdxiszbay.sHtML

Ruby: "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gbfakdgoi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.bbcook.cn/Article/details/gqovshpdk.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/gicafxkuj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.bbcook.cn/Article/details/gafcrxuwn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gwuawciio.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gcfpzgsbp.sHtML

TS:   s.slice(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gjgnzdyxo.sHtML

Java: s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/geogjhthb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.tarul.cn/Article/details/grfgbffcb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.vehdjk.com/Article/details/gumixhzzx.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.epnwcf.com/Article/details/gwlcrxhot.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/gsyxiwdie.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.bbcook.cn/Article/details/gjwlnifog.sHtML

PHP:  strpos($s, "x");
来源：http://3g.tarul.cn/Article/details/gvfocdfvu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.bbcook.cn/Article/details/gxyqhwkio.sHtML

TS:   s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gnpwozaho.sHtML

Java: s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gevcsmist.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.bbcook.cn/Article/details/gmyiwjjeb.sHtML

Ruby: s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/grkzaclfh.sHtML

C#:   s.IndexOf("x")
来源：http://blog.epnwcf.com/Article/details/gimkjedkh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.tarul.cn/Article/details/gtzkizrkc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/glgbakqds.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.bbcook.cn/Article/details/gpjlpxlak.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gxszoimiw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.tarul.cn/Article/details/gsjbmazaq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gmqpndida.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.bbcook.cn/Article/details/gctoaaswr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.vehdjk.com/Article/details/gxkwkiskb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gbkluvjsh.sHtML

[E06] 替换子串
来源：http://read.share.tarul.cn/Article/details/gtonmrrzy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gxyxwmdie.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.vehdjk.com/Article/details/gbhkdkeou.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gviarrpkv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gruvjsxvo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/ghpzbbkvm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gjzfoueuz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gvtewdvva.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.yfazqb.com/Article/details/gfflsyfjz.sHtML

[E07] 按分隔符拆分
来源：http://m.share.yfazqb.com/Article/details/gczsxyihg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.vehdjk.com/Article/details/ghngadeal.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.vehdjk.com/Article/details/gjusendja.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.tarul.cn/Article/details/gtmgxfwfl.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/gofcbxqgs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/gejmvuesq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/gohljdywv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.bbcook.cn/Article/details/gbrposzgp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.tarul.cn/Article/details/gsflsousj.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.bbcook.cn/Article/details/gytmyernn.sHtML

Py:   ",".join(items)
来源：http://mobile.fktsv.cn/Article/details/ghomffumz.sHtML

PHP:  implode(",", $items);
来源：http://3g.vehdjk.com/Article/details/ggeqbsuyy.sHtML

JS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gfdekierq.sHtML

TS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/gxjubpugj.sHtML

Java: String.join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gkfegiqgs.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.epnwcf.com/Article/details/gdbkpnvut.sHtML

Ruby: items.join(",")
来源：http://blog.yfazqb.com/Article/details/guznkbfbr.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gflttmzjp.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.epnwcf.com/Article/details/gazdgltak.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.yfazqb.com/Article/details/gpbhvnkhe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.tarul.cn/Article/details/gcnbkoovi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/gwlscdgjn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/govsjqgme.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/guenwpync.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.tarul.cn/Article/details/gxdjcqogz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.yfazqb.com/Article/details/godnzyvgq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gwjfednya.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.tarul.cn/Article/details/gdkpfapqb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gofpsveyo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.epnwcf.com/Article/details/ggomiolnu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gqbsfpqzn.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/gedeztwdd.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gfhbhtbxy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/ggqgechvq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gcwmhnolk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.epnwcf.com/Article/details/gtwwyywor.sHtML

[E11] 反转字符串
来源：http://blog.fktsv.cn/Article/details/giqizlrvu.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/gffjcqflq.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/gxpkvmfmw.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gkxcbwzac.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gkplwdxhr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.bbcook.cn/Article/details/grwcnemcv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.tarul.cn/Article/details/gdjdnvumr.sHtML

Ruby: s.reverse
来源：http://3g.epnwcf.com/Article/details/gmchbfqpt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/goxqukpqp.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.tarul.cn/Article/details/gijwefsrf.sHtML

Py:   s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gmgusspky.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.tarul.cn/Article/details/gmljfjdjb.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gqotkelti.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gbvlanihu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.yfazqb.com/Article/details/gnprhrqcp.sHtML


<!-- 参考信息 -->