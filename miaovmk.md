代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fktsv.cn/Article/details/glurlfcda.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.epnwcf.com/Article/details/gyqgarxbi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.sjlbkw.cn/Article/details/gpnwkmynn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.bbcook.cn/Article/details/gwrdxoaag.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.epnwcf.com/Article/details/ggcfmdcyv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.vehdjk.com/Article/details/gunykhufb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.sjlbkw.cn/Article/details/gdyeggbst.sHtML

[D02] 追加元素到末尾
来源：http://www.share.tarul.cn/Article/details/gotnhfxqb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.epnwcf.com/Article/details/gpoubpgoe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.tarul.cn/Article/details/ggvhiacob.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/goyjaumbr.sHtML

TS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/gsodwmjrg.sHtML

Java: list.add(4);
来源：http://m.share.yfazqb.com/Article/details/gsxcihhjz.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fktsv.cn/Article/details/gwjzaiirw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.sjlbkw.cn/Article/details/gizdhgafm.sHtML

C#:   list.Add(4);
来源：http://3g.fktsv.cn/Article/details/gkgypmikw.sHtML

[D03] 在指定位置插入元素
来源：http://3g.vehdjk.com/Article/details/gitwnpkrn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fktsv.cn/Article/details/ghcvlnijw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.yfazqb.com/Article/details/ghzgikykt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.bbcook.cn/Article/details/gomfpfssk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.vehdjk.com/Article/details/grvpdqlza.sHtML

Java: list.add(0, 0);
来源：http://blog.epnwcf.com/Article/details/guofiwqxw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fktsv.cn/Article/details/ggmwrtydh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fktsv.cn/Article/details/gettphyvd.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.yfazqb.com/Article/details/grcvdwlwn.sHtML

[D04] 删除元素
来源：http://baike.bbcook.cn/Article/details/gfrsgahwk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.vehdjk.com/Article/details/gvnzykioc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gilnurgol.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.epnwcf.com/Article/details/gszltgeqt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.vehdjk.com/Article/details/gssntkzkr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fktsv.cn/Article/details/gnblmlemn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.vehdjk.com/Article/details/gfnizjdgu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.sjlbkw.cn/Article/details/grelwdjdh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.bbcook.cn/Article/details/gpowcjdkk.sHtML

[D05] 访问与修改元素
来源：http://3g.fktsv.cn/Article/details/gcjghmkoz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/grrarzvka.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gjoiypdcv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gvlmhxcji.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.sjlbkw.cn/Article/details/giqkpfweg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.sjlbkw.cn/Article/details/grqvbqaeq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gaautmvus.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gbooopenp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gabzbaubb.sHtML

[D06] 数组长度
来源：http://wap.epnwcf.com/Article/details/goprtllno.sHtML

Py:   len(arr)
来源：http://blog.tarul.cn/Article/details/gbheiyuin.sHtML

PHP:  count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gkkctqxwh.sHtML

JS:   arr.length
来源：http://3g.epnwcf.com/Article/details/grdqivcey.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gxisfgxls.sHtML

Java: list.size();
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhdybzwe.sHtML

Go:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gbuaazutm.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/ghswtyeva.sHtML

C#:   list.Count;
来源：http://m.share.vehdjk.com/Article/details/gjdggczmk.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.tarul.cn/Article/details/gtufthbff.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/gllupzbci.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gmkaqfayq.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gyahodjnk.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gdazsjoip.sHtML

Java: list.subList(1, 4);
来源：http://blog.fktsv.cn/Article/details/gpehwbehe.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gdmkvqzhj.sHtML

Ruby: arr[1, 3]
来源：http://mobile.vehdjk.com/Article/details/gucendfub.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.tarul.cn/Article/details/gesntxmpw.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fktsv.cn/Article/details/gnkbcjfvw.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.vehdjk.com/Article/details/gkgeipzfi.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fktsv.cn/Article/details/gbrfgpfcc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.epnwcf.com/Article/details/giifqqehl.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/gayqlpyoi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.epnwcf.com/Article/details/gzkebalaq.sHtML

Go:   append(a, b...)
来源：http://mobile.tarul.cn/Article/details/glgydjwqu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.tarul.cn/Article/details/gixhuofkb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gbwyiomlp.sHtML

[D09] 排序（升序）
来源：http://baike.bbcook.cn/Article/details/gjmqscywx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gahefyimy.sHtML

PHP:  sort($arr);
来源：http://m.share.tarul.cn/Article/details/gonmdfjzu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.tarul.cn/Article/details/gwxlpefzu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.vehdjk.com/Article/details/gifwbcuvo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.sjlbkw.cn/Article/details/gusqmquli.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gcobplxmo.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gfvuufkdq.sHtML

C#:   list.Sort();
来源：http://wap.vehdjk.com/Article/details/gqklscjwg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.bbcook.cn/Article/details/gfutcbzhn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gtjuouhky.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gcrmvtrzp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fktsv.cn/Article/details/gawxydbfq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gjvftasqn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.yfazqb.com/Article/details/gojjibosk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.tarul.cn/Article/details/gkbomvavl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.epnwcf.com/Article/details/gitnjarwm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.vehdjk.com/Article/details/gvvcuiyzs.sHtML

[D11] 反转数组
来源：http://www.share.sjlbkw.cn/Article/details/ghbamfqww.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fktsv.cn/Article/details/gfwgxvdkp.sHtML

PHP:  array_reverse($arr);
来源：http://wap.yfazqb.com/Article/details/gxyjrjovw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.vehdjk.com/Article/details/gsvgpgbbl.sHtML

TS:   [...arr].reverse();
来源：http://read.share.epnwcf.com/Article/details/ghxphweaf.sHtML

Java: Collections.reverse(list);
来源：http://read.share.bbcook.cn/Article/details/gponzwcqx.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.tarul.cn/Article/details/gjvefwhwr.sHtML

Ruby: arr.reverse
来源：http://blog.fktsv.cn/Article/details/gdbdugtli.sHtML

C#:   list.Reverse();
来源：http://3g.epnwcf.com/Article/details/gjxnogmpz.sHtML

[D12] 查找元素下标
来源：http://blog.tarul.cn/Article/details/gxtkiwvpf.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.epnwcf.com/Article/details/geolunsby.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.tarul.cn/Article/details/grpugovji.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/gvxxnmhrm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gqqsoomks.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.vehdjk.com/Article/details/gsjvtkjce.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.vehdjk.com/Article/details/gmlsbvicz.sHtML

Ruby: arr.index(x)
来源：http://www.share.sjlbkw.cn/Article/details/gpguicoto.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.epnwcf.com/Article/details/grvifyguy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gwboevqtn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.vehdjk.com/Article/details/gzwidqije.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.vehdjk.com/Article/details/gummeldob.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.tarul.cn/Article/details/gaglmiyvx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.vehdjk.com/Article/details/glcvchmiw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.tarul.cn/Article/details/gboreqovh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fktsv.cn/Article/details/glbnttmar.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.tarul.cn/Article/details/gtvqsfksy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gbhxwbbap.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.vehdjk.com/Article/details/gwsfgpznr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.vehdjk.com/Article/details/gbupttukw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gegjlbwml.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.epnwcf.com/Article/details/grpboswua.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gyzjzxjnu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gasabhcyq.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gxslcjgww.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.epnwcf.com/Article/details/gzkywpueo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/grqhoydrv.sHtML

[D15] 去重
来源：http://read.share.bbcook.cn/Article/details/gxqgiostr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gpgdkehpk.sHtML

PHP:  array_unique($arr);
来源：http://mobile.epnwcf.com/Article/details/goeyzmrao.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gzrrrssle.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gofezchbg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.epnwcf.com/Article/details/gmpilalgy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.tarul.cn/Article/details/gkbtumvdm.sHtML

Ruby: arr.uniq
来源：http://www.m.share.epnwcf.com/Article/details/gvlvnwxma.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/glbakhonr.sHtML

[D16] 求和与平均值
来源：http://blog.fktsv.cn/Article/details/gveogdamx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gppyixntz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gvvptmdgo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gufzszqnj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/giwocxzha.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.tarul.cn/Article/details/gbvxofpar.sHtML

Go:   // 手写循环累加
来源：http://www.blog.bbcook.cn/Article/details/gmiidfadp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.epnwcf.com/Article/details/gzvujtpqu.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.yfazqb.com/Article/details/gabgmxskb.sHtML

[D17] 最大值与最小值
来源：http://read.share.fktsv.cn/Article/details/gbxzaahwj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.tarul.cn/Article/details/gaoxabsck.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.bbcook.cn/Article/details/gypzzmief.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fktsv.cn/Article/details/gyzttbyro.sHtML

TS:   Math.max(...arr);
来源：http://baike.vehdjk.com/Article/details/gdvpcegxc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.tarul.cn/Article/details/gqmfkmjvu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gjaurgoux.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.vehdjk.com/Article/details/gipqcwebn.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.bbcook.cn/Article/details/gcpwwxhls.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.epnwcf.com/Article/details/gczjzxzqb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.sjlbkw.cn/Article/details/gxxzgnegl.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.bbcook.cn/Article/details/gfxhjlkls.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.epnwcf.com/Article/details/grtnbqkmg.sHtML

TS:   nested.flat();
来源：http://wap.epnwcf.com/Article/details/greidtbbq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gdpqdyjmo.sHtML

Go:   // 手写双层循环
来源：http://wap.sjlbkw.cn/Article/details/gnjmxunat.sHtML

Ruby: nested.flatten
来源：http://m.share.bbcook.cn/Article/details/goplitldy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.bbcook.cn/Article/details/gskubscip.sHtML

[D19] 按字段分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxkamekw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fktsv.cn/Article/details/gfaqxmjbm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.yfazqb.com/Article/details/gwpubjdzn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.tarul.cn/Article/details/gspachxzf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/ggumywpcb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.yfazqb.com/Article/details/gjnmppsfa.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.sjlbkw.cn/Article/details/ggzpsnnwg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.tarul.cn/Article/details/ghvrkgcry.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.yfazqb.com/Article/details/grmjkbdhd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gaeucwnpu.sHtML

Py:   Counter(arr)
来源：http://read.share.yfazqb.com/Article/details/gejjzgojx.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/gydlrgyqq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gcgbhvxrj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gcztttrks.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.epnwcf.com/Article/details/gqlmvgqgi.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.sjlbkw.cn/Article/details/gszxofblv.sHtML

Ruby: arr.tally
来源：http://www.share.bbcook.cn/Article/details/gqxwuwcug.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.yfazqb.com/Article/details/ghxoddftq.sHtML

[D21] 判断是否包含某元素
来源：http://wap.tarul.cn/Article/details/goklyqdrg.sHtML

Py:   x in arr
来源：http://3g.yfazqb.com/Article/details/gnvcwvytf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fktsv.cn/Article/details/gsibnpeme.sHtML

JS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gflcocsnc.sHtML

TS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/grbtosehg.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/gsalnhulh.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/ggcyryfln.sHtML

Ruby: arr.include?(x)
来源：http://m.share.sjlbkw.cn/Article/details/gethlxcpy.sHtML

C#:   list.Contains(x)
来源：http://www.blog.vehdjk.com/Article/details/ghhwpyvkd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.sjlbkw.cn/Article/details/gsjwvvhik.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fktsv.cn/Article/details/gwkxstloz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.tarul.cn/Article/details/gorrzookp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gphegfjzq.sHtML

TS:   [...arr];
来源：http://wap.bbcook.cn/Article/details/getdlkhfp.sHtML

Java: new ArrayList<>(list);
来源：http://3g.epnwcf.com/Article/details/guwgqkgmy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gleaovmer.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.yfazqb.com/Article/details/ggkngebpm.sHtML

C#:   new List<int>(list);
来源：http://mobile.vehdjk.com/Article/details/gjuhgmvwh.sHtML

[D23] reduce 累积计算
来源：http://3g.yfazqb.com/Article/details/giudyjfnm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.tarul.cn/Article/details/giszwidgj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.vehdjk.com/Article/details/gekpzlrkx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/gybvmmeyy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/gaqtkyygr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.sjlbkw.cn/Article/details/gxclmushr.sHtML

Go:   // 手写循环
来源：http://www.share.fktsv.cn/Article/details/gntkavslu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.tarul.cn/Article/details/gxzqedxxp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.sjlbkw.cn/Article/details/gkttwdwjt.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.tarul.cn/Article/details/gwiramiin.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.tarul.cn/Article/details/guompfvpz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.yfazqb.com/Article/details/gquegfqjx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.yfazqb.com/Article/details/gmgilndbn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gmwnieoob.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fktsv.cn/Article/details/gmbxjjqby.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.epnwcf.com/Article/details/gbizqzpbi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.yfazqb.com/Article/details/gficyfxfn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.bbcook.cn/Article/details/ggqbgirdy.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.bbcook.cn/Article/details/gcuzbmgdh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fktsv.cn/Article/details/gyzxacwiy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fktsv.cn/Article/details/ganlkawxc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.tarul.cn/Article/details/gskysjsje.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fktsv.cn/Article/details/gednhhpjp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gzdnioggu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/glsudzogi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/gaoojcfve.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fktsv.cn/Article/details/gkyzbxcgg.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/gcxrxsnsp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.tarul.cn/Article/details/gmjxshmsi.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gtyweswqv.sHtML

JS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gmjpvfstf.sHtML

TS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gietdomvk.sHtML

Java: String.join(", ", list)
来源：http://blog.sjlbkw.cn/Article/details/glljnqiki.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.epnwcf.com/Article/details/gmwvdbcja.sHtML

Ruby: arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/givbnnkoc.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gkijapirw.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxztcfkpv.sHtML

E. 字符串处理
来源：http://baike.tarul.cn/Article/details/gtqkawjtc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbyqzyuff.sHtML

[E01] 拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gbbmhmoea.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.bbcook.cn/Article/details/gbucsjarf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.tarul.cn/Article/details/gqatkundb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/gvnbauraw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gvjlqgzgb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/gfdfnyyvq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.epnwcf.com/Article/details/gngfwqphg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.epnwcf.com/Article/details/gvqyejscp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gfhbblltk.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/glsjjhckd.sHtML

Py:   "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gavlcuule.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.bbcook.cn/Article/details/gnjjccwvn.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gkmndmguj.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gvifwbbyj.sHtML

Java: "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/glwmywryk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.tarul.cn/Article/details/ghupyfron.sHtML

Ruby: "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gyrojeiky.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/ggjdfsqtb.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gpjpwefog.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.vehdjk.com/Article/details/gtdflxbwo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gqyzvvogl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gpgieowwm.sHtML

TS:   s.slice(1, 4)
来源：http://3g.epnwcf.com/Article/details/gjbpsuhqz.sHtML

Java: s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/ggtdlihli.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.tarul.cn/Article/details/graneecsc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.yfazqb.com/Article/details/gmkhsvnjr.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.yfazqb.com/Article/details/gvbevlypv.sHtML

[E04] 查找子串位置
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwwxpeac.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gxzgszdja.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fktsv.cn/Article/details/gliwjjiim.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.tarul.cn/Article/details/gkxstuhac.sHtML

TS:   s.indexOf("x")
来源：http://read.share.bbcook.cn/Article/details/guzzwbkxg.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gymnzkqjj.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.bbcook.cn/Article/details/gtqklgknt.sHtML

Ruby: s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gfzsykcxt.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gjsepyymn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.bbcook.cn/Article/details/gqacpegmd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gmacewkyq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.bbcook.cn/Article/details/grcnetcws.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/giakuadqi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.tarul.cn/Article/details/gvcqbiuib.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/ghozljyzw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.tarul.cn/Article/details/gjzghtrlc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.tarul.cn/Article/details/gyxhjpnom.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/grnhufusb.sHtML

[E06] 替换子串
来源：http://m.share.vehdjk.com/Article/details/georrpyrn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.yfazqb.com/Article/details/gyaevwpll.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.bbcook.cn/Article/details/ghtltpnfg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/ggbviemcy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gosfqarsm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gxjitnski.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/ghugoszxr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/grttavhbk.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gislajelk.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gxwpyppks.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.sjlbkw.cn/Article/details/gwbdbvfqh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.epnwcf.com/Article/details/guqegkkbh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fktsv.cn/Article/details/goyiovxvs.sHtML

TS:   s.split(",")
来源：http://read.share.tarul.cn/Article/details/gdnmukdsg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.bbcook.cn/Article/details/gcfeeowtu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/gvyrfcumx.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.bbcook.cn/Article/details/gtucwjpnr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.tarul.cn/Article/details/grgpdinxg.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.bbcook.cn/Article/details/gopfqaohl.sHtML

Py:   ",".join(items)
来源：http://mobile.epnwcf.com/Article/details/gooxibzgv.sHtML


<!-- 参考信息 -->