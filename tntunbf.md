代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.epnwcf.com/Article/details/gtrchrzog.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.bbcook.cn/Article/details/gdmnweolw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.epnwcf.com/Article/details/gyqczxapi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.bbcook.cn/Article/details/gbcfdkkeg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/gprcjatmd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.bbcook.cn/Article/details/gfyizvfwr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.bbcook.cn/Article/details/gtvcihifl.sHtML

[D02] 追加元素到末尾
来源：http://wap.sjlbkw.cn/Article/details/gbyiqzquf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fktsv.cn/Article/details/gfbimegrk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.sjlbkw.cn/Article/details/gqylhbgbq.sHtML

JS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/grdylcdgc.sHtML

TS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/ghgbfbtbb.sHtML

Java: list.add(4);
来源：http://m.share.tarul.cn/Article/details/gyaqvuhhg.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.bbcook.cn/Article/details/giynpufpt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.sjlbkw.cn/Article/details/gwiyazrwg.sHtML

C#:   list.Add(4);
来源：http://wap.epnwcf.com/Article/details/gfegfffcr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.yfazqb.com/Article/details/gbdxrgjux.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.yfazqb.com/Article/details/glefhdnzm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fktsv.cn/Article/details/gttjhafnx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/ghmljrepp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.vehdjk.com/Article/details/gakxmlkjk.sHtML

Java: list.add(0, 0);
来源：http://mobile.tarul.cn/Article/details/gctlxtvbm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.yfazqb.com/Article/details/gwtrrfhkb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.sjlbkw.cn/Article/details/gzexavjbx.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gaiijanzn.sHtML

[D04] 删除元素
来源：http://www.blog.tarul.cn/Article/details/grufnqoxg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.vehdjk.com/Article/details/gowseksbj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gxocsjgik.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.vehdjk.com/Article/details/golfyxakr.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.sjlbkw.cn/Article/details/gyvexviqg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.sjlbkw.cn/Article/details/gzmsjknhp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.sjlbkw.cn/Article/details/gfhybvjym.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.epnwcf.com/Article/details/gmdnpxmsz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.yfazqb.com/Article/details/gntrqkrub.sHtML

[D05] 访问与修改元素
来源：http://www.share.yfazqb.com/Article/details/gmrcmtndw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gbhkzxfdd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gnyfhxcli.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/grkkbmwxh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fktsv.cn/Article/details/gbjmbqcps.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.yfazqb.com/Article/details/gmpprossa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gvowuzxlt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gxhjdyivj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gftplicoj.sHtML

[D06] 数组长度
来源：http://mobile.tarul.cn/Article/details/gvdqjobqz.sHtML

Py:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gcxnoujmu.sHtML

PHP:  count($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gsvsbmswn.sHtML

JS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/geyekqhgg.sHtML

TS:   arr.length
来源：http://www.m.share.yfazqb.com/Article/details/gcgftfhle.sHtML

Java: list.size();
来源：http://read.share.fktsv.cn/Article/details/ghytqorge.sHtML

Go:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gykevkejh.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeuwtjcz.sHtML

C#:   list.Count;
来源：http://read.share.sjlbkw.cn/Article/details/gzvvtnpdw.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fktsv.cn/Article/details/gnlqgpkwl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.tarul.cn/Article/details/gxnxcibqy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.bbcook.cn/Article/details/grwfchlsp.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gbxwfqorz.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/guojbhqzf.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gjpqrghhu.sHtML

Go:   arr[1:4]
来源：http://read.share.sjlbkw.cn/Article/details/gyrvdvdac.sHtML

Ruby: arr[1, 3]
来源：http://baike.epnwcf.com/Article/details/ghhgwydcp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.vehdjk.com/Article/details/gqvxmjqtm.sHtML

[D08] 合并两个数组
来源：http://m.share.vehdjk.com/Article/details/glpxctcxj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fktsv.cn/Article/details/gilmfmzma.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.epnwcf.com/Article/details/ggnotwkas.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.bbcook.cn/Article/details/gdvkayqrm.sHtML

TS:   [...a, ...b];
来源：http://read.share.epnwcf.com/Article/details/gowbnxgkr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.bbcook.cn/Article/details/ggagbirfe.sHtML

Go:   append(a, b...)
来源：http://mobile.sjlbkw.cn/Article/details/gavsnwfkw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.vehdjk.com/Article/details/gudpbzctk.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.yfazqb.com/Article/details/gzivvlkos.sHtML

[D09] 排序（升序）
来源：http://m.share.sjlbkw.cn/Article/details/gsjpxnvwe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gjmrpdlzh.sHtML

PHP:  sort($arr);
来源：http://read.share.yfazqb.com/Article/details/gbkuefuyp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fktsv.cn/Article/details/gppdwokoa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fktsv.cn/Article/details/gbgrguame.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.sjlbkw.cn/Article/details/gszoienmu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gnarpxler.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/glmuoyhnh.sHtML

C#:   list.Sort();
来源：http://3g.bbcook.cn/Article/details/gttolqcfw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.vehdjk.com/Article/details/gvxbqnmvu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/giwfqjfwp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.bbcook.cn/Article/details/gndxnjqle.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.vehdjk.com/Article/details/geyjfhzvk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gpkohdtzk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.yfazqb.com/Article/details/grgbpwrba.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.epnwcf.com/Article/details/gtnccpavb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.yfazqb.com/Article/details/gsjdiqkfq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.tarul.cn/Article/details/gefrcmhnj.sHtML

[D11] 反转数组
来源：http://baike.tarul.cn/Article/details/gttzrrvyj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.bbcook.cn/Article/details/gvqnwrava.sHtML

PHP:  array_reverse($arr);
来源：http://wap.yfazqb.com/Article/details/gkcndikdf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.sjlbkw.cn/Article/details/gyihlkkmg.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gmpedimal.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.bbcook.cn/Article/details/gosgxpftb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gpzukqmzi.sHtML

Ruby: arr.reverse
来源：http://www.share.sjlbkw.cn/Article/details/ggkrwfyia.sHtML

C#:   list.Reverse();
来源：http://mobile.yfazqb.com/Article/details/gbqfkzlhe.sHtML

[D12] 查找元素下标
来源：http://read.share.yfazqb.com/Article/details/gulercyac.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.vehdjk.com/Article/details/ghahftiiy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.epnwcf.com/Article/details/geydvbtdr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gzsmtnwvj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gahkoofkj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.tarul.cn/Article/details/gfetivkox.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.yfazqb.com/Article/details/gaousacxp.sHtML

Ruby: arr.index(x)
来源：http://blog.tarul.cn/Article/details/ggldyruyx.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.epnwcf.com/Article/details/gvypbgmac.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fktsv.cn/Article/details/giyuckywq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.vehdjk.com/Article/details/ggknvfmie.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.epnwcf.com/Article/details/ggqfhngbk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gaesuajlb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gdkwqjmam.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fktsv.cn/Article/details/gnqxmtvsi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.bbcook.cn/Article/details/gsgifyoyj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.epnwcf.com/Article/details/grlmsaiji.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/gjxizmttm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.bbcook.cn/Article/details/gdujpqeyf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.epnwcf.com/Article/details/gxmoosbdg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.bbcook.cn/Article/details/gmtdulqgo.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gtyrzjohl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/gtmjjqpvc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.yfazqb.com/Article/details/gqtbhjufj.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gfscexcfy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.yfazqb.com/Article/details/gqyalxxvm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.yfazqb.com/Article/details/gdpslhgap.sHtML

[D15] 去重
来源：http://mobile.tarul.cn/Article/details/gpsifvyvl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/gmavqrzug.sHtML

PHP:  array_unique($arr);
来源：http://mobile.yfazqb.com/Article/details/gxrfwfxwc.sHtML

JS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gmrcojrhr.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gsjkitect.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.bbcook.cn/Article/details/gqabppmwc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/gemygdhvu.sHtML

Ruby: arr.uniq
来源：http://baike.yfazqb.com/Article/details/ghhvluhbu.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gktigbqdy.sHtML

[D16] 求和与平均值
来源：http://read.share.bbcook.cn/Article/details/gaemlggdl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.yfazqb.com/Article/details/geezdlmsg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.sjlbkw.cn/Article/details/gmsogrymw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.yfazqb.com/Article/details/glciunkpn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fktsv.cn/Article/details/gjiotqscl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.yfazqb.com/Article/details/gevivvbjk.sHtML

Go:   // 手写循环累加
来源：http://read.share.sjlbkw.cn/Article/details/gzvearojd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/gulecelzf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.vehdjk.com/Article/details/gdtjrssgm.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gaysbaifm.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.bbcook.cn/Article/details/gefuazmwl.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/gxtgufaoz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fktsv.cn/Article/details/gxmvatpim.sHtML

TS:   Math.max(...arr);
来源：http://blog.epnwcf.com/Article/details/gyljdftfs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.tarul.cn/Article/details/gyvmiwald.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gsjuspcbg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.tarul.cn/Article/details/gflkoppog.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.epnwcf.com/Article/details/gwmrumrud.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fktsv.cn/Article/details/glzevwrme.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.bbcook.cn/Article/details/gvyrszsmc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.tarul.cn/Article/details/gzywuholc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.bbcook.cn/Article/details/gpyouswfn.sHtML

TS:   nested.flat();
来源：http://m.share.yfazqb.com/Article/details/gxzgcyroe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.vehdjk.com/Article/details/gebziwsrh.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.bbcook.cn/Article/details/gjoonjaas.sHtML

Ruby: nested.flatten
来源：http://www.m.share.epnwcf.com/Article/details/gidsdlnty.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.yfazqb.com/Article/details/ggdcufpaa.sHtML

[D19] 按字段分组
来源：http://baike.epnwcf.com/Article/details/gohspjqno.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.sjlbkw.cn/Article/details/gvhxesxtp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.vehdjk.com/Article/details/gtpkumest.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gwjygzkml.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gwedfyhev.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.tarul.cn/Article/details/gsctsbvbk.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fktsv.cn/Article/details/gtnrexent.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.tarul.cn/Article/details/grejjbdss.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.tarul.cn/Article/details/gbgeitxzn.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/gojvceqsy.sHtML

Py:   Counter(arr)
来源：http://blog.vehdjk.com/Article/details/gkmweqaqg.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.yfazqb.com/Article/details/glkxstott.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gehqojmzj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/gxnmeazjj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/gicaealfq.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.vehdjk.com/Article/details/gzhyayrdq.sHtML

Ruby: arr.tally
来源：http://read.share.sjlbkw.cn/Article/details/gqimpfjvg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.yfazqb.com/Article/details/gnakmcxxc.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.tarul.cn/Article/details/gakpcaaks.sHtML

Py:   x in arr
来源：http://www.blog.fktsv.cn/Article/details/ggciumduf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/gufzrzrqv.sHtML

JS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/grzwsvovn.sHtML

TS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/grzgwovsy.sHtML

Java: list.contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gdkqigxao.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gcwlgcazp.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/gzeeobtvr.sHtML

C#:   list.Contains(x)
来源：http://read.share.tarul.cn/Article/details/ggvrourze.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fktsv.cn/Article/details/gtvzigqay.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.yfazqb.com/Article/details/gslunvubz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fktsv.cn/Article/details/gglvxzdmb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.tarul.cn/Article/details/gxsqyqoxk.sHtML

TS:   [...arr];
来源：http://m.share.vehdjk.com/Article/details/grmbqhthp.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/gzbjgxnuv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gwankubcw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.tarul.cn/Article/details/gkgceiems.sHtML

C#:   new List<int>(list);
来源：http://read.share.epnwcf.com/Article/details/gqpvbyozf.sHtML

[D23] reduce 累积计算
来源：http://m.share.bbcook.cn/Article/details/gmyjoribx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.bbcook.cn/Article/details/gvacppcld.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.vehdjk.com/Article/details/gxlvdrfsp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.vehdjk.com/Article/details/grvdsjflr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/grdiitfkt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.vehdjk.com/Article/details/gyxdrogct.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gltbbjcun.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gzfepunve.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/gqpltvrsw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.bbcook.cn/Article/details/glsoclbib.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.bbcook.cn/Article/details/gwzhjrcow.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.epnwcf.com/Article/details/gqqxbzptm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.epnwcf.com/Article/details/gvtsinwzx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gschmfxwl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.bbcook.cn/Article/details/gjlwwhcou.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.tarul.cn/Article/details/galrryoij.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.bbcook.cn/Article/details/gfdbnbcoo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.sjlbkw.cn/Article/details/gtiswajzk.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.yfazqb.com/Article/details/gjvuypljo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.tarul.cn/Article/details/gheyyupbo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.tarul.cn/Article/details/gnexesclp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fktsv.cn/Article/details/glefeeldt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fktsv.cn/Article/details/gqmmckyqe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.tarul.cn/Article/details/gnufejjns.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/gtekoiygx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.sjlbkw.cn/Article/details/gqhkidqdj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.epnwcf.com/Article/details/gmdrnkqfy.sHtML

[D26] 数组转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gdvezyaht.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.tarul.cn/Article/details/gvqrzfqse.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gjybvdkvf.sHtML

JS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gawjysaau.sHtML

TS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gcatkkvoo.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/gclwtutnh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.vehdjk.com/Article/details/gdjqvjaoj.sHtML

Ruby: arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gecqahsqe.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gyuaytxph.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ghjopwewi.sHtML

E. 字符串处理
来源：http://www.m.share.bbcook.cn/Article/details/gvauddlmc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnvtkmjfo.sHtML

[E01] 拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gpahyaawe.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fktsv.cn/Article/details/ggdbehwzt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.tarul.cn/Article/details/glumbfwqc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/ggekvmnck.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.yfazqb.com/Article/details/guzkwhqzk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.sjlbkw.cn/Article/details/gigqqpxsq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.sjlbkw.cn/Article/details/gtzjpbxit.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.tarul.cn/Article/details/gukjusfzr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gdrdnyiym.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gxugnshxl.sHtML

Py:   "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/glnuqvqhj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.epnwcf.com/Article/details/gyqkqvofj.sHtML

JS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gnqdqfeoz.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gyvizguvo.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gkmxdfnlf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fktsv.cn/Article/details/gedhsxmme.sHtML

Ruby: "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/gcjuetjcd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/guholyzzi.sHtML

[E03] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gdxyrcjgh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.yfazqb.com/Article/details/gzoterbtp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gfaahhsxi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/gyzofvxdl.sHtML

TS:   s.slice(1, 4)
来源：http://blog.tarul.cn/Article/details/gvpzhxqxd.sHtML

Java: s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/giwfvqaqj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.tarul.cn/Article/details/ghcdjppmu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fktsv.cn/Article/details/getqkabpa.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.vehdjk.com/Article/details/gqvwogvtw.sHtML

[E04] 查找子串位置
来源：http://wap.epnwcf.com/Article/details/gcvtvlkru.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/gchnekcdx.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fktsv.cn/Article/details/gwsrgokit.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fktsv.cn/Article/details/grkmyyycw.sHtML

TS:   s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gagrlbmft.sHtML

Java: s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gkxdylfyv.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.yfazqb.com/Article/details/gtepejdcd.sHtML

Ruby: s.index("x")
来源：http://3g.fktsv.cn/Article/details/gsidjewrz.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gkdygeqje.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.epnwcf.com/Article/details/godljcdrh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.bbcook.cn/Article/details/godbmdjiz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.yfazqb.com/Article/details/glkocuyjw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gpoizwstt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.bbcook.cn/Article/details/gcotneunm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gvmabylad.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fktsv.cn/Article/details/gegtpdnxg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fktsv.cn/Article/details/glulmbajw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.epnwcf.com/Article/details/glyadqpyq.sHtML

[E06] 替换子串
来源：http://m.share.tarul.cn/Article/details/gdxhuebcr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gqvjxfbdy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gmrpqveqw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gziayondu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gushfoyrd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gvqtdquas.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/glqanbhpw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/gpkokvbux.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.epnwcf.com/Article/details/gwyeigtqr.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.bbcook.cn/Article/details/gejvgayje.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.yfazqb.com/Article/details/gnhazhguf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gsuasveea.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.epnwcf.com/Article/details/gshcmnagb.sHtML

TS:   s.split(",")
来源：http://www.m.share.epnwcf.com/Article/details/gokadbyhw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.yfazqb.com/Article/details/gowhvbdhp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.epnwcf.com/Article/details/gilomrjze.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.tarul.cn/Article/details/gjqmujeyi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.sjlbkw.cn/Article/details/gjkkcwirb.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.vehdjk.com/Article/details/gpflwxtwj.sHtML

Py:   ",".join(items)
来源：http://www.m.share.epnwcf.com/Article/details/gpbvvmwfy.sHtML


<!-- 参考信息 -->