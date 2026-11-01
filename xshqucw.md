代发 wailian999

[D03] 在指定位置插入元素
来源：http://mobile.tarul.cn/Article/details/gcgfcrehy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.epnwcf.com/Article/details/gtxozqklo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.tarul.cn/Article/details/gnwgvzctk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/ggzcprwxi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fktsv.cn/Article/details/ghznsntol.sHtML

Java: list.add(0, 0);
来源：http://baike.fktsv.cn/Article/details/gzvnaycge.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.sjlbkw.cn/Article/details/ghgnqikrg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.epnwcf.com/Article/details/ghmrxmklo.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/grcnqoxgg.sHtML

[D04] 删除元素
来源：http://blog.bbcook.cn/Article/details/gtcxzzxud.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/gnfixygpf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/geakbfsbk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.yfazqb.com/Article/details/gsslllvgl.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.yfazqb.com/Article/details/gqvxulhpg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.epnwcf.com/Article/details/gkkngxqix.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.tarul.cn/Article/details/gymsyimay.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.bbcook.cn/Article/details/gqzpcroty.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.yfazqb.com/Article/details/groldsolo.sHtML

[D05] 访问与修改元素
来源：http://blog.tarul.cn/Article/details/gelvuwukh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/gisxzikmt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gxdygrjjq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/giwijwmcd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fktsv.cn/Article/details/gsawqstmq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.epnwcf.com/Article/details/guqbrdtyz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/geqkugjrw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gjvukjmpr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.vehdjk.com/Article/details/giuejsmzu.sHtML

[D06] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gqgikkruh.sHtML

Py:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gwntwpagc.sHtML

PHP:  count($arr);
来源：http://m.share.vehdjk.com/Article/details/gfxmjajmy.sHtML

JS:   arr.length
来源：http://mobile.yfazqb.com/Article/details/gopruyozk.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/glzdptarg.sHtML

Java: list.size();
来源：http://www.share.bbcook.cn/Article/details/ghbsywdjh.sHtML

Go:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gmwsfhxhw.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.tarul.cn/Article/details/gsidbsbqy.sHtML

C#:   list.Count;
来源：http://mobile.epnwcf.com/Article/details/gbmaxtcqw.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.epnwcf.com/Article/details/gfoehoyqe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.yfazqb.com/Article/details/gamlkknzn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/gzzuvzynb.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.tarul.cn/Article/details/gonypqhds.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/gqfrthjnz.sHtML

Java: list.subList(1, 4);
来源：http://baike.bbcook.cn/Article/details/gpaxszylu.sHtML

Go:   arr[1:4]
来源：http://blog.tarul.cn/Article/details/gdprqndkg.sHtML

Ruby: arr[1, 3]
来源：http://blog.vehdjk.com/Article/details/goixlapfq.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fktsv.cn/Article/details/gsfvtkoil.sHtML

[D08] 合并两个数组
来源：http://baike.yfazqb.com/Article/details/gqvdohkww.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.bbcook.cn/Article/details/gbufocyow.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.epnwcf.com/Article/details/gbiqyqnro.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.sjlbkw.cn/Article/details/gfhhsqxtz.sHtML

TS:   [...a, ...b];
来源：http://mobile.epnwcf.com/Article/details/gtlhtvmtg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.bbcook.cn/Article/details/gbcjoanwq.sHtML

Go:   append(a, b...)
来源：http://mobile.epnwcf.com/Article/details/gtaveiief.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fktsv.cn/Article/details/grjnglqpd.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.bbcook.cn/Article/details/ghncqvcaa.sHtML

[D09] 排序（升序）
来源：http://read.share.vehdjk.com/Article/details/gxhjpszjb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gcewnxesj.sHtML

PHP:  sort($arr);
来源：http://blog.yfazqb.com/Article/details/gqgkvrfxv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.vehdjk.com/Article/details/gnpcwdlzm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fktsv.cn/Article/details/giuatfwpq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.vehdjk.com/Article/details/gsigiodyn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/ghepyuemm.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gonyvzqct.sHtML

C#:   list.Sort();
来源：http://www.blog.tarul.cn/Article/details/gvxqnlrte.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.epnwcf.com/Article/details/gnrfxgwrh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/guhyhuekh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.tarul.cn/Article/details/gfvipjooc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/gdawoapos.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.epnwcf.com/Article/details/gpeavclrm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.tarul.cn/Article/details/gzlmcdmhr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.yfazqb.com/Article/details/gblmoljmv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.bbcook.cn/Article/details/gjeosmecw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.sjlbkw.cn/Article/details/gfwyuifur.sHtML

[D11] 反转数组
来源：http://www.blog.bbcook.cn/Article/details/ghsxnxjnh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/grwrooqvc.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.epnwcf.com/Article/details/gcgpomxoa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.bbcook.cn/Article/details/goduaosku.sHtML

TS:   [...arr].reverse();
来源：http://mobile.bbcook.cn/Article/details/gipaqvjwa.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fktsv.cn/Article/details/ggdnsdhog.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gogtjzrua.sHtML

Ruby: arr.reverse
来源：http://www.m.share.bbcook.cn/Article/details/glsfvuedw.sHtML

C#:   list.Reverse();
来源：http://www.m.share.tarul.cn/Article/details/gmvkhgsjr.sHtML

[D12] 查找元素下标
来源：http://blog.vehdjk.com/Article/details/gqahtlxgp.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.yfazqb.com/Article/details/gsecuxltx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gctcdmheo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gsntkjjzx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gtjiadlus.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.yfazqb.com/Article/details/ggjkuhnmv.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gdkktchnj.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/gezqtaedw.sHtML

C#:   list.IndexOf(x);
来源：http://baike.yfazqb.com/Article/details/gkwfnqdzx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.vehdjk.com/Article/details/gjnaazysu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.epnwcf.com/Article/details/gzzjceeem.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.vehdjk.com/Article/details/godzeottd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fktsv.cn/Article/details/gkazmvaex.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gcszxsoyh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.vehdjk.com/Article/details/gxvuqkmns.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.epnwcf.com/Article/details/gliyelvif.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.vehdjk.com/Article/details/gjmhbhgnr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fktsv.cn/Article/details/gqwlojrti.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.vehdjk.com/Article/details/gtvwyxpyw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/ggussphjw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.yfazqb.com/Article/details/gwrsexaud.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/grrzkvnfp.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/grxeqtstw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.yfazqb.com/Article/details/gngyzaxbe.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/gcrnptilg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.vehdjk.com/Article/details/gjafiftdf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/glaapckkf.sHtML

[D15] 去重
来源：http://3g.tarul.cn/Article/details/gjfkofkek.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/gpqtrbmrq.sHtML

PHP:  array_unique($arr);
来源：http://m.share.yfazqb.com/Article/details/gqkgxggme.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gcipicmup.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/givncnwuz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/gspzptgxn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.sjlbkw.cn/Article/details/gldcxokrc.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/geyssdaqp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.yfazqb.com/Article/details/gkmffoxxq.sHtML

[D16] 求和与平均值
来源：http://read.share.vehdjk.com/Article/details/glpvvyvda.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.bbcook.cn/Article/details/gqedeyoqj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.bbcook.cn/Article/details/ghsdhrdiy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gakzxegog.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/gfpaeuqcc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.bbcook.cn/Article/details/gwcoqnzxc.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gabzcuonj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fktsv.cn/Article/details/gdoynstkm.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.yfazqb.com/Article/details/gdsiooacr.sHtML

[D17] 最大值与最小值
来源：http://www.share.yfazqb.com/Article/details/gibdsijzs.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxzumskq.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.bbcook.cn/Article/details/gfendwkzs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/gqkkexzku.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.bbcook.cn/Article/details/gtrhqqkfi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.sjlbkw.cn/Article/details/gavwcgqip.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.tarul.cn/Article/details/gikztdrpt.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gfcdmqqvk.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.vehdjk.com/Article/details/gtldpbuif.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.tarul.cn/Article/details/ghrmzlpsw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.sjlbkw.cn/Article/details/gwfnklezy.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/gnrmahqdx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.epnwcf.com/Article/details/gduguijmp.sHtML

TS:   nested.flat();
来源：http://baike.sjlbkw.cn/Article/details/gzznvobbl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.vehdjk.com/Article/details/gocdttmot.sHtML

Go:   // 手写双层循环
来源：http://www.share.bbcook.cn/Article/details/gdrhtnfqb.sHtML

Ruby: nested.flatten
来源：http://wap.tarul.cn/Article/details/ghbcojolb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.vehdjk.com/Article/details/gvrmeyuyh.sHtML

[D19] 按字段分组
来源：http://mobile.yfazqb.com/Article/details/gmsyozlaw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.tarul.cn/Article/details/gpkdemmav.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.sjlbkw.cn/Article/details/gllxuosyk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fktsv.cn/Article/details/gxbotymzo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gljvseavj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.epnwcf.com/Article/details/geanfsbfp.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.epnwcf.com/Article/details/gmyairhpx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.tarul.cn/Article/details/gazzeidzd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.yfazqb.com/Article/details/gybkscjzw.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.tarul.cn/Article/details/ghbrjveoq.sHtML

Py:   Counter(arr)
来源：http://read.share.tarul.cn/Article/details/gnekdgpox.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.epnwcf.com/Article/details/gjmcombar.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/gwfkofjcb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gwuxspnel.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fktsv.cn/Article/details/gjyfstqio.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/gphnlwxnt.sHtML

Ruby: arr.tally
来源：http://read.share.tarul.cn/Article/details/gblnlrgsk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/geyvdjdll.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.sjlbkw.cn/Article/details/gyajuuwjk.sHtML

Py:   x in arr
来源：http://mobile.sjlbkw.cn/Article/details/grsxlrlqh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmrdiyfg.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/goixfuyiy.sHtML

TS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gekvlsger.sHtML

Java: list.contains(x)
来源：http://blog.yfazqb.com/Article/details/gappbkfnk.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.tarul.cn/Article/details/gopyjlsqq.sHtML

Ruby: arr.include?(x)
来源：http://3g.fktsv.cn/Article/details/gdetkjbnl.sHtML

C#:   list.Contains(x)
来源：http://mobile.fktsv.cn/Article/details/goqovczym.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fktsv.cn/Article/details/gctaqrcdl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.sjlbkw.cn/Article/details/gyjoqynrf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/gsrkglsfi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.epnwcf.com/Article/details/gdewsnoqz.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/gylbkwoah.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gngriwfrg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/glvuebdxj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.epnwcf.com/Article/details/gkqhtfpcz.sHtML

C#:   new List<int>(list);
来源：http://baike.vehdjk.com/Article/details/gdpafmahy.sHtML

[D23] reduce 累积计算
来源：http://www.share.vehdjk.com/Article/details/ggsoemiyz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.yfazqb.com/Article/details/gqjygkbjx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.vehdjk.com/Article/details/gplnxmmzp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/ggnpyunuh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gxrfleohx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.vehdjk.com/Article/details/gailxnbcz.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/glgexchyu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.yfazqb.com/Article/details/graeexkyg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.bbcook.cn/Article/details/gpvokfoso.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/gnerwhplu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.epnwcf.com/Article/details/gdzaovcej.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/guhvnhuce.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.yfazqb.com/Article/details/gzwcczzgi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gupzixlnq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.sjlbkw.cn/Article/details/gybraualk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.tarul.cn/Article/details/gxsirtbey.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/gvdssrhhi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.bbcook.cn/Article/details/gpmegddqs.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.bbcook.cn/Article/details/gneszgucv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.tarul.cn/Article/details/gkuhbaoof.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/gzkiyrren.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.vehdjk.com/Article/details/grtwjvguo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/gyjmxjpbm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.tarul.cn/Article/details/geziwbehc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.yfazqb.com/Article/details/gwprqhokn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.vehdjk.com/Article/details/gpbndobls.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.bbcook.cn/Article/details/gmjmqxiby.sHtML

[D26] 数组转字符串
来源：http://3g.sjlbkw.cn/Article/details/gpmlqsxle.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.tarul.cn/Article/details/gkadzqzbf.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/gvzdpzxhj.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/glspenehx.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gpvdkkrio.sHtML

Java: String.join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gkerxjcfi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.bbcook.cn/Article/details/gtmasclkx.sHtML

Ruby: arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gndurjvzt.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gidyywquz.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcsopwmsp.sHtML

E. 字符串处理
来源：http://m.share.epnwcf.com/Article/details/ggfvdjdtp.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqcjmpphv.sHtML

[E01] 拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gkfwooqjw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.bbcook.cn/Article/details/gxafjragl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.sjlbkw.cn/Article/details/gdhhvwjbh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gkjpaldid.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/gilfcwbjd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.tarul.cn/Article/details/gwhkcjwxq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gohtuempr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.bbcook.cn/Article/details/gwgsajmex.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gmiylaorb.sHtML

[E02] 重复字符串
来源：http://baike.tarul.cn/Article/details/gsvvzymbh.sHtML

Py:   "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gfccerjyh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.vehdjk.com/Article/details/gvggafwdv.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gzgzuvsai.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gmmvctsrc.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gtklsrycg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gldwrzhdo.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gvnpnynra.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.epnwcf.com/Article/details/gpyisneqq.sHtML

[E03] 截取子串
来源：http://mobile.tarul.cn/Article/details/gcozwkauf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.tarul.cn/Article/details/goztgjpgt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gczltbztm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gbwzojvwj.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gflalkktt.sHtML

Java: s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/ggrwotqir.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.sjlbkw.cn/Article/details/gpwuhkmyl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.tarul.cn/Article/details/gfnivykgi.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.bbcook.cn/Article/details/gjyxwngfb.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/ggdwmcykw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/guwlhkjco.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fktsv.cn/Article/details/gkrqoxyyp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.bbcook.cn/Article/details/geutaxqnb.sHtML

TS:   s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/gojrowjrp.sHtML

Java: s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gynrpahca.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.bbcook.cn/Article/details/gcqyimowj.sHtML

Ruby: s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gtkvxbvfr.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.tarul.cn/Article/details/gajyrdwqm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.vehdjk.com/Article/details/gmywtavly.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.tarul.cn/Article/details/gdxoqvlnm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.epnwcf.com/Article/details/gfqgveykg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gwwgyrecs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/gvbnuvhsp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/grzvyfikp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.bbcook.cn/Article/details/guafdziut.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.epnwcf.com/Article/details/gxvbfyyda.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.yfazqb.com/Article/details/glfagdgsy.sHtML

[E06] 替换子串
来源：http://www.share.tarul.cn/Article/details/gkmkrkzup.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.vehdjk.com/Article/details/gofyqoyqw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fktsv.cn/Article/details/gsbytkmqn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gnrcfkyly.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gcovpgtlq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gmtverifi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gslmigehi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.yfazqb.com/Article/details/gsktkbqaq.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.yfazqb.com/Article/details/glpnidhiw.sHtML

[E07] 按分隔符拆分
来源：http://3g.yfazqb.com/Article/details/gntzcswov.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.bbcook.cn/Article/details/guylswgey.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.epnwcf.com/Article/details/guomexhzv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fktsv.cn/Article/details/gjpfzzexl.sHtML

TS:   s.split(",")
来源：http://blog.tarul.cn/Article/details/gyyjjljpo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fktsv.cn/Article/details/gayrotvmi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.epnwcf.com/Article/details/grdwauoxm.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.tarul.cn/Article/details/gczkacmbh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.bbcook.cn/Article/details/gmzagvgmw.sHtML

[E08] 数组按分隔符合并
来源：http://blog.sjlbkw.cn/Article/details/guvwqvrnb.sHtML

Py:   ",".join(items)
来源：http://www.blog.tarul.cn/Article/details/gjdfxrrxa.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/gcagrhlvs.sHtML

JS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gezkwgpbe.sHtML

TS:   items.join(",")
来源：http://read.share.yfazqb.com/Article/details/gnzcvjjgd.sHtML

Java: String.join(",", items)
来源：http://read.share.tarul.cn/Article/details/gtgnerizt.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.bbcook.cn/Article/details/ggllmtokh.sHtML

Ruby: items.join(",")
来源：http://www.blog.tarul.cn/Article/details/ggulgsnrw.sHtML

C#:   string.Join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gsgzmmyry.sHtML

[E09] 去除所有空白字符
来源：http://m.share.vehdjk.com/Article/details/gjtbvarfc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.yfazqb.com/Article/details/gsaboizjx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.epnwcf.com/Article/details/gnlbmogyk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gsbbxvdpa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/goinfcygk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gcqpgbjci.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/gzozbshxs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fktsv.cn/Article/details/geegjdsar.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gljexwsil.sHtML


<!-- 参考信息 -->