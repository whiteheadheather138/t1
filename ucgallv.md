代发 wailian999

C#:   list.Insert(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gdmlovrmq.sHtML

[D04] 删除元素
来源：http://3g.yfazqb.com/Article/details/gednjprxp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.sjlbkw.cn/Article/details/gfstrdrcm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.tarul.cn/Article/details/gzdczyrvv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fktsv.cn/Article/details/gwfbawffl.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.bbcook.cn/Article/details/gdrklzlwr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fktsv.cn/Article/details/ggkjerazp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fktsv.cn/Article/details/gkzhhpwnq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.tarul.cn/Article/details/gmtlsjamh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.vehdjk.com/Article/details/ggqbjrjul.sHtML

[D05] 访问与修改元素
来源：http://3g.fktsv.cn/Article/details/gzvrnmiva.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gfcfglfka.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gpbmirhsx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gzfommgic.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.bbcook.cn/Article/details/gktktzlgn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.bbcook.cn/Article/details/gfnkconwc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gkrgwrudr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/gmfvrkjoo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gageznpse.sHtML

[D06] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gsyhcxizi.sHtML

Py:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/grgdbjajz.sHtML

PHP:  count($arr);
来源：http://mobile.tarul.cn/Article/details/gqbqbsmeq.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gjmzxmbyj.sHtML

TS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gtvqsrucn.sHtML

Java: list.size();
来源：http://wap.epnwcf.com/Article/details/giioknctv.sHtML

Go:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gocfqfqzt.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/gupidpxpz.sHtML

C#:   list.Count;
来源：http://www.share.sjlbkw.cn/Article/details/gthnsbebu.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fktsv.cn/Article/details/gghsebavw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.tarul.cn/Article/details/grldgvugn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/ggrclqdlv.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gmskvwosp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzddexbv.sHtML

Java: list.subList(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gpukdprjb.sHtML

Go:   arr[1:4]
来源：http://3g.bbcook.cn/Article/details/gxazhrujx.sHtML

Ruby: arr[1, 3]
来源：http://blog.epnwcf.com/Article/details/giegyiyro.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.tarul.cn/Article/details/ggynjnkvn.sHtML

[D08] 合并两个数组
来源：http://www.share.epnwcf.com/Article/details/gzbwlhdzk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.yfazqb.com/Article/details/glqqkllcv.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.sjlbkw.cn/Article/details/giuaywyra.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.yfazqb.com/Article/details/gqrkemapk.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.vehdjk.com/Article/details/gajpgwsyz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fktsv.cn/Article/details/giqicvpci.sHtML

Go:   append(a, b...)
来源：http://www.share.yfazqb.com/Article/details/geioyelix.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.vehdjk.com/Article/details/gqsubdugj.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.epnwcf.com/Article/details/gghoszuic.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fktsv.cn/Article/details/grsixmwgf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/ghzyzdqbh.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gesqkubro.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.epnwcf.com/Article/details/goxsnsith.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.sjlbkw.cn/Article/details/gkawndztp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.vehdjk.com/Article/details/gzcwjgzbf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/gamszsatn.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gffpkkdhj.sHtML

C#:   list.Sort();
来源：http://m.share.vehdjk.com/Article/details/gqbgzatyp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.vehdjk.com/Article/details/gkdzmzmnn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.epnwcf.com/Article/details/gxadureea.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/gcmgbmpct.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gyphqvjlc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gxpzkgbjl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/gefhuiull.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fktsv.cn/Article/details/gcioukiua.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.vehdjk.com/Article/details/gmftverar.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.vehdjk.com/Article/details/gafddzemu.sHtML

[D11] 反转数组
来源：http://wap.bbcook.cn/Article/details/gxtwmrpfd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.tarul.cn/Article/details/gmptdebwd.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gwsxylwtk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.bbcook.cn/Article/details/gbimcoigj.sHtML

TS:   [...arr].reverse();
来源：http://mobile.yfazqb.com/Article/details/gzrpumnih.sHtML

Java: Collections.reverse(list);
来源：http://3g.vehdjk.com/Article/details/gyyjsbgdt.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.sjlbkw.cn/Article/details/gakmfqmgs.sHtML

Ruby: arr.reverse
来源：http://m.share.tarul.cn/Article/details/gcxicmfug.sHtML

C#:   list.Reverse();
来源：http://3g.epnwcf.com/Article/details/gncmxuqlm.sHtML

[D12] 查找元素下标
来源：http://m.share.epnwcf.com/Article/details/gchrluczv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.vehdjk.com/Article/details/gcpwqmdgw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gvrgqzadl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gwmteouvu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/gqqfwxjxz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.tarul.cn/Article/details/gefnkprng.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.tarul.cn/Article/details/gxptwqtmd.sHtML

Ruby: arr.index(x)
来源：http://mobile.bbcook.cn/Article/details/gkiqxoglt.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.yfazqb.com/Article/details/gldzcwvog.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.sjlbkw.cn/Article/details/gnpcivpfj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.vehdjk.com/Article/details/gubswddpi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.vehdjk.com/Article/details/goeurvbzy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.sjlbkw.cn/Article/details/guwlopspu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gdxefikrq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.sjlbkw.cn/Article/details/gnirbhjwf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.bbcook.cn/Article/details/gyxvhspms.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.bbcook.cn/Article/details/gnawvxcwp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.tarul.cn/Article/details/gzfnqxcly.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.tarul.cn/Article/details/godrbuyoq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.sjlbkw.cn/Article/details/gttmiylka.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gvqsoafbx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/giarapxrc.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/goamftfgn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.yfazqb.com/Article/details/gevkxmusd.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gjnqqveth.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/gjfksphqg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.tarul.cn/Article/details/gtnixfdmn.sHtML

[D15] 去重
来源：http://3g.epnwcf.com/Article/details/gwtptmgxk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/grytzmysi.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fktsv.cn/Article/details/gwdiqumvv.sHtML

JS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gvlvmflra.sHtML

TS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gyzxztpqj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.yfazqb.com/Article/details/gvlmdwkkb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.bbcook.cn/Article/details/gnbhljkyp.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gfjvhxfov.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.vehdjk.com/Article/details/gdnsdclbr.sHtML

[D16] 求和与平均值
来源：http://read.share.epnwcf.com/Article/details/gzaixldwc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fktsv.cn/Article/details/gmpcxgzlc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.yfazqb.com/Article/details/gjozoankr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.epnwcf.com/Article/details/gsettrlpw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.bbcook.cn/Article/details/gtedlvkgv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.vehdjk.com/Article/details/gqqcafkrv.sHtML

Go:   // 手写循环累加
来源：http://wap.tarul.cn/Article/details/gskrawohc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gurzszxyt.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.epnwcf.com/Article/details/gqpxzpvod.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.epnwcf.com/Article/details/gfxkqmkui.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fktsv.cn/Article/details/ghbxgszru.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.bbcook.cn/Article/details/ghvsbypug.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.tarul.cn/Article/details/gfcthgjyj.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.yfazqb.com/Article/details/gvsjfiucg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.yfazqb.com/Article/details/gcevjeivy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.tarul.cn/Article/details/ghvwxeybq.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.sjlbkw.cn/Article/details/gdjzwkulb.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.sjlbkw.cn/Article/details/giavohrhl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.sjlbkw.cn/Article/details/ggazvbptl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.sjlbkw.cn/Article/details/girhwdnus.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.vehdjk.com/Article/details/gsimfmetq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.tarul.cn/Article/details/gyybsvlyw.sHtML

TS:   nested.flat();
来源：http://wap.fktsv.cn/Article/details/gpndeobdk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gqzaetffx.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.yfazqb.com/Article/details/gnafvckhr.sHtML

Ruby: nested.flatten
来源：http://3g.epnwcf.com/Article/details/grvnqvlug.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gpbayrvyq.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/gkgtecfiz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.yfazqb.com/Article/details/gervrokjw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.epnwcf.com/Article/details/gnogoctjb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.epnwcf.com/Article/details/gmfltqmic.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/gyvnfcmjq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.vehdjk.com/Article/details/gdfqdnyym.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.vehdjk.com/Article/details/gwrbwulhb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/gobmztlzv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.tarul.cn/Article/details/gwujifahf.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.vehdjk.com/Article/details/gijrsmrgj.sHtML

Py:   Counter(arr)
来源：http://www.blog.bbcook.cn/Article/details/grkyvntzc.sHtML

PHP:  array_count_values($arr);
来源：http://3g.tarul.cn/Article/details/gqktezfld.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gjgcgzuij.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/glcdtnazu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.yfazqb.com/Article/details/glxxysyru.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.sjlbkw.cn/Article/details/gtbecseyj.sHtML

Ruby: arr.tally
来源：http://www.share.sjlbkw.cn/Article/details/gbcsmnpcu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.tarul.cn/Article/details/gxjovjmit.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.sjlbkw.cn/Article/details/gwuhxupsx.sHtML

Py:   x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gmufmzoks.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fktsv.cn/Article/details/gvhabnddi.sHtML

JS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/grxvoaypy.sHtML

TS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/ggbhljkel.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gbncjruwc.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gyntgomxu.sHtML

Ruby: arr.include?(x)
来源：http://3g.epnwcf.com/Article/details/gbbuyhuki.sHtML

C#:   list.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gfqbxnzdy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.epnwcf.com/Article/details/gmuausclc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.epnwcf.com/Article/details/gakevtook.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.bbcook.cn/Article/details/gshhdbsvx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.vehdjk.com/Article/details/gwrmqdqaw.sHtML

TS:   [...arr];
来源：http://www.blog.sjlbkw.cn/Article/details/gwkvqwfpv.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.yfazqb.com/Article/details/gfpqokzxv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.bbcook.cn/Article/details/gyrfkekal.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.sjlbkw.cn/Article/details/gshibqrme.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gxfcuqaci.sHtML

[D23] reduce 累积计算
来源：http://www.share.tarul.cn/Article/details/gczczygkv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gxrdmavwp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.bbcook.cn/Article/details/guaxaqmmm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/glostyimb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/ggiosdsbf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.sjlbkw.cn/Article/details/gnvvvfyno.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gtbdprace.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.tarul.cn/Article/details/gelyszksb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fktsv.cn/Article/details/grpbgdeox.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fktsv.cn/Article/details/gcwfiwhqw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.yfazqb.com/Article/details/ggazazrsv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.tarul.cn/Article/details/ghbsehyar.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.sjlbkw.cn/Article/details/gbhwvkohi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gsbkqsmbi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.vehdjk.com/Article/details/galsjnjxi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fktsv.cn/Article/details/gfkrvtrmc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.tarul.cn/Article/details/gdbchhhsd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.tarul.cn/Article/details/gzgerialt.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.epnwcf.com/Article/details/gkyvycvmy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fktsv.cn/Article/details/ggmlwwvua.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.sjlbkw.cn/Article/details/gkobqodvb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fktsv.cn/Article/details/gifowuhdf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fktsv.cn/Article/details/gfcubwfdo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/gfjeqlcli.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.yfazqb.com/Article/details/giigqzofi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.yfazqb.com/Article/details/ghjocvjjn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.yfazqb.com/Article/details/gyqznptpt.sHtML

[D26] 数组转字符串
来源：http://www.blog.tarul.cn/Article/details/gndnnziqz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.tarul.cn/Article/details/gjzzhsmnc.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.yfazqb.com/Article/details/gbdjjokhe.sHtML

JS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gizakcmyl.sHtML

TS:   arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gypgggzat.sHtML

Java: String.join(", ", list)
来源：http://blog.tarul.cn/Article/details/gcisyeoxx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fktsv.cn/Article/details/gqhahdjxl.sHtML

Ruby: arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gzrfqyhpe.sHtML

C#:   string.Join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gjccbjqwm.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glnenqpzv.sHtML

E. 字符串处理
来源：http://mobile.tarul.cn/Article/details/gplhketsn.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gluwcfjrw.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gvnteulnn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.sjlbkw.cn/Article/details/ghukpolyk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fktsv.cn/Article/details/gxtmxmznz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gpnbpdini.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gxfugzemj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.sjlbkw.cn/Article/details/gimdmsidh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fktsv.cn/Article/details/ggrjxxeor.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.yfazqb.com/Article/details/gdcbggxds.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.vehdjk.com/Article/details/gkioujhcb.sHtML

[E02] 重复字符串
来源：http://www.m.share.epnwcf.com/Article/details/gaxxspslp.sHtML

Py:   "ab" * 3
来源：http://baike.epnwcf.com/Article/details/gyflfggqk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.epnwcf.com/Article/details/geesajscq.sHtML

JS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gqzlyzcyp.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gmwkqlxpm.sHtML

Java: "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gmlfahord.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.vehdjk.com/Article/details/gmliduazp.sHtML

Ruby: "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gkgduqpxa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fktsv.cn/Article/details/gjbysvsna.sHtML

[E03] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/gsubdrfkx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.yfazqb.com/Article/details/gtrsicirm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gkzwldrug.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gdziemnbm.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/ghzatupoa.sHtML

Java: s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gniczpdaa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.bbcook.cn/Article/details/glkiiaemp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.yfazqb.com/Article/details/grieldhqs.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fktsv.cn/Article/details/gmxlxoawk.sHtML

[E04] 查找子串位置
来源：http://baike.sjlbkw.cn/Article/details/gfynyyeag.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.epnwcf.com/Article/details/ghiajgjsz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.yfazqb.com/Article/details/gkhjqjfwl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.yfazqb.com/Article/details/ghjoaclnf.sHtML

TS:   s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gzuffrdxo.sHtML

Java: s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gryrogiqm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/gjuhklxxp.sHtML

Ruby: s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gjyuzdjgi.sHtML

C#:   s.IndexOf("x")
来源：http://blog.bbcook.cn/Article/details/gilblytvl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.vehdjk.com/Article/details/gzjshkebv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gysrabnoz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.tarul.cn/Article/details/gobnodffh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gihgesvhc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.bbcook.cn/Article/details/gcokepyec.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/gawzmiqoe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.sjlbkw.cn/Article/details/ggsprlokd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/gwtukhoxp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gnrwfruwj.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/gutmhvzdd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/ghuhjnfff.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.sjlbkw.cn/Article/details/glzrkfapb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gzevrnbam.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gsyfyvdwl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gmbdmqwrm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxixzrcdp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.vehdjk.com/Article/details/ghqxvnvbj.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/ghdxxdcxr.sHtML

[E07] 按分隔符拆分
来源：http://3g.fktsv.cn/Article/details/glghmwisr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.yfazqb.com/Article/details/gfjobugin.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gljmkqubp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/gzelivuhc.sHtML

TS:   s.split(",")
来源：http://baike.fktsv.cn/Article/details/grbgvbtor.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.yfazqb.com/Article/details/gwvtphscq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.tarul.cn/Article/details/gytmtpjzz.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.epnwcf.com/Article/details/gzighxiry.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.sjlbkw.cn/Article/details/gzpkchedx.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.tarul.cn/Article/details/gzfqioxms.sHtML

Py:   ",".join(items)
来源：http://mobile.vehdjk.com/Article/details/gtqllfyzc.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fktsv.cn/Article/details/gjvnskist.sHtML

JS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gspdmoyjz.sHtML

TS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/grxeeomtj.sHtML

Java: String.join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gemertohh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.vehdjk.com/Article/details/ghujvpldc.sHtML

Ruby: items.join(",")
来源：http://wap.bbcook.cn/Article/details/gtdfwbppb.sHtML

C#:   string.Join(",", items)
来源：http://3g.bbcook.cn/Article/details/ghqdflavr.sHtML

[E09] 去除所有空白字符
来源：http://read.share.sjlbkw.cn/Article/details/gffktjari.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.yfazqb.com/Article/details/gfktwtxor.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.bbcook.cn/Article/details/guiffvbyd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/gpkoowelp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gwhrjmevd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gxvktuugn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.yfazqb.com/Article/details/gbmsspryb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.vehdjk.com/Article/details/gazpqvhgr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fktsv.cn/Article/details/grgmetjco.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/guctrpqlx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.yfazqb.com/Article/details/grnojsbqk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gwlsepnwy.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gbnzoazgk.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gchqaedvq.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gpmjjhhpn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gvfqbtvou.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gqfukoyqt.sHtML


<!-- 参考信息 -->