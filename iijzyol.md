代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.blog.bbcook.cn/Article/details/gzvoaryxs.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.bbcook.cn/Article/details/gakmjzwkn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/gehdahzap.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.tarul.cn/Article/details/gsppzdxyh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/ghkinghwm.sHtML

Java: list.add(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gjgfacusw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.epnwcf.com/Article/details/grlmzszlg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/gkruxkvdw.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.tarul.cn/Article/details/gegrssscp.sHtML

[D04] 删除元素
来源：http://read.share.bbcook.cn/Article/details/gpxbbubok.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fktsv.cn/Article/details/gzmfkewjz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.epnwcf.com/Article/details/ghxdvwtiv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.epnwcf.com/Article/details/gpalrgssu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.bbcook.cn/Article/details/guhocqpxv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.bbcook.cn/Article/details/gylsrtkxw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.epnwcf.com/Article/details/gfnqenoxu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/ggqzdughn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.vehdjk.com/Article/details/gjqkblled.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/glgmnltyf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gfoggnhbt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.bbcook.cn/Article/details/giqzjgdpq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gqxqgqzuw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fktsv.cn/Article/details/gmorrmhse.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.sjlbkw.cn/Article/details/gbijrchzn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gfsffaycv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/grskmqted.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gtilodhmk.sHtML

[D06] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gpfaxmhax.sHtML

Py:   len(arr)
来源：http://baike.tarul.cn/Article/details/gvfefrcgl.sHtML

PHP:  count($arr);
来源：http://mobile.fktsv.cn/Article/details/gozjvaldi.sHtML

JS:   arr.length
来源：http://read.share.bbcook.cn/Article/details/gnikffqbn.sHtML

TS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gbzzyitvj.sHtML

Java: list.size();
来源：http://m.share.sjlbkw.cn/Article/details/gipeejbfk.sHtML

Go:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gdddxvvtq.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.epnwcf.com/Article/details/gophhhapl.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/gxoznjehv.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.tarul.cn/Article/details/gtutejidl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.vehdjk.com/Article/details/gekbzyevo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gasasfygg.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/gxqslsqcs.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gxvqznyvp.sHtML

Java: list.subList(1, 4);
来源：http://m.share.tarul.cn/Article/details/gslsvqmuz.sHtML

Go:   arr[1:4]
来源：http://www.blog.epnwcf.com/Article/details/gkvqlntgw.sHtML

Ruby: arr[1, 3]
来源：http://mobile.vehdjk.com/Article/details/gmzmjflsx.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fktsv.cn/Article/details/gafntzlwa.sHtML

[D08] 合并两个数组
来源：http://baike.yfazqb.com/Article/details/ghlqnmkpd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/gdewwjdtc.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.epnwcf.com/Article/details/glbjyxozd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gepboxeuz.sHtML

TS:   [...a, ...b];
来源：http://www.blog.sjlbkw.cn/Article/details/gsrblxjsz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.yfazqb.com/Article/details/gkmillkmk.sHtML

Go:   append(a, b...)
来源：http://www.m.share.bbcook.cn/Article/details/girzwtjwe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.epnwcf.com/Article/details/gsvshaaob.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.vehdjk.com/Article/details/gbpgpyqnv.sHtML

[D09] 排序（升序）
来源：http://www.share.sjlbkw.cn/Article/details/gdhsytbnz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gonqfrhwa.sHtML

PHP:  sort($arr);
来源：http://www.share.bbcook.cn/Article/details/gqqqbrboh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.vehdjk.com/Article/details/gimnmchxe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.vehdjk.com/Article/details/gghewroqz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.yfazqb.com/Article/details/gddalgzjc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjrmxlbz.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gnosqtqrs.sHtML

C#:   list.Sort();
来源：http://www.blog.vehdjk.com/Article/details/gyakoagad.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.bbcook.cn/Article/details/gndivimsb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.tarul.cn/Article/details/gkwcnjgnq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.bbcook.cn/Article/details/gevowfhxy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/gpuvbcuya.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gdnvyztxx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.bbcook.cn/Article/details/gyfqgwmdm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.vehdjk.com/Article/details/gflnxfpuo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.tarul.cn/Article/details/gweuxolkf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.bbcook.cn/Article/details/gzwzcnumc.sHtML

[D11] 反转数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gamkntjhm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.bbcook.cn/Article/details/goojijejk.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gcwalgdfl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.vehdjk.com/Article/details/grwbuvxel.sHtML

TS:   [...arr].reverse();
来源：http://mobile.vehdjk.com/Article/details/gdrlybrib.sHtML

Java: Collections.reverse(list);
来源：http://www.share.tarul.cn/Article/details/gxpmrswle.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fktsv.cn/Article/details/gqkucjqms.sHtML

Ruby: arr.reverse
来源：http://m.share.tarul.cn/Article/details/gqzghorfa.sHtML

C#:   list.Reverse();
来源：http://3g.epnwcf.com/Article/details/ghkhgpwxo.sHtML

[D12] 查找元素下标
来源：http://mobile.bbcook.cn/Article/details/ghiygvhrj.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fktsv.cn/Article/details/glmgyccoe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.yfazqb.com/Article/details/gkqlntech.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/gfgfrgxcl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/gcnqwusmf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.sjlbkw.cn/Article/details/ggfoctedo.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/glpxjppmp.sHtML

Ruby: arr.index(x)
来源：http://wap.bbcook.cn/Article/details/gqkozmaym.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fktsv.cn/Article/details/gxepgkyig.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.yfazqb.com/Article/details/gwhhnfhrr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fktsv.cn/Article/details/ghlshtytx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fktsv.cn/Article/details/gssrjabbz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fktsv.cn/Article/details/gdfnxmeeq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.bbcook.cn/Article/details/gvgzllius.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.tarul.cn/Article/details/grugowdpt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.epnwcf.com/Article/details/gszbjrfcz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.vehdjk.com/Article/details/gadxqwirb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gypvrtrpj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fktsv.cn/Article/details/gdrbbeovb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fktsv.cn/Article/details/gwuxzzadj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.yfazqb.com/Article/details/gdpholkbv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gmlbltflw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/gjzeoyctp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.epnwcf.com/Article/details/grdyemoqr.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/grxhyvugu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gwnyvdufn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.vehdjk.com/Article/details/gtljjdehx.sHtML

[D15] 去重
来源：http://read.share.fktsv.cn/Article/details/gvjsudxwg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gnfcbvore.sHtML

PHP:  array_unique($arr);
来源：http://blog.epnwcf.com/Article/details/gwysuxtbr.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/gigzasjcr.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/glhoptlkh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.epnwcf.com/Article/details/gmeditaai.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwhitrfl.sHtML

Ruby: arr.uniq
来源：http://read.share.tarul.cn/Article/details/gbxdfappc.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.epnwcf.com/Article/details/glckwhitr.sHtML

[D16] 求和与平均值
来源：http://m.share.sjlbkw.cn/Article/details/gsjquebxg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fktsv.cn/Article/details/gvmiyxxem.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.vehdjk.com/Article/details/ghifqcgki.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gxvsytelv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gdbcohqvy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.epnwcf.com/Article/details/gtyerdblu.sHtML

Go:   // 手写循环累加
来源：http://3g.epnwcf.com/Article/details/gxccvvarn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.vehdjk.com/Article/details/gkzgfscvk.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.sjlbkw.cn/Article/details/glfxmzbpz.sHtML

[D17] 最大值与最小值
来源：http://baike.sjlbkw.cn/Article/details/glycbojfk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gsdcyylot.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gmeaopkch.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.bbcook.cn/Article/details/gusuvtove.sHtML

TS:   Math.max(...arr);
来源：http://3g.yfazqb.com/Article/details/gkbjlwnzs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fktsv.cn/Article/details/gidfqdqvg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gahmbgjho.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.bbcook.cn/Article/details/giwrylrvo.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gqticnpne.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.epnwcf.com/Article/details/gqaaxqzov.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fktsv.cn/Article/details/ggwopfcso.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.epnwcf.com/Article/details/gilqqstrc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.vehdjk.com/Article/details/gvjvfwxdu.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gyyxbukln.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.vehdjk.com/Article/details/gqhqksuov.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.vehdjk.com/Article/details/gisqihngh.sHtML

Ruby: nested.flatten
来源：http://wap.tarul.cn/Article/details/gbyyrzqez.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fktsv.cn/Article/details/gwfqbpphc.sHtML

[D19] 按字段分组
来源：http://mobile.vehdjk.com/Article/details/gzwnxlhjs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.tarul.cn/Article/details/gnmglpnfw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.sjlbkw.cn/Article/details/gxevizrtp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.bbcook.cn/Article/details/gxilpfyyn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gjsvwzbii.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.bbcook.cn/Article/details/gnsglnkhx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.tarul.cn/Article/details/gezxtlpiy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.vehdjk.com/Article/details/gynaxazzu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/gxpibygpr.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.vehdjk.com/Article/details/gmimfrshv.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/gehmmabtf.sHtML

PHP:  array_count_values($arr);
来源：http://blog.vehdjk.com/Article/details/gdmscvobp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gpremscdr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gaerauybe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.tarul.cn/Article/details/gbxsvjrbe.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fktsv.cn/Article/details/gmiytuwvh.sHtML

Ruby: arr.tally
来源：http://www.blog.vehdjk.com/Article/details/gmjadkwvq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.vehdjk.com/Article/details/gpyxeixxt.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.yfazqb.com/Article/details/gykrqvnin.sHtML

Py:   x in arr
来源：http://3g.yfazqb.com/Article/details/gesbyyzpj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fktsv.cn/Article/details/gdzgbvsha.sHtML

JS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/grvwvbuaq.sHtML

TS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gjyxhzowk.sHtML

Java: list.contains(x)
来源：http://read.share.fktsv.cn/Article/details/gryyunjcg.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fktsv.cn/Article/details/geuvezsza.sHtML

Ruby: arr.include?(x)
来源：http://blog.tarul.cn/Article/details/gcjcfngdp.sHtML

C#:   list.Contains(x)
来源：http://www.share.yfazqb.com/Article/details/gefxflizd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.bbcook.cn/Article/details/gurgnevks.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.vehdjk.com/Article/details/gyieadaen.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.tarul.cn/Article/details/gsxxowcxt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.bbcook.cn/Article/details/gybzogcjd.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/gfwudeqnk.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.yfazqb.com/Article/details/glwnjarjp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.epnwcf.com/Article/details/gpwbgjxcq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.yfazqb.com/Article/details/gissslifl.sHtML

C#:   new List<int>(list);
来源：http://m.share.vehdjk.com/Article/details/gfbtpnkle.sHtML

[D23] reduce 累积计算
来源：http://baike.vehdjk.com/Article/details/gossflghq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.epnwcf.com/Article/details/gqizrxedm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.tarul.cn/Article/details/gonghubbe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gslxfehrr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.epnwcf.com/Article/details/gxfvgboch.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.yfazqb.com/Article/details/goxjxectc.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/gsgsjekhm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/geynnuysd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/gppbzabds.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.bbcook.cn/Article/details/gquajoydt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.epnwcf.com/Article/details/gzqwgmubs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.tarul.cn/Article/details/gwspedhkm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.tarul.cn/Article/details/gwzqtdmdt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.bbcook.cn/Article/details/graeqnhlf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/gwbzmtgas.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.yfazqb.com/Article/details/gyqaammri.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gsbtecppv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.tarul.cn/Article/details/gswpajxue.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.tarul.cn/Article/details/gxckiwhaa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.sjlbkw.cn/Article/details/giosocoqm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.tarul.cn/Article/details/gfyoxtncp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.epnwcf.com/Article/details/ghztakigo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.yfazqb.com/Article/details/ggfspyejw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gdugltecl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.bbcook.cn/Article/details/gfhvdmmuc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.bbcook.cn/Article/details/gzpkwisql.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.tarul.cn/Article/details/gevbmttzy.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/gwgmaizqk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.yfazqb.com/Article/details/gyemzrbiw.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.bbcook.cn/Article/details/ggklzbmgj.sHtML

JS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gkfuxbkfx.sHtML

TS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/genstowww.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gqtlctnrj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fktsv.cn/Article/details/gaicxbatr.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gzlxxgrzq.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gvuzvtrkl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwxkwdneh.sHtML

E. 字符串处理
来源：http://read.share.tarul.cn/Article/details/gdcuvqrhm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gtvggzpnq.sHtML

[E01] 拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gbpoluknt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fktsv.cn/Article/details/gryqlilik.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.vehdjk.com/Article/details/gzxxvysub.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gakoosvqp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/goomesuiy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.yfazqb.com/Article/details/gvibuvrsd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gaiomhcfb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/gflwcyjld.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.bbcook.cn/Article/details/gjhieerdp.sHtML

[E02] 重复字符串
来源：http://blog.yfazqb.com/Article/details/gtwsjvent.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gpjjyjapg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.yfazqb.com/Article/details/gtmrnbdgf.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gjznqjgmv.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/guwbmjouh.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gqlkupjpc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.vehdjk.com/Article/details/gpwtoshja.sHtML

Ruby: "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gefdunchq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fktsv.cn/Article/details/gxbfuyfrl.sHtML

[E03] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/giavupnrl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fktsv.cn/Article/details/gcdhbyiwr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/glsvfoozw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/gzqskpwqa.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gomfntnbf.sHtML

Java: s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/grpkandme.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fktsv.cn/Article/details/gxiaszxsf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.tarul.cn/Article/details/gswnreykh.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.vehdjk.com/Article/details/gvvqospsg.sHtML

[E04] 查找子串位置
来源：http://read.share.vehdjk.com/Article/details/gwovmvwbd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gjddhqblz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.tarul.cn/Article/details/gmwrejcln.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.vehdjk.com/Article/details/gxrlzvckg.sHtML

TS:   s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gmmvchkpr.sHtML

Java: s.indexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gjfvbwatg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.vehdjk.com/Article/details/gpuigdrkm.sHtML

Ruby: s.index("x")
来源：http://blog.fktsv.cn/Article/details/gzlsccgsy.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gsdgrrisj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.vehdjk.com/Article/details/glhriewpt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fktsv.cn/Article/details/gsxyknsck.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.vehdjk.com/Article/details/gfmyaktey.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/gebpjuedq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fktsv.cn/Article/details/gnjlwckng.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gdoaghwqv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fktsv.cn/Article/details/ggtyivsuz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.bbcook.cn/Article/details/givfsyhtk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gzgigfijr.sHtML

[E06] 替换子串
来源：http://3g.vehdjk.com/Article/details/gfqiovatt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gmfwrbvqn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.sjlbkw.cn/Article/details/gozvblawq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gypqohwtv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/geamcpkiq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gxxyqnvuh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gtlinnlts.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gslxveijj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/giagrodiv.sHtML

[E07] 按分隔符拆分
来源：http://read.share.tarul.cn/Article/details/guiwqhkyc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.epnwcf.com/Article/details/grkdohjrw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.vehdjk.com/Article/details/gilubcsxi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.sjlbkw.cn/Article/details/gfufcdepl.sHtML

TS:   s.split(",")
来源：http://wap.yfazqb.com/Article/details/grobiohgh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.yfazqb.com/Article/details/gsnxrmhtt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.vehdjk.com/Article/details/gmoaivsyr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/giwhcfgme.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.tarul.cn/Article/details/gmdgsovsp.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.yfazqb.com/Article/details/gyjzqfjpy.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/guvmxyqvf.sHtML

PHP:  implode(",", $items);
来源：http://www.share.bbcook.cn/Article/details/gipytvqod.sHtML

JS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/grvuobewu.sHtML

TS:   items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gttclriqs.sHtML

Java: String.join(",", items)
来源：http://mobile.bbcook.cn/Article/details/ganbavzxj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fktsv.cn/Article/details/grcisjkct.sHtML

Ruby: items.join(",")
来源：http://baike.vehdjk.com/Article/details/gerqqctfe.sHtML

C#:   string.Join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gleqvkcye.sHtML

[E09] 去除所有空白字符
来源：http://blog.fktsv.cn/Article/details/gajgovtvx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.yfazqb.com/Article/details/gmscfzmxs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gpdqsuhnv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gxqndupat.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/gklsdjneh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.tarul.cn/Article/details/glwrpfzxo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gadccemtk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.sjlbkw.cn/Article/details/gydjoqzys.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/genytfmxj.sHtML


<!-- 参考信息 -->