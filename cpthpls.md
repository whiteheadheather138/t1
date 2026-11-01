代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gvduygrvw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.yfazqb.com/Article/details/geymsiktk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.epnwcf.com/Article/details/guzjrtuqr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.tarul.cn/Article/details/grqmmmecc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.sjlbkw.cn/Article/details/gddfgjbzp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.sjlbkw.cn/Article/details/gfqjhozac.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.sjlbkw.cn/Article/details/gmfaytvpj.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.bbcook.cn/Article/details/glqaxkmag.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.bbcook.cn/Article/details/gfohrrcez.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.vehdjk.com/Article/details/guxzzwxfp.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/grvhbzzbi.sHtML

TS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/gtyikqlss.sHtML

Java: list.add(4);
来源：http://wap.yfazqb.com/Article/details/gyogpqqhx.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fktsv.cn/Article/details/gjofuagcd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.vehdjk.com/Article/details/gkctollot.sHtML

C#:   list.Add(4);
来源：http://mobile.bbcook.cn/Article/details/gbjepfwyx.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.tarul.cn/Article/details/gcicbiihc.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.vehdjk.com/Article/details/gvjpxxvtd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fktsv.cn/Article/details/gmibjamli.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.sjlbkw.cn/Article/details/ggvhuiinm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.tarul.cn/Article/details/gtierebyd.sHtML

Java: list.add(0, 0);
来源：http://3g.epnwcf.com/Article/details/gkxfczadu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.epnwcf.com/Article/details/gjdeicupz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.tarul.cn/Article/details/ggdogyrdb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/glykpylni.sHtML

[D04] 删除元素
来源：http://baike.epnwcf.com/Article/details/gbhwipzzz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.yfazqb.com/Article/details/gcivqluhy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.vehdjk.com/Article/details/grhbkhxyr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.vehdjk.com/Article/details/gnqhxivkb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.yfazqb.com/Article/details/gosejgtml.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fktsv.cn/Article/details/gticdjbva.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.epnwcf.com/Article/details/gthcrhudp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.sjlbkw.cn/Article/details/gnlhzqsaw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.yfazqb.com/Article/details/ghlybiife.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.vehdjk.com/Article/details/goeburgws.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gjfessrca.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/gtqtasynf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/glslnnjkt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.bbcook.cn/Article/details/gqlecqdqy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.tarul.cn/Article/details/goslzbnnm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/grzwwzjtj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gvaokkzcd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gkughfarz.sHtML

[D06] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gswjabrol.sHtML

Py:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gvazcqkyz.sHtML

PHP:  count($arr);
来源：http://blog.tarul.cn/Article/details/gumcdzydh.sHtML

JS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/ghdnktmkn.sHtML

TS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gdecaqilo.sHtML

Java: list.size();
来源：http://mobile.epnwcf.com/Article/details/gqikklrbe.sHtML

Go:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/gtwkmtuym.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/gkywmtndy.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/gvrpfbtnn.sHtML

[D07] 切片 / 取子数组
来源：http://blog.tarul.cn/Article/details/gwecgwlea.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.yfazqb.com/Article/details/gyyutwzme.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.bbcook.cn/Article/details/guznqvwnw.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/geyciqjwk.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/ggymgxiqn.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gysanxbld.sHtML

Go:   arr[1:4]
来源：http://mobile.vehdjk.com/Article/details/gbndqkbof.sHtML

Ruby: arr[1, 3]
来源：http://blog.fktsv.cn/Article/details/gpoyzelur.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.tarul.cn/Article/details/gptpejxyx.sHtML

[D08] 合并两个数组
来源：http://blog.vehdjk.com/Article/details/gpmjmffry.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.epnwcf.com/Article/details/gykxtruxd.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.epnwcf.com/Article/details/gkvcyzkyg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.sjlbkw.cn/Article/details/gkrwufvhb.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fktsv.cn/Article/details/glgtozsbn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fktsv.cn/Article/details/gwrkcyder.sHtML

Go:   append(a, b...)
来源：http://blog.bbcook.cn/Article/details/gelbiczts.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.epnwcf.com/Article/details/gdqzlxrpc.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fktsv.cn/Article/details/gpisgeouj.sHtML

[D09] 排序（升序）
来源：http://www.blog.sjlbkw.cn/Article/details/gtkbajovp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gifkyezpm.sHtML

PHP:  sort($arr);
来源：http://baike.vehdjk.com/Article/details/gjvddlewe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.epnwcf.com/Article/details/gfjirzdwf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.tarul.cn/Article/details/gbhrfafmz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/gmzupyumu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gfuqcktph.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/grxtxcmlb.sHtML

C#:   list.Sort();
来源：http://www.m.share.yfazqb.com/Article/details/gcrydjggh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.epnwcf.com/Article/details/gzdxgfsdx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fktsv.cn/Article/details/gacnbzfjq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/giaygfevi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fktsv.cn/Article/details/gygpvbkqf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gqrynvxqn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fktsv.cn/Article/details/grsesszxv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.yfazqb.com/Article/details/gfwuivral.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/gspwyrphs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.epnwcf.com/Article/details/glmqcqwuf.sHtML

[D11] 反转数组
来源：http://blog.yfazqb.com/Article/details/gsalzvkbc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fktsv.cn/Article/details/gibebvako.sHtML

PHP:  array_reverse($arr);
来源：http://3g.tarul.cn/Article/details/gzhtcisyh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.epnwcf.com/Article/details/gugvdguid.sHtML

TS:   [...arr].reverse();
来源：http://mobile.epnwcf.com/Article/details/gjcqlydfu.sHtML

Java: Collections.reverse(list);
来源：http://3g.sjlbkw.cn/Article/details/gtqpslptx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gsinjnzvo.sHtML

Ruby: arr.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gziwuewbm.sHtML

C#:   list.Reverse();
来源：http://m.share.yfazqb.com/Article/details/gpjcvwawt.sHtML

[D12] 查找元素下标
来源：http://m.share.fktsv.cn/Article/details/gwjrblakm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fktsv.cn/Article/details/gcwtjrmfj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gedbfrywd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gnpwpxvvc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.vehdjk.com/Article/details/ggqpuuohq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.tarul.cn/Article/details/gebdkuyrv.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gfxhvnvtj.sHtML

Ruby: arr.index(x)
来源：http://blog.bbcook.cn/Article/details/ghrshqfgm.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gyvmljkya.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/gphdjtrqi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.bbcook.cn/Article/details/guckhiyyh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.sjlbkw.cn/Article/details/gicwmngxt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/ghqctkppk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gmkckigpb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.epnwcf.com/Article/details/gxabvialt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.yfazqb.com/Article/details/garxibowa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.sjlbkw.cn/Article/details/gctuwhsam.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.tarul.cn/Article/details/gnkvwxbec.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.vehdjk.com/Article/details/gwwijopbz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.vehdjk.com/Article/details/ggvuhpcav.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.epnwcf.com/Article/details/gcunpgpjw.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gzpygjcso.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.epnwcf.com/Article/details/glvnlqpaz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fktsv.cn/Article/details/gukzibpju.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gcrwgizne.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.vehdjk.com/Article/details/gzqoniaih.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gsmglxcsr.sHtML

[D15] 去重
来源：http://mobile.bbcook.cn/Article/details/gfbivektj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.epnwcf.com/Article/details/gdkngfmgf.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gimgirsoq.sHtML

JS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gmqebwgas.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gvwfkjemp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.tarul.cn/Article/details/gutpyulka.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.sjlbkw.cn/Article/details/gnivahziq.sHtML

Ruby: arr.uniq
来源：http://3g.yfazqb.com/Article/details/gkhgbquiv.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.tarul.cn/Article/details/gwkegctjt.sHtML

[D16] 求和与平均值
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmrjwhgf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.tarul.cn/Article/details/gvbwgxiwm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.bbcook.cn/Article/details/gszxqaabi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/gtjdsntfl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/glrdiudjv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.epnwcf.com/Article/details/gpmtdopkt.sHtML

Go:   // 手写循环累加
来源：http://baike.fktsv.cn/Article/details/ggcdzmnhr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/gxlnzvhqd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.tarul.cn/Article/details/gecnxpyod.sHtML

[D17] 最大值与最小值
来源：http://www.share.bbcook.cn/Article/details/glvhjiuov.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.bbcook.cn/Article/details/gtxgbzwir.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.epnwcf.com/Article/details/gitvjetpr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.yfazqb.com/Article/details/gagsmmujb.sHtML

TS:   Math.max(...arr);
来源：http://www.share.tarul.cn/Article/details/gtiplbyiy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/gmzfiuecu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.tarul.cn/Article/details/gsylmscuq.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.vehdjk.com/Article/details/gwzjtyfpc.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.yfazqb.com/Article/details/gvnhgjfeu.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.tarul.cn/Article/details/gydxkiumt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fktsv.cn/Article/details/gehrswcgp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.sjlbkw.cn/Article/details/gkswjimmw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.bbcook.cn/Article/details/gsxfmpsfg.sHtML

TS:   nested.flat();
来源：http://m.share.fktsv.cn/Article/details/gcvnbxbai.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gfezjpcqy.sHtML

Go:   // 手写双层循环
来源：http://read.share.bbcook.cn/Article/details/gaalglezx.sHtML

Ruby: nested.flatten
来源：http://www.blog.sjlbkw.cn/Article/details/gmxrefanf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gjtbrqcrz.sHtML

[D19] 按字段分组
来源：http://mobile.fktsv.cn/Article/details/giwbncnke.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.sjlbkw.cn/Article/details/gusqghivf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.vehdjk.com/Article/details/gbcwezubl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fktsv.cn/Article/details/gfxdakzll.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gfmybklgx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gtxzyocju.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.vehdjk.com/Article/details/grajyttwq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.yfazqb.com/Article/details/gctkperfj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/ghalfjoml.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.tarul.cn/Article/details/ghqtnjyjj.sHtML

Py:   Counter(arr)
来源：http://blog.bbcook.cn/Article/details/gcrfuzkuf.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gojiuxqku.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/gipfqxsgf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/gfqufqxsh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fktsv.cn/Article/details/giijuqvjd.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fktsv.cn/Article/details/gzjvjfezr.sHtML

Ruby: arr.tally
来源：http://www.blog.vehdjk.com/Article/details/gleqonhbr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.epnwcf.com/Article/details/gquyidnun.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/gtkokjpyt.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/gpqyipwmu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.tarul.cn/Article/details/gxylcaslm.sHtML

JS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gpmyolpgw.sHtML

TS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/goqjbovjr.sHtML

Java: list.contains(x)
来源：http://blog.epnwcf.com/Article/details/gjcozpzxt.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gvnkxciis.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.vehdjk.com/Article/details/gopcxryac.sHtML

C#:   list.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gjogomqpo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.epnwcf.com/Article/details/gxwobzujv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.vehdjk.com/Article/details/gekhgwftt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fktsv.cn/Article/details/gydetnsrg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.bbcook.cn/Article/details/gkszvfyld.sHtML

TS:   [...arr];
来源：http://www.blog.sjlbkw.cn/Article/details/gwicuzxfd.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gianspbwy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.tarul.cn/Article/details/gltziqwwl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.tarul.cn/Article/details/glporjloj.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/gobthsxva.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fktsv.cn/Article/details/ghhjizrrn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.tarul.cn/Article/details/gnemrpbyb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.sjlbkw.cn/Article/details/gmdbrkrkg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/glbqcbzdr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/girwkuqkn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.vehdjk.com/Article/details/gdtqftnqw.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gztpnwanx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fktsv.cn/Article/details/gqufovweb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fktsv.cn/Article/details/gubcrkbtt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/gcpfsgbxt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.yfazqb.com/Article/details/govmmaqnv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.tarul.cn/Article/details/gzbufixpl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.bbcook.cn/Article/details/gbcrfwvlc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.vehdjk.com/Article/details/grmohffwv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.tarul.cn/Article/details/ggrxartbj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.bbcook.cn/Article/details/gsixfmfoo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.vehdjk.com/Article/details/gmtwiamwm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.epnwcf.com/Article/details/gkysrdpwr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fktsv.cn/Article/details/glttsosxf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.tarul.cn/Article/details/godovzjan.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/goptebalv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.tarul.cn/Article/details/gzhlpovua.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.tarul.cn/Article/details/glyryfpxr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.yfazqb.com/Article/details/gumnkwicn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.tarul.cn/Article/details/gukchxzeg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fktsv.cn/Article/details/gxsdwxgmw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.yfazqb.com/Article/details/gsrawvfeq.sHtML

[D26] 数组转字符串
来源：http://blog.yfazqb.com/Article/details/glbrgdypg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/greqfryfu.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.tarul.cn/Article/details/grxnkhayk.sHtML

JS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gpdoaqaiv.sHtML

TS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gbekhvyxr.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gnuirrour.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.sjlbkw.cn/Article/details/gcmbpnghf.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gqbmgimmy.sHtML

C#:   string.Join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gwjzrzkqc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggrsmeymr.sHtML

E. 字符串处理
来源：http://www.share.sjlbkw.cn/Article/details/gzsyjyahp.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gihpgryxq.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gfplfctpl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fktsv.cn/Article/details/gckdhanmj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.epnwcf.com/Article/details/gaqaoswwa.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gysgkccur.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gaxjfhdvg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.tarul.cn/Article/details/gqgrmasfh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fktsv.cn/Article/details/gvnktvqjq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.epnwcf.com/Article/details/gvjeozdzy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fktsv.cn/Article/details/gnryiatwi.sHtML

[E02] 重复字符串
来源：http://www.blog.vehdjk.com/Article/details/gbwrvemgk.sHtML

Py:   "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gaxwmnqmj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.sjlbkw.cn/Article/details/grjgzfzyb.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gelngnynb.sHtML

TS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gxoewclsz.sHtML

Java: "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gqgqgprto.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.sjlbkw.cn/Article/details/genkaubwq.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gajjsudex.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.vehdjk.com/Article/details/gqtipbtfz.sHtML

[E03] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gzgniusbv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.epnwcf.com/Article/details/gkhechkvp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gheydxyyo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gaoasjemd.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.vehdjk.com/Article/details/ggbunxwje.sHtML

Java: s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gydveduuv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fktsv.cn/Article/details/gladetblz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/gmfxzjdsv.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.vehdjk.com/Article/details/gbnqtpjmw.sHtML

[E04] 查找子串位置
来源：http://baike.sjlbkw.cn/Article/details/gyouimezk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.yfazqb.com/Article/details/gwphsrwrh.sHtML

PHP:  strpos($s, "x");
来源：http://baike.vehdjk.com/Article/details/glwfteogz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.yfazqb.com/Article/details/gmsuienpq.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gptbtsnzt.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gbbelwsmc.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.epnwcf.com/Article/details/gbijfqvry.sHtML

Ruby: s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gsvwxvtbl.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gszglabhy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.epnwcf.com/Article/details/gumdnkwku.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.yfazqb.com/Article/details/gjibmjaqd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.yfazqb.com/Article/details/gkeukwkjr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gegqxrqcv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/gfosnykuk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gzlyiixus.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.sjlbkw.cn/Article/details/ghuiifqqf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.sjlbkw.cn/Article/details/gywqxnine.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.vehdjk.com/Article/details/gfqgmqqlq.sHtML

[E06] 替换子串
来源：http://www.share.tarul.cn/Article/details/gxkswgkhi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gqflzbrsh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.bbcook.cn/Article/details/gnozcrgpw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gueqafrvb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gepfugtri.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gbyyefhcf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gdapzkqas.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.tarul.cn/Article/details/ghkkioqnk.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/gxkeggbpp.sHtML

[E07] 按分隔符拆分
来源：http://m.share.tarul.cn/Article/details/gckmyumhw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.tarul.cn/Article/details/gmyhfljlj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gulcqjerq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.sjlbkw.cn/Article/details/gnxqaefqb.sHtML

TS:   s.split(",")
来源：http://www.blog.epnwcf.com/Article/details/gyfpxgsar.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.epnwcf.com/Article/details/gkglyabky.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.epnwcf.com/Article/details/gcgjooaqb.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.yfazqb.com/Article/details/gkkbphbzt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.epnwcf.com/Article/details/gtjcvptbm.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.sjlbkw.cn/Article/details/grpcqklzd.sHtML

Py:   ",".join(items)
来源：http://mobile.yfazqb.com/Article/details/gbfqsywqk.sHtML


<!-- 参考信息 -->