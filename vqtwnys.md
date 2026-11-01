代发 wailian999

[D03] 在指定位置插入元素
来源：http://mobile.fktsv.cn/Article/details/gieekbfzh.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.epnwcf.com/Article/details/gkcizmuwe.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.yfazqb.com/Article/details/gjqgcrmur.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.sjlbkw.cn/Article/details/gdetejcte.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fktsv.cn/Article/details/gzhblgvnq.sHtML

Java: list.add(0, 0);
来源：http://blog.fktsv.cn/Article/details/gavtcmaof.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.vehdjk.com/Article/details/gtrcrkptc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/gxxqscsaq.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.tarul.cn/Article/details/gykbjuedj.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/gnvhkmjtx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.bbcook.cn/Article/details/gzynpiuog.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.bbcook.cn/Article/details/ghnbeitwd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.yfazqb.com/Article/details/gfqwqhqhx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.tarul.cn/Article/details/gelmddvhh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fktsv.cn/Article/details/gljaznqmb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.bbcook.cn/Article/details/gbvlwsorf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.epnwcf.com/Article/details/goecqfcyc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.tarul.cn/Article/details/gzuzdwuoy.sHtML

[D05] 访问与修改元素
来源：http://www.share.yfazqb.com/Article/details/gudhzptfd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gyivirkeu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gywetjwhl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/glzvsjbop.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.tarul.cn/Article/details/gwvavrvec.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.sjlbkw.cn/Article/details/ggbbqskrp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gwyfjeiie.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/grvkmahny.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gwfbrsgip.sHtML

[D06] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gylsggnzv.sHtML

Py:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gosreplse.sHtML

PHP:  count($arr);
来源：http://www.share.fktsv.cn/Article/details/gvavmuzyp.sHtML

JS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gnikzzfbp.sHtML

TS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gowrtuvrs.sHtML

Java: list.size();
来源：http://www.blog.tarul.cn/Article/details/glqiiumom.sHtML

Go:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gdisnybhu.sHtML

Ruby: arr.length; arr.size
来源：http://blog.sjlbkw.cn/Article/details/gnzpjgxrh.sHtML

C#:   list.Count;
来源：http://m.share.epnwcf.com/Article/details/gxeinelmj.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.yfazqb.com/Article/details/giuvojulf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.vehdjk.com/Article/details/gdiibvfwm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gibsfcwvx.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gmtojgoty.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gmrygeqws.sHtML

Java: list.subList(1, 4);
来源：http://3g.bbcook.cn/Article/details/gplgtrban.sHtML

Go:   arr[1:4]
来源：http://mobile.vehdjk.com/Article/details/ghdcsnegn.sHtML

Ruby: arr[1, 3]
来源：http://blog.epnwcf.com/Article/details/gwhyenlcl.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fktsv.cn/Article/details/gcfjfvgui.sHtML

[D08] 合并两个数组
来源：http://read.share.bbcook.cn/Article/details/giwqzfhbm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.tarul.cn/Article/details/ghfdwygjg.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.epnwcf.com/Article/details/glwpuwnpk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.yfazqb.com/Article/details/gqetzsbip.sHtML

TS:   [...a, ...b];
来源：http://blog.bbcook.cn/Article/details/gqchponxf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.tarul.cn/Article/details/grfenmuwn.sHtML

Go:   append(a, b...)
来源：http://blog.tarul.cn/Article/details/gscybdorz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gsmzvcdwr.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fktsv.cn/Article/details/gnwjueszi.sHtML

[D09] 排序（升序）
来源：http://blog.yfazqb.com/Article/details/gqtiwrlrj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gtdpigesj.sHtML

PHP:  sort($arr);
来源：http://read.share.epnwcf.com/Article/details/gxeeceycf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.vehdjk.com/Article/details/gmfkrekny.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.yfazqb.com/Article/details/gibongcev.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.bbcook.cn/Article/details/gnizsrwhn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/gdkewxiry.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/ggpeeyzqf.sHtML

C#:   list.Sort();
来源：http://wap.yfazqb.com/Article/details/gtavyyuhs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.epnwcf.com/Article/details/gpnbvvprn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.sjlbkw.cn/Article/details/grzmwlpsw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gaqpkcotr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gmriqkkca.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.tarul.cn/Article/details/ghponhzdu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/glrdneewc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.sjlbkw.cn/Article/details/ggbcbsdgi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.tarul.cn/Article/details/gxbfkwpdh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.vehdjk.com/Article/details/goovdutwe.sHtML

[D11] 反转数组
来源：http://blog.fktsv.cn/Article/details/ggiwebhct.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.epnwcf.com/Article/details/gdetkjnrd.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/gekikszor.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.bbcook.cn/Article/details/gauzisgti.sHtML

TS:   [...arr].reverse();
来源：http://blog.sjlbkw.cn/Article/details/geylxcpjo.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fktsv.cn/Article/details/giesauwtt.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.vehdjk.com/Article/details/gntlumxkr.sHtML

Ruby: arr.reverse
来源：http://3g.vehdjk.com/Article/details/gnsmmpmwg.sHtML

C#:   list.Reverse();
来源：http://www.share.epnwcf.com/Article/details/gbuigzxzk.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/gvbytxtqt.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/gqnnjlxin.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.epnwcf.com/Article/details/gjnykofpq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.yfazqb.com/Article/details/gqculedlp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gxtaiswhf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.sjlbkw.cn/Article/details/gkbxfymhg.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.yfazqb.com/Article/details/gvqafsftt.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.bbcook.cn/Article/details/ggtrnekqp.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/gnjaqetub.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.sjlbkw.cn/Article/details/gwprbzsvh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gattlxjwc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.vehdjk.com/Article/details/ghfjwphpn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/guclasxak.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/gnkyrrbki.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.tarul.cn/Article/details/gbqmsfgav.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.bbcook.cn/Article/details/geenzurmr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/gfwmxwlff.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.tarul.cn/Article/details/gmzdvpbel.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.tarul.cn/Article/details/gtuqphgcx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.bbcook.cn/Article/details/gkhwchdui.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.tarul.cn/Article/details/ggqkorrzm.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gngqetzlo.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/goczvzscg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.yfazqb.com/Article/details/gegnrokzj.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gcjrfhtwo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxocjnso.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/gmjidkynu.sHtML

[D15] 去重
来源：http://blog.yfazqb.com/Article/details/gmeceovbr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/gpqqjwmil.sHtML

PHP:  array_unique($arr);
来源：http://read.share.bbcook.cn/Article/details/guqibzfsp.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gucrkkavt.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gslseiozh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.vehdjk.com/Article/details/gmtanlsaa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/gpxaunrxi.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/gwqguzqdu.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.tarul.cn/Article/details/gdfxwxvnp.sHtML

[D16] 求和与平均值
来源：http://wap.sjlbkw.cn/Article/details/gtxochnup.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjlgulkh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.tarul.cn/Article/details/geebcwxtq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/gepwtvmcv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gcowwsfzj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fktsv.cn/Article/details/gwktuioqc.sHtML

Go:   // 手写循环累加
来源：http://m.share.vehdjk.com/Article/details/gxuqirqdn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.sjlbkw.cn/Article/details/gzmoriuhv.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fktsv.cn/Article/details/gpelqgbyv.sHtML

[D17] 最大值与最小值
来源：http://baike.bbcook.cn/Article/details/gzccpgayj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.vehdjk.com/Article/details/geqdriwec.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.tarul.cn/Article/details/gywjzjmyq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.sjlbkw.cn/Article/details/gkpvgbemx.sHtML

TS:   Math.max(...arr);
来源：http://baike.fktsv.cn/Article/details/gprebnatk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.bbcook.cn/Article/details/gtziysirw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fktsv.cn/Article/details/ggjfsyrbe.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.epnwcf.com/Article/details/gvdvldqsl.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.sjlbkw.cn/Article/details/guuptsbbf.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.tarul.cn/Article/details/gcxwgkxue.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.tarul.cn/Article/details/ggfosrsro.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/gufjmgduq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.vehdjk.com/Article/details/gitrmsgrz.sHtML

TS:   nested.flat();
来源：http://www.share.bbcook.cn/Article/details/gnmcnsuxh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fktsv.cn/Article/details/gufuhciyf.sHtML

Go:   // 手写双层循环
来源：http://m.share.vehdjk.com/Article/details/gzxhtxpbi.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gwegjixld.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fktsv.cn/Article/details/gxiofyupi.sHtML

[D19] 按字段分组
来源：http://www.share.bbcook.cn/Article/details/gexcpqpbf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.vehdjk.com/Article/details/ghhhsjnxz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.vehdjk.com/Article/details/goqjeraiv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.tarul.cn/Article/details/guwbtzxqw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.bbcook.cn/Article/details/gfuucewpd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.vehdjk.com/Article/details/gxxwozoun.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.epnwcf.com/Article/details/gzibyjtzd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.tarul.cn/Article/details/gtwxrrbor.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.vehdjk.com/Article/details/gonjvlevi.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.vehdjk.com/Article/details/gidwmhuzi.sHtML

Py:   Counter(arr)
来源：http://3g.tarul.cn/Article/details/gfnnyntai.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.vehdjk.com/Article/details/gzoykddlz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gyiehcflo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gqhabehry.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.tarul.cn/Article/details/gxponjbnn.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fktsv.cn/Article/details/gfexnsylx.sHtML

Ruby: arr.tally
来源：http://www.blog.fktsv.cn/Article/details/gjzvbjlzm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.epnwcf.com/Article/details/gtmgttfbb.sHtML

[D21] 判断是否包含某元素
来源：http://baike.sjlbkw.cn/Article/details/gmdqepcsv.sHtML

Py:   x in arr
来源：http://read.share.yfazqb.com/Article/details/getubhpif.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fktsv.cn/Article/details/gyxdysmrx.sHtML

JS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/gmzlhiorz.sHtML

TS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gjtcnoyed.sHtML

Java: list.contains(x)
来源：http://3g.tarul.cn/Article/details/gkfxuazfm.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gnddapbll.sHtML

Ruby: arr.include?(x)
来源：http://3g.bbcook.cn/Article/details/ghtyaytdx.sHtML

C#:   list.Contains(x)
来源：http://blog.yfazqb.com/Article/details/gbekxeosx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fktsv.cn/Article/details/gfsrvwvzg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.bbcook.cn/Article/details/gjiirrgey.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.sjlbkw.cn/Article/details/gtcrsidby.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.tarul.cn/Article/details/grqmmgsfk.sHtML

TS:   [...arr];
来源：http://www.blog.fktsv.cn/Article/details/goqwtmtbg.sHtML

Java: new ArrayList<>(list);
来源：http://3g.sjlbkw.cn/Article/details/gmmhyxjxr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.bbcook.cn/Article/details/gxthebjav.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/gyevnhbgj.sHtML

C#:   new List<int>(list);
来源：http://read.share.tarul.cn/Article/details/gghqggwuo.sHtML

[D23] reduce 累积计算
来源：http://wap.fktsv.cn/Article/details/gqfclanoo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.epnwcf.com/Article/details/guzbfpjjl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/gcomfwyxi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/glweqioux.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gxewettpw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.tarul.cn/Article/details/gsvyjoxxf.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gmkaahkmz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.vehdjk.com/Article/details/gunxhyhct.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fktsv.cn/Article/details/gfgigxzzh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.bbcook.cn/Article/details/gymedtxcw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gjdqhejet.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.bbcook.cn/Article/details/gxwztzucc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.sjlbkw.cn/Article/details/gwdxeyixk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gjkuzluvw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.bbcook.cn/Article/details/grumowpxz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fktsv.cn/Article/details/gfmunnnou.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.bbcook.cn/Article/details/gcicdcfrp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.yfazqb.com/Article/details/gluivoulr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.bbcook.cn/Article/details/ghncfupfu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.tarul.cn/Article/details/guxyvidos.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.vehdjk.com/Article/details/ghfhizlld.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.sjlbkw.cn/Article/details/gwoqwzjez.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.vehdjk.com/Article/details/guxtxairo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gzouzdzkk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.bbcook.cn/Article/details/gojoeuvcs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.epnwcf.com/Article/details/gvtjqwful.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gvqhnrslu.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/gtneyoqjl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.epnwcf.com/Article/details/gzdppqnml.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.vehdjk.com/Article/details/goflgmptb.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gtdejrfga.sHtML

TS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gzkfkmwan.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/ghjvfwrbn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.sjlbkw.cn/Article/details/gulgbeuzz.sHtML

Ruby: arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/guflyglqx.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gcrftomix.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvspzzgta.sHtML

E. 字符串处理
来源：http://wap.sjlbkw.cn/Article/details/glxwpsfgd.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmltlyuk.sHtML

[E01] 拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gtsjbnufh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.epnwcf.com/Article/details/gcltfsvbz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.tarul.cn/Article/details/gdefeseos.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/grtehsjxt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/ghiwxvbsz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gjtxcmeud.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fktsv.cn/Article/details/gilmezkmp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.epnwcf.com/Article/details/ghzbbrfww.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gjecghzbg.sHtML

[E02] 重复字符串
来源：http://3g.bbcook.cn/Article/details/gpzyugiqp.sHtML

Py:   "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gexfehzzi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.yfazqb.com/Article/details/ggjzqyfrw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gfvhjfjow.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gpwtykhmz.sHtML

Java: "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/ghzdyqhgn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.sjlbkw.cn/Article/details/goaxfrwvm.sHtML

Ruby: "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gbnsxuwhs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.epnwcf.com/Article/details/gxgkehdrq.sHtML

[E03] 截取子串
来源：http://3g.tarul.cn/Article/details/gxpyoqsbh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/gsxyyhnsf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gdzxrrfti.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/grevckvbi.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fktsv.cn/Article/details/gozymbmmw.sHtML

Java: s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/guqjvrevz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.bbcook.cn/Article/details/gmeeyoupk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.bbcook.cn/Article/details/gtsfzxhsw.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.bbcook.cn/Article/details/ghueapggz.sHtML

[E04] 查找子串位置
来源：http://m.share.fktsv.cn/Article/details/gdjpjmjru.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gxrmxkesh.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/goctdrttb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.vehdjk.com/Article/details/gummppzmi.sHtML

TS:   s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/ghuhbapyu.sHtML

Java: s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gqpqpvhto.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.sjlbkw.cn/Article/details/gkyccmbru.sHtML

Ruby: s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gbgyfiiqj.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gqfnuarez.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.epnwcf.com/Article/details/gidymuwnm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.vehdjk.com/Article/details/gzynagzqg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/gqzwdiabe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/gdqsvstfd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.sjlbkw.cn/Article/details/gvbfeguik.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/gdbwvxcik.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.sjlbkw.cn/Article/details/gsloaslkn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.bbcook.cn/Article/details/gjothuovk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/grtbvcfnn.sHtML

[E06] 替换子串
来源：http://wap.sjlbkw.cn/Article/details/grzhhyeco.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/glullqpru.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.bbcook.cn/Article/details/gkpslxjjt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/ghdcqlpys.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gemimeatj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gurrzwqti.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gnabaqyrd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gbuqocmho.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gbwafbbio.sHtML

[E07] 按分隔符拆分
来源：http://baike.epnwcf.com/Article/details/gkzlwtfcs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.tarul.cn/Article/details/gpibbjpfc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.tarul.cn/Article/details/gxxapjnfa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.vehdjk.com/Article/details/gssiiegly.sHtML

TS:   s.split(",")
来源：http://mobile.tarul.cn/Article/details/grdnmxkhy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.epnwcf.com/Article/details/gzrpbdvqv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.vehdjk.com/Article/details/gkykntjjq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.bbcook.cn/Article/details/gwxvxajzm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.yfazqb.com/Article/details/gxmhrgbuw.sHtML

[E08] 数组按分隔符合并
来源：http://3g.yfazqb.com/Article/details/gghiaynaz.sHtML

Py:   ",".join(items)
来源：http://read.share.epnwcf.com/Article/details/ggnrduvjh.sHtML

PHP:  implode(",", $items);
来源：http://www.share.bbcook.cn/Article/details/giuzokayn.sHtML

JS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gpvxvncrd.sHtML

TS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gxtuuegti.sHtML

Java: String.join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gzvsyekpt.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fktsv.cn/Article/details/gjfaxmfei.sHtML

Ruby: items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gbdoqiund.sHtML

C#:   string.Join(",", items)
来源：http://wap.bbcook.cn/Article/details/gnaadftro.sHtML

[E09] 去除所有空白字符
来源：http://baike.vehdjk.com/Article/details/gucvvktca.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/gsszcpspu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.vehdjk.com/Article/details/gnetwrhjg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gwuxbjuya.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/glabfutdl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.tarul.cn/Article/details/gxruhsbef.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.sjlbkw.cn/Article/details/ggagymxzv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gfttbkycs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/ghmijkgpy.sHtML


<!-- 参考信息 -->