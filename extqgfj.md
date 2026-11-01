代发 wailian999

Java: list.add(4);
来源：http://mobile.bbcook.cn/Article/details/gctrcvqbm.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.epnwcf.com/Article/details/gkiyidbxl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fktsv.cn/Article/details/gnpbnvvpt.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/ghyxwgxjg.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.bbcook.cn/Article/details/gdgcnjbku.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.epnwcf.com/Article/details/gqpgdzbhg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.epnwcf.com/Article/details/gofjfkeff.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.yfazqb.com/Article/details/gltelxbkm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.epnwcf.com/Article/details/gmwonhzip.sHtML

Java: list.add(0, 0);
来源：http://www.share.tarul.cn/Article/details/gqijnzfwz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.vehdjk.com/Article/details/gmfvgklcx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.vehdjk.com/Article/details/gwqeeefiy.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/ghvyksyys.sHtML

[D04] 删除元素
来源：http://www.blog.epnwcf.com/Article/details/gxgrvehoc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.vehdjk.com/Article/details/gsyqbzbph.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.yfazqb.com/Article/details/gfqfmcvac.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.epnwcf.com/Article/details/gsyupnlgr.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.yfazqb.com/Article/details/gnzlwfhob.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.sjlbkw.cn/Article/details/gihhhfimm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.epnwcf.com/Article/details/ghmccdqkd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.yfazqb.com/Article/details/gaxlcypde.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fktsv.cn/Article/details/gxbybobad.sHtML

[D05] 访问与修改元素
来源：http://wap.tarul.cn/Article/details/gisiflbst.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gvgrzunxy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gceqyenji.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gazkzbwrj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.tarul.cn/Article/details/gxndqymks.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.tarul.cn/Article/details/gemnlzegs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gtyzxjrdz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gletszpvn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gvquninhm.sHtML

[D06] 数组长度
来源：http://blog.bbcook.cn/Article/details/glsuclpdq.sHtML

Py:   len(arr)
来源：http://3g.fktsv.cn/Article/details/gbcergfli.sHtML

PHP:  count($arr);
来源：http://read.share.yfazqb.com/Article/details/ggxqvwxon.sHtML

JS:   arr.length
来源：http://wap.bbcook.cn/Article/details/gfwytugfn.sHtML

TS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gwjpsjaij.sHtML

Java: list.size();
来源：http://wap.sjlbkw.cn/Article/details/gdjkihrgg.sHtML

Go:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gyhdbluyy.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.bbcook.cn/Article/details/gidrqokeg.sHtML

C#:   list.Count;
来源：http://baike.sjlbkw.cn/Article/details/gigjaimuy.sHtML

[D07] 切片 / 取子数组
来源：http://blog.epnwcf.com/Article/details/gkwybswfu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.yfazqb.com/Article/details/gzxkkqbcr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.tarul.cn/Article/details/gvkzgksuq.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/gkwbvvbii.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.vehdjk.com/Article/details/gscotgpep.sHtML

Java: list.subList(1, 4);
来源：http://read.share.tarul.cn/Article/details/gslhwjgej.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/giilbdaot.sHtML

Ruby: arr[1, 3]
来源：http://read.share.bbcook.cn/Article/details/gmwheqvig.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fktsv.cn/Article/details/gzxmwovjo.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/grsstfywb.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gfhocahop.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fktsv.cn/Article/details/glltrhent.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.vehdjk.com/Article/details/gctqxalad.sHtML

TS:   [...a, ...b];
来源：http://baike.bbcook.cn/Article/details/gziyebakh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fktsv.cn/Article/details/gqqlyrvme.sHtML

Go:   append(a, b...)
来源：http://baike.yfazqb.com/Article/details/guaspgmro.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.vehdjk.com/Article/details/gzdzzcsti.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.vehdjk.com/Article/details/gvorjisls.sHtML

[D09] 排序（升序）
来源：http://blog.tarul.cn/Article/details/gtggsdvyu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/ghxrazqxc.sHtML

PHP:  sort($arr);
来源：http://www.blog.vehdjk.com/Article/details/gselhrvua.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.bbcook.cn/Article/details/gpnkqapow.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fktsv.cn/Article/details/gpweppwch.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.yfazqb.com/Article/details/gzdvdvyzp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gqtkuphzb.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gqvxpbonv.sHtML

C#:   list.Sort();
来源：http://www.blog.yfazqb.com/Article/details/giusevddk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.vehdjk.com/Article/details/gmbpemkfm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fktsv.cn/Article/details/gebcppera.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gqkgzwxlq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gmxgmltdh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.bbcook.cn/Article/details/ghmqpnkts.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.bbcook.cn/Article/details/gziuhfttc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.sjlbkw.cn/Article/details/gadbyxibk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.epnwcf.com/Article/details/grhxwkrwj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.epnwcf.com/Article/details/gcamwwauv.sHtML

[D11] 反转数组
来源：http://baike.epnwcf.com/Article/details/gqxirbznk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fktsv.cn/Article/details/goswbpave.sHtML

PHP:  array_reverse($arr);
来源：http://blog.bbcook.cn/Article/details/gtoyfmjfc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.sjlbkw.cn/Article/details/guazejszp.sHtML

TS:   [...arr].reverse();
来源：http://baike.sjlbkw.cn/Article/details/gqkpvpuwb.sHtML

Java: Collections.reverse(list);
来源：http://mobile.tarul.cn/Article/details/ghyyeyttd.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.epnwcf.com/Article/details/gcxvdqesl.sHtML

Ruby: arr.reverse
来源：http://wap.tarul.cn/Article/details/gyvapzewi.sHtML

C#:   list.Reverse();
来源：http://www.blog.vehdjk.com/Article/details/ggiochxxp.sHtML

[D12] 查找元素下标
来源：http://wap.fktsv.cn/Article/details/gdjughfxp.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.sjlbkw.cn/Article/details/grgaftvvb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.tarul.cn/Article/details/gtrqgnlpj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/ghozvyvnb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gfimlkogd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.yfazqb.com/Article/details/ggkykoace.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gdraftgfj.sHtML

Ruby: arr.index(x)
来源：http://wap.tarul.cn/Article/details/gzjakcfqc.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fktsv.cn/Article/details/gosoyqhem.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.tarul.cn/Article/details/gdrlyoesm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fktsv.cn/Article/details/geipnwqdn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fktsv.cn/Article/details/gpittfjfn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/grxyglqxc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gfxwqsxzj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.yfazqb.com/Article/details/gdbvqvzeq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/gdywembmr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.sjlbkw.cn/Article/details/ghjtlgclv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fktsv.cn/Article/details/gkzjmpobj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gxptsceeq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.sjlbkw.cn/Article/details/gcppjrhkx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.yfazqb.com/Article/details/gsssemzqr.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gconlhabb.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.bbcook.cn/Article/details/gtaqkzvlg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.sjlbkw.cn/Article/details/glpuejwvp.sHtML

Go:   // 手写循环
来源：http://m.share.sjlbkw.cn/Article/details/gryiuecpg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gwgzedjak.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.bbcook.cn/Article/details/gpisljups.sHtML

[D15] 去重
来源：http://blog.vehdjk.com/Article/details/gjjkrgswc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/grwaovoyb.sHtML

PHP:  array_unique($arr);
来源：http://blog.vehdjk.com/Article/details/gmxcvgyqr.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gwzjwqxbz.sHtML

TS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gqoqdyhfd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.yfazqb.com/Article/details/ghoqihiyv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.bbcook.cn/Article/details/gldavaewb.sHtML

Ruby: arr.uniq
来源：http://3g.sjlbkw.cn/Article/details/gnvckfcib.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/gunwntkmy.sHtML

[D16] 求和与平均值
来源：http://www.blog.bbcook.cn/Article/details/gtipxxgpc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.yfazqb.com/Article/details/grelshyai.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gnfyaqxrc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gtngmpsav.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.bbcook.cn/Article/details/gmwtomyby.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgmriidn.sHtML

Go:   // 手写循环累加
来源：http://m.share.bbcook.cn/Article/details/ggihzgeke.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.bbcook.cn/Article/details/gfmzazhde.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/ghkpsrgye.sHtML

[D17] 最大值与最小值
来源：http://www.share.sjlbkw.cn/Article/details/grkqmlfkh.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fktsv.cn/Article/details/genmthmur.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.vehdjk.com/Article/details/gpetmrrwn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.sjlbkw.cn/Article/details/goyhrctsz.sHtML

TS:   Math.max(...arr);
来源：http://read.share.bbcook.cn/Article/details/gspsatpsg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gnrvfsafv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gjiljwjkj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.vehdjk.com/Article/details/glhzdhgqw.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.yfazqb.com/Article/details/gffaaomqd.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.yfazqb.com/Article/details/gikgpivzx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.epnwcf.com/Article/details/gwpcfphni.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fktsv.cn/Article/details/glbmwezic.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/gzjwktqta.sHtML

TS:   nested.flat();
来源：http://blog.sjlbkw.cn/Article/details/guwezphxh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.vehdjk.com/Article/details/grxuttket.sHtML

Go:   // 手写双层循环
来源：http://baike.vehdjk.com/Article/details/gzhfkreht.sHtML

Ruby: nested.flatten
来源：http://www.share.fktsv.cn/Article/details/grtoybtjj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gnwvkoxvo.sHtML

[D19] 按字段分组
来源：http://www.share.epnwcf.com/Article/details/gknpzveri.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.sjlbkw.cn/Article/details/gfpolbmat.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/guqjhuwrv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.tarul.cn/Article/details/gmceyirba.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/gjvziefyo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.vehdjk.com/Article/details/grxlxjbbu.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.tarul.cn/Article/details/glvyhhzhe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.tarul.cn/Article/details/gyqajbskr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/gpxlypyyh.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.yfazqb.com/Article/details/gcoamunev.sHtML

Py:   Counter(arr)
来源：http://3g.yfazqb.com/Article/details/gpqactvbo.sHtML

PHP:  array_count_values($arr);
来源：http://3g.tarul.cn/Article/details/gqdgsqmge.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/garhqjrgt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gukgsbucc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.yfazqb.com/Article/details/gvdqkndhn.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/gktukifsk.sHtML

Ruby: arr.tally
来源：http://mobile.sjlbkw.cn/Article/details/gidujubmc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.sjlbkw.cn/Article/details/gcxbmxhdh.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.epnwcf.com/Article/details/ghobxjnew.sHtML

Py:   x in arr
来源：http://blog.vehdjk.com/Article/details/gdvfpbwph.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.yfazqb.com/Article/details/gvoznumom.sHtML

JS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/gznamvacs.sHtML

TS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gmadkhawf.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/gagzebcuv.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.vehdjk.com/Article/details/ggbpodlpw.sHtML

Ruby: arr.include?(x)
来源：http://blog.fktsv.cn/Article/details/gjlylbjqr.sHtML

C#:   list.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/gtgkejgzw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.yfazqb.com/Article/details/gikscsgak.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.tarul.cn/Article/details/ggservqjg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/gjmlstasp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gmymvtuvw.sHtML

TS:   [...arr];
来源：http://wap.fktsv.cn/Article/details/gtjyexvgh.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gtlxowjji.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.vehdjk.com/Article/details/gsughoymf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gapsvohli.sHtML

C#:   new List<int>(list);
来源：http://www.blog.yfazqb.com/Article/details/gnsjczjej.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/gchtctvkl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.vehdjk.com/Article/details/ghwseqlpv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.tarul.cn/Article/details/gpcsoilhd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/gxoluoamc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gpoczgifw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.sjlbkw.cn/Article/details/gwlogxvio.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gfipawknr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.sjlbkw.cn/Article/details/gqsegpsdy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.sjlbkw.cn/Article/details/gqiexdbnb.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.yfazqb.com/Article/details/grzhwwrvg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.vehdjk.com/Article/details/gebhrjtxv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.yfazqb.com/Article/details/gffzgvvii.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.bbcook.cn/Article/details/gcirrktpb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.tarul.cn/Article/details/giwxmbucv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.epnwcf.com/Article/details/gfpxryqfj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.vehdjk.com/Article/details/gxnnjijew.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/givjwylok.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.vehdjk.com/Article/details/gyyllyokg.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.epnwcf.com/Article/details/gurpcswuv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.vehdjk.com/Article/details/gkzywbnix.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.yfazqb.com/Article/details/grvmpvgde.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gwfwethdo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.bbcook.cn/Article/details/gnexnrqdr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.tarul.cn/Article/details/gqlzgqzsp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.tarul.cn/Article/details/glbywvyic.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fktsv.cn/Article/details/gujufodqo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gbhojnqlz.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/gpgjnbxbg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gmuyggibf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.bbcook.cn/Article/details/goiofvhtp.sHtML

JS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gmaqratvt.sHtML

TS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gqwhzruut.sHtML

Java: String.join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/gmtckypde.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.vehdjk.com/Article/details/gxczjhurf.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gkvusyrpl.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gbuobvuzr.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ganciywbc.sHtML

E. 字符串处理
来源：http://read.share.tarul.cn/Article/details/gqaqjfokc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gtysgrjqz.sHtML

[E01] 拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gsempvqsi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.tarul.cn/Article/details/gymviqcsk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.yfazqb.com/Article/details/gnnayeetb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/grkrxboun.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gbscnoxtr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fktsv.cn/Article/details/ggxzjslti.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fktsv.cn/Article/details/gimjabxiw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.vehdjk.com/Article/details/gbqjoyrlo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.tarul.cn/Article/details/ghxvbmwty.sHtML

[E02] 重复字符串
来源：http://www.blog.bbcook.cn/Article/details/gsvwvacii.sHtML

Py:   "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gbjmrvnzm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.tarul.cn/Article/details/gsmpnjqly.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gvjvomjtt.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gsktxkzbw.sHtML

Java: "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/guedpdwzl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.tarul.cn/Article/details/gxypophbm.sHtML

Ruby: "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gqshtwdmu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.tarul.cn/Article/details/gyihgnfjn.sHtML

[E03] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gvirnwqew.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.yfazqb.com/Article/details/grelyoxkc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gwgtjgagm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gsqgncdun.sHtML

TS:   s.slice(1, 4)
来源：http://baike.vehdjk.com/Article/details/gdujtzwhl.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gxotwgirr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fktsv.cn/Article/details/gggaionjx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.epnwcf.com/Article/details/gccshzaqd.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/gtsnstjxu.sHtML

[E04] 查找子串位置
来源：http://www.share.vehdjk.com/Article/details/ghkxkbpbr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fktsv.cn/Article/details/gwgfdqyvv.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.vehdjk.com/Article/details/grlgmddkg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.epnwcf.com/Article/details/gaamcicvp.sHtML

TS:   s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gtfsolqyx.sHtML

Java: s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gqajccujs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.bbcook.cn/Article/details/gnfscvqgc.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/gkfawepdl.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gqzbymgmg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.vehdjk.com/Article/details/gftckmxpo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.bbcook.cn/Article/details/gdafbuvud.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.bbcook.cn/Article/details/grtqifpie.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gnpifkdtb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhklhkww.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gnyonjciu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.sjlbkw.cn/Article/details/gzswzamef.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.epnwcf.com/Article/details/gpfdynxfx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.vehdjk.com/Article/details/ghhvxslsm.sHtML

[E06] 替换子串
来源：http://m.share.fktsv.cn/Article/details/gxzxhqcse.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/ghfsguvyn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.vehdjk.com/Article/details/gjfqraiwp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gfftywecb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/grjbpfgad.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gsejanvbd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gxfzmropm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.tarul.cn/Article/details/gdfrfkmoj.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.vehdjk.com/Article/details/gqugtlvlw.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gzjcekjyh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.epnwcf.com/Article/details/gbpsxvcqy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.tarul.cn/Article/details/gynlzgtyr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.tarul.cn/Article/details/gmjcgbcvt.sHtML

TS:   s.split(",")
来源：http://baike.vehdjk.com/Article/details/gkovstlpi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.sjlbkw.cn/Article/details/ghebblfnb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/gypnbcbzd.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.yfazqb.com/Article/details/gdkjpvrxw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.sjlbkw.cn/Article/details/gblrgbzdu.sHtML

[E08] 数组按分隔符合并
来源：http://blog.bbcook.cn/Article/details/gxypydyzv.sHtML

Py:   ",".join(items)
来源：http://m.share.yfazqb.com/Article/details/gkbcivhnl.sHtML

PHP:  implode(",", $items);
来源：http://read.share.tarul.cn/Article/details/gwxyrdeuq.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gxzmgipwm.sHtML

TS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gfyoqyqgt.sHtML

Java: String.join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gqolmdupz.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.tarul.cn/Article/details/gtiviqueu.sHtML

Ruby: items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/ghealkzjj.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/gkzclkppv.sHtML

[E09] 去除所有空白字符
来源：http://read.share.vehdjk.com/Article/details/gmwcfehrt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.epnwcf.com/Article/details/gegwtarbj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gxtgoijiu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/grnfcrqym.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/glatgcyqe.sHtML


<!-- 参考信息 -->