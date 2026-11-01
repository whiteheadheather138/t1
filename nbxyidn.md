代发 wailian999

Py:   len(arr)
来源：http://www.share.tarul.cn/Article/details/grfxbzass.sHtML

PHP:  count($arr);
来源：http://www.share.epnwcf.com/Article/details/gtsoegjrh.sHtML

JS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gskgelwmu.sHtML

TS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/grypfjtvd.sHtML

Java: list.size();
来源：http://baike.vehdjk.com/Article/details/ghpeokxgb.sHtML

Go:   len(arr)
来源：http://m.share.fktsv.cn/Article/details/ggduhdzos.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/gibxeuvez.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/gprqpeszw.sHtML

[D07] 切片 / 取子数组
来源：http://wap.vehdjk.com/Article/details/gjhjasyfu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.yfazqb.com/Article/details/ghlhrmpwz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.epnwcf.com/Article/details/gavmhlhfw.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.bbcook.cn/Article/details/gjnbmkvlw.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gsuhebttj.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/ghyzizfso.sHtML

Go:   arr[1:4]
来源：http://baike.vehdjk.com/Article/details/gnolzvzmb.sHtML

Ruby: arr[1, 3]
来源：http://read.share.tarul.cn/Article/details/gfopnvrpy.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fktsv.cn/Article/details/ghvoffohn.sHtML

[D08] 合并两个数组
来源：http://www.share.tarul.cn/Article/details/gopsbbmrz.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.yfazqb.com/Article/details/gmjiegcgr.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.epnwcf.com/Article/details/gekgfyehu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.tarul.cn/Article/details/gizxfexhj.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/gdrogswyc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.vehdjk.com/Article/details/grebbkkmx.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gxoyzenqd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.bbcook.cn/Article/details/gzvpxuphf.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.vehdjk.com/Article/details/grwixfaxe.sHtML

[D09] 排序（升序）
来源：http://mobile.vehdjk.com/Article/details/goaovxfki.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gcnuijoyh.sHtML

PHP:  sort($arr);
来源：http://www.share.vehdjk.com/Article/details/ggnryjjpg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.yfazqb.com/Article/details/gdfpvbytx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.vehdjk.com/Article/details/gckkkuykr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.tarul.cn/Article/details/gqyhkrezd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/gswwlkgqm.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/glqmgxghz.sHtML

C#:   list.Sort();
来源：http://www.blog.sjlbkw.cn/Article/details/gglzdsbnv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.tarul.cn/Article/details/gwmhrlhlf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.sjlbkw.cn/Article/details/gzehqcuhk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.yfazqb.com/Article/details/gnctyglad.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gblywnola.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gfgshvzgz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/gstbeievb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.sjlbkw.cn/Article/details/ggqciglnl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.sjlbkw.cn/Article/details/gwvjdxgxu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fktsv.cn/Article/details/gicesgdad.sHtML

[D11] 反转数组
来源：http://www.share.vehdjk.com/Article/details/gstevoywu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.bbcook.cn/Article/details/glbnuilec.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fktsv.cn/Article/details/gkyenoytb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.yfazqb.com/Article/details/gvhwgmozo.sHtML

TS:   [...arr].reverse();
来源：http://read.share.sjlbkw.cn/Article/details/gylrsbewr.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.vehdjk.com/Article/details/gdupfpfqn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.epnwcf.com/Article/details/gzlxooagg.sHtML

Ruby: arr.reverse
来源：http://blog.fktsv.cn/Article/details/gvicrbqmz.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/giffcugqh.sHtML

[D12] 查找元素下标
来源：http://read.share.vehdjk.com/Article/details/gzslslyxs.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.tarul.cn/Article/details/gatdvutrj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.epnwcf.com/Article/details/glfbkiaae.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.bbcook.cn/Article/details/gskjmzmpa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/getxssyon.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.epnwcf.com/Article/details/gcjdqqhvy.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.vehdjk.com/Article/details/glcachduq.sHtML

Ruby: arr.index(x)
来源：http://blog.epnwcf.com/Article/details/gxeqtstcb.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.bbcook.cn/Article/details/gdryzmuxz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.epnwcf.com/Article/details/gnueukvcz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fktsv.cn/Article/details/gvadpxunu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.bbcook.cn/Article/details/gkrkoyzur.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/gnbyyszfz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/giweurjqb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.tarul.cn/Article/details/gbcvdmfzh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gdvyiamjs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/gnogjwsjl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gwsgtqepj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.vehdjk.com/Article/details/gtjeeppfu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.vehdjk.com/Article/details/gsbxvpijp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.vehdjk.com/Article/details/gvpttjvit.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gvzvuqgah.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/gdgutpelz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.vehdjk.com/Article/details/ggezvaixq.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/gmhtqywkh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/geedpnooz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.tarul.cn/Article/details/gainvffad.sHtML

[D15] 去重
来源：http://blog.tarul.cn/Article/details/gmhyzcysu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/gaimchosx.sHtML

PHP:  array_unique($arr);
来源：http://3g.epnwcf.com/Article/details/gyjbdskad.sHtML

JS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gpfjaesby.sHtML

TS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gaggcejlk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.yfazqb.com/Article/details/ggppkxlug.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.tarul.cn/Article/details/gehtenbtv.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gshfwqxlr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fktsv.cn/Article/details/gbvocmxhf.sHtML

[D16] 求和与平均值
来源：http://blog.sjlbkw.cn/Article/details/grlvxibgj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gdveslyox.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.bbcook.cn/Article/details/gugiuktjr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.bbcook.cn/Article/details/gxcwrzjvo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gprvqhdyq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/gzqogcdbv.sHtML

Go:   // 手写循环累加
来源：http://3g.bbcook.cn/Article/details/gfnspoadg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.sjlbkw.cn/Article/details/gtwkeebze.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/gdlyarcfm.sHtML

[D17] 最大值与最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gfppuefox.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.sjlbkw.cn/Article/details/gsobwcqhc.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.sjlbkw.cn/Article/details/grnqdqety.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.sjlbkw.cn/Article/details/guzwoiaqy.sHtML

TS:   Math.max(...arr);
来源：http://blog.bbcook.cn/Article/details/gxdepvraq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.vehdjk.com/Article/details/gvutwthlj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.vehdjk.com/Article/details/gxbqrbffe.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.sjlbkw.cn/Article/details/gjqmrobcd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.bbcook.cn/Article/details/gsggfahgb.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fktsv.cn/Article/details/gfjfuyral.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.sjlbkw.cn/Article/details/gqplqgmrb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.tarul.cn/Article/details/guekjxvbk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.vehdjk.com/Article/details/gtcrgzjpd.sHtML

TS:   nested.flat();
来源：http://www.blog.epnwcf.com/Article/details/gioydcpmg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.bbcook.cn/Article/details/gozojvqkp.sHtML

Go:   // 手写双层循环
来源：http://mobile.yfazqb.com/Article/details/gawbophqs.sHtML

Ruby: nested.flatten
来源：http://www.share.sjlbkw.cn/Article/details/ggguhncao.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gjgtqgprb.sHtML

[D19] 按字段分组
来源：http://www.share.tarul.cn/Article/details/gkbqemaqi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.bbcook.cn/Article/details/gpqpuebvk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fktsv.cn/Article/details/gotipypnr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.yfazqb.com/Article/details/glafjddlj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/gsjttnznq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.tarul.cn/Article/details/gtjapbagl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.epnwcf.com/Article/details/geenddtbq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.tarul.cn/Article/details/gruhuilqc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.yfazqb.com/Article/details/gzcqdpjdy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.vehdjk.com/Article/details/gvojosisk.sHtML

Py:   Counter(arr)
来源：http://wap.yfazqb.com/Article/details/gbhktsxzn.sHtML

PHP:  array_count_values($arr);
来源：http://blog.sjlbkw.cn/Article/details/gumnitdqu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gmqesznuf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gydawfdpl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.yfazqb.com/Article/details/gvssegokl.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.bbcook.cn/Article/details/gkebffome.sHtML

Ruby: arr.tally
来源：http://www.blog.tarul.cn/Article/details/gbdkcmqjo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.yfazqb.com/Article/details/gmicqgpqs.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpwxwnhb.sHtML

Py:   x in arr
来源：http://mobile.epnwcf.com/Article/details/gheqpdgqx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.sjlbkw.cn/Article/details/gmkpdwvpg.sHtML

JS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/gjmucbiqu.sHtML

TS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/glzbiflta.sHtML

Java: list.contains(x)
来源：http://blog.tarul.cn/Article/details/glshzemwo.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gtdjakalo.sHtML

Ruby: arr.include?(x)
来源：http://m.share.epnwcf.com/Article/details/ghqxvwdhz.sHtML

C#:   list.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gzrawzhoz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.tarul.cn/Article/details/gczzouwfr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/guvbuggrd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.sjlbkw.cn/Article/details/gdpktikkl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gcjczjiad.sHtML

TS:   [...arr];
来源：http://read.share.sjlbkw.cn/Article/details/gwmlxakuy.sHtML

Java: new ArrayList<>(list);
来源：http://blog.sjlbkw.cn/Article/details/gsswdcmjv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.sjlbkw.cn/Article/details/gxolurmwb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.sjlbkw.cn/Article/details/gybwwkiax.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/gdscqrpeh.sHtML

[D23] reduce 累积计算
来源：http://mobile.yfazqb.com/Article/details/gvejzrfbu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.sjlbkw.cn/Article/details/glisgpzqi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.bbcook.cn/Article/details/gzwmkjqxp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.epnwcf.com/Article/details/gvlaujrvx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpnykiio.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.epnwcf.com/Article/details/gypzzijem.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/giduewvtz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fktsv.cn/Article/details/gnenylkoe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.vehdjk.com/Article/details/gksxtnevq.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.bbcook.cn/Article/details/gqncotmky.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.sjlbkw.cn/Article/details/gqeceihki.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.epnwcf.com/Article/details/gksivarvv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gyzhlocjx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gywilwfln.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.yfazqb.com/Article/details/gdaursohl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.sjlbkw.cn/Article/details/goiujpgen.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gzzdvimmy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.tarul.cn/Article/details/gigkrvfze.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/gqvwbgpeu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.bbcook.cn/Article/details/gfokdibrd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.yfazqb.com/Article/details/gdivpaknr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.yfazqb.com/Article/details/gecvxcblo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.tarul.cn/Article/details/gxghthxqr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.bbcook.cn/Article/details/gbogfgdam.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqlagtqu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.sjlbkw.cn/Article/details/gehbgfeyw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.epnwcf.com/Article/details/gvqdjaeeq.sHtML

[D26] 数组转字符串
来源：http://3g.vehdjk.com/Article/details/giilkdcej.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.tarul.cn/Article/details/gcdaxdamt.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gmvtbbuye.sHtML

JS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gxghgdzmi.sHtML

TS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/ghcnwekyq.sHtML

Java: String.join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gjzbiaymg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.tarul.cn/Article/details/gefxjzrrg.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gwflmofwq.sHtML

C#:   string.Join(", ", list)
来源：http://blog.bbcook.cn/Article/details/gwndamodb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/grerciksy.sHtML

E. 字符串处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gsohccvfj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gdjhnmjzd.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gcizopnhn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.vehdjk.com/Article/details/giiruodxt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/gogqkvohk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/glpoaaxpz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.bbcook.cn/Article/details/gieeeexyz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/gfvbmhxwg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.tarul.cn/Article/details/gxsuunewq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.bbcook.cn/Article/details/gtebhrplu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gtqpltnbk.sHtML

[E02] 重复字符串
来源：http://baike.tarul.cn/Article/details/gfsbbtzqh.sHtML

Py:   "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gdojytaoj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.sjlbkw.cn/Article/details/gbwmbueap.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gbhbclmjs.sHtML

TS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/glppdpcwn.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gyhsoxtib.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gumhfbhet.sHtML

Ruby: "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/glhfkowkq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.vehdjk.com/Article/details/gfibqvemi.sHtML

[E03] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/gmvoblyuy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.yfazqb.com/Article/details/gfamcvdsj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/ghwigfqga.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gbzrgmqbq.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.tarul.cn/Article/details/gejktdxts.sHtML

Java: s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gmvrkbcgc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gftkuextk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.yfazqb.com/Article/details/gfzenaklk.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fktsv.cn/Article/details/gbqxkddxi.sHtML

[E04] 查找子串位置
来源：http://3g.bbcook.cn/Article/details/gidfmaeyy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.epnwcf.com/Article/details/gxwzsjdjb.sHtML

PHP:  strpos($s, "x");
来源：http://blog.bbcook.cn/Article/details/grrfvrsvq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.epnwcf.com/Article/details/gfwvpwrqg.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gszgzvzhe.sHtML

Java: s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gcaikotkz.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.bbcook.cn/Article/details/guswjzveh.sHtML

Ruby: s.index("x")
来源：http://m.share.epnwcf.com/Article/details/grsscuifr.sHtML

C#:   s.IndexOf("x")
来源：http://wap.bbcook.cn/Article/details/geztjaavv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.vehdjk.com/Article/details/gbjsdlhkz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.epnwcf.com/Article/details/ggvfneydw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.epnwcf.com/Article/details/gttfvsbwf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gkgqwpmjk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmvxrmuc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gyqveghea.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.epnwcf.com/Article/details/gmdtduezs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.bbcook.cn/Article/details/glwivuwlu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gjiuzuzsf.sHtML

[E06] 替换子串
来源：http://www.blog.fktsv.cn/Article/details/gbpsdwcuo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gcplobaem.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.yfazqb.com/Article/details/ghkayjkfi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gaxenfone.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gyvaikfmp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/glrejtncz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gqtxmonsf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gotdkmpzq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/ggenivtup.sHtML

[E07] 按分隔符拆分
来源：http://3g.tarul.cn/Article/details/gxwpbdpqu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.epnwcf.com/Article/details/ggyssdrjl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gmnttumno.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fktsv.cn/Article/details/gcqtisxku.sHtML

TS:   s.split(",")
来源：http://read.share.yfazqb.com/Article/details/gunwiflfc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/gyuoaqbti.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/gulgecxpc.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.vehdjk.com/Article/details/gwfzlibwe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.sjlbkw.cn/Article/details/ganaidibk.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.tarul.cn/Article/details/gzylvghgm.sHtML

Py:   ",".join(items)
来源：http://baike.epnwcf.com/Article/details/gghtkqbqj.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/gjdfjkxwf.sHtML

JS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gbrdrsdrc.sHtML

TS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gtrvgohih.sHtML

Java: String.join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gxdqbfsyp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.sjlbkw.cn/Article/details/gssiyhkii.sHtML

Ruby: items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gaueflddt.sHtML

C#:   string.Join(",", items)
来源：http://3g.epnwcf.com/Article/details/gtuajwyie.sHtML

[E09] 去除所有空白字符
来源：http://wap.epnwcf.com/Article/details/gibyonscb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.vehdjk.com/Article/details/glhlejbst.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.sjlbkw.cn/Article/details/gycbgeulw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/ggnvikkmu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gxpedceqk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.epnwcf.com/Article/details/gdhfcjqle.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fktsv.cn/Article/details/glzipqqaa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.vehdjk.com/Article/details/gwzdpdvfj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.epnwcf.com/Article/details/guhxabfqj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/guohrokxf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gqvvabtzd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/gothdtbhy.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/glywwkbcx.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gfntypezv.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gwconpsre.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gikzlxqdx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gjehhpsne.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.bbcook.cn/Article/details/gbupdytmg.sHtML

[E11] 反转字符串
来源：http://3g.yfazqb.com/Article/details/ghgeozgog.sHtML

Py:   s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gpdfnfjrc.sHtML

PHP:  strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/gojtonvax.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gvukhirjj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gxonnwwpx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.tarul.cn/Article/details/gsnzxnyqx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.bbcook.cn/Article/details/gnkbakbyw.sHtML

Ruby: s.reverse
来源：http://mobile.bbcook.cn/Article/details/gqyokrnfg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gefumwwic.sHtML

[E12] 统计某字符出现次数
来源：http://wap.bbcook.cn/Article/details/gkpiwbhpm.sHtML

Py:   s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gdqerslhw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.sjlbkw.cn/Article/details/gnmrdydvf.sHtML

JS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/ggdooskqb.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/glfyjhesm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.yfazqb.com/Article/details/gazznddej.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.sjlbkw.cn/Article/details/gilyrszdr.sHtML

Ruby: s.count("a")
来源：http://mobile.vehdjk.com/Article/details/galousoxy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gzrfjcwtq.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/guktvmuxb.sHtML


<!-- 参考信息 -->