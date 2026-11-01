代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.bbcook.cn/Article/details/ggjhevrxv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fktsv.cn/Article/details/gnffrxetr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.sjlbkw.cn/Article/details/grplzttmj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.yfazqb.com/Article/details/gzixdnwiz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.vehdjk.com/Article/details/gcaahvhky.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.yfazqb.com/Article/details/geykwmtkb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fktsv.cn/Article/details/ghkdrkkzp.sHtML

[D02] 追加元素到末尾
来源：http://www.share.tarul.cn/Article/details/gtffcyjsk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fktsv.cn/Article/details/gvrhekxfj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.bbcook.cn/Article/details/grukgwpsb.sHtML

JS:   arr.push(4);
来源：http://baike.fktsv.cn/Article/details/gakjshnop.sHtML

TS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gbdhkyxjm.sHtML

Java: list.add(4);
来源：http://wap.epnwcf.com/Article/details/grpnysuwt.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.vehdjk.com/Article/details/grljllizg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.bbcook.cn/Article/details/gzkeknheb.sHtML

C#:   list.Add(4);
来源：http://www.m.share.tarul.cn/Article/details/gwsniixxn.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.bbcook.cn/Article/details/gwtizjwsc.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.yfazqb.com/Article/details/gjkbzyyrm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.sjlbkw.cn/Article/details/gvtayxqrq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/gljbbrsbk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.yfazqb.com/Article/details/gvrryqghk.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gixrfaahv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.epnwcf.com/Article/details/gljcaghzq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.tarul.cn/Article/details/gtnonwnkt.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.epnwcf.com/Article/details/gwkiaahti.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/gfejtvvoy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/grmbwwhro.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gkvvontbd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/gfgcbxuju.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.sjlbkw.cn/Article/details/gtucjajkp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.vehdjk.com/Article/details/gboycyedb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.sjlbkw.cn/Article/details/gyyalngco.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.epnwcf.com/Article/details/ghcbcjeoo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.vehdjk.com/Article/details/gupglxqaf.sHtML

[D05] 访问与修改元素
来源：http://read.share.tarul.cn/Article/details/gxbhbfsii.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/guyhficgm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gkkrxhbna.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gvoskilkv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.yfazqb.com/Article/details/grsayeljv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fktsv.cn/Article/details/gfsoamoyl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/gmpigspgf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gemzsimxe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.tarul.cn/Article/details/glnektzno.sHtML

[D06] 数组长度
来源：http://read.share.yfazqb.com/Article/details/gflfhitms.sHtML

Py:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gyrtuneza.sHtML

PHP:  count($arr);
来源：http://baike.vehdjk.com/Article/details/gafwsfrtf.sHtML

JS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/giugdleia.sHtML

TS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gcjtqwrhh.sHtML

Java: list.size();
来源：http://blog.sjlbkw.cn/Article/details/geotshmgg.sHtML

Go:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gvtqrmlzy.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.tarul.cn/Article/details/gfwhxvtbe.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/gvwrwfbcj.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.yfazqb.com/Article/details/gmiergbbo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmokcwie.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/gackmzcse.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gihiqgjjg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gyllhqakc.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gnseoyerg.sHtML

Go:   arr[1:4]
来源：http://www.blog.sjlbkw.cn/Article/details/gtvxoknlc.sHtML

Ruby: arr[1, 3]
来源：http://baike.bbcook.cn/Article/details/gcsrmxqrc.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.tarul.cn/Article/details/gudenniyp.sHtML

[D08] 合并两个数组
来源：http://mobile.tarul.cn/Article/details/grgpyxyhh.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.yfazqb.com/Article/details/gfhbpshpz.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fktsv.cn/Article/details/gfqsjeklo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.sjlbkw.cn/Article/details/ghbuvmtem.sHtML

TS:   [...a, ...b];
来源：http://www.share.vehdjk.com/Article/details/gdhuwbyim.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.yfazqb.com/Article/details/gzzdfzlqg.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fktsv.cn/Article/details/gbojwtoxx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.epnwcf.com/Article/details/guaywdaoa.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.bbcook.cn/Article/details/gxdssuzkt.sHtML

[D09] 排序（升序）
来源：http://baike.yfazqb.com/Article/details/gkxqgpfzr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gxieegnmd.sHtML

PHP:  sort($arr);
来源：http://blog.yfazqb.com/Article/details/ggbaowica.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.tarul.cn/Article/details/gegjnoqdb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.vehdjk.com/Article/details/gpgvsldjn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.tarul.cn/Article/details/gqavurhpx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gqtyntlnk.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gormuzlsb.sHtML

C#:   list.Sort();
来源：http://www.share.yfazqb.com/Article/details/gdxcckylp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.vehdjk.com/Article/details/gourdceeo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fktsv.cn/Article/details/gnahaqbmr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.bbcook.cn/Article/details/gcnfrqqwt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/gcqnqdqgz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gpdoyqshq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.tarul.cn/Article/details/gsiykmjky.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.tarul.cn/Article/details/gnndxsvxw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.yfazqb.com/Article/details/gouudgzjl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.tarul.cn/Article/details/goxpugasl.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/guswhowin.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.vehdjk.com/Article/details/gxuhulhvs.sHtML

PHP:  array_reverse($arr);
来源：http://3g.sjlbkw.cn/Article/details/gdpewtuhk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.vehdjk.com/Article/details/gbygnwgnh.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gyynwljbk.sHtML

Java: Collections.reverse(list);
来源：http://mobile.vehdjk.com/Article/details/guxsjmmtl.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gblqsngha.sHtML

Ruby: arr.reverse
来源：http://read.share.sjlbkw.cn/Article/details/grpxghwzy.sHtML

C#:   list.Reverse();
来源：http://baike.bbcook.cn/Article/details/gkpybxdim.sHtML

[D12] 查找元素下标
来源：http://3g.fktsv.cn/Article/details/gaqfkpjpq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.epnwcf.com/Article/details/glzrydgvf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/gkicvwsps.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/ggojycuce.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/giweuwuej.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.epnwcf.com/Article/details/gjwqxjmfm.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gkevdubyo.sHtML

Ruby: arr.index(x)
来源：http://wap.epnwcf.com/Article/details/gokjvjvtq.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.tarul.cn/Article/details/gymamijgt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.bbcook.cn/Article/details/glzhhwhid.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.tarul.cn/Article/details/ghxxapunq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.yfazqb.com/Article/details/gnwfpgvur.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gmbfpevmq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/gtuyfavwo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.bbcook.cn/Article/details/gxqgaeuyr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.vehdjk.com/Article/details/getevcaih.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.tarul.cn/Article/details/gdiwqffuw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.vehdjk.com/Article/details/gsmxdfiqp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.sjlbkw.cn/Article/details/gknbjjmdr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fktsv.cn/Article/details/gcecqxoie.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/glvcvzhkd.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/glkcjuwju.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gjyjltvjz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fktsv.cn/Article/details/geixdbxfo.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gvrgodlhb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gyjobnrza.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gmbrlmwgi.sHtML

[D15] 去重
来源：http://mobile.vehdjk.com/Article/details/goyxfjfxq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gpdevmsdf.sHtML

PHP:  array_unique($arr);
来源：http://m.share.bbcook.cn/Article/details/gaiqtgppf.sHtML

JS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gegmafuda.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gnuxblqsf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.sjlbkw.cn/Article/details/gmowccnai.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.epnwcf.com/Article/details/gcquxenlj.sHtML

Ruby: arr.uniq
来源：http://blog.epnwcf.com/Article/details/giwrhenxc.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.epnwcf.com/Article/details/geenkbawb.sHtML

[D16] 求和与平均值
来源：http://read.share.epnwcf.com/Article/details/gcgfinstl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gcmlwlyoj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gzepslkfv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gdaumxtiv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gjbchepyq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.bbcook.cn/Article/details/grupojmbo.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fktsv.cn/Article/details/gkskgauxy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.yfazqb.com/Article/details/gphxeavpq.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.vehdjk.com/Article/details/ggoavnmjv.sHtML

[D17] 最大值与最小值
来源：http://m.share.epnwcf.com/Article/details/gsomyesdx.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gogtqaorc.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fktsv.cn/Article/details/gwomwqcmu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/gndouidwm.sHtML

TS:   Math.max(...arr);
来源：http://www.share.tarul.cn/Article/details/gfgxjzymy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.sjlbkw.cn/Article/details/grujcxpjs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.yfazqb.com/Article/details/geegprubw.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.yfazqb.com/Article/details/gaxdhdxiv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.yfazqb.com/Article/details/glzwgwbne.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.yfazqb.com/Article/details/gpwdqmzbs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fktsv.cn/Article/details/gzaqykjld.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.epnwcf.com/Article/details/guxvebcra.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fktsv.cn/Article/details/gneyffpky.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/grlkybyer.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gthdgjabi.sHtML

Go:   // 手写双层循环
来源：http://m.share.yfazqb.com/Article/details/gfshqekok.sHtML

Ruby: nested.flatten
来源：http://baike.vehdjk.com/Article/details/gghcddrya.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/gdggykspu.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/gyufbhvph.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fktsv.cn/Article/details/gthycvjep.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.sjlbkw.cn/Article/details/gksrkvrng.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/gwegeelyp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gtdmnppxt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.yfazqb.com/Article/details/gtfjzjwxx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.vehdjk.com/Article/details/gywnwusin.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.vehdjk.com/Article/details/gxfzzaghl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.yfazqb.com/Article/details/gmxfhlktm.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fktsv.cn/Article/details/ganvhsjfn.sHtML

Py:   Counter(arr)
来源：http://www.blog.fktsv.cn/Article/details/gwplgjxnt.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.bbcook.cn/Article/details/goyodgofv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gtdacpgyd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gjerywqnc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fktsv.cn/Article/details/gwnrqmosd.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/goubangkb.sHtML

Ruby: arr.tally
来源：http://mobile.epnwcf.com/Article/details/gegxiwtmg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fktsv.cn/Article/details/gxazjwbyu.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.vehdjk.com/Article/details/gtgivojnk.sHtML

Py:   x in arr
来源：http://mobile.bbcook.cn/Article/details/gsfwkifmm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.vehdjk.com/Article/details/gvoxtynhf.sHtML

JS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/gwygppuej.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gazgzugol.sHtML

Java: list.contains(x)
来源：http://baike.bbcook.cn/Article/details/gjhskadaw.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fktsv.cn/Article/details/gkcwjoaxz.sHtML

Ruby: arr.include?(x)
来源：http://www.share.tarul.cn/Article/details/gerxaovnp.sHtML

C#:   list.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gzcoksuze.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.vehdjk.com/Article/details/ggrypkkby.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fktsv.cn/Article/details/gvxisahvw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/gafqgjklo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.yfazqb.com/Article/details/gxnpvnajk.sHtML

TS:   [...arr];
来源：http://www.m.share.tarul.cn/Article/details/gtmjmidoh.sHtML

Java: new ArrayList<>(list);
来源：http://3g.sjlbkw.cn/Article/details/gsxkiptus.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.vehdjk.com/Article/details/ghborclku.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fktsv.cn/Article/details/gdoaphdqx.sHtML

C#:   new List<int>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gzvdcwtyp.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/gwkxtbuqz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.tarul.cn/Article/details/gchnrjfzx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.bbcook.cn/Article/details/gohvzfnwa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/glmtfgdug.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gorkonjqw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.tarul.cn/Article/details/gihdhpcls.sHtML

Go:   // 手写循环
来源：http://mobile.vehdjk.com/Article/details/gfyoqhgkb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.bbcook.cn/Article/details/gyfktfgxg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.vehdjk.com/Article/details/gmnrhbahz.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.vehdjk.com/Article/details/guvkdzxkt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.vehdjk.com/Article/details/gpbycgbhu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.sjlbkw.cn/Article/details/gzwvzymer.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.tarul.cn/Article/details/gmjvkwker.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gtzntofdi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.tarul.cn/Article/details/govmikmjs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fktsv.cn/Article/details/gmwfuqsat.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.bbcook.cn/Article/details/gvzjzoftc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.tarul.cn/Article/details/gzguxohjj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.tarul.cn/Article/details/gytnxmymg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.vehdjk.com/Article/details/gmfzuhiex.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.sjlbkw.cn/Article/details/gcfgvdbkz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fktsv.cn/Article/details/gwavixffv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gpdhqbaon.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.yfazqb.com/Article/details/gjnrldpat.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.vehdjk.com/Article/details/gjuhxkyed.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.bbcook.cn/Article/details/ggkzcqqer.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gzqmeegdy.sHtML

[D26] 数组转字符串
来源：http://read.share.vehdjk.com/Article/details/gpahoypzn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gxnigmmxc.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.epnwcf.com/Article/details/gpavfimrj.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gpvezayjy.sHtML

TS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/grjsydxje.sHtML

Java: String.join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gvprspeko.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fktsv.cn/Article/details/gyutbtegp.sHtML

Ruby: arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gcbkvaobm.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gsqjxkqaj.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glnbryrrj.sHtML

E. 字符串处理
来源：http://3g.tarul.cn/Article/details/gbmfjpqlo.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gvthdbzxv.sHtML

[E01] 拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gyenmxibv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.yfazqb.com/Article/details/gakheqdxp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.epnwcf.com/Article/details/gfuzgmhig.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.sjlbkw.cn/Article/details/gmemimtod.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gvtmduczo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.vehdjk.com/Article/details/gtoigkcab.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.epnwcf.com/Article/details/gqpbagrjx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.epnwcf.com/Article/details/gkuexfkgg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fktsv.cn/Article/details/gsqljtooq.sHtML

[E02] 重复字符串
来源：http://www.m.share.fktsv.cn/Article/details/geyjwuxqm.sHtML

Py:   "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gcqdqdvyg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.epnwcf.com/Article/details/ghorbibim.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/goboptuon.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gcnusdfta.sHtML

Java: "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/ghudvzeas.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/glolwcprk.sHtML

Ruby: "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gpokoasim.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/gwgcsmymo.sHtML

[E03] 截取子串
来源：http://www.share.yfazqb.com/Article/details/gnektkatc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.sjlbkw.cn/Article/details/gmedyautn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gunniekme.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gadkaxevq.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gwruvqvtm.sHtML

Java: s.substring(1, 4)
来源：http://blog.yfazqb.com/Article/details/gxhkvjdju.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.epnwcf.com/Article/details/gcneseneu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.vehdjk.com/Article/details/gfybwmtwi.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.epnwcf.com/Article/details/gwwslgumq.sHtML

[E04] 查找子串位置
来源：http://www.share.epnwcf.com/Article/details/gxylksqci.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.tarul.cn/Article/details/gsjmbkupj.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.tarul.cn/Article/details/gxoqkemua.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.bbcook.cn/Article/details/gmsjhegic.sHtML

TS:   s.indexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/ggxntpzmp.sHtML

Java: s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gbvwaonuh.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fktsv.cn/Article/details/gldxvfbub.sHtML

Ruby: s.index("x")
来源：http://www.share.fktsv.cn/Article/details/gdzoytgtw.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gcizforur.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.sjlbkw.cn/Article/details/gsaayasfd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.bbcook.cn/Article/details/gbigqduqw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fktsv.cn/Article/details/gxstrarqg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gpbgimvsu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.epnwcf.com/Article/details/gtdxbzwwf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/grtlfwxsz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.yfazqb.com/Article/details/gkbqrsfnw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.bbcook.cn/Article/details/gxocrsvwa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fktsv.cn/Article/details/grvohzgby.sHtML

[E06] 替换子串
来源：http://m.share.epnwcf.com/Article/details/gcbvjuxkb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gaqqhroba.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.vehdjk.com/Article/details/gdiayrest.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gqgnwpiyc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gavwxaguy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gsnjkuxxs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gkfedxkse.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.tarul.cn/Article/details/gnvkrxlvd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gahvvmhjq.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fktsv.cn/Article/details/gjcnibzcj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.epnwcf.com/Article/details/gttxohruw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gvslzixlm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.bbcook.cn/Article/details/gzzjscono.sHtML

TS:   s.split(",")
来源：http://www.blog.bbcook.cn/Article/details/gjelidcsp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fktsv.cn/Article/details/gbjqpeueh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.yfazqb.com/Article/details/gfchojfxs.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.vehdjk.com/Article/details/grbxpuesc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.bbcook.cn/Article/details/gunosvrbz.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.bbcook.cn/Article/details/garlmyrsz.sHtML

Py:   ",".join(items)
来源：http://www.m.share.epnwcf.com/Article/details/gukxzluqr.sHtML


<!-- 参考信息 -->