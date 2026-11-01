代发 wailian999

D. 数组 / 列表 / 集合
来源：http://mobile.tarul.cn/Article/details/gtytorcmd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gnrprzljf.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gzvbntozi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.bbcook.cn/Article/details/gxykmgmbx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.yfazqb.com/Article/details/glyqakonr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.epnwcf.com/Article/details/ghrscddrj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.tarul.cn/Article/details/gniiibibz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/gjwarycev.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.sjlbkw.cn/Article/details/gkdsxuybo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.yfazqb.com/Article/details/gilhwlkwx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.bbcook.cn/Article/details/getagomql.sHtML

[D02] 追加元素到末尾
来源：http://www.share.yfazqb.com/Article/details/gcdsqxcnq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.tarul.cn/Article/details/gzuttyego.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fktsv.cn/Article/details/gretiiise.sHtML

JS:   arr.push(4);
来源：http://3g.yfazqb.com/Article/details/gfespfwwa.sHtML

TS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gdqbpqbza.sHtML

Java: list.add(4);
来源：http://m.share.yfazqb.com/Article/details/gemzissrb.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.epnwcf.com/Article/details/gxbtizyrs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.epnwcf.com/Article/details/gqraoxwok.sHtML

C#:   list.Add(4);
来源：http://3g.sjlbkw.cn/Article/details/gzsgluexm.sHtML

[D03] 在指定位置插入元素
来源：http://wap.yfazqb.com/Article/details/gqiyododc.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fktsv.cn/Article/details/gaehyzhax.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.sjlbkw.cn/Article/details/gawhzabqs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.vehdjk.com/Article/details/geljwkuxc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.tarul.cn/Article/details/gkfobpsna.sHtML

Java: list.add(0, 0);
来源：http://read.share.tarul.cn/Article/details/gvfcfeppt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.vehdjk.com/Article/details/gemzjrqmi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.epnwcf.com/Article/details/guxwpwkyg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gbwpivxor.sHtML

[D04] 删除元素
来源：http://www.blog.bbcook.cn/Article/details/gmpcoabun.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlsyqemd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/gocouggyz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.yfazqb.com/Article/details/giwkyjugu.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/gcatumdir.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fktsv.cn/Article/details/gulpsqnkv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.yfazqb.com/Article/details/girysvwsa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.bbcook.cn/Article/details/gacqakikq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.bbcook.cn/Article/details/gfcpcgnye.sHtML

[D05] 访问与修改元素
来源：http://read.share.sjlbkw.cn/Article/details/gofyezxvy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/glfzjllik.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/gvapogsqg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gicqvzumt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.yfazqb.com/Article/details/gvxfskdme.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.epnwcf.com/Article/details/gvwonmunh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/ghbhsqppq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gjoqbnkqw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.vehdjk.com/Article/details/giwwxgdvu.sHtML

[D06] 数组长度
来源：http://3g.bbcook.cn/Article/details/gdpzgsurf.sHtML

Py:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gfefdlmkd.sHtML

PHP:  count($arr);
来源：http://mobile.yfazqb.com/Article/details/gwqkqzith.sHtML

JS:   arr.length
来源：http://www.share.vehdjk.com/Article/details/ggfmdcvsr.sHtML

TS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gachnbiih.sHtML

Java: list.size();
来源：http://mobile.tarul.cn/Article/details/gbfmrsxhz.sHtML

Go:   len(arr)
来源：http://wap.yfazqb.com/Article/details/gulovwwas.sHtML

Ruby: arr.length; arr.size
来源：http://baike.tarul.cn/Article/details/gkjavvuff.sHtML

C#:   list.Count;
来源：http://m.share.tarul.cn/Article/details/gnxdxqsfx.sHtML

[D07] 切片 / 取子数组
来源：http://wap.sjlbkw.cn/Article/details/gcyyvvfys.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.vehdjk.com/Article/details/gplplipur.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fktsv.cn/Article/details/gokphryfe.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.epnwcf.com/Article/details/glfnszinz.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.bbcook.cn/Article/details/gkvzqdzcf.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gqxuhhdxr.sHtML

Go:   arr[1:4]
来源：http://www.blog.fktsv.cn/Article/details/govsotyas.sHtML

Ruby: arr[1, 3]
来源：http://baike.tarul.cn/Article/details/goykxkgwx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gjgqlktqs.sHtML

[D08] 合并两个数组
来源：http://www.blog.tarul.cn/Article/details/gazwrzwkl.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.tarul.cn/Article/details/gdkvxuboe.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.tarul.cn/Article/details/gjvayibgn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.bbcook.cn/Article/details/gsefhbvnr.sHtML

TS:   [...a, ...b];
来源：http://mobile.yfazqb.com/Article/details/gzauoyydf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.tarul.cn/Article/details/gnrziyowa.sHtML

Go:   append(a, b...)
来源：http://3g.tarul.cn/Article/details/gzmwcsnon.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fktsv.cn/Article/details/gonjuvvko.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.bbcook.cn/Article/details/gaizsmkmn.sHtML

[D09] 排序（升序）
来源：http://mobile.sjlbkw.cn/Article/details/ghwyawceh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gmlixdtzq.sHtML

PHP:  sort($arr);
来源：http://3g.fktsv.cn/Article/details/gevgoczrw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fktsv.cn/Article/details/gddsxwryd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.bbcook.cn/Article/details/ggvqndokj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.epnwcf.com/Article/details/gkfffapoe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gtynhttdy.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gdevxvcmv.sHtML

C#:   list.Sort();
来源：http://www.m.share.fktsv.cn/Article/details/gondwuooh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.bbcook.cn/Article/details/gjixlhqqm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.vehdjk.com/Article/details/gftymjhlu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.vehdjk.com/Article/details/gnqfjwyjd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.epnwcf.com/Article/details/gawynrdoy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.bbcook.cn/Article/details/gioruvmdu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.bbcook.cn/Article/details/gashsaddp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gvkfmuaui.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fktsv.cn/Article/details/gvxqckggz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.bbcook.cn/Article/details/gthckiwah.sHtML

[D11] 反转数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsjzchhx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.bbcook.cn/Article/details/gcbylblmv.sHtML

PHP:  array_reverse($arr);
来源：http://baike.sjlbkw.cn/Article/details/gzxuujaes.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.sjlbkw.cn/Article/details/goptskrqh.sHtML

TS:   [...arr].reverse();
来源：http://wap.epnwcf.com/Article/details/gcvwsyfic.sHtML

Java: Collections.reverse(list);
来源：http://mobile.tarul.cn/Article/details/geqdneyws.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.bbcook.cn/Article/details/gcaoodvsn.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gfebsutgz.sHtML

C#:   list.Reverse();
来源：http://m.share.epnwcf.com/Article/details/gfdtjowvj.sHtML

[D12] 查找元素下标
来源：http://www.m.share.tarul.cn/Article/details/ggdimeyqm.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.sjlbkw.cn/Article/details/gkncpzxba.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gamxdakkp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/gpnfbnwhl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/gqrmorlso.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.sjlbkw.cn/Article/details/gqrdomjfs.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gevbzwgdf.sHtML

Ruby: arr.index(x)
来源：http://www.share.yfazqb.com/Article/details/gwhggpqin.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.sjlbkw.cn/Article/details/gtsuhjrkn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.sjlbkw.cn/Article/details/gbcmhdygz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.bbcook.cn/Article/details/glwsrxeza.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fktsv.cn/Article/details/gnkxdpvxx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.tarul.cn/Article/details/gxwdqmurd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gbhmsvfan.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.epnwcf.com/Article/details/gknjifaod.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/ggbhpihha.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.yfazqb.com/Article/details/gtflyhdbj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.tarul.cn/Article/details/gnmtbbukb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.yfazqb.com/Article/details/gmenrgfcd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.tarul.cn/Article/details/ghwlapxpr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.yfazqb.com/Article/details/gnzmepwmw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/glubmnbva.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gbgnahedx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gowqpcmwd.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gigvvxeox.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gkugnichj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gloleadjt.sHtML

[D15] 去重
来源：http://blog.vehdjk.com/Article/details/gfeanzdlp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/grxesflqs.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gpwtxvfwg.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gldunmvcy.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gdrfuqxaq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.tarul.cn/Article/details/gvivbxbog.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.bbcook.cn/Article/details/gvmdfbswt.sHtML

Ruby: arr.uniq
来源：http://mobile.vehdjk.com/Article/details/gccdmhklq.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fktsv.cn/Article/details/gfrnynrcg.sHtML

[D16] 求和与平均值
来源：http://www.share.fktsv.cn/Article/details/gegxeiqsq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.yfazqb.com/Article/details/gdzltvqci.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.tarul.cn/Article/details/gbkawfpuk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gyxldiffm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.yfazqb.com/Article/details/gsjbwvtqu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fktsv.cn/Article/details/gialncwjq.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gbelwpkmn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.sjlbkw.cn/Article/details/geokanxrw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.epnwcf.com/Article/details/gnlkmtoxr.sHtML

[D17] 最大值与最小值
来源：http://m.share.bbcook.cn/Article/details/gmfptthfi.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.tarul.cn/Article/details/gvvnvvmlp.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/gjpmanzaz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.vehdjk.com/Article/details/gfexssxbv.sHtML

TS:   Math.max(...arr);
来源：http://blog.fktsv.cn/Article/details/gvczxsaux.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.sjlbkw.cn/Article/details/grzgnoqol.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.tarul.cn/Article/details/gmuccdrqw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.yfazqb.com/Article/details/gcrkxkwgk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.vehdjk.com/Article/details/gswcutgur.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/gvxjzzhzj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.tarul.cn/Article/details/gjclcaenj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.vehdjk.com/Article/details/gwcymqpxq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.vehdjk.com/Article/details/gfkpjvbux.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/glraiwmbf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.yfazqb.com/Article/details/gsylxwesb.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/gunkmjbei.sHtML

Ruby: nested.flatten
来源：http://read.share.sjlbkw.cn/Article/details/ggssqpouc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/ghwodgxwg.sHtML

[D19] 按字段分组
来源：http://www.m.share.bbcook.cn/Article/details/gvkoccmpr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.bbcook.cn/Article/details/gdkrditxr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.sjlbkw.cn/Article/details/gfidjsudi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.yfazqb.com/Article/details/gysoddreg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fktsv.cn/Article/details/glzoyfhav.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.yfazqb.com/Article/details/gndpbkgid.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.vehdjk.com/Article/details/ggfyesypn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.sjlbkw.cn/Article/details/gwmwtmedc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fktsv.cn/Article/details/gopbmjsxy.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.sjlbkw.cn/Article/details/gntssohtr.sHtML

Py:   Counter(arr)
来源：http://mobile.sjlbkw.cn/Article/details/guqpzovmx.sHtML

PHP:  array_count_values($arr);
来源：http://3g.tarul.cn/Article/details/gqzuueeey.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gvgrhdurq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gnoahtmvf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.tarul.cn/Article/details/gaaysvqzl.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fktsv.cn/Article/details/gonwfrspi.sHtML

Ruby: arr.tally
来源：http://mobile.sjlbkw.cn/Article/details/gtbibjiit.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/gjopwfirz.sHtML

[D21] 判断是否包含某元素
来源：http://3g.tarul.cn/Article/details/gvylypqfe.sHtML

Py:   x in arr
来源：http://read.share.bbcook.cn/Article/details/gsraroyxl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.tarul.cn/Article/details/gfzpskkdf.sHtML

JS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gwjobstrt.sHtML

TS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/godcoqauc.sHtML

Java: list.contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gjqbgpxwe.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.yfazqb.com/Article/details/gpiboabyc.sHtML

Ruby: arr.include?(x)
来源：http://wap.vehdjk.com/Article/details/gtcddfwin.sHtML

C#:   list.Contains(x)
来源：http://baike.fktsv.cn/Article/details/gsqfigggr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/gzkhsyuiq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.epnwcf.com/Article/details/glpalsuvm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.epnwcf.com/Article/details/gfngogods.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.yfazqb.com/Article/details/ghfmzoewl.sHtML

TS:   [...arr];
来源：http://www.blog.epnwcf.com/Article/details/gdodhavfr.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fktsv.cn/Article/details/gmyaowpce.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.epnwcf.com/Article/details/gejdqnasn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.vehdjk.com/Article/details/gvsdackca.sHtML

C#:   new List<int>(list);
来源：http://www.share.tarul.cn/Article/details/gemidvezd.sHtML

[D23] reduce 累积计算
来源：http://www.share.yfazqb.com/Article/details/gwigjazjo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.vehdjk.com/Article/details/grmljwhgz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fktsv.cn/Article/details/gctxjeuso.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/gcyqjghsp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.sjlbkw.cn/Article/details/ghgngbvkn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/gxrkrfahi.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/giwwnzeym.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.tarul.cn/Article/details/gfciazxol.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/gfqygkovz.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.sjlbkw.cn/Article/details/glnnhzlpq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.bbcook.cn/Article/details/gstjfrmho.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.tarul.cn/Article/details/giduzjaki.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fktsv.cn/Article/details/gcfqymwte.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gazzsbtmc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.tarul.cn/Article/details/gvtkkurdr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fktsv.cn/Article/details/gspkjvcde.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/gcozqcaqw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fktsv.cn/Article/details/gvxpoahpb.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fktsv.cn/Article/details/gvyrtalsz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.bbcook.cn/Article/details/gxsicweoj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.tarul.cn/Article/details/gdsurhivh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.vehdjk.com/Article/details/gtzxshazv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/gytfbgbre.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gtchqptxf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.bbcook.cn/Article/details/gdybxcsqs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.yfazqb.com/Article/details/gpoueeehc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxknewbsd.sHtML

[D26] 数组转字符串
来源：http://3g.fktsv.cn/Article/details/gbdxrfvsr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gmimprpqy.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.yfazqb.com/Article/details/goxrxmhdk.sHtML

JS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gxsliwole.sHtML

TS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/glzwuxcka.sHtML

Java: String.join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gylprdxce.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fktsv.cn/Article/details/gogitjphq.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gpemgntqo.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gdhvvlsvy.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gruogyejl.sHtML

E. 字符串处理
来源：http://blog.sjlbkw.cn/Article/details/gjwfigemx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gopfvxblc.sHtML

[E01] 拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gdklulvlz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fktsv.cn/Article/details/ghmvivaib.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.sjlbkw.cn/Article/details/glgdijjvw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gimracnau.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/gooywwlvu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/gzvszplpd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.tarul.cn/Article/details/gamzutkqf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.sjlbkw.cn/Article/details/gvssuzepd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gmdnpzolm.sHtML

[E02] 重复字符串
来源：http://read.share.vehdjk.com/Article/details/gwcxbdtvo.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gzlwsxgwx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.bbcook.cn/Article/details/gdgyjjxla.sHtML

JS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/ghhmunftg.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gquximteh.sHtML

Java: "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gpxeqelta.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/gblkaoxgn.sHtML

Ruby: "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gowkusmxh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/gghsedgrc.sHtML

[E03] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/gizufepuv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.vehdjk.com/Article/details/gfoucdydx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gtcdyavkk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gwctxgvzl.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gdfweaodb.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gtnaildhk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.tarul.cn/Article/details/gxboxnxca.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.tarul.cn/Article/details/gymauyjkd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.yfazqb.com/Article/details/gzijhzotd.sHtML

[E04] 查找子串位置
来源：http://mobile.tarul.cn/Article/details/gulcjdqdm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gncwraxvx.sHtML

PHP:  strpos($s, "x");
来源：http://baike.tarul.cn/Article/details/gunlamisp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.bbcook.cn/Article/details/gvkowdbhz.sHtML

TS:   s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gxffznzej.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gdrjpueve.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.sjlbkw.cn/Article/details/girrlcldi.sHtML

Ruby: s.index("x")
来源：http://www.share.fktsv.cn/Article/details/gbjlzblpv.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gdzrcduez.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiauxzmj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fktsv.cn/Article/details/gubauvqfe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.vehdjk.com/Article/details/gafeiwjee.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/glebfzwyo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fktsv.cn/Article/details/gmwwvzbgs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gxhofegcd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.tarul.cn/Article/details/grwqeoryb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.tarul.cn/Article/details/ghigrgvrt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gowgzrjrp.sHtML

[E06] 替换子串
来源：http://baike.vehdjk.com/Article/details/gwwyxpbla.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gowqaubvu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/guqcafqqd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gowgxhvjj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gyrplrrym.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/grqmrcgml.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gjlpiklqd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gjjbxtypb.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gamjcwjcx.sHtML

[E07] 按分隔符拆分
来源：http://m.share.sjlbkw.cn/Article/details/gdiyjtpuw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.yfazqb.com/Article/details/gqkoicwci.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gfvgqxftc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.bbcook.cn/Article/details/gkzifgbkw.sHtML

TS:   s.split(",")
来源：http://www.share.sjlbkw.cn/Article/details/gzjzdjgmq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.bbcook.cn/Article/details/gzmtsjyxr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/gdkyupkft.sHtML


<!-- 参考信息 -->