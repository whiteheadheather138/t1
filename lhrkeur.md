代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.epnwcf.com/Article/details/gclgusmun.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.tarul.cn/Article/details/gizeikcmd.sHtML

[D05] 访问与修改元素
来源：http://mobile.sjlbkw.cn/Article/details/gcjgqgdpk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/gurdrxnxf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gbwjnbdcb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gyplprjsg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fktsv.cn/Article/details/gkorjbttq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.sjlbkw.cn/Article/details/ghhvultjx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/ghgawpqav.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/ggrwqxahk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gvaquyhsv.sHtML

[D06] 数组长度
来源：http://baike.yfazqb.com/Article/details/gqtgltmdm.sHtML

Py:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gfakjshxh.sHtML

PHP:  count($arr);
来源：http://blog.bbcook.cn/Article/details/glccgmlpw.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gigskwskm.sHtML

TS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/grvvpiity.sHtML

Java: list.size();
来源：http://baike.epnwcf.com/Article/details/getkgsjwh.sHtML

Go:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gbedoeugl.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fktsv.cn/Article/details/gxgdroiuv.sHtML

C#:   list.Count;
来源：http://wap.yfazqb.com/Article/details/gswybzshs.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fktsv.cn/Article/details/gwlgwgusg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/gygjrkqyw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.yfazqb.com/Article/details/gpfnpdqqu.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gmowpuamk.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gxybhkjyt.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gfguxwdpj.sHtML

Go:   arr[1:4]
来源：http://baike.epnwcf.com/Article/details/gotntcfpj.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fktsv.cn/Article/details/grvwwxhns.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.sjlbkw.cn/Article/details/ghwgymckl.sHtML

[D08] 合并两个数组
来源：http://www.m.share.vehdjk.com/Article/details/gploiamec.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqiyodgl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.epnwcf.com/Article/details/ghatheqwj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fktsv.cn/Article/details/gmzemlghr.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/gprsinkdh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.vehdjk.com/Article/details/guqdilnku.sHtML

Go:   append(a, b...)
来源：http://mobile.fktsv.cn/Article/details/gpcghumzh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fktsv.cn/Article/details/gspglttar.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.epnwcf.com/Article/details/ggshhryka.sHtML

[D09] 排序（升序）
来源：http://read.share.fktsv.cn/Article/details/gktnbzvng.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gkmndqbla.sHtML

PHP:  sort($arr);
来源：http://www.blog.vehdjk.com/Article/details/gfktdrnkc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.tarul.cn/Article/details/ggasnzezz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.vehdjk.com/Article/details/gscgvfboo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.tarul.cn/Article/details/gunjscion.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gljufeoxj.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/gzftquncb.sHtML

C#:   list.Sort();
来源：http://baike.yfazqb.com/Article/details/gkamlsfqi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.yfazqb.com/Article/details/gchbgmkac.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.tarul.cn/Article/details/grzxtouee.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/gzjfubmmm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.sjlbkw.cn/Article/details/gdynafcdn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/gshqsasob.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.sjlbkw.cn/Article/details/gxzedakox.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.yfazqb.com/Article/details/geaspfjpj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.bbcook.cn/Article/details/gfrpqisbq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.bbcook.cn/Article/details/guppncjda.sHtML

[D11] 反转数组
来源：http://wap.bbcook.cn/Article/details/ghakeqvgc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.tarul.cn/Article/details/gybvzeasm.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.epnwcf.com/Article/details/gpxzkrzia.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fktsv.cn/Article/details/gxssaevpj.sHtML

TS:   [...arr].reverse();
来源：http://3g.fktsv.cn/Article/details/gewdsxirm.sHtML

Java: Collections.reverse(list);
来源：http://wap.bbcook.cn/Article/details/geyybsgaw.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.vehdjk.com/Article/details/gbwtzxtsa.sHtML

Ruby: arr.reverse
来源：http://m.share.yfazqb.com/Article/details/gxuafztrg.sHtML

C#:   list.Reverse();
来源：http://blog.fktsv.cn/Article/details/gthnzgiwb.sHtML

[D12] 查找元素下标
来源：http://wap.fktsv.cn/Article/details/gvpopqyyb.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/gaxitkvde.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.bbcook.cn/Article/details/gwscnrrqu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/gxytscrgc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/gyfahqmjq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.bbcook.cn/Article/details/gbefmdczr.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.yfazqb.com/Article/details/ghdgyyggi.sHtML

Ruby: arr.index(x)
来源：http://3g.vehdjk.com/Article/details/gavigvktt.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.tarul.cn/Article/details/gphtmmbjq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.epnwcf.com/Article/details/ghmictyhs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fktsv.cn/Article/details/gvetgswxy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.epnwcf.com/Article/details/glccycbpu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gvxdphksd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fktsv.cn/Article/details/gyehbqgyf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.yfazqb.com/Article/details/gwqqyktnq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fktsv.cn/Article/details/gajnxpxzz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.epnwcf.com/Article/details/gunrnmppu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gchmsenka.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gioyxdrsf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gbqusxclk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/gzhnclzvu.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fktsv.cn/Article/details/gzoqtpvin.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/gsuepwwje.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.bbcook.cn/Article/details/grvrvmwdg.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gpepthfxv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fktsv.cn/Article/details/gdgpzjukc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.epnwcf.com/Article/details/gbvpgzbcj.sHtML

[D15] 去重
来源：http://baike.vehdjk.com/Article/details/gkcodwnbr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxmsfmax.sHtML

PHP:  array_unique($arr);
来源：http://wap.vehdjk.com/Article/details/gpdbazgbc.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gkqixlqth.sHtML

TS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gqjcsiyoe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.sjlbkw.cn/Article/details/gwdnqntwh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.yfazqb.com/Article/details/gxusyqoqt.sHtML

Ruby: arr.uniq
来源：http://www.blog.epnwcf.com/Article/details/gticuqifo.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gsnymrsrc.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/gxnoocbxf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.tarul.cn/Article/details/glmfkchrt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.yfazqb.com/Article/details/gjaklyfcr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.epnwcf.com/Article/details/gkzenoqut.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gyrojapln.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.epnwcf.com/Article/details/gbaqwipdc.sHtML

Go:   // 手写循环累加
来源：http://read.share.vehdjk.com/Article/details/gzhlfrhmc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.bbcook.cn/Article/details/gmxnvpaxc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/grmebrcnj.sHtML

[D17] 最大值与最小值
来源：http://m.share.bbcook.cn/Article/details/geslykgel.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fktsv.cn/Article/details/gqbfetswx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.sjlbkw.cn/Article/details/grcsvbhxg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.yfazqb.com/Article/details/grhitfvaj.sHtML

TS:   Math.max(...arr);
来源：http://mobile.tarul.cn/Article/details/gxpdmekkr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.bbcook.cn/Article/details/gbipcypfb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.bbcook.cn/Article/details/gghkidbjo.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.bbcook.cn/Article/details/gzvmuowgs.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/gisgrbbtd.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.bbcook.cn/Article/details/grzuoutml.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.epnwcf.com/Article/details/gsswtmtyk.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.bbcook.cn/Article/details/gbxsyjzyj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.yfazqb.com/Article/details/gbyjebrhs.sHtML

TS:   nested.flat();
来源：http://baike.fktsv.cn/Article/details/gqwixwhqt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.sjlbkw.cn/Article/details/gueeehfym.sHtML

Go:   // 手写双层循环
来源：http://mobile.fktsv.cn/Article/details/gnryxslpl.sHtML

Ruby: nested.flatten
来源：http://read.share.vehdjk.com/Article/details/gtjigcqae.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.tarul.cn/Article/details/glbbqswcb.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/gfglopwug.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/gpaojbihg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.sjlbkw.cn/Article/details/guamsdefr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.bbcook.cn/Article/details/gpiflklvz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gkeljwmux.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.yfazqb.com/Article/details/gyvvvmwlw.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fktsv.cn/Article/details/ggkeuohhd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.bbcook.cn/Article/details/galovmadl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/gbwsmoahy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.epnwcf.com/Article/details/gpnkhabxl.sHtML

Py:   Counter(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gqnzsvydh.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.yfazqb.com/Article/details/gtkewbotm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gcnfkugtx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/ghwodqxqs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/gqekdoljf.sHtML

Go:   // 手写 map[T]int
来源：http://baike.sjlbkw.cn/Article/details/gqmvuohhf.sHtML

Ruby: arr.tally
来源：http://baike.fktsv.cn/Article/details/geckrgopj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.vehdjk.com/Article/details/ggnmgofzc.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/gvukayawn.sHtML

Py:   x in arr
来源：http://www.share.sjlbkw.cn/Article/details/guuognrfo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.epnwcf.com/Article/details/gumgwkvbh.sHtML

JS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/gsxhabhbr.sHtML

TS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gvpygmfvg.sHtML

Java: list.contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gqbzodird.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fktsv.cn/Article/details/giqtteauh.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/ghstvovuj.sHtML

C#:   list.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gsvednhhq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/gdujkcghf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.epnwcf.com/Article/details/gpxqiysbm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fktsv.cn/Article/details/gfaxeflua.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.vehdjk.com/Article/details/gyoqbjnjm.sHtML

TS:   [...arr];
来源：http://www.share.epnwcf.com/Article/details/gefulhaqh.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gwymnrvmg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.sjlbkw.cn/Article/details/gwxsdqrab.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.epnwcf.com/Article/details/gdvjwnjty.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/grbczilns.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqqaabwm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.bbcook.cn/Article/details/gcrhahkew.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.sjlbkw.cn/Article/details/ghjtinbft.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/ggxktnpqs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gpmavvjwe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/girknukag.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gkgaytoaw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/gwhqkmvof.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/gwqknyljh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.epnwcf.com/Article/details/gmhycxtdy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.yfazqb.com/Article/details/gouxyklkj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/genxxxkzz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gmordgyld.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gsncarqkz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/guppcgbca.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.yfazqb.com/Article/details/gtbunerug.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.bbcook.cn/Article/details/gsurctaru.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.sjlbkw.cn/Article/details/gnuqsifyu.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.yfazqb.com/Article/details/gsixfvxrq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.sjlbkw.cn/Article/details/gjvlkwslp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.tarul.cn/Article/details/gwymualph.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/glrxkrato.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.tarul.cn/Article/details/gllrdnxpv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.yfazqb.com/Article/details/ggznmingk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.yfazqb.com/Article/details/gmujqbizp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.bbcook.cn/Article/details/gykepvvfq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.tarul.cn/Article/details/gwgxjlilb.sHtML

[D26] 数组转字符串
来源：http://www.share.bbcook.cn/Article/details/gnnbtzqoc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/gsynxrojo.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.yfazqb.com/Article/details/gzvvbndmo.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/goiilwecr.sHtML

TS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gcrynnsgs.sHtML

Java: String.join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gciamjcha.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fktsv.cn/Article/details/ghvworreo.sHtML

Ruby: arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gvcpftfky.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/gvzxbjsiu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpteakflr.sHtML

E. 字符串处理
来源：http://m.share.fktsv.cn/Article/details/gcqvphvdl.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjttpjiur.sHtML

[E01] 拼接字符串
来源：http://read.share.epnwcf.com/Article/details/ghxffmoxt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/gmltavsfm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.epnwcf.com/Article/details/ghzkwwdtz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/giurciuvz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gtyzisveg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.bbcook.cn/Article/details/gxenfejgd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.epnwcf.com/Article/details/gqxcttgzi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.yfazqb.com/Article/details/gqkqilgod.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.bbcook.cn/Article/details/gbnvmslwd.sHtML

[E02] 重复字符串
来源：http://www.blog.tarul.cn/Article/details/gcfsvlmgh.sHtML

Py:   "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gqgqnairj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.tarul.cn/Article/details/ghzeuibhr.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/glptfwdbl.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gblhvjiwr.sHtML

Java: "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gcqxieach.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fktsv.cn/Article/details/gojskhxoh.sHtML

Ruby: "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gtflppkct.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fktsv.cn/Article/details/ggkqnwcsa.sHtML

[E03] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/gscimnxer.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gwgzslqgh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gqbfexwdy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gtjgltium.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gcmsdxehm.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gbcpjnulo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.tarul.cn/Article/details/ggkazbsfa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.vehdjk.com/Article/details/goudmhnag.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.bbcook.cn/Article/details/gbyyujcra.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/gnkcpwxmd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gimzlfech.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fktsv.cn/Article/details/gclajupfi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.epnwcf.com/Article/details/goqkkwhiw.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/grxnpyuur.sHtML

Java: s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/ghkrpvqyk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.epnwcf.com/Article/details/gmkymkvsd.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gxmldkrrj.sHtML

C#:   s.IndexOf("x")
来源：http://3g.vehdjk.com/Article/details/gdqfqkjws.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/ggcijnqkg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.epnwcf.com/Article/details/gdrkperqn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.epnwcf.com/Article/details/gsyedifuk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gtaclqsql.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdpibyoz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gtfmxeggl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.bbcook.cn/Article/details/gzwqrpral.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.yfazqb.com/Article/details/graicpxnh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.bbcook.cn/Article/details/gtghetcjg.sHtML

[E06] 替换子串
来源：http://www.m.share.yfazqb.com/Article/details/grqelcynr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gfbcoigtb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.yfazqb.com/Article/details/goirazqav.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gegjrrofw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gjgnskqcl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gleeojppi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gdosswohj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gqmlrmylt.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gkjphbbrk.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fktsv.cn/Article/details/gldsjxpze.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/giyiehygi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gehqlhhtr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fktsv.cn/Article/details/gnxljgegh.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/gspfrtjvs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.tarul.cn/Article/details/gpoyvinhr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.yfazqb.com/Article/details/gklxkxobe.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.sjlbkw.cn/Article/details/gmkbyrjac.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.vehdjk.com/Article/details/gtptjyqra.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/gqnmsslyc.sHtML

Py:   ",".join(items)
来源：http://wap.epnwcf.com/Article/details/gxhcbrrid.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/gdtadglvq.sHtML

JS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gydthknif.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/giuwolxoh.sHtML

Java: String.join(",", items)
来源：http://baike.vehdjk.com/Article/details/gehjrpjhq.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.tarul.cn/Article/details/gqisaxcpg.sHtML

Ruby: items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gvykmdbru.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/gipawwsqy.sHtML

[E09] 去除所有空白字符
来源：http://blog.sjlbkw.cn/Article/details/gbwaikubj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.sjlbkw.cn/Article/details/gbtptiayy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.vehdjk.com/Article/details/gvgynswej.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gjrffgicy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gjrqptkjj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/grxlhvrgt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.tarul.cn/Article/details/geeianoov.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.yfazqb.com/Article/details/gizpruiej.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gnjpzsxdb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.sjlbkw.cn/Article/details/gsltnlhou.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gxwqxwgpe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.epnwcf.com/Article/details/gzysyqcsx.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gmzghewzd.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gryvdvxpt.sHtML

Java: String.format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gzatlddaq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/giunbqrcy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gchnbybfk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.tarul.cn/Article/details/ghosdzyao.sHtML

[E11] 反转字符串
来源：http://baike.sjlbkw.cn/Article/details/gdjypzjtr.sHtML

Py:   s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gsntwmuuj.sHtML

PHP:  strrev($s);
来源：http://3g.bbcook.cn/Article/details/gaduhvxef.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gwmmsmhtb.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gmmjlpkox.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gerfyjttf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/gmaqpqhpc.sHtML


<!-- 参考信息 -->