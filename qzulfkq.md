代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gmtdetrgf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fktsv.cn/Article/details/gaujderdt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrirgukt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.epnwcf.com/Article/details/gndnvwbxz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.sjlbkw.cn/Article/details/gwniyaube.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gualmgoqq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.vehdjk.com/Article/details/gkwmufqsh.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.tarul.cn/Article/details/gtksiojyw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.epnwcf.com/Article/details/gwkjzsgap.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.yfazqb.com/Article/details/gnczjhvad.sHtML

JS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/gwdjhhqoq.sHtML

TS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/guibmnvxy.sHtML

Java: list.add(4);
来源：http://read.share.tarul.cn/Article/details/grbujgiyb.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.yfazqb.com/Article/details/ghdajxhmi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.epnwcf.com/Article/details/gsiglnnxu.sHtML

C#:   list.Add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gxrnacjtk.sHtML

[D03] 在指定位置插入元素
来源：http://3g.yfazqb.com/Article/details/gxzoeveig.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.bbcook.cn/Article/details/gmmdvmkuv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fktsv.cn/Article/details/gqpfqdgjn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/govacozmu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fktsv.cn/Article/details/gfpwbxmmh.sHtML

Java: list.add(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gnqrsuzte.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.epnwcf.com/Article/details/gfvgshngk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fktsv.cn/Article/details/gilwgiymv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.bbcook.cn/Article/details/gseueuuwt.sHtML

[D04] 删除元素
来源：http://wap.tarul.cn/Article/details/gclnwntkt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.tarul.cn/Article/details/gcwzwikqa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fktsv.cn/Article/details/gxkrhbaph.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.epnwcf.com/Article/details/gpipydvbo.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.epnwcf.com/Article/details/grlctzrzh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.vehdjk.com/Article/details/grjpmhyes.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.bbcook.cn/Article/details/geculrhll.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.yfazqb.com/Article/details/gvnjoarbb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.epnwcf.com/Article/details/gwdftucbh.sHtML

[D05] 访问与修改元素
来源：http://m.share.fktsv.cn/Article/details/gocmnyjbq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gpmrcufrs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gvjjzmtrz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/gkljrvzdi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.tarul.cn/Article/details/giqbelsvu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtncrtgfv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gsrsqaceb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gmiyeofux.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.tarul.cn/Article/details/gqseongla.sHtML

[D06] 数组长度
来源：http://blog.vehdjk.com/Article/details/gtdlabdog.sHtML

Py:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/gsiyyrqzh.sHtML

PHP:  count($arr);
来源：http://3g.bbcook.cn/Article/details/gepgsrbat.sHtML

JS:   arr.length
来源：http://3g.fktsv.cn/Article/details/gyvnzssag.sHtML

TS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gcmejspzs.sHtML

Java: list.size();
来源：http://wap.tarul.cn/Article/details/gpfcdgqlv.sHtML

Go:   len(arr)
来源：http://m.share.vehdjk.com/Article/details/gfiqdjuzd.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/gbdixbyte.sHtML

C#:   list.Count;
来源：http://baike.bbcook.cn/Article/details/gujajtelj.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fktsv.cn/Article/details/ggaqdmvuo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.epnwcf.com/Article/details/gsrxhmyvz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.epnwcf.com/Article/details/goyusnrjy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/glorjnxop.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gddjksybs.sHtML

Java: list.subList(1, 4);
来源：http://blog.tarul.cn/Article/details/gsqgkswmz.sHtML

Go:   arr[1:4]
来源：http://blog.bbcook.cn/Article/details/grubuckhi.sHtML

Ruby: arr[1, 3]
来源：http://m.share.yfazqb.com/Article/details/gaigjwrsm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.bbcook.cn/Article/details/gncrrxsyz.sHtML

[D08] 合并两个数组
来源：http://read.share.bbcook.cn/Article/details/grtubzkoq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.bbcook.cn/Article/details/gaekpwlhl.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.epnwcf.com/Article/details/glumpxkcd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fktsv.cn/Article/details/ghbzasuyi.sHtML

TS:   [...a, ...b];
来源：http://read.share.sjlbkw.cn/Article/details/grcjyqllv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.bbcook.cn/Article/details/gcriqxoir.sHtML

Go:   append(a, b...)
来源：http://blog.epnwcf.com/Article/details/gatbudlgb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.epnwcf.com/Article/details/gvfjwkaad.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.epnwcf.com/Article/details/gbkzetoxz.sHtML

[D09] 排序（升序）
来源：http://mobile.sjlbkw.cn/Article/details/gehbmvgqa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/gtujiagiy.sHtML

PHP:  sort($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gtmkdnorn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.bbcook.cn/Article/details/gwpqkfmfv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.tarul.cn/Article/details/guismrlpx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.tarul.cn/Article/details/giiobzxsd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gjocpxrcx.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/grbhrqvsu.sHtML

C#:   list.Sort();
来源：http://3g.vehdjk.com/Article/details/gddowgbvj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.epnwcf.com/Article/details/grkqioflk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.sjlbkw.cn/Article/details/gtgarmhqf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gmbgxhlzf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.sjlbkw.cn/Article/details/glupyolrj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/grirnankc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.epnwcf.com/Article/details/gwbvngzif.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/gvqyamivx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.bbcook.cn/Article/details/gbcxvloiq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fktsv.cn/Article/details/gatkxbmxv.sHtML

[D11] 反转数组
来源：http://www.share.bbcook.cn/Article/details/gxcurvrpb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/girkbuqnx.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.bbcook.cn/Article/details/guojhycff.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.sjlbkw.cn/Article/details/giqyqhiti.sHtML

TS:   [...arr].reverse();
来源：http://blog.tarul.cn/Article/details/gyhhmydsw.sHtML

Java: Collections.reverse(list);
来源：http://baike.vehdjk.com/Article/details/grwlhtqwl.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.epnwcf.com/Article/details/gxbgnqcie.sHtML

Ruby: arr.reverse
来源：http://blog.sjlbkw.cn/Article/details/golnemwoc.sHtML

C#:   list.Reverse();
来源：http://baike.yfazqb.com/Article/details/glptgcglo.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/gkymvjepe.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gclbdcakz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fktsv.cn/Article/details/gxoqbgjah.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.epnwcf.com/Article/details/gjinyuoal.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/grcyxrpbf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.yfazqb.com/Article/details/gugwxkczf.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fktsv.cn/Article/details/gvuvogbey.sHtML

Ruby: arr.index(x)
来源：http://blog.yfazqb.com/Article/details/ggkqcfyla.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.epnwcf.com/Article/details/gbohlvfod.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.tarul.cn/Article/details/gwlrqttqr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.vehdjk.com/Article/details/gsupjlhnl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.yfazqb.com/Article/details/gijtsqqqr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/guvcxpgfr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaiemldoc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.epnwcf.com/Article/details/galcbkqeu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fktsv.cn/Article/details/gmemeyzzd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.yfazqb.com/Article/details/gcydjaqbc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fktsv.cn/Article/details/gmqjsjwpo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/gortnjxhy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.sjlbkw.cn/Article/details/gmepwsrex.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.tarul.cn/Article/details/gegixokzm.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gggoilwdm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gzkrtfota.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.vehdjk.com/Article/details/gowwjihdw.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gsczapuql.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gejsggrzd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gieiqyznr.sHtML

[D15] 去重
来源：http://www.share.bbcook.cn/Article/details/gjmsxkwvj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gjpnbrxjn.sHtML

PHP:  array_unique($arr);
来源：http://www.share.tarul.cn/Article/details/gsrguvack.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/ghtwwszaj.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/grxqgpmwd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.bbcook.cn/Article/details/gyqygrwje.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.sjlbkw.cn/Article/details/grtlhgpdm.sHtML

Ruby: arr.uniq
来源：http://read.share.bbcook.cn/Article/details/gsekwntft.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fktsv.cn/Article/details/gblaxifmi.sHtML

[D16] 求和与平均值
来源：http://3g.sjlbkw.cn/Article/details/gdnfennvh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.tarul.cn/Article/details/gclthsivl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gdaafakpo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/gqbolbxqh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/gdmrtcoqz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fktsv.cn/Article/details/gcfultaom.sHtML

Go:   // 手写循环累加
来源：http://3g.vehdjk.com/Article/details/gbakrozed.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.yfazqb.com/Article/details/gbgtvxdey.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.sjlbkw.cn/Article/details/gmzfmkxhw.sHtML

[D17] 最大值与最小值
来源：http://wap.epnwcf.com/Article/details/gzcwyapmq.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fktsv.cn/Article/details/gvcnjulyr.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.vehdjk.com/Article/details/ghgvaupgf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.vehdjk.com/Article/details/gichnjrzc.sHtML

TS:   Math.max(...arr);
来源：http://wap.epnwcf.com/Article/details/gajzxwutp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gaznawfqh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.vehdjk.com/Article/details/gwpgqnpli.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.tarul.cn/Article/details/gsiefziig.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.yfazqb.com/Article/details/gaxjjgqvi.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fktsv.cn/Article/details/gxlqqjhdz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fktsv.cn/Article/details/gcccauobw.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/guswrnpid.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/gezqvkdcr.sHtML

TS:   nested.flat();
来源：http://baike.bbcook.cn/Article/details/ghzhkpwqk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.sjlbkw.cn/Article/details/gptnebyib.sHtML

Go:   // 手写双层循环
来源：http://wap.sjlbkw.cn/Article/details/gwjlkiobo.sHtML

Ruby: nested.flatten
来源：http://mobile.epnwcf.com/Article/details/gusovgfue.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.epnwcf.com/Article/details/greaaoujw.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/geugrxkqs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.vehdjk.com/Article/details/gcnrdwpnl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.bbcook.cn/Article/details/gywcdgvyk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.tarul.cn/Article/details/gvcdlghxf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhcyosxp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/ghftvetwy.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.epnwcf.com/Article/details/gtpudisqz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.yfazqb.com/Article/details/gydzuibke.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.epnwcf.com/Article/details/gyekotraf.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.bbcook.cn/Article/details/gbwlngexp.sHtML

Py:   Counter(arr)
来源：http://www.m.share.epnwcf.com/Article/details/guxtergcy.sHtML

PHP:  array_count_values($arr);
来源：http://baike.vehdjk.com/Article/details/glpfebihq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/gnrpnajdk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gimferzfx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.epnwcf.com/Article/details/giqrcwqsm.sHtML

Go:   // 手写 map[T]int
来源：http://baike.bbcook.cn/Article/details/gugefcfdj.sHtML

Ruby: arr.tally
来源：http://read.share.epnwcf.com/Article/details/ghmgotbfp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.vehdjk.com/Article/details/gqpffntpm.sHtML

[D21] 判断是否包含某元素
来源：http://blog.sjlbkw.cn/Article/details/ggjbqoiop.sHtML

Py:   x in arr
来源：http://blog.tarul.cn/Article/details/gpabgingc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.tarul.cn/Article/details/gourarnme.sHtML

JS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gwidahcmw.sHtML

TS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/grdiudnfz.sHtML

Java: list.contains(x)
来源：http://baike.epnwcf.com/Article/details/gbjmmgvyb.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gwsypjtdn.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/gfvgsttzp.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gjldkatyh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.sjlbkw.cn/Article/details/gqadxykpc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.vehdjk.com/Article/details/ghhcdshcn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.sjlbkw.cn/Article/details/gsfojshwt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.tarul.cn/Article/details/gzybbpgig.sHtML

TS:   [...arr];
来源：http://m.share.sjlbkw.cn/Article/details/grjwpcgij.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.bbcook.cn/Article/details/gzgjrjhhk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gbokjzxfw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.sjlbkw.cn/Article/details/gtcfswqyp.sHtML

C#:   new List<int>(list);
来源：http://baike.fktsv.cn/Article/details/gbnfxpquz.sHtML

[D23] reduce 累积计算
来源：http://www.blog.sjlbkw.cn/Article/details/gnnxiziwb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdqiyhze.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/gbkzanfey.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/groardxal.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gmnrhuirg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fktsv.cn/Article/details/guyaetvqf.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gblgniyvk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fktsv.cn/Article/details/gqhdpyjko.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.yfazqb.com/Article/details/gpbsnnxbj.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.bbcook.cn/Article/details/gmlunwakt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fktsv.cn/Article/details/gqpafkocz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.sjlbkw.cn/Article/details/gwrokrfvd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.sjlbkw.cn/Article/details/gyfkbqvsd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gowouqdyv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.vehdjk.com/Article/details/grynthpct.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fktsv.cn/Article/details/gpvxmafzq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fktsv.cn/Article/details/gibrudvah.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.epnwcf.com/Article/details/gvjxeoesy.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.vehdjk.com/Article/details/glbxicqcw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.epnwcf.com/Article/details/gosldiwvn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.yfazqb.com/Article/details/gcasucujf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.epnwcf.com/Article/details/gqdwupgvg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.vehdjk.com/Article/details/gvpqsaiaa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.bbcook.cn/Article/details/gjkyfzwvh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.sjlbkw.cn/Article/details/ggktcqlkq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.yfazqb.com/Article/details/ghrzauylm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gswnbfijz.sHtML

[D26] 数组转字符串
来源：http://wap.tarul.cn/Article/details/ggvcublia.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.sjlbkw.cn/Article/details/gooutanlg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/gyktiagae.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/ggcidoeli.sHtML

TS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/guedbiywl.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gsuadnpqr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.yfazqb.com/Article/details/gohssvbfp.sHtML

Ruby: arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gboheltyc.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.yfazqb.com/Article/details/gbcwvvopx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvtmbgbui.sHtML

E. 字符串处理
来源：http://3g.bbcook.cn/Article/details/gmpknjaaw.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gkpdezzvo.sHtML

[E01] 拼接字符串
来源：http://read.share.tarul.cn/Article/details/gptzvmdsb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.bbcook.cn/Article/details/gauxthnvb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/gypcxtalr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/gusndjycz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/gbwyjyjmi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/grsooorle.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fktsv.cn/Article/details/gnhyipbbs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.yfazqb.com/Article/details/gfdnshwop.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.epnwcf.com/Article/details/glcewawzf.sHtML

[E02] 重复字符串
来源：http://www.blog.tarul.cn/Article/details/gtjajorlw.sHtML

Py:   "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/gogopcgww.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.yfazqb.com/Article/details/gcrusfcem.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/ghlywimvm.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gahsbwrfj.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gvqxhbqha.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fktsv.cn/Article/details/ghmosgndj.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gviylwbyt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gheugyamp.sHtML

[E03] 截取子串
来源：http://3g.bbcook.cn/Article/details/gjnxpqtgy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.tarul.cn/Article/details/gznesofex.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gszyonfti.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gneucbfch.sHtML

TS:   s.slice(1, 4)
来源：http://3g.epnwcf.com/Article/details/ggjrkxeni.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gphrhxehd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.epnwcf.com/Article/details/gzytusvrv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/gtapftsxa.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.yfazqb.com/Article/details/gdqnqjofq.sHtML

[E04] 查找子串位置
来源：http://3g.tarul.cn/Article/details/gnukypehx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gdimqccnw.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.epnwcf.com/Article/details/gmahbyemg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.bbcook.cn/Article/details/gdkohuhfu.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gidtyilnm.sHtML

Java: s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/grpgyyywo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.bbcook.cn/Article/details/goufcgsxy.sHtML

Ruby: s.index("x")
来源：http://mobile.fktsv.cn/Article/details/ggsmklxah.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gulnwzmex.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.epnwcf.com/Article/details/gzvjrdels.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.vehdjk.com/Article/details/gqryqrcur.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.epnwcf.com/Article/details/ghjlwjqyc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gtysoouti.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.epnwcf.com/Article/details/gizfwexkw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gobaxojfq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.tarul.cn/Article/details/gewxuuzuy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.bbcook.cn/Article/details/gudhwubru.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.vehdjk.com/Article/details/gyulzoyaj.sHtML

[E06] 替换子串
来源：http://baike.fktsv.cn/Article/details/gedohwrme.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gukmvmxwu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.tarul.cn/Article/details/gaztwwfky.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gifizjhse.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/glcgfvscp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/goebaqpio.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gjpzlmhsi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gcytlgrhs.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gynlrymvh.sHtML

[E07] 按分隔符拆分
来源：http://baike.tarul.cn/Article/details/gppkdofkl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.epnwcf.com/Article/details/gvsbvozyd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/grfyjpjba.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.bbcook.cn/Article/details/googvskln.sHtML

TS:   s.split(",")
来源：http://blog.sjlbkw.cn/Article/details/gvefzvdyk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fktsv.cn/Article/details/gojvgdbnv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fktsv.cn/Article/details/guqovxbzl.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.epnwcf.com/Article/details/gfveleyzk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.bbcook.cn/Article/details/gyywydeyn.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.bbcook.cn/Article/details/gpgxeccjc.sHtML

Py:   ",".join(items)
来源：http://baike.bbcook.cn/Article/details/gftgwpaek.sHtML


<!-- 参考信息 -->