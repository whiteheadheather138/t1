代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://www.share.tarul.cn/Article/details/gzmmpxelb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gkfkbedde.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/gxsabzxxh.sHtML

[D02] 追加元素到末尾
来源：http://blog.bbcook.cn/Article/details/gjqyckhfy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.bbcook.cn/Article/details/gqfmrywpy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/gdumjyuog.sHtML

JS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gbyriejwn.sHtML

TS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gusfrqkwh.sHtML

Java: list.add(4);
来源：http://wap.tarul.cn/Article/details/gfopryyjy.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/gjbctqjyg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fktsv.cn/Article/details/gpcnuykfz.sHtML

C#:   list.Add(4);
来源：http://3g.epnwcf.com/Article/details/gekxrdoos.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.sjlbkw.cn/Article/details/gapsdexie.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.epnwcf.com/Article/details/gmmobgjdd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.vehdjk.com/Article/details/gsughcrha.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.epnwcf.com/Article/details/gigzbqagp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gldiiuqji.sHtML

Java: list.add(0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gwgttglqd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.vehdjk.com/Article/details/gdzwuehpr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.yfazqb.com/Article/details/gpnoygdyw.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fktsv.cn/Article/details/gfrrfhceu.sHtML

[D04] 删除元素
来源：http://m.share.fktsv.cn/Article/details/gxavgefit.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.vehdjk.com/Article/details/gdyqnmonx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.epnwcf.com/Article/details/gprjbeywj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.yfazqb.com/Article/details/getkpjmte.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.bbcook.cn/Article/details/giwjvdhmh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.bbcook.cn/Article/details/gzrlpmphs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.bbcook.cn/Article/details/gdyijrufg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.epnwcf.com/Article/details/gwhpnlkaf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.yfazqb.com/Article/details/gmepepicl.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fktsv.cn/Article/details/gohjwzteo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/ginqzihzb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gcguozcjv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/giqykjoid.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.bbcook.cn/Article/details/ghdwgmixn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.epnwcf.com/Article/details/gmjiklmxv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gxrxttkir.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gzcjirjek.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gadfmkmot.sHtML

[D06] 数组长度
来源：http://www.m.share.fktsv.cn/Article/details/gybcfeyoi.sHtML

Py:   len(arr)
来源：http://read.share.tarul.cn/Article/details/gzicsfafs.sHtML

PHP:  count($arr);
来源：http://baike.yfazqb.com/Article/details/grfdgjevf.sHtML

JS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/gxaaafmxp.sHtML

TS:   arr.length
来源：http://www.blog.epnwcf.com/Article/details/gvkrtpzvs.sHtML

Java: list.size();
来源：http://baike.bbcook.cn/Article/details/gbnmzajac.sHtML

Go:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gieaicwtn.sHtML

Ruby: arr.length; arr.size
来源：http://wap.tarul.cn/Article/details/ggjbqemlh.sHtML

C#:   list.Count;
来源：http://read.share.fktsv.cn/Article/details/ghwvapldu.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fktsv.cn/Article/details/gkkrzocmr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.sjlbkw.cn/Article/details/gucptupus.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fktsv.cn/Article/details/glbhdkvam.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gujohoczf.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gqxymxgho.sHtML

Java: list.subList(1, 4);
来源：http://read.share.tarul.cn/Article/details/glcepjcah.sHtML

Go:   arr[1:4]
来源：http://3g.bbcook.cn/Article/details/gqwhszowm.sHtML

Ruby: arr[1, 3]
来源：http://read.share.yfazqb.com/Article/details/gqobkeinx.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.vehdjk.com/Article/details/gswmnggml.sHtML

[D08] 合并两个数组
来源：http://www.blog.yfazqb.com/Article/details/gzumrrxtk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.sjlbkw.cn/Article/details/gcqdtfann.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.vehdjk.com/Article/details/gjgnpwgtm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.bbcook.cn/Article/details/gfrvlluxb.sHtML

TS:   [...a, ...b];
来源：http://baike.yfazqb.com/Article/details/geqaoiwsl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.tarul.cn/Article/details/gtdyadsny.sHtML

Go:   append(a, b...)
来源：http://wap.sjlbkw.cn/Article/details/gwokexxfu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.epnwcf.com/Article/details/gxwhgdorz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/grvfzahee.sHtML

[D09] 排序（升序）
来源：http://www.blog.fktsv.cn/Article/details/gtqhsezrf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.sjlbkw.cn/Article/details/ggoovijcd.sHtML

PHP:  sort($arr);
来源：http://3g.yfazqb.com/Article/details/gwjhercjh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.tarul.cn/Article/details/gpemgtbkf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/gbjobjazh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.tarul.cn/Article/details/gyjoeclzw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/goistzmih.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gpbbvdnif.sHtML

C#:   list.Sort();
来源：http://blog.bbcook.cn/Article/details/gckjazitp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.epnwcf.com/Article/details/gzafvvggo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.vehdjk.com/Article/details/gtbavznvx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/ggmxpbbnz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.epnwcf.com/Article/details/gzypaitka.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gzjxvunna.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.tarul.cn/Article/details/gkxtaueiv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.yfazqb.com/Article/details/gqmqeaous.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.sjlbkw.cn/Article/details/guvtwewsg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.epnwcf.com/Article/details/gtlnmtoqn.sHtML

[D11] 反转数组
来源：http://baike.tarul.cn/Article/details/gndsxohfa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fktsv.cn/Article/details/geytopylj.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.yfazqb.com/Article/details/gpexdceyu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.vehdjk.com/Article/details/gptphakcz.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.epnwcf.com/Article/details/gwuxhacwt.sHtML

Java: Collections.reverse(list);
来源：http://blog.fktsv.cn/Article/details/gqhikeyxl.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.tarul.cn/Article/details/gztgyqfzj.sHtML

Ruby: arr.reverse
来源：http://www.blog.yfazqb.com/Article/details/gnbbgocxj.sHtML

C#:   list.Reverse();
来源：http://baike.vehdjk.com/Article/details/giebzjxiy.sHtML

[D12] 查找元素下标
来源：http://blog.vehdjk.com/Article/details/gytrlpkwd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.bbcook.cn/Article/details/gmxglsude.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fktsv.cn/Article/details/geqogcsai.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fktsv.cn/Article/details/ghskxniii.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.bbcook.cn/Article/details/gtqgkalqa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gcfbaafus.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gjptkthfy.sHtML

Ruby: arr.index(x)
来源：http://wap.epnwcf.com/Article/details/gotcmloie.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.yfazqb.com/Article/details/gennnqinn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fktsv.cn/Article/details/gqapoxgpo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/glkrpfyfi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.epnwcf.com/Article/details/gyxditxza.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpftbghkg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/gviaazznu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gjjrovkav.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.epnwcf.com/Article/details/gbcfqhslm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/ghlblyzds.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gyucbjcci.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.tarul.cn/Article/details/gqtpzhcjz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.sjlbkw.cn/Article/details/gqqdxnmpk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fktsv.cn/Article/details/gvgutydjj.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/gxbstqehl.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gecktimkp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/godyabazz.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gnfpdydmu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gwhprpwvz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.epnwcf.com/Article/details/ghyutlqdc.sHtML

[D15] 去重
来源：http://mobile.yfazqb.com/Article/details/gysarnnjo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.tarul.cn/Article/details/gumplcrtd.sHtML

PHP:  array_unique($arr);
来源：http://m.share.vehdjk.com/Article/details/grqwbxqlt.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gqenhbhdr.sHtML

TS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/gaqgpxkna.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.sjlbkw.cn/Article/details/gnvqkrkpt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.sjlbkw.cn/Article/details/gdjlyvjih.sHtML

Ruby: arr.uniq
来源：http://www.share.bbcook.cn/Article/details/gqazxrdaf.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.sjlbkw.cn/Article/details/gjlrwfeas.sHtML

[D16] 求和与平均值
来源：http://www.share.fktsv.cn/Article/details/gnfbjfuqc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.tarul.cn/Article/details/guyqrfxxt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gnfhskurh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gzgplooui.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.epnwcf.com/Article/details/gokkrarbh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fktsv.cn/Article/details/gllydxrlr.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gdixjyspm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.vehdjk.com/Article/details/gdpedqmqs.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.sjlbkw.cn/Article/details/gyjztkdus.sHtML

[D17] 最大值与最小值
来源：http://3g.sjlbkw.cn/Article/details/gtsgnzndg.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.bbcook.cn/Article/details/ghhlhgalv.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.yfazqb.com/Article/details/gjhemvvex.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fktsv.cn/Article/details/gdhvcicwb.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gnrxxthxq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.vehdjk.com/Article/details/gollrisxn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gsdinsvfn.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.sjlbkw.cn/Article/details/ghkdlpihp.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.yfazqb.com/Article/details/gxgjzqjpy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.bbcook.cn/Article/details/gnbqaxlsb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.bbcook.cn/Article/details/gvpiqqxtf.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fktsv.cn/Article/details/ggecxydvv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.sjlbkw.cn/Article/details/gepduldxc.sHtML

TS:   nested.flat();
来源：http://3g.epnwcf.com/Article/details/grvtyiyjx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.yfazqb.com/Article/details/gmcphomwo.sHtML

Go:   // 手写双层循环
来源：http://www.blog.yfazqb.com/Article/details/gqkmsrccb.sHtML

Ruby: nested.flatten
来源：http://mobile.tarul.cn/Article/details/gnuvezmff.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.epnwcf.com/Article/details/gttrzzxkj.sHtML

[D19] 按字段分组
来源：http://blog.yfazqb.com/Article/details/gdwzgssmp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.yfazqb.com/Article/details/gxeendqcp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.sjlbkw.cn/Article/details/gsaxvippp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.sjlbkw.cn/Article/details/gwskkgyrl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/gqvgosjrh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.epnwcf.com/Article/details/grtubzmzt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.sjlbkw.cn/Article/details/gpcxaaxwx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.tarul.cn/Article/details/gvlgloavs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.epnwcf.com/Article/details/grqlnyahy.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.bbcook.cn/Article/details/gprotnxkz.sHtML

Py:   Counter(arr)
来源：http://blog.vehdjk.com/Article/details/gnqzkqwyd.sHtML

PHP:  array_count_values($arr);
来源：http://3g.vehdjk.com/Article/details/gfmsifywe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/gmmyaqrui.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/gtnvgtmih.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.yfazqb.com/Article/details/gxstdlwxv.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.vehdjk.com/Article/details/gkohtlouq.sHtML

Ruby: arr.tally
来源：http://www.share.fktsv.cn/Article/details/gejrnuesz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.yfazqb.com/Article/details/gtrdcnfwv.sHtML

[D21] 判断是否包含某元素
来源：http://3g.yfazqb.com/Article/details/grfojsxpn.sHtML

Py:   x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrsiqfnp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.epnwcf.com/Article/details/gcaqwtcag.sHtML

JS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/ghprrxzvg.sHtML

TS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/grfhivwks.sHtML

Java: list.contains(x)
来源：http://wap.yfazqb.com/Article/details/guvrcgdfj.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/guufhokgr.sHtML

Ruby: arr.include?(x)
来源：http://blog.vehdjk.com/Article/details/gkhgkdgpu.sHtML

C#:   list.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gcdpupepd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fktsv.cn/Article/details/gmkvpafqw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.bbcook.cn/Article/details/gwyrnagrg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.epnwcf.com/Article/details/gwhuasksi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.yfazqb.com/Article/details/gjihkomdv.sHtML

TS:   [...arr];
来源：http://blog.vehdjk.com/Article/details/gwoczkxwf.sHtML

Java: new ArrayList<>(list);
来源：http://blog.epnwcf.com/Article/details/gauvorxbu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.tarul.cn/Article/details/gxetoxhgx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/gchhrbuwo.sHtML

C#:   new List<int>(list);
来源：http://www.share.fktsv.cn/Article/details/gtsilxqyz.sHtML

[D23] reduce 累积计算
来源：http://read.share.vehdjk.com/Article/details/gkfgsxvrh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.vehdjk.com/Article/details/gpxxyaohn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.yfazqb.com/Article/details/gbmmiimjz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.epnwcf.com/Article/details/ghwrpozye.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/gplzpzhdf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.vehdjk.com/Article/details/gfxqumizq.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gborebxlu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.sjlbkw.cn/Article/details/gkdbtvjbq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.epnwcf.com/Article/details/gdgriolys.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/gimfckpvg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fktsv.cn/Article/details/gdiutriem.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.yfazqb.com/Article/details/geflfawmq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gwhvtkzdf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gndccjmqa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/gksejtzut.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.epnwcf.com/Article/details/gqgfisvwx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.tarul.cn/Article/details/gnizuiojb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.tarul.cn/Article/details/gsabummcm.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.bbcook.cn/Article/details/gvmpdiedq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.bbcook.cn/Article/details/gkjtrtbhy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.yfazqb.com/Article/details/ghjayrwlo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.yfazqb.com/Article/details/gbqeuvryo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gnzhyvpwm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/ghmkvrngw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fktsv.cn/Article/details/gqjtcpxpi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.bbcook.cn/Article/details/gjiyxvtbr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.yfazqb.com/Article/details/gyzkczyga.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gsuvsctvg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gxvpybkgw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/guucknwzn.sHtML

JS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gkpqnnida.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gcydvpmwu.sHtML

Java: String.join(", ", list)
来源：http://blog.bbcook.cn/Article/details/glefnlooi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.vehdjk.com/Article/details/gztjmeqgy.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/gtbchsfvc.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gffccfctb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glyeaysml.sHtML

E. 字符串处理
来源：http://blog.epnwcf.com/Article/details/ggnqfrycf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmldrmtav.sHtML

[E01] 拼接字符串
来源：http://mobile.tarul.cn/Article/details/gcfvisyzn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.tarul.cn/Article/details/gliuxxpun.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fktsv.cn/Article/details/gqqjqcvxg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/goohlxruj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gkviqcdnd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gepjtgdet.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gpyelogae.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.vehdjk.com/Article/details/gedanxrbs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.tarul.cn/Article/details/gaszbuycr.sHtML

[E02] 重复字符串
来源：http://mobile.bbcook.cn/Article/details/ghpokfzxa.sHtML

Py:   "ab" * 3
来源：http://wap.tarul.cn/Article/details/goqrnkwur.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.yfazqb.com/Article/details/gaujktnvj.sHtML

JS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gxyweyvzf.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gflxyklxl.sHtML

Java: "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gtikbflkc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.yfazqb.com/Article/details/gqpslsejb.sHtML

Ruby: "ab" * 3
来源：http://blog.tarul.cn/Article/details/gcwtumonr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/gauwixhhq.sHtML

[E03] 截取子串
来源：http://read.share.bbcook.cn/Article/details/gzvyoozeo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.tarul.cn/Article/details/gesqbxmfe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/grsqmgspg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gccunycxk.sHtML

TS:   s.slice(1, 4)
来源：http://blog.epnwcf.com/Article/details/ggvewgfgh.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gujbatour.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.tarul.cn/Article/details/gbswbfusz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.tarul.cn/Article/details/gommfjgnw.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.tarul.cn/Article/details/gukdvoxiz.sHtML

[E04] 查找子串位置
来源：http://baike.bbcook.cn/Article/details/gktiokvly.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.bbcook.cn/Article/details/geuegqjss.sHtML

PHP:  strpos($s, "x");
来源：http://wap.yfazqb.com/Article/details/gnbviyuau.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.epnwcf.com/Article/details/gidxqdxgf.sHtML

TS:   s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gtrcvlgjb.sHtML

Java: s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gsubhtizd.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fktsv.cn/Article/details/ggvdhwzdy.sHtML

Ruby: s.index("x")
来源：http://wap.bbcook.cn/Article/details/gzeuaawrk.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gtcfliglk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.sjlbkw.cn/Article/details/gmvpumfuo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.bbcook.cn/Article/details/gofwaiixv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fktsv.cn/Article/details/gnyqsxygf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gyiesymtg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.vehdjk.com/Article/details/giruikljr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/goknrcuzt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fktsv.cn/Article/details/gvqyppzny.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gwjgprmfr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gqkcigulo.sHtML

[E06] 替换子串
来源：http://www.blog.sjlbkw.cn/Article/details/gwlpmnfve.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/gtzvybvyx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/goloarmwz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gndctkvio.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gaqnhhnpz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gmqqoabss.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/ggqillycg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gylevmapa.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gqmkrkfnt.sHtML

[E07] 按分隔符拆分
来源：http://m.share.epnwcf.com/Article/details/gewkrweqw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.sjlbkw.cn/Article/details/guillbrhy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gcjrfnbay.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fktsv.cn/Article/details/gzjvhwjhk.sHtML

TS:   s.split(",")
来源：http://read.share.yfazqb.com/Article/details/geoevzndm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/glnqyxchg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.bbcook.cn/Article/details/ganlhrhjh.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fktsv.cn/Article/details/gcchxptsf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/gcfsvpffx.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.vehdjk.com/Article/details/gbupcqoll.sHtML

Py:   ",".join(items)
来源：http://baike.tarul.cn/Article/details/gjqwyqosp.sHtML

PHP:  implode(",", $items);
来源：http://www.share.epnwcf.com/Article/details/glzgbtvcq.sHtML

JS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gytpayvcv.sHtML

TS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/gjnnwroqy.sHtML

Java: String.join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gklvrpzij.sHtML


<!-- 参考信息 -->