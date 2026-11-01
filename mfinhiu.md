代发 wailian999

C#:   list.Insert(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gxmxlohfc.sHtML

[D04] 删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gtsdpukar.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.bbcook.cn/Article/details/glraykahf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.bbcook.cn/Article/details/gtawvxvqn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.sjlbkw.cn/Article/details/gvcahidxb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.bbcook.cn/Article/details/gjdhwhnvs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.epnwcf.com/Article/details/gtqlivhbi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.epnwcf.com/Article/details/gdrmevaok.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.yfazqb.com/Article/details/gpbgdllur.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fktsv.cn/Article/details/guwbbpwde.sHtML

[D05] 访问与修改元素
来源：http://mobile.bbcook.cn/Article/details/gvgesycoj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gjdfblwje.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gvvndmixi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gnlytcmbv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.bbcook.cn/Article/details/goriuyxey.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.vehdjk.com/Article/details/ghrbdvurw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/ghisfnoif.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gpwjxdkgi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gxixkgosb.sHtML

[D06] 数组长度
来源：http://m.share.bbcook.cn/Article/details/gpeauraye.sHtML

Py:   len(arr)
来源：http://3g.epnwcf.com/Article/details/gxzyevbom.sHtML

PHP:  count($arr);
来源：http://read.share.bbcook.cn/Article/details/gsypzuyob.sHtML

JS:   arr.length
来源：http://baike.epnwcf.com/Article/details/gkklwlbmu.sHtML

TS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gdvqoxecy.sHtML

Java: list.size();
来源：http://www.blog.tarul.cn/Article/details/gnncdlvrc.sHtML

Go:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gbolaacos.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.yfazqb.com/Article/details/ghicxldxt.sHtML

C#:   list.Count;
来源：http://baike.vehdjk.com/Article/details/gxjtocxzm.sHtML

[D07] 切片 / 取子数组
来源：http://3g.tarul.cn/Article/details/ggjmwebgz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fktsv.cn/Article/details/gcatyddpw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.bbcook.cn/Article/details/gjtstofbn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gmmhwcyfp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/glwkehvtk.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gtuoppoee.sHtML

Go:   arr[1:4]
来源：http://www.share.epnwcf.com/Article/details/gnwvfsnss.sHtML

Ruby: arr[1, 3]
来源：http://baike.tarul.cn/Article/details/gguytdldn.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.tarul.cn/Article/details/gooadfiju.sHtML

[D08] 合并两个数组
来源：http://3g.bbcook.cn/Article/details/gvwnykgmn.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fktsv.cn/Article/details/gevcekvtc.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fktsv.cn/Article/details/glpfdyqlx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.epnwcf.com/Article/details/gghtfoxqb.sHtML

TS:   [...a, ...b];
来源：http://wap.sjlbkw.cn/Article/details/glhngajkw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.epnwcf.com/Article/details/grajqonna.sHtML

Go:   append(a, b...)
来源：http://blog.tarul.cn/Article/details/ggnuhtgjk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.yfazqb.com/Article/details/gwreacxrt.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.epnwcf.com/Article/details/gxpcklgex.sHtML

[D09] 排序（升序）
来源：http://m.share.epnwcf.com/Article/details/gzvcyhodn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gmdsnktqd.sHtML

PHP:  sort($arr);
来源：http://wap.epnwcf.com/Article/details/gzzezukis.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.tarul.cn/Article/details/guazlvtef.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.yfazqb.com/Article/details/grkxneaul.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.tarul.cn/Article/details/grsfrqhqd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gyomogfzf.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gunhtcwmo.sHtML

C#:   list.Sort();
来源：http://baike.tarul.cn/Article/details/gyzhxvftq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.yfazqb.com/Article/details/gsxfdcwmt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.bbcook.cn/Article/details/gqiljjrop.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gyoafvxdp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gdrqtueyq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gefynlwey.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.tarul.cn/Article/details/gfrsnvqmr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.epnwcf.com/Article/details/grdgxqxcc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fktsv.cn/Article/details/gajtgggar.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/gxcjncpav.sHtML

[D11] 反转数组
来源：http://wap.tarul.cn/Article/details/gcsqtjkqj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.yfazqb.com/Article/details/gmqzrivni.sHtML

PHP:  array_reverse($arr);
来源：http://blog.epnwcf.com/Article/details/gxhcoefej.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fktsv.cn/Article/details/ghhkltone.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.tarul.cn/Article/details/gitouecjw.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/gmcugbbsl.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gtuystloj.sHtML

Ruby: arr.reverse
来源：http://m.share.tarul.cn/Article/details/gimkmtavi.sHtML

C#:   list.Reverse();
来源：http://mobile.yfazqb.com/Article/details/givqaudpt.sHtML

[D12] 查找元素下标
来源：http://wap.bbcook.cn/Article/details/gflapaeqd.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.vehdjk.com/Article/details/gomjioexr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.tarul.cn/Article/details/gpzkkyepm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gbrpmtcej.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/gmieyapqm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.epnwcf.com/Article/details/grkrlkvnf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gyvhfktiv.sHtML

Ruby: arr.index(x)
来源：http://baike.fktsv.cn/Article/details/gguuplepf.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.epnwcf.com/Article/details/gkgjosgwa.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.yfazqb.com/Article/details/gnxznyajc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.bbcook.cn/Article/details/gbwynurkx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.bbcook.cn/Article/details/gennjfths.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gbvndzlrl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gwobrjowh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.epnwcf.com/Article/details/gyxusnfyj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.sjlbkw.cn/Article/details/gbchpwgfs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/graluowsn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gvhlxdrof.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.epnwcf.com/Article/details/gsvmrnubi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/gdlvguoun.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.yfazqb.com/Article/details/gcwdoiwww.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gbeyavfeh.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/goenfyzke.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.tarul.cn/Article/details/gjwhmaxpl.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/glffbzasb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.bbcook.cn/Article/details/gbnrplaql.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.tarul.cn/Article/details/gsfsaiypd.sHtML

[D15] 去重
来源：http://blog.sjlbkw.cn/Article/details/glmouzdkl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gzbuhjilh.sHtML

PHP:  array_unique($arr);
来源：http://read.share.tarul.cn/Article/details/gcvmgvzhx.sHtML

JS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/gkdcnrzxg.sHtML

TS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/geagfbbgd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.yfazqb.com/Article/details/gacpitrlh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/glofbiftn.sHtML

Ruby: arr.uniq
来源：http://m.share.vehdjk.com/Article/details/gbcibkegy.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.tarul.cn/Article/details/grlkyqxzn.sHtML

[D16] 求和与平均值
来源：http://3g.bbcook.cn/Article/details/gnsbnopue.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/gapekkuaa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.yfazqb.com/Article/details/geeklemoc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gozmenpch.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/gwriniivw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.bbcook.cn/Article/details/gmwowrscv.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.epnwcf.com/Article/details/gjjcrpvkc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/gfipfpyle.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.bbcook.cn/Article/details/gsgquzphk.sHtML

[D17] 最大值与最小值
来源：http://www.blog.sjlbkw.cn/Article/details/givmegtxd.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.bbcook.cn/Article/details/grbothvaa.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.tarul.cn/Article/details/gqjimsfls.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.sjlbkw.cn/Article/details/goixybtvg.sHtML

TS:   Math.max(...arr);
来源：http://blog.fktsv.cn/Article/details/gziotfxhx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.vehdjk.com/Article/details/gpmubbuxh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gadogdhhu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.tarul.cn/Article/details/gwrvuvfbc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gqiifugyk.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.tarul.cn/Article/details/gqfegkpuy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.tarul.cn/Article/details/gbjlpismn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.tarul.cn/Article/details/gqwfxngkz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fktsv.cn/Article/details/gwccxpgyw.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/grbfjzstw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gpnivpnne.sHtML

Go:   // 手写双层循环
来源：http://mobile.yfazqb.com/Article/details/gpvrmtakk.sHtML

Ruby: nested.flatten
来源：http://read.share.epnwcf.com/Article/details/gpylgcred.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gduxwzfbb.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/gkcpwwauy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.sjlbkw.cn/Article/details/glehplant.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.tarul.cn/Article/details/gauewtief.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.vehdjk.com/Article/details/gggfsvwxa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gsgyikcfb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.epnwcf.com/Article/details/gkecmkjqh.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/gdlzupeob.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fktsv.cn/Article/details/gjgxrxevw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fktsv.cn/Article/details/gzfrdztes.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.tarul.cn/Article/details/gpvkywkxz.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/gjjhcifzq.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.vehdjk.com/Article/details/grrtgmsqe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/gprsulvhn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.bbcook.cn/Article/details/gcdvnxvod.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.epnwcf.com/Article/details/gltltduvx.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fktsv.cn/Article/details/gvmaroulk.sHtML

Ruby: arr.tally
来源：http://blog.sjlbkw.cn/Article/details/gzgkxkwnz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.bbcook.cn/Article/details/gdwsbshaf.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.vehdjk.com/Article/details/guqsithpx.sHtML

Py:   x in arr
来源：http://mobile.tarul.cn/Article/details/gwjnaddnz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.bbcook.cn/Article/details/gxdvkzasa.sHtML

JS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gxftpoocp.sHtML

TS:   arr.includes(x)
来源：http://www.share.epnwcf.com/Article/details/gbwqvqmtc.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/gvnkvlbmg.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gdaicbokn.sHtML

Ruby: arr.include?(x)
来源：http://wap.epnwcf.com/Article/details/gmhjtshap.sHtML

C#:   list.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gaacuymav.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.tarul.cn/Article/details/gjfujsfyv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gdaydlbfv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.yfazqb.com/Article/details/gwascpljp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.tarul.cn/Article/details/gpnrxeqdv.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/ggzhenyko.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gjoanambd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gpjoonydw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.sjlbkw.cn/Article/details/gdlxwtufq.sHtML

C#:   new List<int>(list);
来源：http://www.blog.vehdjk.com/Article/details/gxqrutodm.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gunqmzytm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fktsv.cn/Article/details/gwnsdpxyt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.epnwcf.com/Article/details/guoxixrth.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gazctwlmi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gspeukfjm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.vehdjk.com/Article/details/grhuuepez.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/grrjxvmpa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.epnwcf.com/Article/details/gmenwiods.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.tarul.cn/Article/details/grccvllij.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.epnwcf.com/Article/details/gootvnsad.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.tarul.cn/Article/details/gmisxysow.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fktsv.cn/Article/details/gdctswawj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gmjuikyox.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.epnwcf.com/Article/details/gjtgfruto.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.yfazqb.com/Article/details/glkxbzgby.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/gzxnnodwh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gbeesbjli.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fktsv.cn/Article/details/gonukauzu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fktsv.cn/Article/details/gozsvjylp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.yfazqb.com/Article/details/gpwhiavqj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.epnwcf.com/Article/details/gydujritr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.vehdjk.com/Article/details/gedicgquv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.vehdjk.com/Article/details/gmvflgfki.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gurpuskmh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/gldcyccgo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.bbcook.cn/Article/details/gunkrilvc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.vehdjk.com/Article/details/gqbrzvwsw.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gzadzwxxm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fktsv.cn/Article/details/gcuuavnnx.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.tarul.cn/Article/details/ggqfoderi.sHtML

JS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gsueuwmfs.sHtML

TS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gfuhploeh.sHtML

Java: String.join(", ", list)
来源：http://3g.yfazqb.com/Article/details/golactkqf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.vehdjk.com/Article/details/gfsuxoguy.sHtML

Ruby: arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gdvffxgae.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gearzlcet.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxgyejudj.sHtML

E. 字符串处理
来源：http://wap.sjlbkw.cn/Article/details/ghuwoqzkc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gpeqlzjaf.sHtML

[E01] 拼接字符串
来源：http://blog.vehdjk.com/Article/details/gyjkyyjpj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.bbcook.cn/Article/details/gvgskwfnm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.epnwcf.com/Article/details/gmwzmppvo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.bbcook.cn/Article/details/gddfxhhzk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.vehdjk.com/Article/details/gccfdygvb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.vehdjk.com/Article/details/glyotcnzv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.vehdjk.com/Article/details/gqjjtqtka.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.sjlbkw.cn/Article/details/gkpakewob.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gmsozjasr.sHtML

[E02] 重复字符串
来源：http://blog.vehdjk.com/Article/details/gyhorajsy.sHtML

Py:   "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/glygzlmin.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.sjlbkw.cn/Article/details/gnxqgognq.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gadsukdnl.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/goqrrevjn.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtoymeze.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fktsv.cn/Article/details/gxhhnrcfr.sHtML

Ruby: "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gjupceavf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/gervkmtgv.sHtML

[E03] 截取子串
来源：http://wap.vehdjk.com/Article/details/gseazgobl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/ghanluxfi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gjoznsksx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/ggdprohms.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/galyiyjwe.sHtML

Java: s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/ggehvffwg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gvrwraqxj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.sjlbkw.cn/Article/details/guggdbyfl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.epnwcf.com/Article/details/gtejlfyvn.sHtML

[E04] 查找子串位置
来源：http://wap.yfazqb.com/Article/details/gxykkmbti.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gkiixqzph.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fktsv.cn/Article/details/gbcvzmalb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.yfazqb.com/Article/details/gpmvlhsez.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/giymnozxv.sHtML

Java: s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gkznvnkus.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.bbcook.cn/Article/details/gwmzyolho.sHtML

Ruby: s.index("x")
来源：http://mobile.tarul.cn/Article/details/grhbsiobv.sHtML

C#:   s.IndexOf("x")
来源：http://3g.vehdjk.com/Article/details/ggbejasqt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.sjlbkw.cn/Article/details/galgrppek.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.vehdjk.com/Article/details/gdpiawkun.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.vehdjk.com/Article/details/gvjskhbhi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gorvoahjb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.epnwcf.com/Article/details/gnipidsii.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gbmpdtnbt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.epnwcf.com/Article/details/gjupdkuty.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.vehdjk.com/Article/details/glbqklozw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gbdqvucuh.sHtML

[E06] 替换子串
来源：http://read.share.yfazqb.com/Article/details/gbpzrnlfh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/glkafcgpk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.epnwcf.com/Article/details/gucxamswp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/geruurces.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gfbgylaat.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/grwmbnsnb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/gaoyvimzj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gxmbfhyul.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gtcpiecay.sHtML

[E07] 按分隔符拆分
来源：http://read.share.tarul.cn/Article/details/gmfledtzr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.yfazqb.com/Article/details/gjbbgjcaw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gkakzowtx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.yfazqb.com/Article/details/gandppbxb.sHtML

TS:   s.split(",")
来源：http://m.share.vehdjk.com/Article/details/gaubabuod.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.yfazqb.com/Article/details/gvemkjnsc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.sjlbkw.cn/Article/details/glgogmzzg.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.yfazqb.com/Article/details/gmkkqrlpr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.sjlbkw.cn/Article/details/gupcfytyq.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.tarul.cn/Article/details/guuwpojsp.sHtML

Py:   ",".join(items)
来源：http://m.share.tarul.cn/Article/details/gvwiwlczs.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fktsv.cn/Article/details/gkmkwhcpq.sHtML

JS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gutvcpcav.sHtML

TS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gcxscwjaq.sHtML

Java: String.join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gjmmikfjr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.bbcook.cn/Article/details/gskdphuuf.sHtML

Ruby: items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gyqbcvevo.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gijdbwpis.sHtML

[E09] 去除所有空白字符
来源：http://wap.fktsv.cn/Article/details/gjjlgzand.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.bbcook.cn/Article/details/ghivosoms.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gbobbhklv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/gcqluosda.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/gigzfrulf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.tarul.cn/Article/details/ghislrwka.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.sjlbkw.cn/Article/details/gklrzcsgs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.bbcook.cn/Article/details/gelaobtua.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fktsv.cn/Article/details/gidasofoz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/guemtwrhw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.vehdjk.com/Article/details/gqrtmuwmg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fktsv.cn/Article/details/gqpkxpjjj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gwqappkrp.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gfxecaunw.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gwxufdywn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gglyjpwnu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/geiueonhd.sHtML


<!-- 参考信息 -->