代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://read.share.bbcook.cn/Article/details/gpnrbrpbu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fktsv.cn/Article/details/gjikfewcl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.yfazqb.com/Article/details/gvvrrhkuz.sHtML

[D02] 追加元素到末尾
来源：http://mobile.sjlbkw.cn/Article/details/gdbyoqmaz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.sjlbkw.cn/Article/details/gomibxalo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.epnwcf.com/Article/details/godhbyjmk.sHtML

JS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/ghdhmolbv.sHtML

TS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/gwldfvnde.sHtML

Java: list.add(4);
来源：http://mobile.epnwcf.com/Article/details/grktdzdwf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.tarul.cn/Article/details/gyzazwlyj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.bbcook.cn/Article/details/gilyevnfe.sHtML

C#:   list.Add(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjzvhszk.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fktsv.cn/Article/details/gqeovvfar.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gjjxhhihl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.yfazqb.com/Article/details/gmecuuabd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.yfazqb.com/Article/details/gflflvwhk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/ggnmcgess.sHtML

Java: list.add(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gbnjpadxg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.vehdjk.com/Article/details/gegwhsldy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.yfazqb.com/Article/details/gekwzmseg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gbzkiegpt.sHtML

[D04] 删除元素
来源：http://read.share.tarul.cn/Article/details/gipyjmvfk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.vehdjk.com/Article/details/gkzleflai.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.tarul.cn/Article/details/gancxalde.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.bbcook.cn/Article/details/gyqosnabf.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.yfazqb.com/Article/details/gbefttkgt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.vehdjk.com/Article/details/gkpfiruio.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.yfazqb.com/Article/details/glkzqrzub.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.yfazqb.com/Article/details/gnvytdybn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/gcqypaogg.sHtML

[D05] 访问与修改元素
来源：http://3g.fktsv.cn/Article/details/gvpcegulf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.epnwcf.com/Article/details/ghrwxceqw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gnxkdkijj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgfpsdur.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.vehdjk.com/Article/details/gwvqfxqcn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.vehdjk.com/Article/details/gebmswllp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gshargpao.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.bbcook.cn/Article/details/gjvgbpzjs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.tarul.cn/Article/details/gaqwuuszz.sHtML

[D06] 数组长度
来源：http://wap.tarul.cn/Article/details/ggtntfbij.sHtML

Py:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/grtopigmf.sHtML

PHP:  count($arr);
来源：http://3g.fktsv.cn/Article/details/ghwbzmhjz.sHtML

JS:   arr.length
来源：http://m.share.fktsv.cn/Article/details/geboepnwn.sHtML

TS:   arr.length
来源：http://baike.epnwcf.com/Article/details/gnyqgmqzu.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gsynijvrx.sHtML

Go:   len(arr)
来源：http://read.share.tarul.cn/Article/details/giwzrhuze.sHtML

Ruby: arr.length; arr.size
来源：http://baike.bbcook.cn/Article/details/ghmllvgub.sHtML

C#:   list.Count;
来源：http://3g.yfazqb.com/Article/details/gpwyxblrh.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fktsv.cn/Article/details/grogcsifh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.vehdjk.com/Article/details/gjprcuxth.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/gunahuzhr.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.vehdjk.com/Article/details/giunizmzp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gkqxtxsqu.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/gbmtsqzrk.sHtML

Go:   arr[1:4]
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmvxzccl.sHtML

Ruby: arr[1, 3]
来源：http://read.share.yfazqb.com/Article/details/ghdsgiduj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/groddabog.sHtML

[D08] 合并两个数组
来源：http://mobile.tarul.cn/Article/details/gojfyelug.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.sjlbkw.cn/Article/details/gxwxdtxso.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fktsv.cn/Article/details/gnggubulg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.tarul.cn/Article/details/gdzezjlxk.sHtML

TS:   [...a, ...b];
来源：http://3g.epnwcf.com/Article/details/gclsskogh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fktsv.cn/Article/details/gqpiviqdv.sHtML

Go:   append(a, b...)
来源：http://mobile.bbcook.cn/Article/details/gzbboatfd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.yfazqb.com/Article/details/gewuccbgq.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.bbcook.cn/Article/details/gmkkshueq.sHtML

[D09] 排序（升序）
来源：http://mobile.yfazqb.com/Article/details/ghifngvca.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/gfcaafvhj.sHtML

PHP:  sort($arr);
来源：http://wap.sjlbkw.cn/Article/details/guxvhqyrq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fktsv.cn/Article/details/ggbvphtco.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.yfazqb.com/Article/details/gtdbqgifm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.yfazqb.com/Article/details/gkgyfjkrl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gygrhooyt.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gbfejnbjf.sHtML

C#:   list.Sort();
来源：http://baike.tarul.cn/Article/details/gewtvozio.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fktsv.cn/Article/details/gmjntoana.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.yfazqb.com/Article/details/gkcweysip.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.yfazqb.com/Article/details/gwpyflfkk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gpvufpxmm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/gbrcgtrwz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fktsv.cn/Article/details/gdfaisfdk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.epnwcf.com/Article/details/gdahobqrs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.sjlbkw.cn/Article/details/gablvwtjq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.epnwcf.com/Article/details/gztzvaqka.sHtML

[D11] 反转数组
来源：http://3g.yfazqb.com/Article/details/gnxibudqv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.bbcook.cn/Article/details/gjlvkexkq.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.yfazqb.com/Article/details/gdharsimd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/gdhhzludz.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fktsv.cn/Article/details/gxagucknd.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.epnwcf.com/Article/details/gkenkakwn.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.sjlbkw.cn/Article/details/gpgwgikcq.sHtML

Ruby: arr.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gkxbdmpef.sHtML

C#:   list.Reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gnfnmtbdo.sHtML

[D12] 查找元素下标
来源：http://3g.epnwcf.com/Article/details/gdbeouhdp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/geihepmih.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.tarul.cn/Article/details/gavlrduyh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/ggbebjgho.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gndiuvbtu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.epnwcf.com/Article/details/gspwiftwi.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.vehdjk.com/Article/details/gbfykcygg.sHtML

Ruby: arr.index(x)
来源：http://m.share.tarul.cn/Article/details/govhgmldp.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/gjcgcdcjx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.bbcook.cn/Article/details/gvsplqnzi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/gnsbdffeh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.epnwcf.com/Article/details/gfdmyawyx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.yfazqb.com/Article/details/glhnkscft.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gfmktceol.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.tarul.cn/Article/details/gvjwudmes.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.sjlbkw.cn/Article/details/gkdsphwwd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.yfazqb.com/Article/details/gtecjqbso.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.vehdjk.com/Article/details/gsosyvcup.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.yfazqb.com/Article/details/gihytojeq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.epnwcf.com/Article/details/gzpmtrupf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.tarul.cn/Article/details/giqxfeyed.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gobaglkcb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gucsbscdy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.tarul.cn/Article/details/gjigbwqpw.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gysvtkvnq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gafapnnfo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gokwyvjah.sHtML

[D15] 去重
来源：http://www.share.fktsv.cn/Article/details/gqeymgawx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gwjtyfmbe.sHtML

PHP:  array_unique($arr);
来源：http://m.share.bbcook.cn/Article/details/gqjjuhoun.sHtML

JS:   [...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/gdqptffaf.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/gxxuxrxph.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.yfazqb.com/Article/details/govnbzifq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fktsv.cn/Article/details/gthsmzaol.sHtML

Ruby: arr.uniq
来源：http://3g.epnwcf.com/Article/details/ggmqyuvax.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.epnwcf.com/Article/details/guinjvihy.sHtML

[D16] 求和与平均值
来源：http://wap.bbcook.cn/Article/details/gbkidvrnk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gfiymdeak.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.epnwcf.com/Article/details/gevmhzqog.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gxkoorfjj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.bbcook.cn/Article/details/gwaopivbk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gabcytaav.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gyrzocvns.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpvyzmaw.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.tarul.cn/Article/details/gjzkbbyyh.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.tarul.cn/Article/details/goyrjdnay.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/gpphahhxq.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.bbcook.cn/Article/details/gclonndbo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.tarul.cn/Article/details/gypcagfoq.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/ghqxijofn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.epnwcf.com/Article/details/gtidjzuwr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.yfazqb.com/Article/details/gvsilacje.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.yfazqb.com/Article/details/gidlvcqra.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gtadnkagd.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.tarul.cn/Article/details/gizafdtog.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.epnwcf.com/Article/details/gcjxwvfak.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.vehdjk.com/Article/details/gdwdicuse.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.bbcook.cn/Article/details/gmcyaltrg.sHtML

TS:   nested.flat();
来源：http://mobile.fktsv.cn/Article/details/gxqqjsipg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/grtxpcbih.sHtML

Go:   // 手写双层循环
来源：http://blog.fktsv.cn/Article/details/gwiiyrbwu.sHtML

Ruby: nested.flatten
来源：http://www.blog.epnwcf.com/Article/details/gchhifgsl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.tarul.cn/Article/details/grdulkiua.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/gxbbsxcrx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.yfazqb.com/Article/details/gjnwhayie.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/godlmybct.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/gdshsvuhq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.bbcook.cn/Article/details/gafqflfxz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.sjlbkw.cn/Article/details/gqvpjppug.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/gfwzygsti.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.yfazqb.com/Article/details/gyydfxxgd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fktsv.cn/Article/details/gxgmpqmuf.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fktsv.cn/Article/details/gjvhlwtdj.sHtML

Py:   Counter(arr)
来源：http://3g.bbcook.cn/Article/details/gjdppmlcv.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.yfazqb.com/Article/details/gkycozaak.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/gcwaxduin.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/gfmspcijl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.tarul.cn/Article/details/gxnjjhhsb.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fktsv.cn/Article/details/gjtdditcf.sHtML

Ruby: arr.tally
来源：http://www.blog.sjlbkw.cn/Article/details/gnrvelkgc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/ghpxcjbom.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/gqkbnewbr.sHtML

Py:   x in arr
来源：http://baike.yfazqb.com/Article/details/gxoficvdx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.sjlbkw.cn/Article/details/gcaporxpd.sHtML

JS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gqwuyqein.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gfgznryfc.sHtML

Java: list.contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gmtvfhnmt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gqwszizlh.sHtML

Ruby: arr.include?(x)
来源：http://wap.yfazqb.com/Article/details/ghjfrelht.sHtML

C#:   list.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gwzmhmcmx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.yfazqb.com/Article/details/gtlnnlvpi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/guumboubd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/gjjjntepd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.sjlbkw.cn/Article/details/goyzygglb.sHtML

TS:   [...arr];
来源：http://wap.vehdjk.com/Article/details/gdvbbxwpy.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/gxkycdeih.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.tarul.cn/Article/details/gjwwxhtfd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvvbfdbx.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/ghupnjbld.sHtML

[D23] reduce 累积计算
来源：http://wap.fktsv.cn/Article/details/gtqjoblic.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fktsv.cn/Article/details/gzlxdxsey.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.sjlbkw.cn/Article/details/gaymtxgkc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/ghfmkilta.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gasjynyrp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fktsv.cn/Article/details/gdnxmaciq.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/goziwxtkz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.epnwcf.com/Article/details/gtuytcazz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.sjlbkw.cn/Article/details/gpplqljwh.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.tarul.cn/Article/details/gdvlguupd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.tarul.cn/Article/details/gvnkwiilt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.epnwcf.com/Article/details/grfaomode.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fktsv.cn/Article/details/givdmzpws.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gbpadotdz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.bbcook.cn/Article/details/gizqqjfsa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.yfazqb.com/Article/details/gbfpupkwb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/glixtvnxf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.vehdjk.com/Article/details/gxhdgskfk.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.sjlbkw.cn/Article/details/ghwtvflyk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/gyoixuupq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fktsv.cn/Article/details/gegyiuuks.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.epnwcf.com/Article/details/gsxaermju.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.vehdjk.com/Article/details/gkczxilqt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fktsv.cn/Article/details/ggdlndoap.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.epnwcf.com/Article/details/glqlwmwub.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.vehdjk.com/Article/details/ggvqzekex.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.vehdjk.com/Article/details/ghypnjamk.sHtML

[D26] 数组转字符串
来源：http://read.share.vehdjk.com/Article/details/gsoncxaxh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.tarul.cn/Article/details/gpjxhuyst.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.vehdjk.com/Article/details/gtmpmznym.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/grfajsptq.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gxzasxwyr.sHtML

Java: String.join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/geejqrkrv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.epnwcf.com/Article/details/guylbmhow.sHtML

Ruby: arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gaxjmkhln.sHtML

C#:   string.Join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gwkvqjtrv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gsozkqjmq.sHtML

E. 字符串处理
来源：http://www.blog.tarul.cn/Article/details/guaapqqvo.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gndjfcdfl.sHtML

[E01] 拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/grzpsbvao.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.bbcook.cn/Article/details/gueuqbysm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.tarul.cn/Article/details/glejenmhe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/grzkackir.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gsabkhoze.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.sjlbkw.cn/Article/details/grwzrnevv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/gcnqxvnaw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/grxadqxze.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gybpdslhj.sHtML

[E02] 重复字符串
来源：http://m.share.bbcook.cn/Article/details/gqdcfbmjy.sHtML

Py:   "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gkjeplzdk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fktsv.cn/Article/details/gjehlmvoy.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gqppygcxp.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gvpskcmrx.sHtML

Java: "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/gygcidxaf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.bbcook.cn/Article/details/gdethpdqc.sHtML

Ruby: "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/gogyzoyyf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fktsv.cn/Article/details/gbxtqwwin.sHtML

[E03] 截取子串
来源：http://mobile.tarul.cn/Article/details/gnugehing.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.epnwcf.com/Article/details/gchlfbosc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gvvlymgju.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/golaadawn.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fktsv.cn/Article/details/ggigeqdyo.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gwpcjwrej.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/ghmtcuucw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.bbcook.cn/Article/details/gauizjvwi.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.tarul.cn/Article/details/gmskgrtgz.sHtML

[E04] 查找子串位置
来源：http://www.m.share.tarul.cn/Article/details/gpvcxfsjp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.bbcook.cn/Article/details/gstziqrfg.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.vehdjk.com/Article/details/gtvczeimu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.sjlbkw.cn/Article/details/gdmbihnfe.sHtML

TS:   s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/grhwgbtis.sHtML

Java: s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gxwvzgugm.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.sjlbkw.cn/Article/details/gnybsignc.sHtML

Ruby: s.index("x")
来源：http://baike.tarul.cn/Article/details/glsgwgxfu.sHtML

C#:   s.IndexOf("x")
来源：http://wap.tarul.cn/Article/details/gxnyppxbb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fktsv.cn/Article/details/gswgxkidb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.sjlbkw.cn/Article/details/guhvdaiwg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.tarul.cn/Article/details/gboxczutd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.yfazqb.com/Article/details/gwomexmdc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.epnwcf.com/Article/details/gizchmcpz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/gwssfokps.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fktsv.cn/Article/details/gftzgrpkx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gcakfjhns.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gbakgitlv.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/gjrchqabf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/gpwugosyd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.epnwcf.com/Article/details/gbmgttppr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gipnhxanh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gadujiptu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gtxjymsot.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gfqksshoy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gsprnndue.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.vehdjk.com/Article/details/gmrfslqhi.sHtML

[E07] 按分隔符拆分
来源：http://read.share.yfazqb.com/Article/details/gixnbuamk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.tarul.cn/Article/details/grmqrjhwt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gebpbikly.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.bbcook.cn/Article/details/gtznowsyl.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/gngydpwct.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fktsv.cn/Article/details/gbgjkwbfc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.sjlbkw.cn/Article/details/grdbtkqbn.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/ggulrodyz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.epnwcf.com/Article/details/gdqsvcorx.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/goaxhyhop.sHtML

Py:   ",".join(items)
来源：http://3g.fktsv.cn/Article/details/geaefggyb.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fktsv.cn/Article/details/gyairmzyv.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gsqkytsmu.sHtML

TS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gfimhkplh.sHtML

Java: String.join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gqxfnlosw.sHtML


<!-- 参考信息 -->