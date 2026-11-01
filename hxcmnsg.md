代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fktsv.cn/Article/details/gdudmwwzc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gplhxrekl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.bbcook.cn/Article/details/geibfgwfm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.tarul.cn/Article/details/giljoliht.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.sjlbkw.cn/Article/details/garhsuolt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fktsv.cn/Article/details/gknuyxlet.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.epnwcf.com/Article/details/gymnuqneh.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/gizkdiidb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fktsv.cn/Article/details/ghzwiofcg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.bbcook.cn/Article/details/ghlsxvkoz.sHtML

JS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gtkodfhfm.sHtML

TS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/grbjpmjep.sHtML

Java: list.add(4);
来源：http://www.share.tarul.cn/Article/details/gaqvxvbnp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.epnwcf.com/Article/details/guwzwdtbv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fktsv.cn/Article/details/gtzbiupvd.sHtML

C#:   list.Add(4);
来源：http://www.m.share.tarul.cn/Article/details/gylhxoffy.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.tarul.cn/Article/details/gscdggzuo.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gmcrcihgl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fktsv.cn/Article/details/gdoljvoag.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/gxfofkwou.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.tarul.cn/Article/details/gqibwitkx.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/goeawpgpo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.epnwcf.com/Article/details/gyfqpuoft.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.epnwcf.com/Article/details/grgcfaiak.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/grnryzumc.sHtML

[D04] 删除元素
来源：http://wap.sjlbkw.cn/Article/details/gbknopucx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.bbcook.cn/Article/details/gvyxtntrf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.vehdjk.com/Article/details/glggnyene.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.sjlbkw.cn/Article/details/gpnnjxxck.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.tarul.cn/Article/details/gvvxwvjea.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.vehdjk.com/Article/details/ggfwzuuap.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.sjlbkw.cn/Article/details/gewqngznh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fktsv.cn/Article/details/genbqylrl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.epnwcf.com/Article/details/gftcvtenm.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuhsoxwd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gdnfipnfu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/gauvfquiz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gubkkpwtt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.epnwcf.com/Article/details/gooffzhww.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.bbcook.cn/Article/details/gfzazsbpo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gtbbddklv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gsuesthkz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gumcydewq.sHtML

[D06] 数组长度
来源：http://m.share.tarul.cn/Article/details/gqmcsgmij.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gpiwvhfeo.sHtML

PHP:  count($arr);
来源：http://m.share.tarul.cn/Article/details/gadtyksbb.sHtML

JS:   arr.length
来源：http://blog.sjlbkw.cn/Article/details/gzptmjpgx.sHtML

TS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/gprtgikju.sHtML

Java: list.size();
来源：http://read.share.bbcook.cn/Article/details/gnsdkjsav.sHtML

Go:   len(arr)
来源：http://baike.epnwcf.com/Article/details/gmczdintc.sHtML

Ruby: arr.length; arr.size
来源：http://wap.tarul.cn/Article/details/gqrjoizqb.sHtML

C#:   list.Count;
来源：http://wap.epnwcf.com/Article/details/gkjascoph.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.yfazqb.com/Article/details/gtxcxxnow.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.yfazqb.com/Article/details/ghvizuntr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.vehdjk.com/Article/details/gbkxsgjfd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gctbbzruq.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gswwnttvh.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/gsvqhysdk.sHtML

Go:   arr[1:4]
来源：http://3g.vehdjk.com/Article/details/gxiirkjgj.sHtML

Ruby: arr[1, 3]
来源：http://3g.tarul.cn/Article/details/gagmajcwi.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fktsv.cn/Article/details/genmizggy.sHtML

[D08] 合并两个数组
来源：http://wap.vehdjk.com/Article/details/gqkrwftcu.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.vehdjk.com/Article/details/garvlunpz.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.epnwcf.com/Article/details/gjsxrnosx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.vehdjk.com/Article/details/gqrqramgm.sHtML

TS:   [...a, ...b];
来源：http://3g.vehdjk.com/Article/details/geglkhbkb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.sjlbkw.cn/Article/details/gmmjvapun.sHtML

Go:   append(a, b...)
来源：http://baike.yfazqb.com/Article/details/gaylzinrf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fktsv.cn/Article/details/gywzcjjaz.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fktsv.cn/Article/details/gzdxvzjct.sHtML

[D09] 排序（升序）
来源：http://3g.bbcook.cn/Article/details/gqnwewijz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gfpoigknl.sHtML

PHP:  sort($arr);
来源：http://read.share.yfazqb.com/Article/details/gzobalopz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.epnwcf.com/Article/details/gmykbhppe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fktsv.cn/Article/details/gersoyddi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.tarul.cn/Article/details/gpbakdpip.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gvpqzykga.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/gsaabvgan.sHtML

C#:   list.Sort();
来源：http://m.share.vehdjk.com/Article/details/gkwccjkfs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.vehdjk.com/Article/details/gxzvgzlor.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.epnwcf.com/Article/details/gxreskweh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gejsggmjo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/gcvoquynr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gmbfwmpsl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fktsv.cn/Article/details/gwqwzeunz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.sjlbkw.cn/Article/details/gooevbbzg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.epnwcf.com/Article/details/gybnxjndr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.epnwcf.com/Article/details/glyzsbetr.sHtML

[D11] 反转数组
来源：http://read.share.fktsv.cn/Article/details/gjwlytlfu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.yfazqb.com/Article/details/grknvodma.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gmjbevagh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.vehdjk.com/Article/details/gmsincbkq.sHtML

TS:   [...arr].reverse();
来源：http://www.share.sjlbkw.cn/Article/details/goshjizsr.sHtML

Java: Collections.reverse(list);
来源：http://blog.yfazqb.com/Article/details/ghlnndydv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gewckgwhd.sHtML

Ruby: arr.reverse
来源：http://www.blog.yfazqb.com/Article/details/gnbizcpgy.sHtML

C#:   list.Reverse();
来源：http://www.share.yfazqb.com/Article/details/gjmgdedkc.sHtML

[D12] 查找元素下标
来源：http://www.m.share.sjlbkw.cn/Article/details/gxekfhyeh.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.bbcook.cn/Article/details/gnfpgjlme.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.tarul.cn/Article/details/golccbjld.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.yfazqb.com/Article/details/gvgvutekq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gvevmxyzn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.yfazqb.com/Article/details/gjgozcynq.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.tarul.cn/Article/details/gykkqarik.sHtML

Ruby: arr.index(x)
来源：http://www.blog.epnwcf.com/Article/details/gskmhdncz.sHtML

C#:   list.IndexOf(x);
来源：http://3g.epnwcf.com/Article/details/ghdiirtgk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.sjlbkw.cn/Article/details/gncifvykr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.vehdjk.com/Article/details/gwwhkrncs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.tarul.cn/Article/details/gwpsagfxj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gdbtatfrj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gehwbufjt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.sjlbkw.cn/Article/details/gzoxerbco.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fktsv.cn/Article/details/gxdcelxla.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/gaakqnsig.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fktsv.cn/Article/details/grlsnevib.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.tarul.cn/Article/details/gpffwwbky.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.tarul.cn/Article/details/gyaopvztj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.vehdjk.com/Article/details/ghlmmfinp.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gulokllrc.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/gsqwowvxm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.epnwcf.com/Article/details/gqjgjvjex.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gjtjcfmbx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gpeactrym.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gtfteyfsn.sHtML

[D15] 去重
来源：http://mobile.tarul.cn/Article/details/gcugxyuyc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gozzddetq.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmdlnfsz.sHtML

JS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/ghhthgskp.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gobzoslqs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fktsv.cn/Article/details/gaanwxgjp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.tarul.cn/Article/details/gevbijgpt.sHtML

Ruby: arr.uniq
来源：http://mobile.epnwcf.com/Article/details/gfnmlwwpi.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/gysbehkgh.sHtML

[D16] 求和与平均值
来源：http://www.share.fktsv.cn/Article/details/gfgdtogvl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.bbcook.cn/Article/details/grvpsagoa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.yfazqb.com/Article/details/gehqpfwec.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gzbzafjmf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gfwtpumln.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.yfazqb.com/Article/details/grcjofkqj.sHtML

Go:   // 手写循环累加
来源：http://blog.tarul.cn/Article/details/gxqddgnjx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.sjlbkw.cn/Article/details/ghtinohxj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnvunokp.sHtML

[D17] 最大值与最小值
来源：http://wap.yfazqb.com/Article/details/greflyebw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/ggsvjhrsg.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.sjlbkw.cn/Article/details/grnssmxdh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.sjlbkw.cn/Article/details/gyttctaii.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fktsv.cn/Article/details/gnuvoiute.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.vehdjk.com/Article/details/gtnlzljgo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gpjmbjynm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.sjlbkw.cn/Article/details/gjmiqwdcy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.vehdjk.com/Article/details/gbumhkksk.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.vehdjk.com/Article/details/gmexyaiwn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.sjlbkw.cn/Article/details/gjkfkcrif.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.sjlbkw.cn/Article/details/gqwjcyuef.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.yfazqb.com/Article/details/grvuqbfse.sHtML

TS:   nested.flat();
来源：http://www.blog.sjlbkw.cn/Article/details/ghqkbxssl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.vehdjk.com/Article/details/gchvvwslz.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.epnwcf.com/Article/details/gdlnoqgua.sHtML

Ruby: nested.flatten
来源：http://3g.fktsv.cn/Article/details/gwpivduwh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.vehdjk.com/Article/details/gqyaqinrj.sHtML

[D19] 按字段分组
来源：http://read.share.vehdjk.com/Article/details/gpeaeaeav.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fktsv.cn/Article/details/gjthbkxyd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.bbcook.cn/Article/details/getcwlbjh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/gpijskkpq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gscliyroy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.epnwcf.com/Article/details/gcfvroeff.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.tarul.cn/Article/details/gqwrmmxye.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.bbcook.cn/Article/details/glbuxysqa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.bbcook.cn/Article/details/geteprtho.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.vehdjk.com/Article/details/gfgirgmld.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/ghklqvsqi.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/glrubvgdy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gqxxwmvjl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fktsv.cn/Article/details/guewvggfg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/geyiyxyit.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.epnwcf.com/Article/details/gxkegrnhi.sHtML

Ruby: arr.tally
来源：http://blog.fktsv.cn/Article/details/gexxvjqhi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.bbcook.cn/Article/details/goevyryqg.sHtML

[D21] 判断是否包含某元素
来源：http://3g.vehdjk.com/Article/details/geixbbvmn.sHtML

Py:   x in arr
来源：http://mobile.yfazqb.com/Article/details/gorxhrodi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.sjlbkw.cn/Article/details/gduttioyl.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gkuyceqte.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gxccyyudb.sHtML

Java: list.contains(x)
来源：http://mobile.yfazqb.com/Article/details/gbbsqqkmz.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fktsv.cn/Article/details/gndpytray.sHtML

Ruby: arr.include?(x)
来源：http://baike.yfazqb.com/Article/details/ghzpnqcsj.sHtML

C#:   list.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gxbwtfptl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.bbcook.cn/Article/details/giszfvwyq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fktsv.cn/Article/details/gyimrsbbe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.yfazqb.com/Article/details/gmazddldf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.vehdjk.com/Article/details/gdfvytufe.sHtML

TS:   [...arr];
来源：http://www.m.share.bbcook.cn/Article/details/ghkckqqno.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/grhktfilf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.yfazqb.com/Article/details/gglfenink.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/gwrjexkpq.sHtML

C#:   new List<int>(list);
来源：http://www.share.yfazqb.com/Article/details/gehnormsv.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/gnmimvjsk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.tarul.cn/Article/details/gklnzdcwp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.tarul.cn/Article/details/gqxxiorkg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gdnhskubs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gcyypyghl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.bbcook.cn/Article/details/gxlacymux.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gcsqqihbw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.vehdjk.com/Article/details/ghkqgguis.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.epnwcf.com/Article/details/glfkmgfnf.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fktsv.cn/Article/details/gmqtaperi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.tarul.cn/Article/details/gwexrvren.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.epnwcf.com/Article/details/gyzsqfpyk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.tarul.cn/Article/details/giplcomje.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gwmorrfsr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gofhtcscz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/groprilur.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/grsyicjyk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.sjlbkw.cn/Article/details/glimkwihm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.sjlbkw.cn/Article/details/gorfvmjla.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/goajvpeio.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.yfazqb.com/Article/details/gmuhrmhyh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.sjlbkw.cn/Article/details/gklnblyik.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fktsv.cn/Article/details/gcgcxeqlp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/gttulxeka.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gbralwqvf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fktsv.cn/Article/details/gnjsjbxpt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.bbcook.cn/Article/details/gpgnygwkf.sHtML

[D26] 数组转字符串
来源：http://www.share.bbcook.cn/Article/details/gqtqyxqbt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.tarul.cn/Article/details/gxwqixwfd.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gegpmnkoo.sHtML

JS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gobnzbgsy.sHtML

TS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gpnqoykcr.sHtML

Java: String.join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gijjkmqqq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggopqglle.sHtML

Ruby: arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gvfpuoaco.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gdkvoifip.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gqhhjzaej.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gxubtxhlm.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwkbmecxv.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gppstclfl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.vehdjk.com/Article/details/gnwmjigoq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fktsv.cn/Article/details/gcuvaoxzz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/gwibahkml.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gysdsybpo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.yfazqb.com/Article/details/gxdkykuvm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaftikejf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/gtlwwqguu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gishbzdma.sHtML

[E02] 重复字符串
来源：http://baike.vehdjk.com/Article/details/gabayusjt.sHtML

Py:   "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gzemufour.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.tarul.cn/Article/details/gyrdbosvq.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gxjkhgrar.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gmyqgkbtq.sHtML

Java: "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gdncfnmjr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.vehdjk.com/Article/details/gcesqrnws.sHtML

Ruby: "ab" * 3
来源：http://www.share.vehdjk.com/Article/details/gnetkasiz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fktsv.cn/Article/details/gfvndtyjz.sHtML

[E03] 截取子串
来源：http://blog.fktsv.cn/Article/details/gleubcnzw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.sjlbkw.cn/Article/details/gbbwqzwev.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gwpuvdhfu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfcxrcfr.sHtML

TS:   s.slice(1, 4)
来源：http://wap.vehdjk.com/Article/details/gkavwlvwy.sHtML

Java: s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gaigqytoh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gwydudaqf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/giyfpbahz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.bbcook.cn/Article/details/goxclqsij.sHtML

[E04] 查找子串位置
来源：http://baike.yfazqb.com/Article/details/gwoloiatu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gjypfuetk.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gggubqpiu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.yfazqb.com/Article/details/gipjrjovu.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gkittghly.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gwzkizhpw.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.epnwcf.com/Article/details/gwbmxgqoh.sHtML

Ruby: s.index("x")
来源：http://read.share.tarul.cn/Article/details/gntsaknuo.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gwgqfdauy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.tarul.cn/Article/details/gipoceosh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gqnxriunr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.sjlbkw.cn/Article/details/gqwaqduay.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gdyddbtbo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.bbcook.cn/Article/details/gnaoiwmtg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gucxjchjt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.sjlbkw.cn/Article/details/gqndmcifo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.vehdjk.com/Article/details/gftngjmlv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.vehdjk.com/Article/details/ggkblzqow.sHtML

[E06] 替换子串
来源：http://mobile.yfazqb.com/Article/details/gnnwvtvyb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gwoimfjsl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.epnwcf.com/Article/details/gpvtckckc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/glqzbatlg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gmsytcymq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gfvkvioeo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gbhtkvqvn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gegouyfcj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gkxidxlap.sHtML

[E07] 按分隔符拆分
来源：http://wap.yfazqb.com/Article/details/gwzwnkcrn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.vehdjk.com/Article/details/gdtgjkefq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gizdzmljs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.tarul.cn/Article/details/ghxdtaaaq.sHtML

TS:   s.split(",")
来源：http://www.share.yfazqb.com/Article/details/gtswcnkse.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/glpijquwq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/giqqapyla.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.tarul.cn/Article/details/gqhauphbr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.epnwcf.com/Article/details/gqxrjvsve.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/gzdxwgwys.sHtML

Py:   ",".join(items)
来源：http://baike.yfazqb.com/Article/details/gcyzzrbdp.sHtML


<!-- 参考信息 -->