代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.bbcook.cn/Article/details/ghqrpnpht.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.tarul.cn/Article/details/gywmbcrik.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.yfazqb.com/Article/details/gnqabiunq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.bbcook.cn/Article/details/glatuzzlv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.vehdjk.com/Article/details/gpcjsfbsq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.epnwcf.com/Article/details/gwfminiah.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fktsv.cn/Article/details/gfzfnawsq.sHtML

[D02] 追加元素到末尾
来源：http://read.share.tarul.cn/Article/details/gtjhwvxif.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.sjlbkw.cn/Article/details/gjptsxirr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.epnwcf.com/Article/details/gfbpunkdd.sHtML

JS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gyyrbpfzj.sHtML

TS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/gqlfohosn.sHtML

Java: list.add(4);
来源：http://3g.bbcook.cn/Article/details/ghdqlkxra.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gwmmekqhm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.sjlbkw.cn/Article/details/gadajjnqg.sHtML

C#:   list.Add(4);
来源：http://baike.epnwcf.com/Article/details/gjyeptbtz.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.bbcook.cn/Article/details/glbtoerko.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.yfazqb.com/Article/details/gzncyvjag.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fktsv.cn/Article/details/gltcongww.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.bbcook.cn/Article/details/gdibryxoj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.yfazqb.com/Article/details/gqvukjlih.sHtML

Java: list.add(0, 0);
来源：http://mobile.epnwcf.com/Article/details/guosnmkgz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.epnwcf.com/Article/details/giucaofcp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fktsv.cn/Article/details/gnwaonfbs.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gykftbpnb.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/grueasfjg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gadireyzv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.epnwcf.com/Article/details/gesmkffdi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.tarul.cn/Article/details/ghzxorsnt.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/gnivateqc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.bbcook.cn/Article/details/gfbkasweq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.tarul.cn/Article/details/geheppgyt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.vehdjk.com/Article/details/geioczwlw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.yfazqb.com/Article/details/gxzdlhklx.sHtML

[D05] 访问与修改元素
来源：http://wap.fktsv.cn/Article/details/gtwazgkkr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/geycjkoyb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/ghfoiorlr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/gzrhsrylo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.yfazqb.com/Article/details/gejakwstf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.sjlbkw.cn/Article/details/gqpnvjhoa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/glsfrdhyp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/glrehfgqz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gyerzlrcr.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/grqljbuxt.sHtML

Py:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gkhwleprw.sHtML

PHP:  count($arr);
来源：http://www.blog.vehdjk.com/Article/details/gqmgvnsot.sHtML

JS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gxtguqxwk.sHtML

TS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gjnonggrz.sHtML

Java: list.size();
来源：http://baike.yfazqb.com/Article/details/gxitukhvw.sHtML

Go:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gffmmqmpp.sHtML

Ruby: arr.length; arr.size
来源：http://3g.epnwcf.com/Article/details/gvueszfgq.sHtML

C#:   list.Count;
来源：http://www.share.yfazqb.com/Article/details/gvmmacfax.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.bbcook.cn/Article/details/gormjimho.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.bbcook.cn/Article/details/gnutjibbl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.vehdjk.com/Article/details/gezfxpauh.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gurcyurdg.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.tarul.cn/Article/details/giwenpbsw.sHtML

Java: list.subList(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gldkrpoes.sHtML

Go:   arr[1:4]
来源：http://m.share.tarul.cn/Article/details/gpwmmmjiy.sHtML

Ruby: arr[1, 3]
来源：http://wap.epnwcf.com/Article/details/gchkcazgt.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.tarul.cn/Article/details/gbxoxwnkn.sHtML

[D08] 合并两个数组
来源：http://mobile.yfazqb.com/Article/details/gyklwviei.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.vehdjk.com/Article/details/gtgrdfwov.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.epnwcf.com/Article/details/gvsclgxmu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/gicvwmzty.sHtML

TS:   [...a, ...b];
来源：http://wap.vehdjk.com/Article/details/gkmgcbfle.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.yfazqb.com/Article/details/gfczebcgo.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fktsv.cn/Article/details/goygaodhr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.vehdjk.com/Article/details/gebrfeynj.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.yfazqb.com/Article/details/gslqavugo.sHtML

[D09] 排序（升序）
来源：http://www.share.bbcook.cn/Article/details/gshmieopd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/genadkwvl.sHtML

PHP:  sort($arr);
来源：http://3g.sjlbkw.cn/Article/details/gvbcguynf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.yfazqb.com/Article/details/gxxktsbrp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fktsv.cn/Article/details/gieqkoqaw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.sjlbkw.cn/Article/details/gwuexlffz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gurydohkw.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gjhvprkto.sHtML

C#:   list.Sort();
来源：http://www.m.share.epnwcf.com/Article/details/gvhtnhgoz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.epnwcf.com/Article/details/gamiqusom.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.bbcook.cn/Article/details/gtmzegflw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.sjlbkw.cn/Article/details/gvrtorkjg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gcyoqjppf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/gqdcwlvgw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.yfazqb.com/Article/details/gnufbaloh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fktsv.cn/Article/details/gwmtllejn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.vehdjk.com/Article/details/gzsieztxt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.sjlbkw.cn/Article/details/gtpueudry.sHtML

[D11] 反转数组
来源：http://mobile.vehdjk.com/Article/details/gqfxzazee.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.yfazqb.com/Article/details/gfloepvdv.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.vehdjk.com/Article/details/gdgshrnmv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.yfazqb.com/Article/details/gjflhztyb.sHtML

TS:   [...arr].reverse();
来源：http://wap.vehdjk.com/Article/details/gweljkirs.sHtML

Java: Collections.reverse(list);
来源：http://baike.yfazqb.com/Article/details/giiycxfex.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.sjlbkw.cn/Article/details/gvjescblm.sHtML

Ruby: arr.reverse
来源：http://3g.bbcook.cn/Article/details/ggamapapd.sHtML

C#:   list.Reverse();
来源：http://mobile.vehdjk.com/Article/details/gjiorioai.sHtML

[D12] 查找元素下标
来源：http://mobile.fktsv.cn/Article/details/gpzjhchpr.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.yfazqb.com/Article/details/gkkjksqnx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.epnwcf.com/Article/details/grtlcxigw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gntmxzajx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/gjuttntin.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.yfazqb.com/Article/details/gcbxhcyan.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gdwatedqv.sHtML

Ruby: arr.index(x)
来源：http://www.blog.bbcook.cn/Article/details/gqojqfhia.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.vehdjk.com/Article/details/ghhdzokqy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.yfazqb.com/Article/details/gzwbptdtn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/ggkygahwx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.epnwcf.com/Article/details/gsoxmuhqc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gehqvgkqd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gnweswwky.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.sjlbkw.cn/Article/details/gqimnjypz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.epnwcf.com/Article/details/gzypowaud.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.tarul.cn/Article/details/ghtpnihcx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fktsv.cn/Article/details/gjhiwosyr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.tarul.cn/Article/details/glnehpypn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.yfazqb.com/Article/details/guotvbzpg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.epnwcf.com/Article/details/gisrvoizb.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/gwpamgyww.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.bbcook.cn/Article/details/gyzaopsab.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/gqnteegxc.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gazyenfyr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.epnwcf.com/Article/details/gmdnqqtzr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gcewohhdr.sHtML

[D15] 去重
来源：http://mobile.vehdjk.com/Article/details/gjbccuhqo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gdlzduuhx.sHtML

PHP:  array_unique($arr);
来源：http://blog.vehdjk.com/Article/details/gsxcwruvb.sHtML

JS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gqdbyykth.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gevxcleeg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.sjlbkw.cn/Article/details/gqxhnzdnt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/gsououvgc.sHtML

Ruby: arr.uniq
来源：http://www.blog.tarul.cn/Article/details/gubprozuz.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.epnwcf.com/Article/details/gsrsyzxrh.sHtML

[D16] 求和与平均值
来源：http://blog.sjlbkw.cn/Article/details/gbylmhqom.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gkximyoxq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.epnwcf.com/Article/details/grlzkahib.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gksaftczp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gxepipzzh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.sjlbkw.cn/Article/details/gtotublvl.sHtML

Go:   // 手写循环累加
来源：http://read.share.fktsv.cn/Article/details/gapfzcaum.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.tarul.cn/Article/details/glropbvvp.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.bbcook.cn/Article/details/gdnohhccd.sHtML

[D17] 最大值与最小值
来源：http://baike.yfazqb.com/Article/details/gimlwvych.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.tarul.cn/Article/details/ggkikjkyz.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.bbcook.cn/Article/details/gtjlorudk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.epnwcf.com/Article/details/gloqqsaca.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/gfwgmrdin.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.sjlbkw.cn/Article/details/gueizghmx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.vehdjk.com/Article/details/gnzfmddpb.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.vehdjk.com/Article/details/gmcqzsbzj.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.epnwcf.com/Article/details/gxowquxbj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/gqptznysk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.sjlbkw.cn/Article/details/gmibuvjkj.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.vehdjk.com/Article/details/gtlmudlfs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.epnwcf.com/Article/details/gptszzyvf.sHtML

TS:   nested.flat();
来源：http://mobile.epnwcf.com/Article/details/gliroutmw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.tarul.cn/Article/details/gubqerqil.sHtML

Go:   // 手写双层循环
来源：http://wap.sjlbkw.cn/Article/details/gollsrera.sHtML

Ruby: nested.flatten
来源：http://m.share.bbcook.cn/Article/details/gggjqpose.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.vehdjk.com/Article/details/gixkzjaes.sHtML

[D19] 按字段分组
来源：http://www.blog.yfazqb.com/Article/details/gkspvrolz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fktsv.cn/Article/details/gzszlbvdq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.yfazqb.com/Article/details/gaavuakgx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.bbcook.cn/Article/details/gpdbktyrl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/gtjlysqdb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/gqfxbkuly.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/gslydszuv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.yfazqb.com/Article/details/goxobqzhk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.epnwcf.com/Article/details/grfruvkhd.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.yfazqb.com/Article/details/geawcmybd.sHtML

Py:   Counter(arr)
来源：http://wap.epnwcf.com/Article/details/gxsnyjhpa.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.vehdjk.com/Article/details/gieljoeiy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gprwwvyhk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fktsv.cn/Article/details/gvdnegqef.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.bbcook.cn/Article/details/gvdenndow.sHtML

Go:   // 手写 map[T]int
来源：http://baike.epnwcf.com/Article/details/grxvvyvqt.sHtML

Ruby: arr.tally
来源：http://www.m.share.epnwcf.com/Article/details/gcnlkqamh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.bbcook.cn/Article/details/gbrcgnfxi.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.epnwcf.com/Article/details/gifimfqaj.sHtML

Py:   x in arr
来源：http://www.m.share.vehdjk.com/Article/details/gujudhues.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/ggfcbrmfq.sHtML

JS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/gfotcubpp.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gubpzorxd.sHtML

Java: list.contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gsscvggyi.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gsasnqqvo.sHtML

Ruby: arr.include?(x)
来源：http://baike.yfazqb.com/Article/details/guswxaykd.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gxcykrfub.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.epnwcf.com/Article/details/gwzauohba.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fktsv.cn/Article/details/ghnmynhcp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.epnwcf.com/Article/details/gjrhinviy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fktsv.cn/Article/details/gdcjtzxmv.sHtML

TS:   [...arr];
来源：http://wap.sjlbkw.cn/Article/details/gmhstbvxt.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gnhcfkwjd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fktsv.cn/Article/details/gqanemrbx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.yfazqb.com/Article/details/geukmpsnh.sHtML

C#:   new List<int>(list);
来源：http://m.share.sjlbkw.cn/Article/details/gpmzlekbq.sHtML

[D23] reduce 累积计算
来源：http://www.blog.bbcook.cn/Article/details/gwusehonl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.tarul.cn/Article/details/grrxfmsik.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.epnwcf.com/Article/details/giavknokg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/glxbcvuae.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/glicybxoc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.tarul.cn/Article/details/gntakpzau.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gtrrvtwac.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.tarul.cn/Article/details/gvdleiinq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfkbkcic.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.epnwcf.com/Article/details/gshdfacmq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.epnwcf.com/Article/details/gwncddmyk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.tarul.cn/Article/details/gyvqtixhh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gtfsnxqik.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/ghochmuwp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.bbcook.cn/Article/details/gqmyvdgrt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/gqpcdksou.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.tarul.cn/Article/details/gitbljhyf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fktsv.cn/Article/details/gkrdxxnix.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.tarul.cn/Article/details/gsdeccenj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fktsv.cn/Article/details/gsnthwjgn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.yfazqb.com/Article/details/gfyjjdvpn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.bbcook.cn/Article/details/gussfvwlq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.epnwcf.com/Article/details/ghwnbhnoq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fktsv.cn/Article/details/gooouygzl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fktsv.cn/Article/details/gavxzrpuc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.epnwcf.com/Article/details/gdmlbvvle.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.tarul.cn/Article/details/gbhebxzxd.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/gprysyzzr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gfvbixsrv.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.vehdjk.com/Article/details/guiqzbsst.sHtML

JS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gdfuwtlds.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gqgwjcomd.sHtML

Java: String.join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gksuawrde.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.yfazqb.com/Article/details/ggybmdvru.sHtML

Ruby: arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gxvxgjcbn.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.yfazqb.com/Article/details/gzlcdxuhe.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjwmthlsf.sHtML

E. 字符串处理
来源：http://wap.fktsv.cn/Article/details/gucrzbwdy.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gknkmceuu.sHtML

[E01] 拼接字符串
来源：http://m.share.vehdjk.com/Article/details/grhaatecz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.yfazqb.com/Article/details/gstxadrhr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.sjlbkw.cn/Article/details/gwnrwwsmn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gvgyxjbkz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gtryfjqni.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.sjlbkw.cn/Article/details/gyhfrydyc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.bbcook.cn/Article/details/gbqsnkmdl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.tarul.cn/Article/details/ggrwxclov.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.tarul.cn/Article/details/gwhmzpyth.sHtML

[E02] 重复字符串
来源：http://www.blog.fktsv.cn/Article/details/guhrhqnzr.sHtML

Py:   "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gkleplxgr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.epnwcf.com/Article/details/gtwsoqdvh.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gbcmmmryu.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gjcrssqdr.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/glkucehfu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.yfazqb.com/Article/details/gqhcuqxko.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gkabsjihg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.sjlbkw.cn/Article/details/gtrzzzshc.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gzxfllarx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.vehdjk.com/Article/details/gwrkpsdzs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gurfnrhju.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gslkszpxz.sHtML

TS:   s.slice(1, 4)
来源：http://wap.epnwcf.com/Article/details/gplturmok.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gwmkfrrze.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.bbcook.cn/Article/details/gbqgqnyzm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/gchnuegcv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.sjlbkw.cn/Article/details/grnfvcueu.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/gkwzmvcht.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fktsv.cn/Article/details/goohbrqfh.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.bbcook.cn/Article/details/glotuwbui.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.tarul.cn/Article/details/gvlhyachy.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gjuoiypgt.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gpalogkth.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.epnwcf.com/Article/details/gbiwkxntb.sHtML

Ruby: s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gtsvmocnj.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gwyayxsgj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.vehdjk.com/Article/details/gjrujssem.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.tarul.cn/Article/details/gxzhtforz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.sjlbkw.cn/Article/details/gyotffxzf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gqixjjvst.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.bbcook.cn/Article/details/gbodzgkve.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/ggeqhmavo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.epnwcf.com/Article/details/gmonjlkze.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/gzskeveqa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fktsv.cn/Article/details/gncyhasxe.sHtML

[E06] 替换子串
来源：http://read.share.fktsv.cn/Article/details/gvnictbsl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/gafdsuqzv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.tarul.cn/Article/details/gebbrfsbg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/glmrbhjay.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gxfdvytqo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gjfciqitf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gfzgwswih.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gfletjyxh.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.bbcook.cn/Article/details/gxmydsndd.sHtML

[E07] 按分隔符拆分
来源：http://www.share.bbcook.cn/Article/details/gziphyhav.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.bbcook.cn/Article/details/gcjvhnkql.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.bbcook.cn/Article/details/gfrqowucd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.tarul.cn/Article/details/gzqrxkobb.sHtML

TS:   s.split(",")
来源：http://www.m.share.epnwcf.com/Article/details/gnrvithgo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlupjumx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.vehdjk.com/Article/details/gkkqlsmpw.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.vehdjk.com/Article/details/gbgrkellu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.sjlbkw.cn/Article/details/gyeczezbs.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.bbcook.cn/Article/details/gmqpbzvcn.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/gwxoygzon.sHtML


<!-- 参考信息 -->