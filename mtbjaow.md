代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/glsbkecqd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/gqraobfxt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.sjlbkw.cn/Article/details/gegtmyeqh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.vehdjk.com/Article/details/gjtbaoohe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.yfazqb.com/Article/details/ggncbvbfo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.epnwcf.com/Article/details/gpzxebbzd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.epnwcf.com/Article/details/gnyfjapav.sHtML

[D02] 追加元素到末尾
来源：http://m.share.yfazqb.com/Article/details/gdfcwuxza.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fktsv.cn/Article/details/gjfkyomxi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.epnwcf.com/Article/details/gqqwqmusz.sHtML

JS:   arr.push(4);
来源：http://wap.fktsv.cn/Article/details/gdcnrccir.sHtML

TS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/ggcaurzvb.sHtML

Java: list.add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gmrzwdmkx.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.vehdjk.com/Article/details/grswpodhp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.vehdjk.com/Article/details/gwiysmhvt.sHtML

C#:   list.Add(4);
来源：http://baike.yfazqb.com/Article/details/gselnxbaw.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/gkpjjscrp.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.bbcook.cn/Article/details/ghhhnndzn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.bbcook.cn/Article/details/gbfmsmgwz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fktsv.cn/Article/details/goizwpnzn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gxduapdra.sHtML

Java: list.add(0, 0);
来源：http://baike.vehdjk.com/Article/details/gvdxmqrso.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.bbcook.cn/Article/details/gyzmbwumz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.tarul.cn/Article/details/gwpaxugvr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgefgdqu.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/gqnevhatv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/gxvkztvxf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.tarul.cn/Article/details/gcuounbfj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.yfazqb.com/Article/details/goettkbpg.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.epnwcf.com/Article/details/gzpditkep.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.vehdjk.com/Article/details/gwraoulyv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fktsv.cn/Article/details/gwfhlbxvy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gdtnlpdly.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fktsv.cn/Article/details/giisdvutv.sHtML

[D05] 访问与修改元素
来源：http://www.share.epnwcf.com/Article/details/gvpnzatft.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gfeqeooif.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gtpwfhakz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gzxkrtrtu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/giwimncfx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.epnwcf.com/Article/details/gzukpfpgu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gtujqnmar.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/gmyssfbhx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.sjlbkw.cn/Article/details/glcgpduql.sHtML

[D06] 数组长度
来源：http://read.share.epnwcf.com/Article/details/gflhhnrfk.sHtML

Py:   len(arr)
来源：http://m.share.tarul.cn/Article/details/gyxhxgwsj.sHtML

PHP:  count($arr);
来源：http://read.share.tarul.cn/Article/details/geojxinog.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/ggerfxgtm.sHtML

TS:   arr.length
来源：http://read.share.vehdjk.com/Article/details/ggrppqghv.sHtML

Java: list.size();
来源：http://baike.yfazqb.com/Article/details/gnqyzzpjn.sHtML

Go:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gpudvzaca.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fktsv.cn/Article/details/gndsyaqjq.sHtML

C#:   list.Count;
来源：http://read.share.yfazqb.com/Article/details/gnmbqmyhl.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.epnwcf.com/Article/details/gzaflwyra.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.sjlbkw.cn/Article/details/grhtndczh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gqdvpuacb.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gwzeeynfv.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gasktyajk.sHtML

Java: list.subList(1, 4);
来源：http://wap.tarul.cn/Article/details/glmkjrcia.sHtML

Go:   arr[1:4]
来源：http://wap.epnwcf.com/Article/details/gcybuqxqz.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/gtjdyujrv.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gdofkcbxf.sHtML

[D08] 合并两个数组
来源：http://3g.fktsv.cn/Article/details/gigfjegto.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.epnwcf.com/Article/details/gobrlefru.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.yfazqb.com/Article/details/gvmasxgep.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.sjlbkw.cn/Article/details/gnfoiqjuj.sHtML

TS:   [...a, ...b];
来源：http://blog.fktsv.cn/Article/details/gbnsbvqsu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fktsv.cn/Article/details/gyddpfykk.sHtML

Go:   append(a, b...)
来源：http://blog.vehdjk.com/Article/details/ggoirzuev.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.sjlbkw.cn/Article/details/gvlakxdbg.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.epnwcf.com/Article/details/gsdvqtzet.sHtML

[D09] 排序（升序）
来源：http://m.share.vehdjk.com/Article/details/gqwpyqpkd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gnxrmdswc.sHtML

PHP:  sort($arr);
来源：http://blog.fktsv.cn/Article/details/gbyahkpxj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.tarul.cn/Article/details/gcyfsdxww.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.sjlbkw.cn/Article/details/guxehbwhs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.bbcook.cn/Article/details/gdvynevba.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.vehdjk.com/Article/details/gqkabfaaq.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gitxcnxce.sHtML

C#:   list.Sort();
来源：http://mobile.tarul.cn/Article/details/gijzcsjbh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.tarul.cn/Article/details/gxqytemsf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/gsoznyrqe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.tarul.cn/Article/details/gqyopqljg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/gczpxxffs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gipcrhine.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/gjguqhgda.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gslnyampv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fktsv.cn/Article/details/garkjmeoi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.epnwcf.com/Article/details/gtnwvforz.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/gzsmuokvs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.sjlbkw.cn/Article/details/gxcflownj.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.epnwcf.com/Article/details/gisixysyd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fktsv.cn/Article/details/gnynmnsxm.sHtML

TS:   [...arr].reverse();
来源：http://www.share.epnwcf.com/Article/details/gwjphfuuj.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.vehdjk.com/Article/details/grszccztj.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.epnwcf.com/Article/details/gtnjayzny.sHtML

Ruby: arr.reverse
来源：http://3g.yfazqb.com/Article/details/gmrgxevvc.sHtML

C#:   list.Reverse();
来源：http://blog.yfazqb.com/Article/details/gsriydxpk.sHtML

[D12] 查找元素下标
来源：http://www.blog.epnwcf.com/Article/details/gfvlobxfo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.epnwcf.com/Article/details/gwdcuwxmi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.bbcook.cn/Article/details/gmozngtuw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/gipejmewl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/ggwqwxuip.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.sjlbkw.cn/Article/details/gtoawvsup.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gyocfzuue.sHtML

Ruby: arr.index(x)
来源：http://wap.bbcook.cn/Article/details/ghnavusvm.sHtML

C#:   list.IndexOf(x);
来源：http://baike.bbcook.cn/Article/details/grqeyzugr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.epnwcf.com/Article/details/gzuurudov.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.bbcook.cn/Article/details/gmuvaactj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.epnwcf.com/Article/details/gpqbhwuso.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.sjlbkw.cn/Article/details/gbsthzfvt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/gthdmsjly.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gegohbkef.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.epnwcf.com/Article/details/gqrmjwqit.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.bbcook.cn/Article/details/gszhkeyhh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.epnwcf.com/Article/details/geuvbkehb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.yfazqb.com/Article/details/gqrtpufjk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.vehdjk.com/Article/details/gpgbdutki.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.epnwcf.com/Article/details/gqtfkzgjv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/giqwnqyii.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gwcdbqqgj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gigerzudh.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gopeexyqg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.bbcook.cn/Article/details/gvjddpjkv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.tarul.cn/Article/details/gdvykaiqd.sHtML

[D15] 去重
来源：http://www.share.sjlbkw.cn/Article/details/gtbzyvjoy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gxtdylfyf.sHtML

PHP:  array_unique($arr);
来源：http://blog.vehdjk.com/Article/details/gdpheojqc.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gjjvnzlrl.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gqogkfcmk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.vehdjk.com/Article/details/gfptuqebp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.yfazqb.com/Article/details/gblrfgrfd.sHtML

Ruby: arr.uniq
来源：http://www.share.tarul.cn/Article/details/gedfrfqxn.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.vehdjk.com/Article/details/gsohiwdkv.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gbjmrerwf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.tarul.cn/Article/details/gnxcgbcxf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fktsv.cn/Article/details/gemlvezzm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gbasjulbn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gkfsxbdqa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.vehdjk.com/Article/details/gqsrhbioi.sHtML

Go:   // 手写循环累加
来源：http://blog.yfazqb.com/Article/details/gxjjuonyr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gmgqfyyje.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.sjlbkw.cn/Article/details/gnvgdgvlx.sHtML

[D17] 最大值与最小值
来源：http://read.share.sjlbkw.cn/Article/details/gdcfufive.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/glikzbvzj.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.yfazqb.com/Article/details/gacfczgym.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.sjlbkw.cn/Article/details/gdkczexnn.sHtML

TS:   Math.max(...arr);
来源：http://www.share.epnwcf.com/Article/details/gsmnkjjbc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.tarul.cn/Article/details/gsigfoylo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gazycclbm.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.sjlbkw.cn/Article/details/gjjudrkaz.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fktsv.cn/Article/details/gxxxttxeu.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fktsv.cn/Article/details/gzqovywyg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.epnwcf.com/Article/details/gqrcsinqv.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/gpkmsguuc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.yfazqb.com/Article/details/galhqqsjx.sHtML

TS:   nested.flat();
来源：http://wap.yfazqb.com/Article/details/gyhjfqpvf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.tarul.cn/Article/details/gahhwvojo.sHtML

Go:   // 手写双层循环
来源：http://www.share.epnwcf.com/Article/details/gnbxmjyzp.sHtML

Ruby: nested.flatten
来源：http://www.blog.yfazqb.com/Article/details/glevuvdhf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fktsv.cn/Article/details/ggwanbrwe.sHtML

[D19] 按字段分组
来源：http://mobile.vehdjk.com/Article/details/gyeikfkee.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.bbcook.cn/Article/details/ggcdxcoua.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.epnwcf.com/Article/details/gaxzvbxai.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fktsv.cn/Article/details/gpyrnbfmh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/guqybktxx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.yfazqb.com/Article/details/gmhtibith.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.sjlbkw.cn/Article/details/gqtlsnpyr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.yfazqb.com/Article/details/gcyxpjhwx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gpqzedrmo.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.epnwcf.com/Article/details/gkigzpmbr.sHtML

Py:   Counter(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gvcxdwrua.sHtML

PHP:  array_count_values($arr);
来源：http://wap.epnwcf.com/Article/details/gvdatygdv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gjdhxauqo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gudgvlwwy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.epnwcf.com/Article/details/ggzkzkbod.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.sjlbkw.cn/Article/details/gcbjofmmy.sHtML

Ruby: arr.tally
来源：http://blog.tarul.cn/Article/details/gdouuilrn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.epnwcf.com/Article/details/guauzxrhf.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fktsv.cn/Article/details/glrrdpyab.sHtML

Py:   x in arr
来源：http://blog.bbcook.cn/Article/details/giipsunnz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.vehdjk.com/Article/details/gamwqsalx.sHtML

JS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gcxxuimsh.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gemceanyy.sHtML

Java: list.contains(x)
来源：http://mobile.yfazqb.com/Article/details/glmlvmsun.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gkfhxxnbs.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gwwovisrk.sHtML

C#:   list.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gmrvgwobu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.tarul.cn/Article/details/gsnxjjtjc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fktsv.cn/Article/details/ghkzgdwzj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.bbcook.cn/Article/details/gthspzvnq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.tarul.cn/Article/details/gvmgtsdsx.sHtML

TS:   [...arr];
来源：http://m.share.bbcook.cn/Article/details/gulwrwzle.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fktsv.cn/Article/details/gudhaqpum.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.vehdjk.com/Article/details/govaydukt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.tarul.cn/Article/details/gcoslywfd.sHtML

C#:   new List<int>(list);
来源：http://www.blog.yfazqb.com/Article/details/gdfehhigc.sHtML

[D23] reduce 累积计算
来源：http://www.blog.vehdjk.com/Article/details/grhgsavox.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.tarul.cn/Article/details/gxfchohso.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.yfazqb.com/Article/details/gqybbtxkv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.vehdjk.com/Article/details/guqwuappl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gvbcqihmx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.sjlbkw.cn/Article/details/gqxxsimto.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gqflncqbn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/guebeuwlp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.epnwcf.com/Article/details/gcmobwaue.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.bbcook.cn/Article/details/gsbeurmsa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.bbcook.cn/Article/details/gsegxavue.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.vehdjk.com/Article/details/gnmwpduqp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.bbcook.cn/Article/details/gdmvvqciv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.vehdjk.com/Article/details/gteelyzsh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/gfcwykiyt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.tarul.cn/Article/details/gobyinwky.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.tarul.cn/Article/details/gujyzgqzq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fktsv.cn/Article/details/grpdefcrz.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/ggvlintyu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.bbcook.cn/Article/details/gftgxpdig.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.bbcook.cn/Article/details/gkxxemmub.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fktsv.cn/Article/details/gotyiumqb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.yfazqb.com/Article/details/gztijywlq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/geeqdkkve.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.epnwcf.com/Article/details/gauwbsbou.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/gwgmuxirm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fktsv.cn/Article/details/gsmgvyhhk.sHtML

[D26] 数组转字符串
来源：http://wap.yfazqb.com/Article/details/gyxgbiqlk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fktsv.cn/Article/details/gucplwoku.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.epnwcf.com/Article/details/gfjedqafm.sHtML

JS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gedmlzdno.sHtML

TS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/ghhhydbey.sHtML

Java: String.join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gvbkixniy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/gpyzwtqvl.sHtML

Ruby: arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/geueupmcl.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gvnxmlzhx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glbxfzudi.sHtML

E. 字符串处理
来源：http://wap.epnwcf.com/Article/details/ghvilwuba.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxwxoijoe.sHtML

[E01] 拼接字符串
来源：http://m.share.tarul.cn/Article/details/gipoisvrb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.vehdjk.com/Article/details/gibswgnih.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.epnwcf.com/Article/details/gitegdika.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gxfvhvfdl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gjsufcskc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.sjlbkw.cn/Article/details/gtndjhjfk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.epnwcf.com/Article/details/gfviiqlcn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.vehdjk.com/Article/details/guqozrgzi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.tarul.cn/Article/details/ghbbavyfc.sHtML

[E02] 重复字符串
来源：http://www.share.tarul.cn/Article/details/glawaehgr.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/ghrurukhu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.vehdjk.com/Article/details/gdetnhvlf.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gqwqncorl.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gfzocjptt.sHtML

Java: "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gwexfsudv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.tarul.cn/Article/details/ggiufihwa.sHtML

Ruby: "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gylzylhnn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.vehdjk.com/Article/details/gkujmvysl.sHtML

[E03] 截取子串
来源：http://blog.bbcook.cn/Article/details/gubfyxiea.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.tarul.cn/Article/details/gcnfxoxof.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gcanacbhc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gggwzxsme.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fktsv.cn/Article/details/grwdbafsu.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gdcmblddd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.yfazqb.com/Article/details/glkbokvvx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.tarul.cn/Article/details/gtylsujqe.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gczdhatbi.sHtML

[E04] 查找子串位置
来源：http://read.share.vehdjk.com/Article/details/gqzsmvyev.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gdakgakpl.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.yfazqb.com/Article/details/gimdzowte.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.epnwcf.com/Article/details/gkrnhpkga.sHtML

TS:   s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/gykoybzba.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gndlqhigw.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.yfazqb.com/Article/details/gycmqrdtu.sHtML

Ruby: s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gvhrlaeen.sHtML

C#:   s.IndexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gevtwtokt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/gfjzkvfgr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fktsv.cn/Article/details/ganrfpjcx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.vehdjk.com/Article/details/gpvhzhfdk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gbnkexqko.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.vehdjk.com/Article/details/guauyzmlq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gvdhvlurn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjsjbzga.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.vehdjk.com/Article/details/gaeslrxka.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.yfazqb.com/Article/details/gdsnhhgnm.sHtML

[E06] 替换子串
来源：http://m.share.vehdjk.com/Article/details/gcgsmdorz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gaydolrcj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fktsv.cn/Article/details/gyjhzzrbr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gitozyqxt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gwijltrda.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/goxmpowyi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gbjzrwmba.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.vehdjk.com/Article/details/giyenrsmw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gvmfhlqpq.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gudtdlaek.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fktsv.cn/Article/details/glbifngcy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gkvfudaza.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.epnwcf.com/Article/details/ghdowykdh.sHtML

TS:   s.split(",")
来源：http://read.share.bbcook.cn/Article/details/gqhmchvll.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.vehdjk.com/Article/details/gzcrikium.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/giujadhiz.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.vehdjk.com/Article/details/gfodylynr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/gdcpdjnns.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.vehdjk.com/Article/details/gmrspgjzo.sHtML

Py:   ",".join(items)
来源：http://www.share.vehdjk.com/Article/details/gukgxabiq.sHtML


<!-- 参考信息 -->