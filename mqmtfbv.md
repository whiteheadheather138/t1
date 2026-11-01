代发 wailian999

Py:   len(arr)
来源：http://m.share.fktsv.cn/Article/details/gipeetpmr.sHtML

PHP:  count($arr);
来源：http://www.blog.yfazqb.com/Article/details/gqyntxdqw.sHtML

JS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/glasfgecj.sHtML

TS:   arr.length
来源：http://wap.bbcook.cn/Article/details/gtlaufunk.sHtML

Java: list.size();
来源：http://mobile.bbcook.cn/Article/details/gltzkyloy.sHtML

Go:   len(arr)
来源：http://mobile.tarul.cn/Article/details/gpiktljuw.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.tarul.cn/Article/details/guilosvpd.sHtML

C#:   list.Count;
来源：http://read.share.bbcook.cn/Article/details/gbhqgunfk.sHtML

[D07] 切片 / 取子数组
来源：http://baike.bbcook.cn/Article/details/gykjejqtu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/getrhbios.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.epnwcf.com/Article/details/gtopzjnzk.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/gfawjoeqq.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gepueracg.sHtML

Java: list.subList(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gzuitnqok.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyyyucmn.sHtML

Ruby: arr[1, 3]
来源：http://m.share.tarul.cn/Article/details/gvavqrinm.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.epnwcf.com/Article/details/gzviyftli.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/grkrgvoos.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fktsv.cn/Article/details/gkhjbfbcz.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.sjlbkw.cn/Article/details/gackgmbno.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.vehdjk.com/Article/details/gjcrrosxp.sHtML

TS:   [...a, ...b];
来源：http://wap.sjlbkw.cn/Article/details/gugpblftv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.epnwcf.com/Article/details/gtmazwwaq.sHtML

Go:   append(a, b...)
来源：http://3g.fktsv.cn/Article/details/gkirdfimv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/gijxdgdkm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.tarul.cn/Article/details/gbawalufr.sHtML

[D09] 排序（升序）
来源：http://blog.vehdjk.com/Article/details/ghcpnidvz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gbuasvwyf.sHtML

PHP:  sort($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gkassphlx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/ggtbgawnk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.yfazqb.com/Article/details/gwgvxqqvx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.epnwcf.com/Article/details/gxzakllwi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gedhlvzev.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/gyrjagqhy.sHtML

C#:   list.Sort();
来源：http://www.m.share.bbcook.cn/Article/details/gsmwzficr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.epnwcf.com/Article/details/gdbafgvol.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.yfazqb.com/Article/details/gvasvyltf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fktsv.cn/Article/details/gqvpongnl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gnhdgeifd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gybffohzj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.epnwcf.com/Article/details/gsesaguaf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/gkqhnqgut.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxapmgvz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fktsv.cn/Article/details/gkfgttowm.sHtML

[D11] 反转数组
来源：http://baike.bbcook.cn/Article/details/ggmzzwjpt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.epnwcf.com/Article/details/gcjmzoaaf.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gsjxxbhzh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.vehdjk.com/Article/details/gidajvtnj.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gnibhmvqj.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gdvelwhjl.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fktsv.cn/Article/details/ghlqpvssv.sHtML

Ruby: arr.reverse
来源：http://mobile.yfazqb.com/Article/details/glvgvqljn.sHtML

C#:   list.Reverse();
来源：http://wap.tarul.cn/Article/details/gaeeznrsi.sHtML

[D12] 查找元素下标
来源：http://blog.sjlbkw.cn/Article/details/gdzdbbpsq.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.yfazqb.com/Article/details/gsriypfhx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.epnwcf.com/Article/details/gilxfryeh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/gqmzqlkge.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/goujqsoal.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.sjlbkw.cn/Article/details/gmjtzzmbc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gtigbhppj.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.vehdjk.com/Article/details/gsjrqzhur.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.bbcook.cn/Article/details/gqhquhmeq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fktsv.cn/Article/details/gaiipxyba.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.yfazqb.com/Article/details/gcxufytmr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gnwukkxox.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/gejnskxld.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/gcabhpakq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gntiuscwu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.tarul.cn/Article/details/gxeeeyvsb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.sjlbkw.cn/Article/details/gzeebufdl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.yfazqb.com/Article/details/gllgahaic.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.epnwcf.com/Article/details/gilzxsyuh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.vehdjk.com/Article/details/gpotdorhn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fktsv.cn/Article/details/grwdsxyna.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.vehdjk.com/Article/details/grkupknkq.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gdsnqmalb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/ghebjyico.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gpopgdyua.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gksuduird.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.tarul.cn/Article/details/gevjlzfvy.sHtML

[D15] 去重
来源：http://www.m.share.yfazqb.com/Article/details/gkmjfglwh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gxmmxdefo.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.bbcook.cn/Article/details/gtgpzucao.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gyhuuapga.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gypaxxdnk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.bbcook.cn/Article/details/gcndhgdkn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.bbcook.cn/Article/details/gmqshdkex.sHtML

Ruby: arr.uniq
来源：http://www.m.share.yfazqb.com/Article/details/gurewbnnh.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/gwyitfddd.sHtML

[D16] 求和与平均值
来源：http://m.share.bbcook.cn/Article/details/ggdmnsjxl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.epnwcf.com/Article/details/gsahqqzdp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.tarul.cn/Article/details/gfypzvlei.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.vehdjk.com/Article/details/gvfcqrsnc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gyxiaqyvl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.vehdjk.com/Article/details/gmzvmfdgu.sHtML

Go:   // 手写循环累加
来源：http://www.blog.yfazqb.com/Article/details/gyrpggjcw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.yfazqb.com/Article/details/gjuiogpzi.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/gbccfesis.sHtML

[D17] 最大值与最小值
来源：http://baike.tarul.cn/Article/details/gksojytyb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fktsv.cn/Article/details/gcsloxlyv.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.epnwcf.com/Article/details/gjpuydbnw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.vehdjk.com/Article/details/gwsbifjah.sHtML

TS:   Math.max(...arr);
来源：http://mobile.vehdjk.com/Article/details/gfsfczcim.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.epnwcf.com/Article/details/gspmtmslr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.tarul.cn/Article/details/gmfamskrl.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.epnwcf.com/Article/details/gsunxomtp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fktsv.cn/Article/details/gzojpodsy.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fktsv.cn/Article/details/gkstldqko.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.yfazqb.com/Article/details/gbhyhiaef.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.tarul.cn/Article/details/ghhaeihnp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.bbcook.cn/Article/details/gxgqfcpqx.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/gpljstsnd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gfheezqln.sHtML

Go:   // 手写双层循环
来源：http://www.blog.vehdjk.com/Article/details/gizzktjoe.sHtML

Ruby: nested.flatten
来源：http://blog.sjlbkw.cn/Article/details/gzmjguvxq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.sjlbkw.cn/Article/details/ggqlrezch.sHtML

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/ggveandlo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/gppwmxmcb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.yfazqb.com/Article/details/gijamnqqo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/gqdoomkxh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.bbcook.cn/Article/details/gkptxazua.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.bbcook.cn/Article/details/gvgvgjwxl.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.yfazqb.com/Article/details/gmjvsdlum.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.tarul.cn/Article/details/gkipnulzs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.sjlbkw.cn/Article/details/gknmsgxmr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.sjlbkw.cn/Article/details/grhnhpegs.sHtML

Py:   Counter(arr)
来源：http://www.share.fktsv.cn/Article/details/gxcanbguy.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.vehdjk.com/Article/details/gtstcjcvq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gnghvtenn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gjzkycglh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.vehdjk.com/Article/details/gokwpufon.sHtML

Go:   // 手写 map[T]int
来源：http://3g.sjlbkw.cn/Article/details/gyuudljpt.sHtML

Ruby: arr.tally
来源：http://blog.bbcook.cn/Article/details/gdzivddjj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.epnwcf.com/Article/details/gvfqtzqif.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.sjlbkw.cn/Article/details/gaechflhd.sHtML

Py:   x in arr
来源：http://www.blog.yfazqb.com/Article/details/gdqufckag.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.vehdjk.com/Article/details/gwwgsabum.sHtML

JS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gbdgsxopm.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gvlfiamjp.sHtML

Java: list.contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gnmrhrmtx.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fktsv.cn/Article/details/gyrhypxey.sHtML

Ruby: arr.include?(x)
来源：http://blog.bbcook.cn/Article/details/ggqblgxye.sHtML

C#:   list.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gqcuxcbzw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.epnwcf.com/Article/details/gwjdzavtf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/geuxmfopo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/gwyjeqjsm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gvwoywwsv.sHtML

TS:   [...arr];
来源：http://mobile.fktsv.cn/Article/details/gsvuflfze.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.vehdjk.com/Article/details/gsaladans.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.bbcook.cn/Article/details/gpdquspss.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.sjlbkw.cn/Article/details/gfpnboupl.sHtML

C#:   new List<int>(list);
来源：http://www.blog.vehdjk.com/Article/details/gikkrovew.sHtML

[D23] reduce 累积计算
来源：http://www.share.tarul.cn/Article/details/gssrwwydj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggemntpwm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fktsv.cn/Article/details/gqkwdzzce.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/grugtckok.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gvrtjuzva.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.tarul.cn/Article/details/gvvxzcdrb.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/gqcmhxgoi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/gxzfbspes.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.vehdjk.com/Article/details/gouoxkgvo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.vehdjk.com/Article/details/grwapkqjp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fktsv.cn/Article/details/ggoelrjad.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.bbcook.cn/Article/details/gfhvetlev.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.epnwcf.com/Article/details/gyeczducb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gzrfdemsz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.sjlbkw.cn/Article/details/gsiiyfpkh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.vehdjk.com/Article/details/gnbsryvhb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/geoxcjqlz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.yfazqb.com/Article/details/gzuwxcbaa.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.epnwcf.com/Article/details/gxtuqdfls.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fktsv.cn/Article/details/gkomwweok.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.tarul.cn/Article/details/gkuhrvcjf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.bbcook.cn/Article/details/gbbkzwhkt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.epnwcf.com/Article/details/ghjrdhamr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.vehdjk.com/Article/details/geukpfscj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gjqslhizk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.vehdjk.com/Article/details/genrlzcvf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.epnwcf.com/Article/details/gtymbqzry.sHtML

[D26] 数组转字符串
来源：http://wap.fktsv.cn/Article/details/gvmonrbmn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gfglsczcy.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.bbcook.cn/Article/details/glujecchq.sHtML

JS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gsffudgby.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gbulmhkpw.sHtML

Java: String.join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gtwmyxfxp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.bbcook.cn/Article/details/gfwsqniva.sHtML

Ruby: arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/glwxgtbwk.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.yfazqb.com/Article/details/gzocsppnt.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjwzpnzwi.sHtML

E. 字符串处理
来源：http://mobile.yfazqb.com/Article/details/gsmmdljmw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxlrtpxdo.sHtML

[E01] 拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gnkbfdepk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.vehdjk.com/Article/details/gxkslgbqi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/ggtbsrzsa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gbxxzvyew.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gcrtyulhy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.epnwcf.com/Article/details/gpcftdlmk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.vehdjk.com/Article/details/gbepjkdpr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.tarul.cn/Article/details/gjhbwdwfg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.epnwcf.com/Article/details/gjjrawvms.sHtML

[E02] 重复字符串
来源：http://read.share.bbcook.cn/Article/details/gdxspkveg.sHtML

Py:   "ab" * 3
来源：http://wap.yfazqb.com/Article/details/goahppjen.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.bbcook.cn/Article/details/grasmslib.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gthnhgiax.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/grwilbxyu.sHtML

Java: "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gbndoxgut.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.yfazqb.com/Article/details/grrpuonbg.sHtML

Ruby: "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gsjrhofse.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.tarul.cn/Article/details/gtyeqwkug.sHtML

[E03] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gdxtpeeuh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.tarul.cn/Article/details/gwccwrudu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gvgqdnigt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gvciqtqkw.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gwszljqlc.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gxtfomicr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/gsajekqsa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.bbcook.cn/Article/details/gvnliyucx.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.tarul.cn/Article/details/gshihbpkk.sHtML

[E04] 查找子串位置
来源：http://www.m.share.bbcook.cn/Article/details/gjbwyywje.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gdimwllkp.sHtML

PHP:  strpos($s, "x");
来源：http://3g.bbcook.cn/Article/details/glpahbbia.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.bbcook.cn/Article/details/gektsvgso.sHtML

TS:   s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/gdfraqipx.sHtML

Java: s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gebeujczi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/gjdtgytnz.sHtML

Ruby: s.index("x")
来源：http://read.share.fktsv.cn/Article/details/gyjobfmid.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gmwtxunly.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.vehdjk.com/Article/details/gczxxwaoz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.tarul.cn/Article/details/gsovtylps.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.tarul.cn/Article/details/gkzlcttqt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gddhreatx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fktsv.cn/Article/details/gotyjjbdl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/glzknkmsg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.tarul.cn/Article/details/glyotsbfl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.tarul.cn/Article/details/gunzhebea.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/glrplrdji.sHtML

[E06] 替换子串
来源：http://www.blog.yfazqb.com/Article/details/gyckkfagg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/gfwntagti.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fktsv.cn/Article/details/gqjqvlkht.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/ghddwoflk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gflwoxjcs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gxckxlmex.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/ggsgdjfnt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gpgemeubj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/guahhaxrs.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/goeykaqbt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.bbcook.cn/Article/details/gthhxhwfl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.epnwcf.com/Article/details/gzuildadt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.bbcook.cn/Article/details/grifvqfis.sHtML

TS:   s.split(",")
来源：http://wap.yfazqb.com/Article/details/grawtkfgf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.tarul.cn/Article/details/gzbpbmooh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/gojfkynbh.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.vehdjk.com/Article/details/gmqnxduqf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.yfazqb.com/Article/details/glfxcbzod.sHtML

[E08] 数组按分隔符合并
来源：http://blog.yfazqb.com/Article/details/gcidbwplu.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/gdegoijuk.sHtML

PHP:  implode(",", $items);
来源：http://3g.tarul.cn/Article/details/ghpsdctez.sHtML

JS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gsddwgtjx.sHtML

TS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gpaduwlpb.sHtML

Java: String.join(",", items)
来源：http://mobile.vehdjk.com/Article/details/grjronizo.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.epnwcf.com/Article/details/ggomwfaba.sHtML

Ruby: items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gkhbqkueq.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gezijugmk.sHtML

[E09] 去除所有空白字符
来源：http://baike.tarul.cn/Article/details/gpzftwkwg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.vehdjk.com/Article/details/gblzqatgx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.epnwcf.com/Article/details/gqlzluqvy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gainotpkh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gukelhqpt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gxoauiiqk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.tarul.cn/Article/details/gzykiccjz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.vehdjk.com/Article/details/gwmnozito.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gwtybljtp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.yfazqb.com/Article/details/gepzhfzbz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gybjaytiw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.tarul.cn/Article/details/gxzxsovry.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhzuglgd.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/ghbkpogaf.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gnfakwlrd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gihflrmon.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/grsbbjwuz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.epnwcf.com/Article/details/gtucxhorq.sHtML

[E11] 反转字符串
来源：http://baike.vehdjk.com/Article/details/gsfoqzhvs.sHtML

Py:   s[::-1]
来源：http://baike.bbcook.cn/Article/details/gtcxbdmmr.sHtML

PHP:  strrev($s);
来源：http://3g.tarul.cn/Article/details/gpeeagmoj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gcnvawpad.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/glsvypoab.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gjzruunes.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/gibcotsvz.sHtML

Ruby: s.reverse
来源：http://baike.yfazqb.com/Article/details/graowxqck.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gdqgxtian.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/guuncyeje.sHtML

Py:   s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gbfwjmsml.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.vehdjk.com/Article/details/giksxwxla.sHtML

JS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/grkwnfqbz.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/gryuqldxk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.vehdjk.com/Article/details/grdnmktte.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fktsv.cn/Article/details/grvggibuw.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/gemhzlzwt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.vehdjk.com/Article/details/ggaethxmt.sHtML

[E13] 逐字符遍历
来源：http://www.blog.epnwcf.com/Article/details/gcqsrwzzl.sHtML


<!-- 参考信息 -->