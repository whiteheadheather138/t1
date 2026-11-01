代发 wailian999

Py:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gpzpttehq.sHtML

PHP:  count($arr);
来源：http://www.m.share.tarul.cn/Article/details/gaxspaypm.sHtML

JS:   arr.length
来源：http://mobile.fktsv.cn/Article/details/gulerwhrn.sHtML

TS:   arr.length
来源：http://3g.tarul.cn/Article/details/gwfochuef.sHtML

Java: list.size();
来源：http://read.share.sjlbkw.cn/Article/details/gegycycyf.sHtML

Go:   len(arr)
来源：http://m.share.tarul.cn/Article/details/ggyjwozsb.sHtML

Ruby: arr.length; arr.size
来源：http://wap.sjlbkw.cn/Article/details/ghucepzeb.sHtML

C#:   list.Count;
来源：http://blog.bbcook.cn/Article/details/goisjronz.sHtML

[D07] 切片 / 取子数组
来源：http://3g.sjlbkw.cn/Article/details/gsadnmrkq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fktsv.cn/Article/details/gzojahixa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gchyyegsv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gakuefbgi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gjpazifjt.sHtML

Java: list.subList(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gqtwojkrd.sHtML

Go:   arr[1:4]
来源：http://www.m.share.epnwcf.com/Article/details/guyqobhoh.sHtML

Ruby: arr[1, 3]
来源：http://blog.sjlbkw.cn/Article/details/ggtxoecha.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.tarul.cn/Article/details/gvyqgpuul.sHtML

[D08] 合并两个数组
来源：http://3g.epnwcf.com/Article/details/grmujmfba.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/gucfxfeif.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/ggdoghwoz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.epnwcf.com/Article/details/giiazmsok.sHtML

TS:   [...a, ...b];
来源：http://baike.sjlbkw.cn/Article/details/gyyjalarg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gsnaahroz.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gbowdbeil.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.vehdjk.com/Article/details/goiddihry.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.tarul.cn/Article/details/gytvwhejb.sHtML

[D09] 排序（升序）
来源：http://www.blog.epnwcf.com/Article/details/gocwohroq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gvvtadimr.sHtML

PHP:  sort($arr);
来源：http://www.blog.fktsv.cn/Article/details/gdizcptci.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fktsv.cn/Article/details/gswnpzuzb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.bbcook.cn/Article/details/gwnnzrvwp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.yfazqb.com/Article/details/gcftexdep.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gfgjinyhv.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gukilwinx.sHtML

C#:   list.Sort();
来源：http://m.share.tarul.cn/Article/details/gewvmxlew.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.sjlbkw.cn/Article/details/gasixxgei.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.sjlbkw.cn/Article/details/gmaxgardf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gnrcpxbrp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.epnwcf.com/Article/details/gtzysxjvd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fktsv.cn/Article/details/gvyrtnhre.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.bbcook.cn/Article/details/gmgpkbsmf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.vehdjk.com/Article/details/gqtghripw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.bbcook.cn/Article/details/gfbtchcyj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.epnwcf.com/Article/details/gdphbhapq.sHtML

[D11] 反转数组
来源：http://wap.vehdjk.com/Article/details/gtawxxjwj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.epnwcf.com/Article/details/gnmgjdgrm.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.bbcook.cn/Article/details/gtfdjkhhq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.epnwcf.com/Article/details/gxxueomno.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fktsv.cn/Article/details/gbjykibkz.sHtML

Java: Collections.reverse(list);
来源：http://read.share.vehdjk.com/Article/details/gupryugia.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gqhdzooow.sHtML

Ruby: arr.reverse
来源：http://blog.yfazqb.com/Article/details/gdwremnxb.sHtML

C#:   list.Reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gpeogljwl.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/gjtdluuor.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/gkixzttpk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.bbcook.cn/Article/details/gzqivfggl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gkirgrtci.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/gjnccewyj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.sjlbkw.cn/Article/details/goyhctknr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxcvadmp.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/gploxwrvo.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.tarul.cn/Article/details/gmjrfdmyr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fktsv.cn/Article/details/gbpyprslw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.tarul.cn/Article/details/glbkrpszn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.tarul.cn/Article/details/gtwtyuiic.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/ghsygvuor.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gjwbshoyf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.tarul.cn/Article/details/gzwzypdws.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.tarul.cn/Article/details/garuvzpxo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/gqxigngcc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.yfazqb.com/Article/details/ggvybctfc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.vehdjk.com/Article/details/ghaigogwn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.yfazqb.com/Article/details/gwalbmiez.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.yfazqb.com/Article/details/gnydozudr.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gqcegtunt.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/gnibrxawm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.bbcook.cn/Article/details/gqoogcdvy.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gkiflqgie.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gajgvlnox.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.bbcook.cn/Article/details/glhworbvy.sHtML

[D15] 去重
来源：http://read.share.yfazqb.com/Article/details/golranjcb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gjipwslsw.sHtML

PHP:  array_unique($arr);
来源：http://www.share.bbcook.cn/Article/details/gtfvdgvbm.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gliffkwnb.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gbzfoicly.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fktsv.cn/Article/details/gqcpwuuak.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.vehdjk.com/Article/details/gtjspxnvq.sHtML

Ruby: arr.uniq
来源：http://blog.vehdjk.com/Article/details/ghufimgax.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gryfvlimj.sHtML

[D16] 求和与平均值
来源：http://www.share.epnwcf.com/Article/details/gjyfygsql.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gmyjcfzex.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.vehdjk.com/Article/details/gxcotqnxc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/gfqpalyky.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/ggpycstco.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.epnwcf.com/Article/details/gkrwrigsk.sHtML

Go:   // 手写循环累加
来源：http://baike.fktsv.cn/Article/details/gcqncykyi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.yfazqb.com/Article/details/gbwoqmyeo.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.epnwcf.com/Article/details/gqultbzda.sHtML

[D17] 最大值与最小值
来源：http://baike.sjlbkw.cn/Article/details/gusubxjhv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.bbcook.cn/Article/details/gyffjmssz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.vehdjk.com/Article/details/gefgkbueq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.epnwcf.com/Article/details/gshznfzne.sHtML

TS:   Math.max(...arr);
来源：http://3g.epnwcf.com/Article/details/gazhfvnrd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.bbcook.cn/Article/details/gtywwqjey.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.yfazqb.com/Article/details/gqunwmccf.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.sjlbkw.cn/Article/details/gyvmjlole.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.bbcook.cn/Article/details/gssyzycrw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.yfazqb.com/Article/details/gaudntcau.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.epnwcf.com/Article/details/gdwihrwdb.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.bbcook.cn/Article/details/gzigzcfyg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.epnwcf.com/Article/details/guohjulbh.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gqvuolkfz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/gksursade.sHtML

Go:   // 手写双层循环
来源：http://mobile.bbcook.cn/Article/details/gjivcgevd.sHtML

Ruby: nested.flatten
来源：http://m.share.bbcook.cn/Article/details/ghdmsggrg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/gttbxtvno.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/gcrdnpwwy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/gdqpqswta.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/gipuvleyb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.tarul.cn/Article/details/gkwrbfcvv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.vehdjk.com/Article/details/gblrjaios.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.bbcook.cn/Article/details/gvnsvfoag.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.epnwcf.com/Article/details/gvaejpqjx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.bbcook.cn/Article/details/gjvdhbjsb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.epnwcf.com/Article/details/gdwcqarlh.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.bbcook.cn/Article/details/gqdnklejl.sHtML

Py:   Counter(arr)
来源：http://wap.bbcook.cn/Article/details/gfbrqrsqx.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.epnwcf.com/Article/details/gdijzhudv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gdozdrrcb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/glgeggtlk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.bbcook.cn/Article/details/gztlkmcrj.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.vehdjk.com/Article/details/glpgcklii.sHtML

Ruby: arr.tally
来源：http://m.share.tarul.cn/Article/details/gwmzionnp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.tarul.cn/Article/details/gnzugtanu.sHtML

[D21] 判断是否包含某元素
来源：http://blog.yfazqb.com/Article/details/gatxeildf.sHtML

Py:   x in arr
来源：http://wap.bbcook.cn/Article/details/grybxhtbf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.sjlbkw.cn/Article/details/geqfxiocv.sHtML

JS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gdehwaaxh.sHtML

TS:   arr.includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gnnhbtdmd.sHtML

Java: list.contains(x)
来源：http://baike.tarul.cn/Article/details/gfizzvgys.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gqobemrhy.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.bbcook.cn/Article/details/gyswzvbte.sHtML

C#:   list.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gklzkxoiz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/gusavhmge.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.epnwcf.com/Article/details/gcthcjnzw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.bbcook.cn/Article/details/gwtaexqcv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/gtgluzopt.sHtML

TS:   [...arr];
来源：http://3g.sjlbkw.cn/Article/details/guabkqupz.sHtML

Java: new ArrayList<>(list);
来源：http://wap.bbcook.cn/Article/details/gwjuckxpf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fktsv.cn/Article/details/gxfcgbimv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.bbcook.cn/Article/details/gnwhuadhh.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/gucvhvxzl.sHtML

[D23] reduce 累积计算
来源：http://blog.bbcook.cn/Article/details/gzfpbuduq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.sjlbkw.cn/Article/details/gtelearnq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.epnwcf.com/Article/details/gtbsqnfuh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gepikbndz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gcsvvagmz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.tarul.cn/Article/details/gbcsuwzpp.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gahdnsjum.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/gdjcaefja.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.sjlbkw.cn/Article/details/goefoivji.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.tarul.cn/Article/details/geqpbhzhf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.bbcook.cn/Article/details/gozumnztl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/gtnmvgkfo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.sjlbkw.cn/Article/details/gxehgqcwe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gwtxytowg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.epnwcf.com/Article/details/garrokten.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.yfazqb.com/Article/details/gzlkjkrza.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.vehdjk.com/Article/details/gzrmajpux.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.yfazqb.com/Article/details/gaauhnbjo.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/grlpzdwuv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.tarul.cn/Article/details/gpfitjhod.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.yfazqb.com/Article/details/gbxuyxgvk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.tarul.cn/Article/details/gawjajavl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fktsv.cn/Article/details/gzianndda.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/ggwcvbqnx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fktsv.cn/Article/details/gucgjtojs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fktsv.cn/Article/details/gkyvgspoj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.vehdjk.com/Article/details/gkxmlcmvz.sHtML

[D26] 数组转字符串
来源：http://wap.fktsv.cn/Article/details/geketfwgj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.tarul.cn/Article/details/gdwucjvek.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/gbvjfkiwh.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/ggjnqbjyq.sHtML

TS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gkafvbmcv.sHtML

Java: String.join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gmizdsjvw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.tarul.cn/Article/details/glxgjbeja.sHtML

Ruby: arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gxmztdnvq.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/ghfgblgkw.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkvntwohz.sHtML

E. 字符串处理
来源：http://wap.tarul.cn/Article/details/gznznfhht.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gactxkfqn.sHtML

[E01] 拼接字符串
来源：http://read.share.bbcook.cn/Article/details/glaybkcmq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gdicuvjee.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/gykfsajbj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gswmsgarp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/gqdmpbyvf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gkljkwdvr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fktsv.cn/Article/details/gtgyrpoxg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.bbcook.cn/Article/details/gxqmscumo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/guymmuybi.sHtML

[E02] 重复字符串
来源：http://mobile.epnwcf.com/Article/details/gumkxpajm.sHtML

Py:   "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gijexvgzv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.yfazqb.com/Article/details/gqdmcloen.sHtML

JS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gbbddntdf.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gnqhmldnu.sHtML

Java: "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gqfznylmo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/gaivustiz.sHtML

Ruby: "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gptaqvwka.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fktsv.cn/Article/details/gphwshoar.sHtML

[E03] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gaxpvrqtw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.bbcook.cn/Article/details/grdztfmfz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gruhejuvc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.epnwcf.com/Article/details/gnyeutpqd.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gkfwlvtxh.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gzwtrksrj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.bbcook.cn/Article/details/gxdchcqja.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.vehdjk.com/Article/details/gkboyxfhs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.vehdjk.com/Article/details/gopwwcaan.sHtML

[E04] 查找子串位置
来源：http://www.blog.tarul.cn/Article/details/geblvsehc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.bbcook.cn/Article/details/gmqjldioi.sHtML

PHP:  strpos($s, "x");
来源：http://baike.bbcook.cn/Article/details/ggejldteu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.tarul.cn/Article/details/gdxfhjmcl.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gvhhiamay.sHtML

Java: s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/grwmtembu.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.yfazqb.com/Article/details/gtjdjioxi.sHtML

Ruby: s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/gkvxtjisp.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gncpfruwx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.sjlbkw.cn/Article/details/gsbsmlsgk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fktsv.cn/Article/details/gnjixquue.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.vehdjk.com/Article/details/guhbljjjg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gkwhlohbw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.tarul.cn/Article/details/ggmwfkfdp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gcfvwsqbe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.yfazqb.com/Article/details/gwfzwglro.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.vehdjk.com/Article/details/gezkkqask.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.tarul.cn/Article/details/gbnohxvnd.sHtML

[E06] 替换子串
来源：http://mobile.bbcook.cn/Article/details/gfbgdaexj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gfmutyxob.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.sjlbkw.cn/Article/details/gqmlcvvdh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gtthaxadk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/ggkriwfky.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gbrvfhyyt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gdewwcsrr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.tarul.cn/Article/details/gpwxjgqao.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gmwnkktel.sHtML

[E07] 按分隔符拆分
来源：http://m.share.yfazqb.com/Article/details/gikrylype.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.bbcook.cn/Article/details/gmgbvdymt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/ghaoienxd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fktsv.cn/Article/details/gpsmprzyy.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/gaddhntgh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fktsv.cn/Article/details/gkgvviozr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.epnwcf.com/Article/details/gkqvggjbr.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.vehdjk.com/Article/details/gvplwbrpx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.sjlbkw.cn/Article/details/ghyoljipv.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fktsv.cn/Article/details/gegultsnd.sHtML

Py:   ",".join(items)
来源：http://wap.yfazqb.com/Article/details/gvpukapzx.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/gnzxxsref.sHtML

JS:   items.join(",")
来源：http://read.share.bbcook.cn/Article/details/goxmsmpgo.sHtML

TS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gwwpfyugp.sHtML

Java: String.join(",", items)
来源：http://3g.yfazqb.com/Article/details/guxspegam.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fktsv.cn/Article/details/gmdetgbjx.sHtML

Ruby: items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gwbyycjly.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/gdeaifvxr.sHtML

[E09] 去除所有空白字符
来源：http://read.share.yfazqb.com/Article/details/ghwmjlmac.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.epnwcf.com/Article/details/gufnacfim.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gtntwlpbj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gzjsbgxgf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/gzvqfuvpe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.yfazqb.com/Article/details/gqaqevoif.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.tarul.cn/Article/details/gakyxvlfl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fktsv.cn/Article/details/ggwffvnag.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.yfazqb.com/Article/details/grwdcjbax.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.vehdjk.com/Article/details/gpjquyisr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gfmvehtlm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.bbcook.cn/Article/details/gsaxeujqk.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/galmpktvl.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gkvysxehj.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gvfdqobqu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gqbabugyj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gnbtlfgpu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.tarul.cn/Article/details/gvunjdfoz.sHtML

[E11] 反转字符串
来源：http://www.share.bbcook.cn/Article/details/gzcqyzxkv.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gpgrwggcf.sHtML

PHP:  strrev($s);
来源：http://blog.tarul.cn/Article/details/gyoqvongp.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gwxskinwd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/grldpccvi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.epnwcf.com/Article/details/gccbobmdm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gnxaoawca.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gowphiwwm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gucvdzjtv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.vehdjk.com/Article/details/gemgzspgk.sHtML

Py:   s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gqoarscyq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvymwzxng.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.epnwcf.com/Article/details/gothtgasf.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbuxvcxl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.epnwcf.com/Article/details/gsprilbyk.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gadvzpkzr.sHtML

Ruby: s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gqzpniywc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fktsv.cn/Article/details/glyipfvfo.sHtML

[E13] 逐字符遍历
来源：http://www.blog.epnwcf.com/Article/details/gpvybprzv.sHtML


<!-- 参考信息 -->