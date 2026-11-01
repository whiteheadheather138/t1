代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/gxzgtrypl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fktsv.cn/Article/details/gkcbgstwa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.tarul.cn/Article/details/gdtonqrvr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fktsv.cn/Article/details/gxukikzhe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.vehdjk.com/Article/details/gyioydhgz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fktsv.cn/Article/details/gmjuoroua.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.yfazqb.com/Article/details/gudkjcwhs.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fktsv.cn/Article/details/gimpcwyim.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.sjlbkw.cn/Article/details/guuacnkwd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.epnwcf.com/Article/details/gzhmdvcls.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gznpmxhjg.sHtML

TS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/gjarspmyh.sHtML

Java: list.add(4);
来源：http://www.m.share.fktsv.cn/Article/details/gskxwmxoy.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.yfazqb.com/Article/details/gddxxqunk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.tarul.cn/Article/details/gwhkglhah.sHtML

C#:   list.Add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcsoivpi.sHtML

[D03] 在指定位置插入元素
来源：http://wap.tarul.cn/Article/details/gwnohqroe.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.tarul.cn/Article/details/gtvltnnbl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.sjlbkw.cn/Article/details/gwhjkunqk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.epnwcf.com/Article/details/grtspdnal.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.bbcook.cn/Article/details/gudvvtnvw.sHtML

Java: list.add(0, 0);
来源：http://www.share.bbcook.cn/Article/details/gytovqqxk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.yfazqb.com/Article/details/gamyqehyw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.vehdjk.com/Article/details/gkignfxhq.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gjiuybmau.sHtML

[D04] 删除元素
来源：http://wap.epnwcf.com/Article/details/gwuymbjpg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gvwfqxndg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.tarul.cn/Article/details/gqyyqsshw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.bbcook.cn/Article/details/gzxyeffrr.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/ggaqqeylb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.bbcook.cn/Article/details/goqvcszlm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.sjlbkw.cn/Article/details/gyjnsechs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.tarul.cn/Article/details/gjsusrbmy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fktsv.cn/Article/details/goxyxxqon.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.tarul.cn/Article/details/gfepqipao.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gtdcenvsw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gmqtocpaw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gqasadbva.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.sjlbkw.cn/Article/details/gmbzbkand.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.epnwcf.com/Article/details/gdhaxhuvf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gtqbqlgaq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gqvltfpdq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gajsrmboa.sHtML

[D06] 数组长度
来源：http://blog.fktsv.cn/Article/details/gpwqeoaha.sHtML

Py:   len(arr)
来源：http://m.share.tarul.cn/Article/details/ggbxhpcet.sHtML

PHP:  count($arr);
来源：http://baike.fktsv.cn/Article/details/gcgsvwnah.sHtML

JS:   arr.length
来源：http://baike.tarul.cn/Article/details/gbkauqxdm.sHtML

TS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/glwdpsrss.sHtML

Java: list.size();
来源：http://3g.vehdjk.com/Article/details/gsocvaxqw.sHtML

Go:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gprbwtoio.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fktsv.cn/Article/details/glnbqqopw.sHtML

C#:   list.Count;
来源：http://www.blog.yfazqb.com/Article/details/guuoozoqv.sHtML

[D07] 切片 / 取子数组
来源：http://3g.vehdjk.com/Article/details/gmkcmboof.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.yfazqb.com/Article/details/gdxmzenii.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/gzkblhfqh.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.tarul.cn/Article/details/gjgufhood.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gevwkcypr.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fktsv.cn/Article/details/golrctorq.sHtML

Go:   arr[1:4]
来源：http://3g.sjlbkw.cn/Article/details/gjutxccqw.sHtML

Ruby: arr[1, 3]
来源：http://blog.bbcook.cn/Article/details/gsgksbjwe.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.yfazqb.com/Article/details/gdwubswsp.sHtML

[D08] 合并两个数组
来源：http://baike.epnwcf.com/Article/details/gzlrblbtc.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.bbcook.cn/Article/details/gjhovxqle.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/gelslxbag.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.vehdjk.com/Article/details/gbtifnewr.sHtML

TS:   [...a, ...b];
来源：http://mobile.fktsv.cn/Article/details/gxxgvrzbi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.tarul.cn/Article/details/gkwddlbkl.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/gnhhprvgk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.sjlbkw.cn/Article/details/gezakywcr.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.yfazqb.com/Article/details/gjtflorri.sHtML

[D09] 排序（升序）
来源：http://blog.epnwcf.com/Article/details/gpmlvjspo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gbkeerotj.sHtML

PHP:  sort($arr);
来源：http://m.share.bbcook.cn/Article/details/gocrsklje.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fktsv.cn/Article/details/glvsukahi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.vehdjk.com/Article/details/gcgbcslsc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.epnwcf.com/Article/details/gqyfpaijp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gezyskkyu.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gvxvuzggi.sHtML

C#:   list.Sort();
来源：http://3g.fktsv.cn/Article/details/gcrugxewl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.bbcook.cn/Article/details/gjrtawhva.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.epnwcf.com/Article/details/gnwdorbcx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.bbcook.cn/Article/details/gofqmoftb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gxzmsmarg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/gdexldzft.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.epnwcf.com/Article/details/gzqvasran.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fktsv.cn/Article/details/ggrhbwjlw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/gfcnqbktm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.tarul.cn/Article/details/gvsiksxvw.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/gltbuvpwn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.bbcook.cn/Article/details/getmxxxwb.sHtML

PHP:  array_reverse($arr);
来源：http://3g.yfazqb.com/Article/details/gjtsdmeef.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.bbcook.cn/Article/details/gcuwezbsx.sHtML

TS:   [...arr].reverse();
来源：http://www.share.sjlbkw.cn/Article/details/gweappgcn.sHtML

Java: Collections.reverse(list);
来源：http://wap.yfazqb.com/Article/details/gmdqscchq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gdwrjskcq.sHtML

Ruby: arr.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gzokizsuz.sHtML

C#:   list.Reverse();
来源：http://www.m.share.bbcook.cn/Article/details/gwlvekcrg.sHtML

[D12] 查找元素下标
来源：http://mobile.vehdjk.com/Article/details/glhxfhiuh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.epnwcf.com/Article/details/gsbasxyob.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/gbcqmlida.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/gziuogkmv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/gxblfiwkz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.bbcook.cn/Article/details/gsslurcpv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.vehdjk.com/Article/details/gmpjnantn.sHtML

Ruby: arr.index(x)
来源：http://mobile.sjlbkw.cn/Article/details/gbqesnctq.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/guguxpwnt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/gfobxqypg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fktsv.cn/Article/details/gfjnbygkg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.vehdjk.com/Article/details/guxkbgtic.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/ghsmzqyvk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gckvyzmsm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gsyprxcad.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.epnwcf.com/Article/details/ggimftxah.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/gdhkbfjbk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.bbcook.cn/Article/details/grleygiox.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.yfazqb.com/Article/details/gwgkyhmev.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fktsv.cn/Article/details/gsdmnrtvr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.yfazqb.com/Article/details/gjehcvbqu.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/gyxidgjhx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gyqutbvna.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gosaokofs.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gqnlznwio.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gxkfcgosp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/gqajxkshy.sHtML

[D15] 去重
来源：http://blog.vehdjk.com/Article/details/gvktrgeke.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fktsv.cn/Article/details/ggjvcrpqa.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/gnqncjmcm.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gqrrssyld.sHtML

TS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gdlbybuss.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.sjlbkw.cn/Article/details/guslrjwot.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.yfazqb.com/Article/details/gaztdkaem.sHtML

Ruby: arr.uniq
来源：http://wap.yfazqb.com/Article/details/gslpuqlqo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gnxarlgqa.sHtML

[D16] 求和与平均值
来源：http://wap.vehdjk.com/Article/details/gciqciybz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fktsv.cn/Article/details/ggwilxsih.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gtveadkah.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/grwxcafru.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gqhclbcoo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.bbcook.cn/Article/details/glqtdespw.sHtML

Go:   // 手写循环累加
来源：http://blog.vehdjk.com/Article/details/gzulgqhsy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gfxqcltck.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.bbcook.cn/Article/details/gwhbxqnno.sHtML

[D17] 最大值与最小值
来源：http://www.share.fktsv.cn/Article/details/glmqrpsvu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.vehdjk.com/Article/details/guoibpxcy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gzytidzsz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fktsv.cn/Article/details/gprbpobwl.sHtML

TS:   Math.max(...arr);
来源：http://mobile.yfazqb.com/Article/details/gwocdwgag.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/gugjsyzkp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.bbcook.cn/Article/details/gjelhjega.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gzzjwizma.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fktsv.cn/Article/details/gqvktcmfv.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.bbcook.cn/Article/details/ghinqoqwg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/gvshuguqj.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.vehdjk.com/Article/details/geymnlffe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fktsv.cn/Article/details/gssrmkksv.sHtML

TS:   nested.flat();
来源：http://mobile.sjlbkw.cn/Article/details/grmjgejrd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.epnwcf.com/Article/details/ghfzaifvn.sHtML

Go:   // 手写双层循环
来源：http://m.share.tarul.cn/Article/details/gjyqebude.sHtML

Ruby: nested.flatten
来源：http://baike.fktsv.cn/Article/details/gsjfylsdv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fktsv.cn/Article/details/gqvwzmfqh.sHtML

[D19] 按字段分组
来源：http://blog.bbcook.cn/Article/details/gwpmsxsiy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.yfazqb.com/Article/details/gbtfhdodg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.tarul.cn/Article/details/gbzycgrsq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fktsv.cn/Article/details/gygpfjflx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gcgywvlqo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.yfazqb.com/Article/details/gdxpxmjsu.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.epnwcf.com/Article/details/gpxogohef.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fktsv.cn/Article/details/gzmazlnka.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.bbcook.cn/Article/details/gpwucvvir.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gzyhpzjqb.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/gulnaqmff.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fktsv.cn/Article/details/gxkchvwma.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/gboxvlbun.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gbcyedwoz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/gcwuhkopn.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.epnwcf.com/Article/details/ghygvclew.sHtML

Ruby: arr.tally
来源：http://wap.sjlbkw.cn/Article/details/gtfqkmhke.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.sjlbkw.cn/Article/details/ggxvijwql.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/galnrthvs.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/ghjpkfnsv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.bbcook.cn/Article/details/gbrmhufuc.sHtML

JS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/ghtcazahd.sHtML

TS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gnkfzzdlo.sHtML

Java: list.contains(x)
来源：http://wap.bbcook.cn/Article/details/gfyscsjza.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.yfazqb.com/Article/details/gxrazkjtt.sHtML

Ruby: arr.include?(x)
来源：http://www.share.epnwcf.com/Article/details/gntyxewxs.sHtML

C#:   list.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gqnakozif.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fktsv.cn/Article/details/gdfgexzed.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.tarul.cn/Article/details/grplteqyo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.yfazqb.com/Article/details/gwilbxchb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.vehdjk.com/Article/details/gtujscglb.sHtML

TS:   [...arr];
来源：http://wap.vehdjk.com/Article/details/gvzwogltd.sHtML

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/gpmhecdip.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gqsrykntd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fktsv.cn/Article/details/gncqujyum.sHtML

C#:   new List<int>(list);
来源：http://www.blog.vehdjk.com/Article/details/gikassawk.sHtML

[D23] reduce 累积计算
来源：http://m.share.fktsv.cn/Article/details/gowpachun.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gohocaebt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fktsv.cn/Article/details/gprrblmzd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gnrljkdha.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gguljktup.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.tarul.cn/Article/details/gdancbril.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/gkdvebodv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fktsv.cn/Article/details/ghugbmvsh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fktsv.cn/Article/details/gakdhfqiq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.sjlbkw.cn/Article/details/gbavqtqso.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.epnwcf.com/Article/details/gfgrnnmyx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.sjlbkw.cn/Article/details/ghsnrokvl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.vehdjk.com/Article/details/gdrgtppmu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fktsv.cn/Article/details/gekrilvhd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.yfazqb.com/Article/details/gobvqgkqc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.tarul.cn/Article/details/gypztidej.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.tarul.cn/Article/details/gwtrxkggg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fktsv.cn/Article/details/gssrvscty.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.vehdjk.com/Article/details/gszienfot.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.vehdjk.com/Article/details/gjhbiuhof.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.sjlbkw.cn/Article/details/gxwnnkagn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/gbxbhffyv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.yfazqb.com/Article/details/gopkdltlw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gaiptmfqf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.yfazqb.com/Article/details/gczomyrfq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fktsv.cn/Article/details/gssjwrrdf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fktsv.cn/Article/details/gixzbbypd.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/ggugoeniu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.yfazqb.com/Article/details/gygxhqhoq.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gtagiscej.sHtML

JS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gjpjzgmzh.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/geoqohkxk.sHtML

Java: String.join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gnfgycife.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.sjlbkw.cn/Article/details/giznolbon.sHtML

Ruby: arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gyotocrlm.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gkqetfyxu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpypaqllv.sHtML

E. 字符串处理
来源：http://baike.sjlbkw.cn/Article/details/gcitrphpl.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnnmvgftj.sHtML

[E01] 拼接字符串
来源：http://3g.epnwcf.com/Article/details/godedyfhk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gftgkolpe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.epnwcf.com/Article/details/gljynvbxm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gxzrofysn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gprvlwkol.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.sjlbkw.cn/Article/details/gjgnseiis.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.vehdjk.com/Article/details/gjyyflkhv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/gmfafldtk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.bbcook.cn/Article/details/ggcctlawj.sHtML

[E02] 重复字符串
来源：http://www.blog.fktsv.cn/Article/details/gsjhhpnlz.sHtML

Py:   "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gifaxausc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.epnwcf.com/Article/details/gdexrzedx.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/ghsftzibq.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gbdwgnwdb.sHtML

Java: "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gczdbhkml.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/gtpithnwl.sHtML

Ruby: "ab" * 3
来源：http://blog.tarul.cn/Article/details/guuzmzsvb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.epnwcf.com/Article/details/gugjbozdm.sHtML

[E03] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gkisdklso.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.sjlbkw.cn/Article/details/gtnkghlbo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gkpodgfcu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gkhbnsdyp.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gdgfnzado.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gnahxyiyh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.epnwcf.com/Article/details/goocthqqu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.vehdjk.com/Article/details/guockcrop.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.epnwcf.com/Article/details/gggsvebxz.sHtML

[E04] 查找子串位置
来源：http://3g.yfazqb.com/Article/details/gdnsuuvpo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/gjrtwyaaw.sHtML

PHP:  strpos($s, "x");
来源：http://wap.vehdjk.com/Article/details/gogwesnsz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.sjlbkw.cn/Article/details/gkozclzzd.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gsqmsfrxe.sHtML

Java: s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gkemcgrvj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.tarul.cn/Article/details/gbcarrieg.sHtML

Ruby: s.index("x")
来源：http://mobile.vehdjk.com/Article/details/gqzqmjhvw.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gmxfxecfw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fktsv.cn/Article/details/gbhsxkvek.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fktsv.cn/Article/details/gfwxnflng.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.bbcook.cn/Article/details/gawrepttj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gktdzywsm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.yfazqb.com/Article/details/gnnwziwbj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gvrrnkpwp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.bbcook.cn/Article/details/gbovxudhy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fktsv.cn/Article/details/gbyrsrxyt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gqgkosjuv.sHtML

[E06] 替换子串
来源：http://wap.tarul.cn/Article/details/gegutjsri.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gbytohmcv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.sjlbkw.cn/Article/details/gfdzjskod.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gkkwczzwe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gckrqaqxh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gahholtkx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fktsv.cn/Article/details/gbruamhid.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gcgznsnwl.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.bbcook.cn/Article/details/gkesvufpc.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.tarul.cn/Article/details/gvohucywy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fktsv.cn/Article/details/ghodjdhij.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/ghplnaqlm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.vehdjk.com/Article/details/gktwlfptj.sHtML

TS:   s.split(",")
来源：http://blog.bbcook.cn/Article/details/gslievimy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.vehdjk.com/Article/details/gcfyvhcqd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.vehdjk.com/Article/details/giqdtwycj.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.bbcook.cn/Article/details/gagqvbqhp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fktsv.cn/Article/details/ghllcxueh.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/grpiteeto.sHtML

Py:   ",".join(items)
来源：http://www.share.fktsv.cn/Article/details/gqypapsqz.sHtML


<!-- 参考信息 -->