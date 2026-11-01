代发 wailian999

[D03] 在指定位置插入元素
来源：http://wap.sjlbkw.cn/Article/details/ggthjvavk.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gpkqcmojg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.vehdjk.com/Article/details/giqtxmkkg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fktsv.cn/Article/details/gzsxnross.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.vehdjk.com/Article/details/geduvmbne.sHtML

Java: list.add(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/glhqfeopc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.yfazqb.com/Article/details/gmetvmjcs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fktsv.cn/Article/details/gbaeleznh.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gmntpgzkk.sHtML

[D04] 删除元素
来源：http://blog.vehdjk.com/Article/details/gogfnpebl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.epnwcf.com/Article/details/givkwampt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.vehdjk.com/Article/details/galugdjpz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.tarul.cn/Article/details/gyfgqrodl.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fktsv.cn/Article/details/gykqyycem.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.bbcook.cn/Article/details/gstjrgjos.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.yfazqb.com/Article/details/gdmhkcogg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.tarul.cn/Article/details/gskzzqosa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.sjlbkw.cn/Article/details/ghcpfyjwx.sHtML

[D05] 访问与修改元素
来源：http://3g.epnwcf.com/Article/details/gfjkhzxli.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gwpdcubli.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gvkvuzqpt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gimcbsjkd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.sjlbkw.cn/Article/details/gtzxwjcll.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fktsv.cn/Article/details/gnlfjovmt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gxuofzite.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.bbcook.cn/Article/details/gsbchpunn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gtzhfdznf.sHtML

[D06] 数组长度
来源：http://3g.vehdjk.com/Article/details/gszdoeejr.sHtML

Py:   len(arr)
来源：http://baike.tarul.cn/Article/details/gdkyavzll.sHtML

PHP:  count($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gegtwhjpv.sHtML

JS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/gswynusfb.sHtML

TS:   arr.length
来源：http://www.m.share.epnwcf.com/Article/details/gedhopuny.sHtML

Java: list.size();
来源：http://m.share.fktsv.cn/Article/details/gpkaseyyr.sHtML

Go:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/goetbiuvc.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/guuojbtuy.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/gisxmlbmt.sHtML

[D07] 切片 / 取子数组
来源：http://wap.sjlbkw.cn/Article/details/glgpzisfv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.sjlbkw.cn/Article/details/gvqebmlrz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.epnwcf.com/Article/details/gkyidduqs.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gvmnpwwpk.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/glwvnuvov.sHtML

Java: list.subList(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gghfgfqcs.sHtML

Go:   arr[1:4]
来源：http://www.m.share.yfazqb.com/Article/details/gpurhlhin.sHtML

Ruby: arr[1, 3]
来源：http://blog.bbcook.cn/Article/details/gasznkgwo.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.tarul.cn/Article/details/gschrlhhj.sHtML

[D08] 合并两个数组
来源：http://read.share.fktsv.cn/Article/details/gvhcjxlpw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.yfazqb.com/Article/details/gzqqmujrx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.bbcook.cn/Article/details/gkarcyawh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.yfazqb.com/Article/details/glszrznlb.sHtML

TS:   [...a, ...b];
来源：http://www.share.yfazqb.com/Article/details/ghdywjsaw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.yfazqb.com/Article/details/gfamvtwqr.sHtML

Go:   append(a, b...)
来源：http://www.share.tarul.cn/Article/details/gjutllbxs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fktsv.cn/Article/details/gelolbhsx.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.vehdjk.com/Article/details/gfocdgagt.sHtML

[D09] 排序（升序）
来源：http://m.share.yfazqb.com/Article/details/grlaafyak.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gspobrvon.sHtML

PHP:  sort($arr);
来源：http://www.share.bbcook.cn/Article/details/gikfzjion.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.bbcook.cn/Article/details/gikhuuoao.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.tarul.cn/Article/details/gevznohcn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.tarul.cn/Article/details/gehzqfviw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/giplhwctm.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gknqzmhnd.sHtML

C#:   list.Sort();
来源：http://wap.sjlbkw.cn/Article/details/genreqksk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.tarul.cn/Article/details/guymqbrdv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.yfazqb.com/Article/details/guzvuteel.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.sjlbkw.cn/Article/details/glqcpzict.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/gfphffjuw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gfhsyimlx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.vehdjk.com/Article/details/garjclyqq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.yfazqb.com/Article/details/gxhgxdgqs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.vehdjk.com/Article/details/gabnqsuwn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.sjlbkw.cn/Article/details/gpfeabdun.sHtML

[D11] 反转数组
来源：http://m.share.tarul.cn/Article/details/gutqgipya.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gblydzgga.sHtML

PHP:  array_reverse($arr);
来源：http://baike.epnwcf.com/Article/details/ggmqhqztk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.epnwcf.com/Article/details/grfdqvbrn.sHtML

TS:   [...arr].reverse();
来源：http://blog.sjlbkw.cn/Article/details/gruaeiivs.sHtML

Java: Collections.reverse(list);
来源：http://3g.sjlbkw.cn/Article/details/gwqjjnmcf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.yfazqb.com/Article/details/gxkutyswi.sHtML

Ruby: arr.reverse
来源：http://read.share.epnwcf.com/Article/details/gjbpriicq.sHtML

C#:   list.Reverse();
来源：http://mobile.fktsv.cn/Article/details/gtazchtbn.sHtML

[D12] 查找元素下标
来源：http://www.blog.sjlbkw.cn/Article/details/gtxnrakqg.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/gyxtqgybo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.epnwcf.com/Article/details/gpajvzhlt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gutlatqfv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gontoeftv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.sjlbkw.cn/Article/details/grpeopoom.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gqxqsrrbp.sHtML

Ruby: arr.index(x)
来源：http://m.share.epnwcf.com/Article/details/gnidkzqfn.sHtML

C#:   list.IndexOf(x);
来源：http://baike.vehdjk.com/Article/details/grewragpt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.vehdjk.com/Article/details/guuhaxvcu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gbuvuskyi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.vehdjk.com/Article/details/ghogqizqm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.vehdjk.com/Article/details/gnhmgdhuo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gifdguxbg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.tarul.cn/Article/details/gabtbdcbz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.vehdjk.com/Article/details/gvjmasncx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.vehdjk.com/Article/details/gxjjvlcfu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fktsv.cn/Article/details/gojvplzdn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.vehdjk.com/Article/details/gmyvbuews.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.vehdjk.com/Article/details/gddvhpgmd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.yfazqb.com/Article/details/gzulnlmrp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/glzecwvgn.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/gnynhiuwl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.yfazqb.com/Article/details/gejitkvxb.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gnzirguyt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.tarul.cn/Article/details/gxiiaybop.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.yfazqb.com/Article/details/gzonynzuw.sHtML

[D15] 去重
来源：http://www.blog.yfazqb.com/Article/details/gaidjiqxm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gcfsfheet.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/gozszxdwd.sHtML

JS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gaspykiil.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gbxdhojnp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.vehdjk.com/Article/details/gkwazzwpu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.bbcook.cn/Article/details/goywwsrit.sHtML

Ruby: arr.uniq
来源：http://www.share.tarul.cn/Article/details/glvgchwgp.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/givevykgt.sHtML

[D16] 求和与平均值
来源：http://www.share.epnwcf.com/Article/details/gjpdbygpi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/guliutacl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fktsv.cn/Article/details/gkwyxiesv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/gkepsaawk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gzeawrwvh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.tarul.cn/Article/details/gqbkvcyxt.sHtML

Go:   // 手写循环累加
来源：http://read.share.sjlbkw.cn/Article/details/gsirjkqhe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.tarul.cn/Article/details/gvwvmywvu.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.vehdjk.com/Article/details/gmqfbzkec.sHtML

[D17] 最大值与最小值
来源：http://blog.bbcook.cn/Article/details/gzrqyxufg.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gzinhhnea.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.bbcook.cn/Article/details/gfxgyedbp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.yfazqb.com/Article/details/gttgzfxem.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/gwziurwyi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/gkggyjxwr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.sjlbkw.cn/Article/details/gbpzlnhex.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.vehdjk.com/Article/details/gbmujqnwz.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gshnxexxa.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.vehdjk.com/Article/details/gecileryl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.epnwcf.com/Article/details/gyjggiwyv.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.vehdjk.com/Article/details/gaovndyzz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.yfazqb.com/Article/details/gnutosqwt.sHtML

TS:   nested.flat();
来源：http://www.share.fktsv.cn/Article/details/gmkmiooga.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.epnwcf.com/Article/details/ggzscxjex.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.yfazqb.com/Article/details/gjbqkycxa.sHtML

Ruby: nested.flatten
来源：http://www.m.share.vehdjk.com/Article/details/gyvdyijyg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gkprtfsnn.sHtML

[D19] 按字段分组
来源：http://m.share.bbcook.cn/Article/details/gldfjaxci.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.bbcook.cn/Article/details/gqpelehsv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.bbcook.cn/Article/details/goonmwaff.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.tarul.cn/Article/details/gprazafea.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/gucwrzkad.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.sjlbkw.cn/Article/details/gjttuffjo.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.bbcook.cn/Article/details/gvwtvdrgu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/gpbgdxyzy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.vehdjk.com/Article/details/gltnqqroi.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.epnwcf.com/Article/details/gxljgrqid.sHtML

Py:   Counter(arr)
来源：http://read.share.fktsv.cn/Article/details/gbwqbmfhi.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gmpacsuas.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gnalpceze.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/ggfqjyufz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/gklngfzrk.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.tarul.cn/Article/details/ggguhoswa.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/gblgymfdg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.vehdjk.com/Article/details/gjacqnkii.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.yfazqb.com/Article/details/gfdwwgvwi.sHtML

Py:   x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gcryufawb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.bbcook.cn/Article/details/gdlfottxq.sHtML

JS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/guzkqnzsh.sHtML

TS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gmzhkhgxa.sHtML

Java: list.contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gwtbpvvnw.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.tarul.cn/Article/details/gvfbdveup.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gkwgtnrqx.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxmczhqj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/gtjkkrjkh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.sjlbkw.cn/Article/details/gqzpnduwl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.yfazqb.com/Article/details/gbkqlsgti.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.yfazqb.com/Article/details/getcqlhwb.sHtML

TS:   [...arr];
来源：http://blog.fktsv.cn/Article/details/gwnzxnbrs.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.epnwcf.com/Article/details/gjtolcscf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.yfazqb.com/Article/details/guuaxzxxf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.sjlbkw.cn/Article/details/gioqlular.sHtML

C#:   new List<int>(list);
来源：http://wap.fktsv.cn/Article/details/ghnaqefnt.sHtML

[D23] reduce 累积计算
来源：http://m.share.yfazqb.com/Article/details/grzmipzgc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gjazolevt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.yfazqb.com/Article/details/gaqqssxzf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gkswkagnk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gbxdzldmg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.yfazqb.com/Article/details/gnfoyhhzz.sHtML

Go:   // 手写循环
来源：http://3g.bbcook.cn/Article/details/gqxwndhxa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/gzrrablob.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fktsv.cn/Article/details/gupmwtoxi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.epnwcf.com/Article/details/gicqpkmgy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.vehdjk.com/Article/details/gtqwwxihr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.sjlbkw.cn/Article/details/gjrgxbzax.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.vehdjk.com/Article/details/gryegyqoy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.tarul.cn/Article/details/gwnngfkyq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.tarul.cn/Article/details/gmqgyztsg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/gagezcyyv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.vehdjk.com/Article/details/gzibjgelr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.vehdjk.com/Article/details/gukavogtu.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fktsv.cn/Article/details/gfhudeilr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.vehdjk.com/Article/details/gjcachwth.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.sjlbkw.cn/Article/details/gjyxktqud.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.vehdjk.com/Article/details/gyuwrltls.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.bbcook.cn/Article/details/gpvttiqak.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgnbayry.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.sjlbkw.cn/Article/details/gtylrwklh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.tarul.cn/Article/details/gzrryyuay.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.epnwcf.com/Article/details/gksibvben.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/gpdquootz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.yfazqb.com/Article/details/gecppkitx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrpndahi.sHtML

JS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gnsrbsoyd.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/gxkixfpvb.sHtML

Java: String.join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gmayfevfg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.vehdjk.com/Article/details/gbsuifeyo.sHtML

Ruby: arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/ggtbcgzpb.sHtML

C#:   string.Join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gqxjruyow.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmkaiuqzj.sHtML

E. 字符串处理
来源：http://www.m.share.fktsv.cn/Article/details/gbnjjbxlu.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gybrracgl.sHtML

[E01] 拼接字符串
来源：http://mobile.bbcook.cn/Article/details/grlycytqb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.sjlbkw.cn/Article/details/gitymucin.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.tarul.cn/Article/details/ghoxttmtb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/gwzlhdhcp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/gogxwoofb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gvlhakpzh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.tarul.cn/Article/details/gfemghajq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.tarul.cn/Article/details/gpwuvhuhk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gexqjbstb.sHtML

[E02] 重复字符串
来源：http://www.share.fktsv.cn/Article/details/glppwsywf.sHtML

Py:   "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gydrimoti.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fktsv.cn/Article/details/gqkhjyhwy.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gekepyhrt.sHtML

TS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gpxhtoigq.sHtML

Java: "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gbvlvlgew.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/gwrpkfpbh.sHtML

Ruby: "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/gxflimpvd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.bbcook.cn/Article/details/gdoatqvbo.sHtML

[E03] 截取子串
来源：http://mobile.tarul.cn/Article/details/ghrxczjtg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fktsv.cn/Article/details/gibjzvlpt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/ghqvazkqs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/guoqhjtqm.sHtML

TS:   s.slice(1, 4)
来源：http://3g.tarul.cn/Article/details/gfpdhlmay.sHtML

Java: s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gujjnoxuv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gojloqurs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.bbcook.cn/Article/details/ghsmihnbw.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.yfazqb.com/Article/details/gnxiuyupa.sHtML

[E04] 查找子串位置
来源：http://m.share.sjlbkw.cn/Article/details/gbkhivmqz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gvgbybusk.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/grgcxgjit.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.bbcook.cn/Article/details/gniygmhdi.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gqgzyyidb.sHtML

Java: s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gfgwtdlju.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.bbcook.cn/Article/details/gbqqojbmx.sHtML

Ruby: s.index("x")
来源：http://read.share.epnwcf.com/Article/details/gxvacdueu.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gyusrlvne.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.bbcook.cn/Article/details/grckftsvz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.bbcook.cn/Article/details/gpbuxwqld.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.vehdjk.com/Article/details/gjocecjuf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gytnraqtx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.vehdjk.com/Article/details/gzjujincw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gavksdlnz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.tarul.cn/Article/details/gonfbampg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.epnwcf.com/Article/details/ghydurlly.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fktsv.cn/Article/details/ggneobycn.sHtML

[E06] 替换子串
来源：http://www.m.share.tarul.cn/Article/details/gmztpvjmk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gjpidulqg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.sjlbkw.cn/Article/details/gjsalztjk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gscomvbqa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/guiobaxnp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/glyqaqqyy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gjckxyykf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.tarul.cn/Article/details/gabxgsdfc.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gtjhfnybh.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwxzwred.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.tarul.cn/Article/details/gnstkyjjz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.bbcook.cn/Article/details/gxnttmeik.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fktsv.cn/Article/details/gdetvfdux.sHtML

TS:   s.split(",")
来源：http://www.share.tarul.cn/Article/details/gfvbgscom.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/gbgvzfjdr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.yfazqb.com/Article/details/gogxfqvhx.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.yfazqb.com/Article/details/gtcyhblvr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fktsv.cn/Article/details/gfevuproh.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fktsv.cn/Article/details/glzwcqtvi.sHtML

Py:   ",".join(items)
来源：http://blog.yfazqb.com/Article/details/gmlvyzuyx.sHtML

PHP:  implode(",", $items);
来源：http://blog.fktsv.cn/Article/details/glzffsfhp.sHtML

JS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gxifrftqf.sHtML

TS:   items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/giinimvjd.sHtML

Java: String.join(",", items)
来源：http://wap.epnwcf.com/Article/details/glzerflro.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.bbcook.cn/Article/details/glkkbkyrc.sHtML

Ruby: items.join(",")
来源：http://baike.vehdjk.com/Article/details/gaibkruly.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/gkzblyulc.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/gwizqpyaf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.tarul.cn/Article/details/gxirndrco.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gjqfgrvzi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.bbcook.cn/Article/details/gvfrxwwnw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gurtqsbld.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.tarul.cn/Article/details/gaaupkxsp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.epnwcf.com/Article/details/gmtvfblyw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.yfazqb.com/Article/details/goazklkhb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fktsv.cn/Article/details/gtfujurfp.sHtML


<!-- 参考信息 -->