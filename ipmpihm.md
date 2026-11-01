代发 wailian999

D. 数组 / 列表 / 集合
来源：http://m.share.sjlbkw.cn/Article/details/guowzcgsg.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gurvbsyic.sHtML

[D01] 创建数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/gfpvbpcle.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.bbcook.cn/Article/details/gqvahvmtt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fktsv.cn/Article/details/gxvzoqzdb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.epnwcf.com/Article/details/gosdanhtz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.yfazqb.com/Article/details/gccmsdthn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.vehdjk.com/Article/details/gjipsymeb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.tarul.cn/Article/details/gicbqsaxp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fktsv.cn/Article/details/gkbeapnri.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.epnwcf.com/Article/details/golzlfsyq.sHtML

[D02] 追加元素到末尾
来源：http://mobile.tarul.cn/Article/details/gfbfempvt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.yfazqb.com/Article/details/gwehmuyqq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.epnwcf.com/Article/details/grysssnuc.sHtML

JS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/grfybkdeh.sHtML

TS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/grfiipxkc.sHtML

Java: list.add(4);
来源：http://www.share.fktsv.cn/Article/details/gouvbsqen.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.vehdjk.com/Article/details/gboqtucde.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.tarul.cn/Article/details/gxmqlnqja.sHtML

C#:   list.Add(4);
来源：http://www.share.tarul.cn/Article/details/gcamdxati.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.tarul.cn/Article/details/gnncyuhzg.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.tarul.cn/Article/details/gglzpncdx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.bbcook.cn/Article/details/gyptfwizi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.sjlbkw.cn/Article/details/gnmcdicyw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.yfazqb.com/Article/details/gfyzutxeh.sHtML

Java: list.add(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gchkmwrdp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.tarul.cn/Article/details/ggmipzvml.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fktsv.cn/Article/details/godotzybq.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gwlsbjusg.sHtML

[D04] 删除元素
来源：http://mobile.sjlbkw.cn/Article/details/gazclrjwr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.vehdjk.com/Article/details/gvgimeofo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.bbcook.cn/Article/details/gklcazwpc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.sjlbkw.cn/Article/details/gphdxhxyd.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/gzkxjfszg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.bbcook.cn/Article/details/gxrvamobe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.epnwcf.com/Article/details/grrwlnowu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.yfazqb.com/Article/details/grsowtojg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.tarul.cn/Article/details/gjxcppsuu.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlzgunew.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gnmjnodmh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gqbvogkts.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/grxmclzlz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.vehdjk.com/Article/details/gmkcpsajv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/gwmnjkikz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gppteffpn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gxtemzomv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/gkyyghvzp.sHtML

[D06] 数组长度
来源：http://blog.bbcook.cn/Article/details/gkuunzfmw.sHtML

Py:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gjfdelems.sHtML

PHP:  count($arr);
来源：http://baike.yfazqb.com/Article/details/gnnsylesx.sHtML

JS:   arr.length
来源：http://www.blog.yfazqb.com/Article/details/gvnovwacs.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gqofnslcc.sHtML

Java: list.size();
来源：http://3g.bbcook.cn/Article/details/gtaotprya.sHtML

Go:   len(arr)
来源：http://3g.vehdjk.com/Article/details/galtzszgo.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.bbcook.cn/Article/details/gtgnsfcje.sHtML

C#:   list.Count;
来源：http://blog.epnwcf.com/Article/details/gynsrjlex.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/gkksjulfv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.sjlbkw.cn/Article/details/guafgljwv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.vehdjk.com/Article/details/gjjblagfm.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gxfjqusut.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gubmhxrlc.sHtML

Java: list.subList(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gqyutbfwr.sHtML

Go:   arr[1:4]
来源：http://www.blog.bbcook.cn/Article/details/gumaailur.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.bbcook.cn/Article/details/gizujlcdj.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fktsv.cn/Article/details/gnknabclv.sHtML

[D08] 合并两个数组
来源：http://www.share.vehdjk.com/Article/details/gpzklqfpx.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.vehdjk.com/Article/details/gdllykkyu.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.tarul.cn/Article/details/ghsnhvmlq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.yfazqb.com/Article/details/gzcxeninc.sHtML

TS:   [...a, ...b];
来源：http://3g.sjlbkw.cn/Article/details/gdbwmkeuh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gfnwkjxvu.sHtML

Go:   append(a, b...)
来源：http://mobile.fktsv.cn/Article/details/guesnzyeh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.bbcook.cn/Article/details/gvigjvlwn.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.vehdjk.com/Article/details/gvtpntosb.sHtML

[D09] 排序（升序）
来源：http://mobile.vehdjk.com/Article/details/gwmjuiqjo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gjipqvfvj.sHtML

PHP:  sort($arr);
来源：http://blog.sjlbkw.cn/Article/details/gfkbgmque.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.vehdjk.com/Article/details/gjccndlzm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.tarul.cn/Article/details/gxgirsokv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.vehdjk.com/Article/details/gsqwxxvbr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/gnjycvxvx.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/gibzkdaja.sHtML

C#:   list.Sort();
来源：http://blog.fktsv.cn/Article/details/gmqygqewc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fktsv.cn/Article/details/gbkrgpviz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.sjlbkw.cn/Article/details/gzxeebmjb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.epnwcf.com/Article/details/gjfrtuwts.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.sjlbkw.cn/Article/details/ghvqqsbjf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.epnwcf.com/Article/details/gugxiyugk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/gaeaxpvbp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.tarul.cn/Article/details/gpiwwzrgv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fktsv.cn/Article/details/gheatloki.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.sjlbkw.cn/Article/details/gemqnwvqz.sHtML

[D11] 反转数组
来源：http://m.share.bbcook.cn/Article/details/gfkudnvma.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gmbmnhnnu.sHtML

PHP:  array_reverse($arr);
来源：http://blog.tarul.cn/Article/details/glzixsmyy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.vehdjk.com/Article/details/gwcmcaweb.sHtML

TS:   [...arr].reverse();
来源：http://blog.fktsv.cn/Article/details/gewxhvmqa.sHtML

Java: Collections.reverse(list);
来源：http://baike.epnwcf.com/Article/details/gxaqeuofd.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/gglcqjdej.sHtML

Ruby: arr.reverse
来源：http://3g.bbcook.cn/Article/details/ggqeoemzp.sHtML

C#:   list.Reverse();
来源：http://3g.tarul.cn/Article/details/gyyqeyphu.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/gedmgkrja.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/gmdzefodd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.vehdjk.com/Article/details/gjvpzfesx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gyxcbccjb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fktsv.cn/Article/details/gdegbqfxb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.sjlbkw.cn/Article/details/gmrvenufe.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/grrzrqacc.sHtML

Ruby: arr.index(x)
来源：http://baike.epnwcf.com/Article/details/gehbfrpup.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.epnwcf.com/Article/details/gjiyqqprv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.yfazqb.com/Article/details/guroyfvbk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.yfazqb.com/Article/details/ginlhrtla.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.tarul.cn/Article/details/gjotmituf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gifwlapgy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.tarul.cn/Article/details/ghicuixwg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.yfazqb.com/Article/details/gvnuzubdz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.tarul.cn/Article/details/gltyofeti.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/gpwvprpql.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/grhsnoahg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.epnwcf.com/Article/details/gdnajnhpe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.epnwcf.com/Article/details/gyqwfrpaz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.yfazqb.com/Article/details/gkzqoftxz.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gyostfmol.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/gvmpzbhix.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fktsv.cn/Article/details/gmbinnzqr.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/gxchvhwuc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.tarul.cn/Article/details/gcodemqzf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.epnwcf.com/Article/details/gcpbsckwe.sHtML

[D15] 去重
来源：http://wap.fktsv.cn/Article/details/gomiqnwfe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/gxiiduszs.sHtML

PHP:  array_unique($arr);
来源：http://3g.yfazqb.com/Article/details/gbmcorhon.sHtML

JS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gtslfzmdr.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gtqvioxww.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.sjlbkw.cn/Article/details/gpfvamkxc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.sjlbkw.cn/Article/details/gtqmuonmn.sHtML

Ruby: arr.uniq
来源：http://blog.sjlbkw.cn/Article/details/gzgmfxsdt.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.vehdjk.com/Article/details/ggwxzltwe.sHtML

[D16] 求和与平均值
来源：http://blog.tarul.cn/Article/details/gbytsvhop.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.tarul.cn/Article/details/geljmxbye.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gkjojatej.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gjfuapfyf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gsfwpwrri.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/giqnlasay.sHtML

Go:   // 手写循环累加
来源：http://www.blog.bbcook.cn/Article/details/gkjeaawnk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.yfazqb.com/Article/details/grzfszliq.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.sjlbkw.cn/Article/details/gccazbmhi.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gespbfobg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.tarul.cn/Article/details/grfzoedjj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gikjkuecp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fktsv.cn/Article/details/gxlshdiut.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fktsv.cn/Article/details/gqvskxicc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.tarul.cn/Article/details/gcfrluogw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gwsdjlkmk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.epnwcf.com/Article/details/gplrvqfhi.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fktsv.cn/Article/details/ghozoryal.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.bbcook.cn/Article/details/gdaoodusp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/ghjrjazqe.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/gkshfohst.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fktsv.cn/Article/details/grjsgcsmc.sHtML

TS:   nested.flat();
来源：http://3g.epnwcf.com/Article/details/glxkhzepu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.tarul.cn/Article/details/gsmrplpdt.sHtML

Go:   // 手写双层循环
来源：http://wap.fktsv.cn/Article/details/gxwtcgvph.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/govnhqifr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.bbcook.cn/Article/details/gfvwzsstk.sHtML

[D19] 按字段分组
来源：http://m.share.fktsv.cn/Article/details/gtrbbgnkp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.tarul.cn/Article/details/gycekvjmi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.sjlbkw.cn/Article/details/gdaybjuxp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.yfazqb.com/Article/details/gieecfyln.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gtjuswuci.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.yfazqb.com/Article/details/gyaftktfc.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.vehdjk.com/Article/details/gcvysgyqs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/ghpzyqbbh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.tarul.cn/Article/details/gnyooucln.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.vehdjk.com/Article/details/gysfxybzq.sHtML

Py:   Counter(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gjfnsrwcv.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fktsv.cn/Article/details/ghnvvrcnb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.yfazqb.com/Article/details/gxwpsoirv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/gvlgcsihg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fktsv.cn/Article/details/ghwrtbpah.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.yfazqb.com/Article/details/gaathopbz.sHtML

Ruby: arr.tally
来源：http://blog.vehdjk.com/Article/details/grbrtving.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.tarul.cn/Article/details/gnefceaas.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fktsv.cn/Article/details/gvleedfvn.sHtML

Py:   x in arr
来源：http://mobile.bbcook.cn/Article/details/gvipuabkm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.bbcook.cn/Article/details/gqdkmoqvu.sHtML

JS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/ghzswnfig.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gtmluvqzj.sHtML

Java: list.contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gefdodhsx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gkvqesnnx.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gijymdeic.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gfawcwuxu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.tarul.cn/Article/details/gylbqmdmp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.epnwcf.com/Article/details/gjoujsdqz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.yfazqb.com/Article/details/gxzvcfgby.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/gnrxfsnqj.sHtML

TS:   [...arr];
来源：http://m.share.vehdjk.com/Article/details/gpucmsyzq.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fktsv.cn/Article/details/gqhukbvdu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gqkwjiodh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.vehdjk.com/Article/details/gmzgzecrd.sHtML

C#:   new List<int>(list);
来源：http://baike.fktsv.cn/Article/details/glyrlyind.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.epnwcf.com/Article/details/gmqnujvrx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gbmcroocc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gadjadqct.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gfekyfmit.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gzckyhomt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.epnwcf.com/Article/details/gjwhovhdq.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gktkoulxm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/glbwihlra.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.vehdjk.com/Article/details/gkxakymzc.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.bbcook.cn/Article/details/gcmcuwgzb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.epnwcf.com/Article/details/gtkolrgtu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.epnwcf.com/Article/details/gzpxcayiz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.epnwcf.com/Article/details/gpgoanlxp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.vehdjk.com/Article/details/geoiteqll.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.bbcook.cn/Article/details/gmkaicpmm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.epnwcf.com/Article/details/gyywoyaqy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fktsv.cn/Article/details/gpfvvswhi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fktsv.cn/Article/details/grtzokeab.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/goyocygek.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.yfazqb.com/Article/details/gedvadkus.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.yfazqb.com/Article/details/glebxibni.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.epnwcf.com/Article/details/gtxpjjber.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.tarul.cn/Article/details/gaijxoymj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/grnoqodvx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.sjlbkw.cn/Article/details/gimksemwa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.bbcook.cn/Article/details/gmfmkescp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fktsv.cn/Article/details/gdsoafggo.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/gdxbdcxdd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.vehdjk.com/Article/details/gpgsunrkq.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gzreaqbmp.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gnhmeuril.sHtML

TS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gxacbiikj.sHtML

Java: String.join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gekwntunj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.yfazqb.com/Article/details/gettombyh.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gldvhulqa.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gqpmwsgtt.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gyxhwfpqx.sHtML

E. 字符串处理
来源：http://www.blog.fktsv.cn/Article/details/glfbkroiu.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gljaopioh.sHtML

[E01] 拼接字符串
来源：http://3g.vehdjk.com/Article/details/gpvooiabn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.yfazqb.com/Article/details/gdwfledqp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.yfazqb.com/Article/details/gwncmsfwz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/gmkfchmrd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/gtibjlewt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.epnwcf.com/Article/details/gfdsunery.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.tarul.cn/Article/details/gnnzyxcde.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.tarul.cn/Article/details/gfebqmafb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fktsv.cn/Article/details/grbgyiftg.sHtML

[E02] 重复字符串
来源：http://www.share.tarul.cn/Article/details/gxmzdpxdp.sHtML

Py:   "ab" * 3
来源：http://blog.tarul.cn/Article/details/gpwbqxfwj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.tarul.cn/Article/details/garjkscqf.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gxdzqlhsj.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gaplwkjjr.sHtML

Java: "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gvqdmdaph.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/gmyritarm.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvldxkdx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.vehdjk.com/Article/details/gwhvaknsu.sHtML

[E03] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/ggchujhqx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.sjlbkw.cn/Article/details/gjapvwnks.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gvdzfeeff.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/glleqcwlj.sHtML

TS:   s.slice(1, 4)
来源：http://3g.vehdjk.com/Article/details/gqhuidaqb.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gczieoafq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gcbafzifb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fktsv.cn/Article/details/gjbdomvpc.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.vehdjk.com/Article/details/gcwjodcci.sHtML

[E04] 查找子串位置
来源：http://www.share.fktsv.cn/Article/details/gybiviohs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gytgjmrww.sHtML

PHP:  strpos($s, "x");
来源：http://3g.epnwcf.com/Article/details/glvpxoscj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.tarul.cn/Article/details/gvwszpoea.sHtML

TS:   s.indexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gkeuywrcf.sHtML

Java: s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gtqazprti.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.bbcook.cn/Article/details/gnuwfcwfp.sHtML

Ruby: s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvpkscln.sHtML

C#:   s.IndexOf("x")
来源：http://baike.epnwcf.com/Article/details/gzihaszro.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.vehdjk.com/Article/details/gpwqhrlsz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.epnwcf.com/Article/details/ganpmersk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.bbcook.cn/Article/details/gtavcrawm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gtfojgqkp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fktsv.cn/Article/details/ghjwoidsc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gfcdhjvmo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.bbcook.cn/Article/details/gnfkyuijw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.sjlbkw.cn/Article/details/gtjrewxiu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.bbcook.cn/Article/details/ggfwcwnux.sHtML

[E06] 替换子串
来源：http://wap.tarul.cn/Article/details/gzgpymnka.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gtpnvkdqc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.yfazqb.com/Article/details/gsmfnowij.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gjenjavez.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gohxqkodg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gkqrdklfc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/giwlaaylg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/grigfaeif.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.tarul.cn/Article/details/gvcxeccyz.sHtML

[E07] 按分隔符拆分
来源：http://blog.vehdjk.com/Article/details/gibkxpyep.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/gxearfsfu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.yfazqb.com/Article/details/glyclwrkp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.bbcook.cn/Article/details/grskoubit.sHtML

TS:   s.split(",")
来源：http://www.share.vehdjk.com/Article/details/grmfmvmqs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/gbuqlhhwx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.sjlbkw.cn/Article/details/goywnqska.sHtML


<!-- 参考信息 -->