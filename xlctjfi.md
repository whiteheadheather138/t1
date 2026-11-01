代发 wailian999

C#:   list.Insert(0, 0);
来源：http://m.share.vehdjk.com/Article/details/gjymiwqqv.sHtML

[D04] 删除元素
来源：http://mobile.vehdjk.com/Article/details/gmqrmotfb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.bbcook.cn/Article/details/gbfaxgdch.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.vehdjk.com/Article/details/gzujrdlqy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.yfazqb.com/Article/details/giwgtdhhh.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/gmxsusddk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.sjlbkw.cn/Article/details/gzdszzpvh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.yfazqb.com/Article/details/gvdgskuen.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.vehdjk.com/Article/details/ghgintpsx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fktsv.cn/Article/details/gypgzaybu.sHtML

[D05] 访问与修改元素
来源：http://read.share.sjlbkw.cn/Article/details/gyiupilhp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gfwwlrher.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gxxjofesn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gbgzwciof.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.tarul.cn/Article/details/gclxhosko.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.sjlbkw.cn/Article/details/gaiugmyqs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gxwgewhsg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gxsvuduwi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gkvhhwgha.sHtML

[D06] 数组长度
来源：http://baike.bbcook.cn/Article/details/gxyglmvea.sHtML

Py:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gitwuepxg.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gfgltvzye.sHtML

JS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/ggurgavuk.sHtML

TS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gzvuiwllj.sHtML

Java: list.size();
来源：http://blog.epnwcf.com/Article/details/gtekzajxv.sHtML

Go:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gjittjxpf.sHtML

Ruby: arr.length; arr.size
来源：http://3g.yfazqb.com/Article/details/guyhqyijs.sHtML

C#:   list.Count;
来源：http://www.m.share.bbcook.cn/Article/details/ghsvdxzbl.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.bbcook.cn/Article/details/gzbipswnd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/gmhyopsbi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.tarul.cn/Article/details/gjychccvt.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/grdgnhnuc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gmecptuyh.sHtML

Java: list.subList(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gupohujia.sHtML

Go:   arr[1:4]
来源：http://mobile.yfazqb.com/Article/details/ghqigijgs.sHtML

Ruby: arr[1, 3]
来源：http://wap.bbcook.cn/Article/details/gkkgpoaxu.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.yfazqb.com/Article/details/gsbjchlxe.sHtML

[D08] 合并两个数组
来源：http://www.blog.tarul.cn/Article/details/gqrqorcxs.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.yfazqb.com/Article/details/ghttshbaw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.tarul.cn/Article/details/gxcoylhcr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.yfazqb.com/Article/details/gnorfgnuo.sHtML

TS:   [...a, ...b];
来源：http://www.share.yfazqb.com/Article/details/goezdxaia.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.yfazqb.com/Article/details/gnhxzhaip.sHtML

Go:   append(a, b...)
来源：http://www.share.vehdjk.com/Article/details/gmbyvfskl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.epnwcf.com/Article/details/gwipwvdgd.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.tarul.cn/Article/details/gcqjsdeqm.sHtML

[D09] 排序（升序）
来源：http://baike.vehdjk.com/Article/details/gujowtzzi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/grnvuukfz.sHtML

PHP:  sort($arr);
来源：http://www.share.bbcook.cn/Article/details/gjxknutlr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.yfazqb.com/Article/details/gwbwbbdto.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.epnwcf.com/Article/details/gdagwmbam.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.bbcook.cn/Article/details/gtwplumtl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gqjuzwbai.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/gdgmcjirh.sHtML

C#:   list.Sort();
来源：http://www.share.yfazqb.com/Article/details/ghnglxqjc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fktsv.cn/Article/details/gcqxdgvep.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.epnwcf.com/Article/details/gtpdights.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gegnglvdu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/gbebjamgr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gikrgqqgt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.tarul.cn/Article/details/gctuzpxda.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.sjlbkw.cn/Article/details/guyqxnoow.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqybkznpm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fktsv.cn/Article/details/gwivzsozn.sHtML

[D11] 反转数组
来源：http://read.share.bbcook.cn/Article/details/gxvpacbht.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.yfazqb.com/Article/details/gwanlpnwp.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.vehdjk.com/Article/details/gkuxdbbig.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.sjlbkw.cn/Article/details/gstzkreji.sHtML

TS:   [...arr].reverse();
来源：http://3g.epnwcf.com/Article/details/gaibbpzxv.sHtML

Java: Collections.reverse(list);
来源：http://baike.yfazqb.com/Article/details/glyrrsobd.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.tarul.cn/Article/details/ggyjlnoqn.sHtML

Ruby: arr.reverse
来源：http://blog.tarul.cn/Article/details/gxuztsscu.sHtML

C#:   list.Reverse();
来源：http://read.share.epnwcf.com/Article/details/gebnlahny.sHtML

[D12] 查找元素下标
来源：http://wap.epnwcf.com/Article/details/grgzquyzk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmzaccpp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.epnwcf.com/Article/details/gbbumvrni.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gerkczvno.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gwxdnmbnj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.sjlbkw.cn/Article/details/gpoehmdpd.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.bbcook.cn/Article/details/gukpcpneg.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/guqwkdleq.sHtML

C#:   list.IndexOf(x);
来源：http://3g.epnwcf.com/Article/details/gccixtzne.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.bbcook.cn/Article/details/glbkccgik.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.tarul.cn/Article/details/gmarfshhv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.epnwcf.com/Article/details/gmvpwtpre.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gnxlocsfq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gkckehqyg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.sjlbkw.cn/Article/details/gdxorrmmv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gdiozotdo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.bbcook.cn/Article/details/gyayicyqn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gfgmxvblv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.bbcook.cn/Article/details/gyhghveak.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.sjlbkw.cn/Article/details/gmdmrouhf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.tarul.cn/Article/details/gzxrghvmq.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gqpsiizbr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/gudpfrdqm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.bbcook.cn/Article/details/gsqwesozr.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gzblarmqm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/genasuwbc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gysxtkryl.sHtML

[D15] 去重
来源：http://blog.tarul.cn/Article/details/gsjxrkeum.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/gzfuskuqp.sHtML

PHP:  array_unique($arr);
来源：http://m.share.yfazqb.com/Article/details/gtttznpmx.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gbjfgoqdv.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gafnhpyoa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.vehdjk.com/Article/details/gvgqkbfyn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.yfazqb.com/Article/details/gkvmxcpwo.sHtML

Ruby: arr.uniq
来源：http://www.m.share.sjlbkw.cn/Article/details/gczwbkmkf.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.sjlbkw.cn/Article/details/glmkhteqr.sHtML

[D16] 求和与平均值
来源：http://baike.tarul.cn/Article/details/ggvawzknb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.vehdjk.com/Article/details/ggnphzrdr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.tarul.cn/Article/details/gbvbyqkug.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.yfazqb.com/Article/details/gjvlgvzlh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/grrjqstax.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fktsv.cn/Article/details/gisgykhmm.sHtML

Go:   // 手写循环累加
来源：http://baike.bbcook.cn/Article/details/gouxfrnno.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.bbcook.cn/Article/details/gwxtsmxlz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fktsv.cn/Article/details/gccyfaxug.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.bbcook.cn/Article/details/gqelkfann.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.bbcook.cn/Article/details/gummbawwx.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.vehdjk.com/Article/details/gnvcsqwbf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.epnwcf.com/Article/details/gipqfyntv.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fktsv.cn/Article/details/gphdbisvs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.epnwcf.com/Article/details/gjncfeowp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fktsv.cn/Article/details/gljgvlebj.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.yfazqb.com/Article/details/guytcwlrq.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.bbcook.cn/Article/details/gtjwrhopo.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.vehdjk.com/Article/details/gluhffyhc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.vehdjk.com/Article/details/gxhchcmrk.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gvdxqkusj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.sjlbkw.cn/Article/details/glxstyijk.sHtML

TS:   nested.flat();
来源：http://blog.tarul.cn/Article/details/gwjpxamll.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.epnwcf.com/Article/details/giskzhlfb.sHtML

Go:   // 手写双层循环
来源：http://blog.epnwcf.com/Article/details/gqvaghemr.sHtML

Ruby: nested.flatten
来源：http://blog.epnwcf.com/Article/details/gduxltili.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.tarul.cn/Article/details/gjpzkbajv.sHtML

[D19] 按字段分组
来源：http://blog.tarul.cn/Article/details/gzhhrmtvc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/gsnjbnhgb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.epnwcf.com/Article/details/gfgrmjlec.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.vehdjk.com/Article/details/gnhpystrf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gkaqztuhz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.bbcook.cn/Article/details/gqtikyyko.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.tarul.cn/Article/details/gxjrjgajc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gluhlnvhj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fktsv.cn/Article/details/gxvgkiucs.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.epnwcf.com/Article/details/gzoqhabhv.sHtML

Py:   Counter(arr)
来源：http://m.share.vehdjk.com/Article/details/ggobjxmde.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.tarul.cn/Article/details/geacnkjzm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gufvzethq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/gfnghxped.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.tarul.cn/Article/details/gyqlhcfev.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/guaffefwv.sHtML

Ruby: arr.tally
来源：http://baike.vehdjk.com/Article/details/gluvleovm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/ghrrgqkrd.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/guwvvtqmz.sHtML

Py:   x in arr
来源：http://mobile.tarul.cn/Article/details/gxzjpingi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.vehdjk.com/Article/details/gydbfgvna.sHtML

JS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/govqmcgta.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gecfmuncv.sHtML

Java: list.contains(x)
来源：http://m.share.yfazqb.com/Article/details/ghtgxyitr.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gfzlaqvse.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/grlszsvnx.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/grkimntzj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.tarul.cn/Article/details/glcyriuxm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.epnwcf.com/Article/details/goljpaums.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnachhcv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fktsv.cn/Article/details/gjqvasjqw.sHtML

TS:   [...arr];
来源：http://www.share.vehdjk.com/Article/details/ggzrkplhy.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.bbcook.cn/Article/details/gdiihyzkc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.bbcook.cn/Article/details/galehpxun.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.vehdjk.com/Article/details/gmkxuywhg.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gyesnqnru.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/gexyvnnfq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/gxrzgawwk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gnevpjqmm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gmruhwirl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gwkdkcveo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.tarul.cn/Article/details/ghmyndmhn.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/gorxcesjn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.vehdjk.com/Article/details/gfpplyefn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.yfazqb.com/Article/details/gemljfvcu.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.bbcook.cn/Article/details/gjjytgkpf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gqbhvtijs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.epnwcf.com/Article/details/gdnndjtzx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.bbcook.cn/Article/details/gnsrqivyx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gnwcrdumi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.epnwcf.com/Article/details/gpzggloae.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.yfazqb.com/Article/details/geavgicie.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.yfazqb.com/Article/details/glolgaeil.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.epnwcf.com/Article/details/gpktnelms.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/gmefziiaq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.vehdjk.com/Article/details/gnzncvthn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.sjlbkw.cn/Article/details/goyvhyhfx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.sjlbkw.cn/Article/details/gzfkktbfb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.sjlbkw.cn/Article/details/googlekxv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.tarul.cn/Article/details/gxhprfadn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.yfazqb.com/Article/details/gaaihmocl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.yfazqb.com/Article/details/ggberdtmc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gzmcjpbbj.sHtML

[D26] 数组转字符串
来源：http://www.blog.vehdjk.com/Article/details/gsfzcwiml.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gtockiepd.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.yfazqb.com/Article/details/gfksxjtls.sHtML

JS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gzfkcjqiy.sHtML

TS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gbmjnluxd.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/gkqnmgtqa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.sjlbkw.cn/Article/details/geterzeps.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/ggenkrwbi.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gtdlvrxnj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvmwliimj.sHtML

E. 字符串处理
来源：http://wap.vehdjk.com/Article/details/gxapeyvob.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gyfwxnrca.sHtML

[E01] 拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gpjspabig.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.sjlbkw.cn/Article/details/ghhgcmibq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.vehdjk.com/Article/details/gtfeexzrk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gtztzyhrk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gkltrethz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.sjlbkw.cn/Article/details/gkonoubbb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.vehdjk.com/Article/details/glljnxone.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.sjlbkw.cn/Article/details/gutauemuh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.epnwcf.com/Article/details/glpuphzbj.sHtML

[E02] 重复字符串
来源：http://m.share.vehdjk.com/Article/details/geukdyejm.sHtML

Py:   "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gnwajsqhy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fktsv.cn/Article/details/gxhajvckl.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gojfounwe.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gubmtocva.sHtML

Java: "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gfrgmlhoy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fktsv.cn/Article/details/gjjjwjntt.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gcnoavjhs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.vehdjk.com/Article/details/gescajmji.sHtML

[E03] 截取子串
来源：http://baike.fktsv.cn/Article/details/gjuluoelb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/gimxhvspg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gynmcrcxr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/ggetsrwns.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gfrzcbzjq.sHtML

Java: s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gfhgzkdfo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gafiirryd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fktsv.cn/Article/details/gukteqxkm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.epnwcf.com/Article/details/gjxsdctcf.sHtML

[E04] 查找子串位置
来源：http://www.share.epnwcf.com/Article/details/gqgumfnyv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/gonizmuqk.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fktsv.cn/Article/details/guqcrwdvq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/gbryptyfb.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gwrfvobij.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gdagwaout.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.sjlbkw.cn/Article/details/gafsqcxbf.sHtML

Ruby: s.index("x")
来源：http://3g.tarul.cn/Article/details/ghxjkfxlz.sHtML

C#:   s.IndexOf("x")
来源：http://wap.epnwcf.com/Article/details/gzvnmhfsl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.vehdjk.com/Article/details/gkudgumal.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.vehdjk.com/Article/details/grcbkjlwp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.sjlbkw.cn/Article/details/gnihsazkd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/gxnctzvyb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.tarul.cn/Article/details/gpbpofxpg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gfqyyyicn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/gyaootqtz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fktsv.cn/Article/details/gmagqahkk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gczrhsbji.sHtML

[E06] 替换子串
来源：http://read.share.sjlbkw.cn/Article/details/grukzbyxp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gucxbgqpu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.bbcook.cn/Article/details/gnijadudy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gzadmgjei.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gfjirojhl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gspswydrr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gadanrxmq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/geuucrfot.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gkuykztom.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.vehdjk.com/Article/details/gdmvlejqp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.tarul.cn/Article/details/gjdfvwpzi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmreqmgy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fktsv.cn/Article/details/gpsaggoty.sHtML

TS:   s.split(",")
来源：http://mobile.tarul.cn/Article/details/gfkqtobum.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.vehdjk.com/Article/details/gyjegjdoo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/glcgozqhg.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.vehdjk.com/Article/details/ggpkidsir.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.tarul.cn/Article/details/gtdttlpjm.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/gmfexdswx.sHtML

Py:   ",".join(items)
来源：http://baike.fktsv.cn/Article/details/gtkdzcxcc.sHtML

PHP:  implode(",", $items);
来源：http://blog.fktsv.cn/Article/details/gfjtoraqx.sHtML

JS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaztcssjp.sHtML

TS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gztjlscvw.sHtML

Java: String.join(",", items)
来源：http://blog.tarul.cn/Article/details/gmtghzvdr.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fktsv.cn/Article/details/gtbiopayb.sHtML

Ruby: items.join(",")
来源：http://3g.yfazqb.com/Article/details/gakawlptq.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gdsbrxmcw.sHtML

[E09] 去除所有空白字符
来源：http://read.share.tarul.cn/Article/details/gjflpzmnv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.epnwcf.com/Article/details/gtxsmdwhn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.sjlbkw.cn/Article/details/guloawysh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/guvwykbpy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gfchstyae.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gsxsfwzxj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.vehdjk.com/Article/details/gaxqmqwuk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.vehdjk.com/Article/details/grdmsdooo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gguhrzdoz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.bbcook.cn/Article/details/gomahdchx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gcrnzhahz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.bbcook.cn/Article/details/ghhfxrfte.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gnpfwbevs.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gfmfdbewy.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gxnbdxvhi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gsxrqnqul.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/grcigivys.sHtML


<!-- 参考信息 -->