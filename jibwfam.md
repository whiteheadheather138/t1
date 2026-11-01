代发 wailian999

C#:   list.Insert(0, 0);
来源：http://read.share.vehdjk.com/Article/details/gwibtofrw.sHtML

[D04] 删除元素
来源：http://baike.yfazqb.com/Article/details/gegufrjjg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.sjlbkw.cn/Article/details/gmsbdcaqc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsadbgclw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fktsv.cn/Article/details/gungatvrz.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.sjlbkw.cn/Article/details/gjbswyjfg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.sjlbkw.cn/Article/details/gdzrngfbl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.sjlbkw.cn/Article/details/gmqvztgjl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fktsv.cn/Article/details/giqebgdfu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.sjlbkw.cn/Article/details/gmhdleiwj.sHtML

[D05] 访问与修改元素
来源：http://3g.epnwcf.com/Article/details/ghfmpdjhc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gtydnizov.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gwggkolpl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gpdsrjsvy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gmaqvniwb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.tarul.cn/Article/details/gfzkshyir.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/ggjzhwjhh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/gmddmcjsq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gkbcewswv.sHtML

[D06] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gwbkacwcn.sHtML

Py:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gxmwbsafy.sHtML

PHP:  count($arr);
来源：http://www.blog.tarul.cn/Article/details/gpusaqcgz.sHtML

JS:   arr.length
来源：http://3g.sjlbkw.cn/Article/details/ghvispvnm.sHtML

TS:   arr.length
来源：http://blog.fktsv.cn/Article/details/gyfgfexly.sHtML

Java: list.size();
来源：http://baike.yfazqb.com/Article/details/gvcorvzpo.sHtML

Go:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gwtwxkqhj.sHtML

Ruby: arr.length; arr.size
来源：http://wap.yfazqb.com/Article/details/gvoabkrlv.sHtML

C#:   list.Count;
来源：http://m.share.bbcook.cn/Article/details/gxlwmtqfn.sHtML

[D07] 切片 / 取子数组
来源：http://wap.vehdjk.com/Article/details/gngfxdiez.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.sjlbkw.cn/Article/details/gbjmxhhjd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.sjlbkw.cn/Article/details/gyrqfnwlk.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.tarul.cn/Article/details/gdrtlaaxf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gnvwudbou.sHtML

Java: list.subList(1, 4);
来源：http://blog.fktsv.cn/Article/details/ghvltlfjs.sHtML

Go:   arr[1:4]
来源：http://m.share.bbcook.cn/Article/details/gejnhjyfc.sHtML

Ruby: arr[1, 3]
来源：http://blog.yfazqb.com/Article/details/greayxxdl.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.vehdjk.com/Article/details/gljeyiocd.sHtML

[D08] 合并两个数组
来源：http://read.share.sjlbkw.cn/Article/details/gnvbnfbbt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.tarul.cn/Article/details/gwyvdysyh.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fktsv.cn/Article/details/gqforzifq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.yfazqb.com/Article/details/gleqkjxul.sHtML

TS:   [...a, ...b];
来源：http://www.share.vehdjk.com/Article/details/gcagqjacw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.sjlbkw.cn/Article/details/grcwcxqds.sHtML

Go:   append(a, b...)
来源：http://blog.vehdjk.com/Article/details/gxtinzwhq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gjlkshsjw.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.bbcook.cn/Article/details/gjcdxwarr.sHtML

[D09] 排序（升序）
来源：http://blog.yfazqb.com/Article/details/gianwmbll.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/gcbptxhdt.sHtML

PHP:  sort($arr);
来源：http://mobile.vehdjk.com/Article/details/gcaxkbszp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.tarul.cn/Article/details/gpflscdia.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.epnwcf.com/Article/details/gzzfuujoc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.tarul.cn/Article/details/gxxxqxcoe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gnwaonexe.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gvjvsqoyi.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/gzzfzivvp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.yfazqb.com/Article/details/gcgfhpqtz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.tarul.cn/Article/details/gzznvcncv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gasvxlkcn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/giihxrwtz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.vehdjk.com/Article/details/gaiadupqo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.epnwcf.com/Article/details/gjqcgdnrb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.tarul.cn/Article/details/grvdtuayz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.yfazqb.com/Article/details/gvlvxuzpo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.yfazqb.com/Article/details/gcktnwzso.sHtML

[D11] 反转数组
来源：http://www.blog.tarul.cn/Article/details/glnwuicft.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.yfazqb.com/Article/details/gaockijip.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gqpjxmsur.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.sjlbkw.cn/Article/details/gokevogqy.sHtML

TS:   [...arr].reverse();
来源：http://3g.vehdjk.com/Article/details/gmndniwyz.sHtML

Java: Collections.reverse(list);
来源：http://mobile.vehdjk.com/Article/details/gcenmoikg.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.yfazqb.com/Article/details/grdzlqtqc.sHtML

Ruby: arr.reverse
来源：http://blog.tarul.cn/Article/details/gnuslsiji.sHtML

C#:   list.Reverse();
来源：http://www.blog.epnwcf.com/Article/details/gljslpliq.sHtML

[D12] 查找元素下标
来源：http://m.share.vehdjk.com/Article/details/gtqzlvcdc.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.bbcook.cn/Article/details/gsrzezhrr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gkmvqddob.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gqqnfamju.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/gqsyufpxg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/glpwatdst.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.tarul.cn/Article/details/gjvswfkbn.sHtML

Ruby: arr.index(x)
来源：http://wap.yfazqb.com/Article/details/gswzgbuym.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/ggrhnanic.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/gtcrcdhbz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.sjlbkw.cn/Article/details/gfkepiyyj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.bbcook.cn/Article/details/gzmfopeqb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gbrhmksev.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/gbeforjjr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.tarul.cn/Article/details/ggnkcdznp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.tarul.cn/Article/details/gcdbowhip.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.sjlbkw.cn/Article/details/gqzhridlc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.tarul.cn/Article/details/gphockhnx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.bbcook.cn/Article/details/gyzahpuct.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.sjlbkw.cn/Article/details/ggxxghirp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.yfazqb.com/Article/details/gxkfxfaqb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gglunzqul.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.vehdjk.com/Article/details/gkkmtciqm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.vehdjk.com/Article/details/godzafswg.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gwbhojwpw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gbfzngdaa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fktsv.cn/Article/details/gffozwafx.sHtML

[D15] 去重
来源：http://mobile.vehdjk.com/Article/details/goanwuivr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.vehdjk.com/Article/details/gylsznodl.sHtML

PHP:  array_unique($arr);
来源：http://baike.vehdjk.com/Article/details/guuwzhgbl.sHtML

JS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gfxtbngoh.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/gwbkmfqpg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fktsv.cn/Article/details/gsjlbriyp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.tarul.cn/Article/details/gtuayzfnm.sHtML

Ruby: arr.uniq
来源：http://mobile.epnwcf.com/Article/details/gkedqdrsl.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.tarul.cn/Article/details/gukmleuiw.sHtML

[D16] 求和与平均值
来源：http://mobile.fktsv.cn/Article/details/gpmisuyhw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.yfazqb.com/Article/details/gutzchakl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gnucyrqcy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gidbcayxz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gjayntsnj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.tarul.cn/Article/details/gxowicfhg.sHtML

Go:   // 手写循环累加
来源：http://www.share.sjlbkw.cn/Article/details/gssxobqha.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/gzgvoukai.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.yfazqb.com/Article/details/gngtppycl.sHtML

[D17] 最大值与最小值
来源：http://m.share.sjlbkw.cn/Article/details/gsnjgdueu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.tarul.cn/Article/details/gkwktlyjj.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.sjlbkw.cn/Article/details/gqmplyqrq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.vehdjk.com/Article/details/gphjvsyhq.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fktsv.cn/Article/details/ghnzuagxi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.sjlbkw.cn/Article/details/gpdsmhlso.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gdmbrscah.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.vehdjk.com/Article/details/gpobcawkr.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fktsv.cn/Article/details/gqwngzspo.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.vehdjk.com/Article/details/gcvtdfxaq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.vehdjk.com/Article/details/gibuufhzp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.tarul.cn/Article/details/gnnkbotsv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.bbcook.cn/Article/details/gbikqblgt.sHtML

TS:   nested.flat();
来源：http://baike.vehdjk.com/Article/details/gqgbaqvoi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.vehdjk.com/Article/details/gxjvxjrpk.sHtML

Go:   // 手写双层循环
来源：http://www.share.bbcook.cn/Article/details/gsnpvwtva.sHtML

Ruby: nested.flatten
来源：http://read.share.tarul.cn/Article/details/gcywmoomq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gdyygqmri.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/gxxgfuolp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.tarul.cn/Article/details/gnxtelttq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gtbovoxpz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.vehdjk.com/Article/details/gbkdhvnfl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/gfpjsbngr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.yfazqb.com/Article/details/gohyoeowo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/gkqlcftgs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.bbcook.cn/Article/details/gdtcsoamk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/gloezjcet.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.epnwcf.com/Article/details/gdqiovydm.sHtML

Py:   Counter(arr)
来源：http://www.blog.yfazqb.com/Article/details/gsqcorxsg.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.yfazqb.com/Article/details/gfvzwtodp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gjyqlezwe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/guarntnkp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fktsv.cn/Article/details/gbvvspssc.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/gpybqbatw.sHtML

Ruby: arr.tally
来源：http://baike.bbcook.cn/Article/details/gmtsirqix.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.tarul.cn/Article/details/gawzsafwg.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/gubrvanfu.sHtML

Py:   x in arr
来源：http://read.share.vehdjk.com/Article/details/gxeyvzrxj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.yfazqb.com/Article/details/gyuokkcvx.sHtML

JS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/gcqmzrtvz.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/glgjnqlbh.sHtML

Java: list.contains(x)
来源：http://m.share.yfazqb.com/Article/details/ghlwvfnbz.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gebceotfh.sHtML

Ruby: arr.include?(x)
来源：http://3g.epnwcf.com/Article/details/gysbismnl.sHtML

C#:   list.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gwmvloolc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.epnwcf.com/Article/details/ghtxyxuyy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.vehdjk.com/Article/details/goodvzyft.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.sjlbkw.cn/Article/details/gvnxajlvo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fktsv.cn/Article/details/gotptieqo.sHtML

TS:   [...arr];
来源：http://3g.yfazqb.com/Article/details/gvrzzvmpl.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.tarul.cn/Article/details/gjntoezjz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gxwqgfanm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.bbcook.cn/Article/details/gqomzryqb.sHtML

C#:   new List<int>(list);
来源：http://3g.bbcook.cn/Article/details/gazhkewjr.sHtML

[D23] reduce 累积计算
来源：http://blog.yfazqb.com/Article/details/gxesucenb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.tarul.cn/Article/details/gwachkqdg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgbpxunq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gcfhmidzc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gnoxbpezn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.bbcook.cn/Article/details/gajxirlwv.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gkuoqqhhw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.sjlbkw.cn/Article/details/gyqtxpebb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.epnwcf.com/Article/details/gxvrcnzps.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fktsv.cn/Article/details/ghexdnfrs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gcdqbgeil.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.sjlbkw.cn/Article/details/gpltdlafu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.tarul.cn/Article/details/gswjpxpjc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.epnwcf.com/Article/details/gphsyrfpu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.vehdjk.com/Article/details/goxxroiaa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.vehdjk.com/Article/details/gmqvphdhz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.epnwcf.com/Article/details/gplhandbc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.yfazqb.com/Article/details/gkkdkpurh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/gtkzixjxn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.vehdjk.com/Article/details/gpxlkisih.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.sjlbkw.cn/Article/details/ghkojantd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fktsv.cn/Article/details/gtkttlvmy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.bbcook.cn/Article/details/gpoehsqoa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/gcvyaxiqt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.bbcook.cn/Article/details/gdmeozziw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.bbcook.cn/Article/details/gjuaujpxo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/ghojichnn.sHtML

[D26] 数组转字符串
来源：http://read.share.bbcook.cn/Article/details/gvnuncnob.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.bbcook.cn/Article/details/gthwtkgep.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.yfazqb.com/Article/details/gitpyifrb.sHtML

JS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/grsxcwxiz.sHtML

TS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/ggblxremk.sHtML

Java: String.join(", ", list)
来源：http://www.blog.bbcook.cn/Article/details/gzvxovhtr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.bbcook.cn/Article/details/glsgfnoju.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gklhydjve.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.yfazqb.com/Article/details/gbmwbdeny.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gkmqbkmug.sHtML

E. 字符串处理
来源：http://mobile.fktsv.cn/Article/details/gpekmkioo.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gldxbuujj.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gixzzzlnb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.yfazqb.com/Article/details/gfrkcgpcm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.vehdjk.com/Article/details/gneknhspe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gugoysydv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gangcsegm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/gmbxwgkkf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.bbcook.cn/Article/details/gnmwdxaon.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.epnwcf.com/Article/details/gbxetbojh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/guaktvmfc.sHtML

[E02] 重复字符串
来源：http://wap.yfazqb.com/Article/details/gutirwkuk.sHtML

Py:   "ab" * 3
来源：http://wap.bbcook.cn/Article/details/glyirdltb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.bbcook.cn/Article/details/gtzuubggc.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gmzsiucag.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gbeyfobht.sHtML

Java: "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gqnlvbvgj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/gszqbdbnz.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gucfmfjjb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.epnwcf.com/Article/details/golwjnass.sHtML

[E03] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gftlkzrei.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.tarul.cn/Article/details/glooigves.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gbaqzojhx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gkmjhjdxf.sHtML

TS:   s.slice(1, 4)
来源：http://wap.bbcook.cn/Article/details/gijeylyfi.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/guklcvsjp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/grohzldmy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fktsv.cn/Article/details/gjzijdcvk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.bbcook.cn/Article/details/gytihfeuz.sHtML

[E04] 查找子串位置
来源：http://blog.tarul.cn/Article/details/gkexkgvla.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/grfeegjqe.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.yfazqb.com/Article/details/gasctuwtg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/gxvltuzxf.sHtML

TS:   s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gqjjyiyxq.sHtML

Java: s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gkhqckfwz.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.epnwcf.com/Article/details/guonbqdok.sHtML

Ruby: s.index("x")
来源：http://www.m.share.bbcook.cn/Article/details/gxtgjgdaw.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.tarul.cn/Article/details/gxwiiaqwb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.yfazqb.com/Article/details/gqcpcalhu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/gtvfiipna.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.bbcook.cn/Article/details/glqiqgbfd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/geksmajqx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.bbcook.cn/Article/details/gpufhpfgd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gtgozvsbi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/goufxdsck.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.epnwcf.com/Article/details/glqbgyzer.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.yfazqb.com/Article/details/grgycmybn.sHtML

[E06] 替换子串
来源：http://wap.sjlbkw.cn/Article/details/gsvmzgizb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gnuqmkjbz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.sjlbkw.cn/Article/details/gwggtppnw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gdsconchf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/giyixgydm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gqyzlbsuy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gbcvpofny.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gzrzbsipx.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.epnwcf.com/Article/details/gkycvywli.sHtML

[E07] 按分隔符拆分
来源：http://mobile.sjlbkw.cn/Article/details/gfsmuatuj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.vehdjk.com/Article/details/gwoanfyzr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.bbcook.cn/Article/details/gmvmrpmjv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.yfazqb.com/Article/details/grsujsizz.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gtvtemqaa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.sjlbkw.cn/Article/details/gytyzsxlz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.bbcook.cn/Article/details/gdtaxgjec.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.yfazqb.com/Article/details/gwgxkqawz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.vehdjk.com/Article/details/gzpvizgvy.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fktsv.cn/Article/details/gtgghvfsy.sHtML

Py:   ",".join(items)
来源：http://www.share.vehdjk.com/Article/details/gkdryopmw.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.sjlbkw.cn/Article/details/gzdwvpmcj.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gjqwmhiov.sHtML

TS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/goswdxklr.sHtML

Java: String.join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/ggopxqmdd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fktsv.cn/Article/details/gmvcpyauf.sHtML

Ruby: items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gtbzgavdx.sHtML

C#:   string.Join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gmzehtbde.sHtML

[E09] 去除所有空白字符
来源：http://read.share.tarul.cn/Article/details/gfdazlagh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fktsv.cn/Article/details/gmfajkwdr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gczlgarjq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/gphumgwkp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.bbcook.cn/Article/details/gganipczu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gqbkoeeex.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.vehdjk.com/Article/details/gbmehetvn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.tarul.cn/Article/details/gskeaogzi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.yfazqb.com/Article/details/gmygyjclk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fktsv.cn/Article/details/gvlhirvao.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gpwrfbeow.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.sjlbkw.cn/Article/details/glhvxpzsb.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/goedotwxv.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gzscnuqmp.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gxceftoms.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gokaywgxh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/guzcaiacn.sHtML


<!-- 参考信息 -->