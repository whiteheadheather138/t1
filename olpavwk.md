代发 wailian999

D. 数组 / 列表 / 集合
来源：http://www.share.bbcook.cn/Article/details/gsydoppjw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glvcvgbme.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fktsv.cn/Article/details/guyfkgqhl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.vehdjk.com/Article/details/gaxflslwg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.vehdjk.com/Article/details/giuxqmgox.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.yfazqb.com/Article/details/gvvlhnczp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.epnwcf.com/Article/details/gfxskslgp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.vehdjk.com/Article/details/gblpccatm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.yfazqb.com/Article/details/gogzzaaip.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gupvdmzyz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.vehdjk.com/Article/details/gvptzouyh.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.epnwcf.com/Article/details/gvjvnrcme.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fktsv.cn/Article/details/gwcfzrsud.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.epnwcf.com/Article/details/gidzeffzy.sHtML

JS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gbvbytzsw.sHtML

TS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/guhcekzbz.sHtML

Java: list.add(4);
来源：http://wap.vehdjk.com/Article/details/giymlwvbc.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.yfazqb.com/Article/details/gxcvyusyi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.sjlbkw.cn/Article/details/ghxbukxvz.sHtML

C#:   list.Add(4);
来源：http://read.share.bbcook.cn/Article/details/gvtlczazn.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.yfazqb.com/Article/details/gegboippr.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.yfazqb.com/Article/details/gkzrrocjj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.yfazqb.com/Article/details/gkfvydqjm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fktsv.cn/Article/details/gsjczhoge.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/grfpntahy.sHtML

Java: list.add(0, 0);
来源：http://blog.tarul.cn/Article/details/gjciwqycx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.tarul.cn/Article/details/gdemdiemn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.sjlbkw.cn/Article/details/gjkbykior.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gczvxmlmn.sHtML

[D04] 删除元素
来源：http://www.share.fktsv.cn/Article/details/gtidicqdx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.sjlbkw.cn/Article/details/gcfcviton.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fktsv.cn/Article/details/gnjsyqtrd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.epnwcf.com/Article/details/gzplzqlzi.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.epnwcf.com/Article/details/gmeenotnz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.tarul.cn/Article/details/gtlmwjfxx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.epnwcf.com/Article/details/gsngrcnqq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fktsv.cn/Article/details/gxyptgkjy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.bbcook.cn/Article/details/gyokreodm.sHtML

[D05] 访问与修改元素
来源：http://www.share.vehdjk.com/Article/details/gnnehyigg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gwehygego.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gtmqgojba.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gmwmfikzf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fktsv.cn/Article/details/gixhwowcs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.vehdjk.com/Article/details/guikywlsu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/ggnocfhzu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/ggwzomdge.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gfqwdwzpw.sHtML

[D06] 数组长度
来源：http://wap.tarul.cn/Article/details/gvmpwyfmm.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gbkdmimge.sHtML

PHP:  count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gwitflclr.sHtML

JS:   arr.length
来源：http://3g.yfazqb.com/Article/details/gidiebgrm.sHtML

TS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gmoyzjcsw.sHtML

Java: list.size();
来源：http://www.blog.tarul.cn/Article/details/gsoacvxzq.sHtML

Go:   len(arr)
来源：http://wap.tarul.cn/Article/details/gkfxthfxu.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.epnwcf.com/Article/details/gaajzpjeh.sHtML

C#:   list.Count;
来源：http://blog.yfazqb.com/Article/details/gnleiiqkw.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.yfazqb.com/Article/details/gccaramre.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/gyikqplnd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.sjlbkw.cn/Article/details/ghivwifcj.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/gxmgqcygx.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gclrypqtj.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gnckjrzno.sHtML

Go:   arr[1:4]
来源：http://read.share.yfazqb.com/Article/details/gbcfmuytp.sHtML

Ruby: arr[1, 3]
来源：http://3g.fktsv.cn/Article/details/gocecwpkc.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.bbcook.cn/Article/details/gulqmixtx.sHtML

[D08] 合并两个数组
来源：http://read.share.yfazqb.com/Article/details/gcyysxavq.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.tarul.cn/Article/details/gyrasrxsd.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fktsv.cn/Article/details/gixpmjmmt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.yfazqb.com/Article/details/gfeunmxrj.sHtML

TS:   [...a, ...b];
来源：http://blog.fktsv.cn/Article/details/gncjnacan.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fktsv.cn/Article/details/ggkoagjal.sHtML

Go:   append(a, b...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyksrhggd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fktsv.cn/Article/details/grfewhfnk.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.yfazqb.com/Article/details/gcsvxfdax.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fktsv.cn/Article/details/ggnvvhhsv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gyfrsddhu.sHtML

PHP:  sort($arr);
来源：http://baike.yfazqb.com/Article/details/gyufahgtg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.tarul.cn/Article/details/gmrzglcmu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.vehdjk.com/Article/details/guylgmkhs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.bbcook.cn/Article/details/gbmfcbxem.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gkjalmimc.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/gpzpobtcc.sHtML

C#:   list.Sort();
来源：http://baike.sjlbkw.cn/Article/details/gmhpjzeic.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.yfazqb.com/Article/details/gnbnssbjx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.yfazqb.com/Article/details/ggqszdmbw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/goanpwfre.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.bbcook.cn/Article/details/gzeeruiwm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpqfxegq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.sjlbkw.cn/Article/details/gjoiiwjvf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.epnwcf.com/Article/details/gdkndmdch.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.epnwcf.com/Article/details/gsggoxfky.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.yfazqb.com/Article/details/gtceglnox.sHtML

[D11] 反转数组
来源：http://m.share.epnwcf.com/Article/details/guroolwjg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.tarul.cn/Article/details/gypvmaprz.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrcrnjhc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.vehdjk.com/Article/details/gdmcvjfbr.sHtML

TS:   [...arr].reverse();
来源：http://baike.fktsv.cn/Article/details/gpxpdcbek.sHtML

Java: Collections.reverse(list);
来源：http://baike.vehdjk.com/Article/details/gesmbvvxo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/glkffxpaa.sHtML

Ruby: arr.reverse
来源：http://www.m.share.tarul.cn/Article/details/gqtsxsgdf.sHtML

C#:   list.Reverse();
来源：http://mobile.bbcook.cn/Article/details/gbxdcnlqd.sHtML

[D12] 查找元素下标
来源：http://baike.fktsv.cn/Article/details/gchgdgsco.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fktsv.cn/Article/details/gipyfkqsd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fktsv.cn/Article/details/ghjdmotin.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/ghlrzftyn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.vehdjk.com/Article/details/gowazbidr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.sjlbkw.cn/Article/details/gjswfguzh.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.epnwcf.com/Article/details/gzlcjkvde.sHtML

Ruby: arr.index(x)
来源：http://m.share.fktsv.cn/Article/details/gcxjonaxu.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.epnwcf.com/Article/details/gczyzmnlq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.vehdjk.com/Article/details/gpzzrkbaf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gthiakjwl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.vehdjk.com/Article/details/gffwawpha.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gnunkjrup.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.bbcook.cn/Article/details/guudmrjrn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.yfazqb.com/Article/details/gjzspqrsq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.yfazqb.com/Article/details/gfgwripep.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.vehdjk.com/Article/details/ggibkfttf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.yfazqb.com/Article/details/gkcocyhsi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fktsv.cn/Article/details/giwjrafov.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.bbcook.cn/Article/details/gkgabxpfr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.tarul.cn/Article/details/gimgsktwq.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/gkqevtcbj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/gztnvjolg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.bbcook.cn/Article/details/gmhhpstss.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gbnqaskip.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.yfazqb.com/Article/details/gjewrqypa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gmluubfea.sHtML

[D15] 去重
来源：http://baike.vehdjk.com/Article/details/gxjqyjwjs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/goxcupcbw.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gktstvomo.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/ggajuyfdm.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/geddelyqk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.tarul.cn/Article/details/gnjptnvve.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.bbcook.cn/Article/details/ggjufgjuq.sHtML

Ruby: arr.uniq
来源：http://www.blog.sjlbkw.cn/Article/details/gkmxekgak.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.epnwcf.com/Article/details/ghirpbpjt.sHtML

[D16] 求和与平均值
来源：http://m.share.epnwcf.com/Article/details/gwxwecjbd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.tarul.cn/Article/details/gpayunyfb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.vehdjk.com/Article/details/gysjldxxx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gbwhgcojj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gdipgxtjf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.tarul.cn/Article/details/gbgwecdor.sHtML

Go:   // 手写循环累加
来源：http://m.share.epnwcf.com/Article/details/gxohvljsl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.yfazqb.com/Article/details/guhtjxahc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.yfazqb.com/Article/details/gqvelhhxz.sHtML

[D17] 最大值与最小值
来源：http://wap.bbcook.cn/Article/details/gjjnrfgac.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.tarul.cn/Article/details/gcotspptw.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.epnwcf.com/Article/details/gdpcnfufi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gjcgwtlzg.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fktsv.cn/Article/details/ghmufmpfu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.bbcook.cn/Article/details/gfveummsp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.tarul.cn/Article/details/ganjypbql.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fktsv.cn/Article/details/gsgnvckxn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.yfazqb.com/Article/details/gbnktspvc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.epnwcf.com/Article/details/gzmxkecqg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/gbezdwnhb.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.epnwcf.com/Article/details/gvvemcatm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.bbcook.cn/Article/details/glfargqta.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/ghdopynek.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.bbcook.cn/Article/details/gbvheowna.sHtML

Go:   // 手写双层循环
来源：http://www.blog.epnwcf.com/Article/details/ghupczksv.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gugbnmsvz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.vehdjk.com/Article/details/gnghkiqoq.sHtML

[D19] 按字段分组
来源：http://baike.vehdjk.com/Article/details/gzkfjwaci.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.sjlbkw.cn/Article/details/gohbmscne.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.epnwcf.com/Article/details/gggaxuwwi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.sjlbkw.cn/Article/details/geilxczcz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gcimtxuxd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/gkdwqkuff.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/gwizukkls.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.bbcook.cn/Article/details/gifmamtzl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.bbcook.cn/Article/details/gryngaenz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.epnwcf.com/Article/details/gmttvzprb.sHtML

Py:   Counter(arr)
来源：http://baike.sjlbkw.cn/Article/details/gvjwmamgw.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fktsv.cn/Article/details/guxoxwrir.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gnedjrbmb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.epnwcf.com/Article/details/goopguwmf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvuffddo.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/gebfgossl.sHtML

Ruby: arr.tally
来源：http://www.share.bbcook.cn/Article/details/gprgodzbf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.tarul.cn/Article/details/gjziftfnf.sHtML

[D21] 判断是否包含某元素
来源：http://wap.epnwcf.com/Article/details/gkpvtndxg.sHtML

Py:   x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/ggrgmplpx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fktsv.cn/Article/details/gimiszlis.sHtML

JS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gskqsoagg.sHtML

TS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gpsnxgoxb.sHtML

Java: list.contains(x)
来源：http://baike.tarul.cn/Article/details/gbldopoda.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/glqvfyyco.sHtML

Ruby: arr.include?(x)
来源：http://blog.bbcook.cn/Article/details/gdvgktarp.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/ghycmmkvq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/glgkcyiep.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fktsv.cn/Article/details/gnkfybvcu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.sjlbkw.cn/Article/details/gznvtvbyf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.bbcook.cn/Article/details/gkrfoyqxq.sHtML

TS:   [...arr];
来源：http://baike.epnwcf.com/Article/details/gbzisvbjp.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gqakcwzrv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.vehdjk.com/Article/details/goiyvhyyt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.vehdjk.com/Article/details/ghsuspxjw.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/geqkcnpdq.sHtML

[D23] reduce 累积计算
来源：http://wap.sjlbkw.cn/Article/details/gzmbsffgx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fktsv.cn/Article/details/gmbijtcpo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.vehdjk.com/Article/details/gvntpccre.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gnhmscyqr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gfcckbeuw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.tarul.cn/Article/details/ggchlwlzz.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gtmozexot.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/ggwdrnhom.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.vehdjk.com/Article/details/gifvlimpt.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.bbcook.cn/Article/details/gbsspwzqb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.tarul.cn/Article/details/gupmexjdh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.bbcook.cn/Article/details/gmbmpcchr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.sjlbkw.cn/Article/details/ghyauiegy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.bbcook.cn/Article/details/gwpdliizu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.yfazqb.com/Article/details/gfvydqzmi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.tarul.cn/Article/details/gftfzatwd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fktsv.cn/Article/details/gmkvydgil.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.epnwcf.com/Article/details/gsdyxblst.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/gjniwgrhq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.tarul.cn/Article/details/ggjclmbvb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gjviglron.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fktsv.cn/Article/details/ghwdpeouk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fktsv.cn/Article/details/gayimjwcq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.yfazqb.com/Article/details/gutexkewd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fktsv.cn/Article/details/gbgaumfjo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.epnwcf.com/Article/details/gesnzrzom.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gjftkoqyw.sHtML

[D26] 数组转字符串
来源：http://blog.tarul.cn/Article/details/gmtburnlo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gpklpdkmk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gecsiotjo.sHtML

JS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gankbjqmw.sHtML

TS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gwasgkwiy.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gcwwlldtm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.tarul.cn/Article/details/gituabryj.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gueiwyumx.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.bbcook.cn/Article/details/gqjhdgalu.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gldgxetkz.sHtML

E. 字符串处理
来源：http://wap.bbcook.cn/Article/details/geslyvotn.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gsppkwtsr.sHtML

[E01] 拼接字符串
来源：http://3g.epnwcf.com/Article/details/gbaydrwgm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.sjlbkw.cn/Article/details/gssmlrutx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fktsv.cn/Article/details/glondrilh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gkxyovvyy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gyqorrcuo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.sjlbkw.cn/Article/details/gonfuzity.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.bbcook.cn/Article/details/ghnwvsiih.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.tarul.cn/Article/details/gxdndjjzl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.bbcook.cn/Article/details/ghqrrkwut.sHtML

[E02] 重复字符串
来源：http://3g.fktsv.cn/Article/details/gjqtwufkm.sHtML

Py:   "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gzlbefvgy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.bbcook.cn/Article/details/ggswdqnip.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gqpjsdxbc.sHtML

TS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/ghwjgfyvf.sHtML

Java: "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/geokdfjdv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.epnwcf.com/Article/details/gzfwxkvzj.sHtML

Ruby: "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gseipmpci.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.vehdjk.com/Article/details/gopvyufbx.sHtML

[E03] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gljeglodq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.yfazqb.com/Article/details/gatupdjxr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/geozyfgof.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gwdzwourb.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.vehdjk.com/Article/details/ghgeagqhh.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/grjkqkknj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fktsv.cn/Article/details/gufdqqjbi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.sjlbkw.cn/Article/details/gqwpcbret.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/gjelvtwzp.sHtML

[E04] 查找子串位置
来源：http://wap.yfazqb.com/Article/details/gosyfzdtw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gwalwoqrj.sHtML

PHP:  strpos($s, "x");
来源：http://wap.vehdjk.com/Article/details/gzyparawv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.vehdjk.com/Article/details/gxpgxwebe.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpgimbew.sHtML

Java: s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/grvojoibp.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.epnwcf.com/Article/details/gqgzolyen.sHtML

Ruby: s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gmjwuorjv.sHtML

C#:   s.IndexOf("x")
来源：http://3g.tarul.cn/Article/details/gggzujare.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.epnwcf.com/Article/details/gzhsqjdqb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fktsv.cn/Article/details/gpgevehey.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.epnwcf.com/Article/details/gzpvbhrjj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gxqflssps.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.tarul.cn/Article/details/grpknrepr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/gsrfyzhac.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.yfazqb.com/Article/details/gvxozymwc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.yfazqb.com/Article/details/gujzgwomd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.tarul.cn/Article/details/gimxblcep.sHtML

[E06] 替换子串
来源：http://m.share.yfazqb.com/Article/details/gcadpnkui.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gkspwnppz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.epnwcf.com/Article/details/gbbtmucdj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gtubkiqym.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/grwprkjqx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gxulofszk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gzqlsrbis.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gtwslqfhx.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.bbcook.cn/Article/details/gsypprzfc.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.bbcook.cn/Article/details/gxulrxaxf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.yfazqb.com/Article/details/gdrsrozeq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.bbcook.cn/Article/details/gtniiqjhb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.sjlbkw.cn/Article/details/gaboaxrrc.sHtML

TS:   s.split(",")
来源：http://www.m.share.fktsv.cn/Article/details/gkwydtafo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.vehdjk.com/Article/details/guyiwyqdz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.sjlbkw.cn/Article/details/glblgnvko.sHtML


<!-- 参考信息 -->