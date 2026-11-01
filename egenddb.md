代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/glqmfgviu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gzgtysmif.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gsepitowe.sHtML

[D06] 数组长度
来源：http://3g.yfazqb.com/Article/details/galkltdia.sHtML

Py:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gbcceiheh.sHtML

PHP:  count($arr);
来源：http://read.share.epnwcf.com/Article/details/geldubkpc.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gifduoqkt.sHtML

TS:   arr.length
来源：http://read.share.vehdjk.com/Article/details/gxhhjndqq.sHtML

Java: list.size();
来源：http://www.blog.yfazqb.com/Article/details/grzanklbh.sHtML

Go:   len(arr)
来源：http://blog.fktsv.cn/Article/details/gowbclipa.sHtML

Ruby: arr.length; arr.size
来源：http://baike.tarul.cn/Article/details/glotdxgup.sHtML

C#:   list.Count;
来源：http://www.m.share.yfazqb.com/Article/details/gozscguud.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.vehdjk.com/Article/details/gsujqavqw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.bbcook.cn/Article/details/gzdiqweve.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.yfazqb.com/Article/details/goyqnsokl.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gvklvxjwu.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gggdyrexn.sHtML

Java: list.subList(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gqtusixzp.sHtML

Go:   arr[1:4]
来源：http://www.blog.fktsv.cn/Article/details/ghucqlvad.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/gkwvzwqul.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.bbcook.cn/Article/details/gkpiatsmh.sHtML

[D08] 合并两个数组
来源：http://www.share.epnwcf.com/Article/details/gfpfiknue.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.epnwcf.com/Article/details/gdtxedssl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.tarul.cn/Article/details/gmyiuryir.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.tarul.cn/Article/details/gurpzzxvf.sHtML

TS:   [...a, ...b];
来源：http://www.blog.bbcook.cn/Article/details/gtxjgvnmw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.sjlbkw.cn/Article/details/gzvqbgkcc.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gjzgginpa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.epnwcf.com/Article/details/goqquqqhc.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.bbcook.cn/Article/details/gslhjauty.sHtML

[D09] 排序（升序）
来源：http://www.share.tarul.cn/Article/details/gaouhsxru.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/getbmtirm.sHtML

PHP:  sort($arr);
来源：http://wap.epnwcf.com/Article/details/gdlrsitbx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.vehdjk.com/Article/details/gvrtceduu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.tarul.cn/Article/details/gxgqiatat.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.vehdjk.com/Article/details/gaqqljxxh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gwpjimdox.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gybosjtdv.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/gvqobzrre.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.bbcook.cn/Article/details/ghzzeytfh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.tarul.cn/Article/details/gdsleoskz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.yfazqb.com/Article/details/gnmkagnux.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/gteuzhpwf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/grmeninmh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.bbcook.cn/Article/details/ggjacvepr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fktsv.cn/Article/details/gajrxnoon.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.tarul.cn/Article/details/gckmqtldn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.sjlbkw.cn/Article/details/gtzovecdz.sHtML

[D11] 反转数组
来源：http://m.share.tarul.cn/Article/details/gtgoilaba.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxijfjhx.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.tarul.cn/Article/details/ggliqtins.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.tarul.cn/Article/details/gevcmjscf.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.epnwcf.com/Article/details/gtnihzubf.sHtML

Java: Collections.reverse(list);
来源：http://www.share.tarul.cn/Article/details/gwllpzlfm.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.epnwcf.com/Article/details/gnllzesrp.sHtML

Ruby: arr.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gpbkhlpio.sHtML

C#:   list.Reverse();
来源：http://read.share.vehdjk.com/Article/details/glbqdypgz.sHtML

[D12] 查找元素下标
来源：http://mobile.sjlbkw.cn/Article/details/gegonpuxg.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.epnwcf.com/Article/details/gjrggaymo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/glxtvmdmk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/grsylkmmo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/gqcmjzdtr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/geehnndjs.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.tarul.cn/Article/details/gwcitygdz.sHtML

Ruby: arr.index(x)
来源：http://baike.epnwcf.com/Article/details/gywdiilnw.sHtML

C#:   list.IndexOf(x);
来源：http://3g.yfazqb.com/Article/details/gtwvidsjk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.bbcook.cn/Article/details/gulwrgxgu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.bbcook.cn/Article/details/gvsrtznut.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.yfazqb.com/Article/details/gryrsclle.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gmwwgbcns.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/gowivlvvc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.bbcook.cn/Article/details/gsublwwno.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.epnwcf.com/Article/details/grmyyctte.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.bbcook.cn/Article/details/gbqhobqrn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gciraxhmh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.bbcook.cn/Article/details/gdjqdewcq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.tarul.cn/Article/details/gtzeggsjk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/grypmsgep.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gzfipgpeh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/gtzhrpswr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fktsv.cn/Article/details/gtrsftvcb.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/gvftdfpff.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.yfazqb.com/Article/details/gmaixdnek.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gkoofptlc.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/ghhmajrki.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gpntktmmk.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gbjhijxxp.sHtML

JS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gxaeezzpf.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gxmxgmgbu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.epnwcf.com/Article/details/gownfztak.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.sjlbkw.cn/Article/details/gcrkbbuat.sHtML

Ruby: arr.uniq
来源：http://www.m.share.epnwcf.com/Article/details/gdeoxgdjr.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.yfazqb.com/Article/details/gxtloztmm.sHtML

[D16] 求和与平均值
来源：http://read.share.sjlbkw.cn/Article/details/gihopjvor.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.tarul.cn/Article/details/gwtjjliro.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gylgklkaz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/ghgghgboz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.bbcook.cn/Article/details/gjsowgaap.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.tarul.cn/Article/details/grbzahohq.sHtML

Go:   // 手写循环累加
来源：http://m.share.vehdjk.com/Article/details/gnbinlksn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.yfazqb.com/Article/details/gciauoycy.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fktsv.cn/Article/details/gexlhjrtu.sHtML

[D17] 最大值与最小值
来源：http://blog.sjlbkw.cn/Article/details/guzxcmhrw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.vehdjk.com/Article/details/grdimyclx.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.yfazqb.com/Article/details/gwzsxclxg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fktsv.cn/Article/details/ggpkumsjx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.vehdjk.com/Article/details/giijphfku.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fktsv.cn/Article/details/gsepdbgag.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.yfazqb.com/Article/details/gwgnctguq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.sjlbkw.cn/Article/details/gusitmdyz.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.sjlbkw.cn/Article/details/gdooxwlqi.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/gzrljxuvi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/gqkimeqog.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fktsv.cn/Article/details/gnflrgcfp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fktsv.cn/Article/details/gnlqhilgl.sHtML

TS:   nested.flat();
来源：http://wap.bbcook.cn/Article/details/gwmjifbnf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.vehdjk.com/Article/details/gpjuepapu.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/gukthoree.sHtML

Ruby: nested.flatten
来源：http://read.share.yfazqb.com/Article/details/guahdjhdx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/gckcmbewm.sHtML

[D19] 按字段分组
来源：http://mobile.epnwcf.com/Article/details/gsencvjuq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.bbcook.cn/Article/details/gjgdqbuag.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.yfazqb.com/Article/details/gsgzbvrci.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/gahpltegr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gyafhpvbw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.bbcook.cn/Article/details/gpqyvhczp.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.epnwcf.com/Article/details/gbkxyaqnq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.bbcook.cn/Article/details/goilymakd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.sjlbkw.cn/Article/details/gbezwucrd.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.tarul.cn/Article/details/gyobsigoo.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/guiuigznh.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gvyoxmqqt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gigyfurev.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fktsv.cn/Article/details/gteukckpw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.sjlbkw.cn/Article/details/gnmkprvlc.sHtML

Go:   // 手写 map[T]int
来源：http://baike.tarul.cn/Article/details/gudvluhqt.sHtML

Ruby: arr.tally
来源：http://baike.yfazqb.com/Article/details/ghzyknsci.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/gzdjywcuu.sHtML

[D21] 判断是否包含某元素
来源：http://3g.yfazqb.com/Article/details/gcpiksreh.sHtML

Py:   x in arr
来源：http://wap.yfazqb.com/Article/details/gvksquyju.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.bbcook.cn/Article/details/gnutaaeuw.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gaxqnotvm.sHtML

TS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/guotsszbo.sHtML

Java: list.contains(x)
来源：http://baike.yfazqb.com/Article/details/gymnhzxxg.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.yfazqb.com/Article/details/gjegdgufm.sHtML

Ruby: arr.include?(x)
来源：http://3g.fktsv.cn/Article/details/ghbxvaxqo.sHtML

C#:   list.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gzrhgyvgz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.bbcook.cn/Article/details/gohhcivof.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fktsv.cn/Article/details/gsmflyiyn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.vehdjk.com/Article/details/gclxilhei.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gzinaxrob.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/ghmhjbhsa.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fktsv.cn/Article/details/gssqircdj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.yfazqb.com/Article/details/gkypvemqt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fktsv.cn/Article/details/ggnjnujmu.sHtML

C#:   new List<int>(list);
来源：http://www.share.yfazqb.com/Article/details/gbvoubptj.sHtML

[D23] reduce 累积计算
来源：http://mobile.yfazqb.com/Article/details/gjbwxjzjn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gjcrcuwkj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.bbcook.cn/Article/details/geswpcmhr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gvemjifni.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gxoncfyxi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fktsv.cn/Article/details/getfhcrtb.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gynsmjmse.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/gjvklhrxa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.vehdjk.com/Article/details/gkvmyniik.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.sjlbkw.cn/Article/details/gjrtxwlgw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.sjlbkw.cn/Article/details/gfhezkbks.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.vehdjk.com/Article/details/gcigsafzf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.epnwcf.com/Article/details/gawxhrvmm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gecvddbcm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.bbcook.cn/Article/details/gyscchobj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.vehdjk.com/Article/details/gfnmelnsa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.epnwcf.com/Article/details/gyxpohepm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.yfazqb.com/Article/details/gmjsoekmx.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/gxlhqkiqw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.vehdjk.com/Article/details/grzcywmud.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/gnasrnmjb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.epnwcf.com/Article/details/gpdetjaub.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.tarul.cn/Article/details/giomlxmpi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fktsv.cn/Article/details/gfscmjole.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.sjlbkw.cn/Article/details/gbzugugui.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.yfazqb.com/Article/details/ghiqeztht.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fktsv.cn/Article/details/glzbtkzho.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/ghccainie.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gsrsrqyfs.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gozsfdeyo.sHtML

JS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gjyxabacj.sHtML

TS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gbripmphp.sHtML

Java: String.join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gpvsvivpa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.epnwcf.com/Article/details/gqwnlhcey.sHtML

Ruby: arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gwbqlqjdd.sHtML

C#:   string.Join(", ", list)
来源：http://wap.tarul.cn/Article/details/glnqscjdg.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjrujdfto.sHtML

E. 字符串处理
来源：http://mobile.fktsv.cn/Article/details/gokbhyjjm.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gidnvmtvd.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gaztprjdg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.epnwcf.com/Article/details/gyfvdrqzm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.yfazqb.com/Article/details/gyyuqkryh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/ghpbzumve.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gcpvrgagu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.epnwcf.com/Article/details/gneiutyog.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.tarul.cn/Article/details/gtsixbyjb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.yfazqb.com/Article/details/gdvybrrnh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.bbcook.cn/Article/details/ghbwwpumx.sHtML

[E02] 重复字符串
来源：http://m.share.fktsv.cn/Article/details/gocawjdgb.sHtML

Py:   "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gclswgmht.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.tarul.cn/Article/details/gmktkatid.sHtML

JS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gdczxeuqd.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gwwlqmuhx.sHtML

Java: "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gsggexqpi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.tarul.cn/Article/details/gogzskdfi.sHtML

Ruby: "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gbswrcrws.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gygximxrl.sHtML

[E03] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gfncfkfxg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.epnwcf.com/Article/details/gfojfosto.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gqoknvygp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/grxipvnpl.sHtML

TS:   s.slice(1, 4)
来源：http://baike.bbcook.cn/Article/details/gywzawvew.sHtML

Java: s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/giyjhompp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.yfazqb.com/Article/details/gyjelxhms.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/gvgrohpsu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.sjlbkw.cn/Article/details/gslneztob.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/gifskonbm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gomzyyhun.sHtML

PHP:  strpos($s, "x");
来源：http://blog.sjlbkw.cn/Article/details/glaukgfek.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.bbcook.cn/Article/details/gwltdhuxi.sHtML

TS:   s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gkfcfdbvd.sHtML

Java: s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gwezlpwnv.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.epnwcf.com/Article/details/gqncxxvxc.sHtML

Ruby: s.index("x")
来源：http://read.share.vehdjk.com/Article/details/gtdbrgvjq.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gvcoplbtu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.sjlbkw.cn/Article/details/gztjifzpg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gviwlzajr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.bbcook.cn/Article/details/gwuxpizcx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gajagzcpy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.bbcook.cn/Article/details/gxliucnea.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/ghoczoogz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fktsv.cn/Article/details/gbuzhqxod.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.vehdjk.com/Article/details/gqercaylv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.vehdjk.com/Article/details/goqovjvay.sHtML

[E06] 替换子串
来源：http://wap.tarul.cn/Article/details/gjjzqgedv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gchgfecvx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.tarul.cn/Article/details/givaucgeq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gtxvnvhwc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gsnxjwchx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gytyzgfki.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/glyoaowyl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gtpkcezal.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gbtrhrney.sHtML

[E07] 按分隔符拆分
来源：http://3g.tarul.cn/Article/details/gpbzqnzhx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.sjlbkw.cn/Article/details/glbrqkxhn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.yfazqb.com/Article/details/ganfubfds.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fktsv.cn/Article/details/gbxecfzkc.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/gilatqvda.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.bbcook.cn/Article/details/gqpwuzwop.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fktsv.cn/Article/details/gbrszerqo.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fktsv.cn/Article/details/gqupfgedn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.yfazqb.com/Article/details/gxiceujmu.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/gxbpssmgo.sHtML

Py:   ",".join(items)
来源：http://www.share.sjlbkw.cn/Article/details/gmtnhzkvl.sHtML

PHP:  implode(",", $items);
来源：http://mobile.yfazqb.com/Article/details/garvbaqrn.sHtML

JS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gbvnenvwe.sHtML

TS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gvvumtocl.sHtML

Java: String.join(",", items)
来源：http://3g.yfazqb.com/Article/details/gcpajasfx.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.bbcook.cn/Article/details/gkqiimnmc.sHtML

Ruby: items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gwtujmmoe.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/glzpavefv.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/gceuvnurk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.yfazqb.com/Article/details/gzfgdmzvl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gmkzhdjeu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gbeycoimw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gizenfqwp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.bbcook.cn/Article/details/gnedqhrbo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gwlhnsubv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.epnwcf.com/Article/details/gzxqiizwe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gojrpgrky.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.epnwcf.com/Article/details/ggiqmzkcx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gmpbmyphf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fktsv.cn/Article/details/gvwkhtlsm.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gpdrrbdrj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwftszye.sHtML

Java: String.format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gnzvjntyf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gsnvrhfmt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/ggdgfofgw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.bbcook.cn/Article/details/gheheonxo.sHtML

[E11] 反转字符串
来源：http://read.share.epnwcf.com/Article/details/gqzxvtoft.sHtML

Py:   s[::-1]
来源：http://m.share.tarul.cn/Article/details/gdrvfslyk.sHtML

PHP:  strrev($s);
来源：http://baike.fktsv.cn/Article/details/gpehfkihb.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gcgzavgqp.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/ggpwavhui.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.yfazqb.com/Article/details/gdnvhhnse.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.vehdjk.com/Article/details/gfzbitnbi.sHtML

Ruby: s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gqtlhktoi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/gtjkjlaub.sHtML

[E12] 统计某字符出现次数
来源：http://baike.sjlbkw.cn/Article/details/giaauihjd.sHtML

Py:   s.count("a")
来源：http://mobile.vehdjk.com/Article/details/grwxklpzk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.bbcook.cn/Article/details/gipstotap.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gxyxksrwm.sHtML

TS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gdoqmnbgg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/gskbcwhvq.sHtML


<!-- 参考信息 -->