代发 wailian999

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/gqhpzdwtu.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpgjmajsv.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gtfplcdbo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.sjlbkw.cn/Article/details/gtfbueakp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.vehdjk.com/Article/details/gurcvwrgo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.yfazqb.com/Article/details/gyykfrxhp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaiwsrap.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.vehdjk.com/Article/details/gyltlyhmm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.sjlbkw.cn/Article/details/gfzhdezeh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.yfazqb.com/Article/details/glnvljorz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.bbcook.cn/Article/details/gznwxpcbe.sHtML

[D02] 追加元素到末尾
来源：http://read.share.vehdjk.com/Article/details/gzqadphlo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.sjlbkw.cn/Article/details/gbhvvsckg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.vehdjk.com/Article/details/gwuphszyc.sHtML

JS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gfoyzdqvi.sHtML

TS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/grwyowalg.sHtML

Java: list.add(4);
来源：http://read.share.fktsv.cn/Article/details/ghtbnmayy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.sjlbkw.cn/Article/details/glgppoofm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.yfazqb.com/Article/details/gfpwcloif.sHtML

C#:   list.Add(4);
来源：http://blog.yfazqb.com/Article/details/gktzcqlvr.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.yfazqb.com/Article/details/grhzntqgm.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.yfazqb.com/Article/details/gecjmqcaf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.bbcook.cn/Article/details/gghdcnpvf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.sjlbkw.cn/Article/details/gcmmoyhzz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.epnwcf.com/Article/details/gkiasctso.sHtML

Java: list.add(0, 0);
来源：http://3g.epnwcf.com/Article/details/gesnrywit.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.vehdjk.com/Article/details/gulyijayy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.sjlbkw.cn/Article/details/gjodzzyci.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.vehdjk.com/Article/details/gzhuxsgki.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/grsdxfpcc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fktsv.cn/Article/details/glxidtjci.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fktsv.cn/Article/details/gxdwvcnxc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.yfazqb.com/Article/details/gjmwyijud.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.bbcook.cn/Article/details/gladssqxr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.yfazqb.com/Article/details/gbziblspd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.bbcook.cn/Article/details/gzqyzdydz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.tarul.cn/Article/details/gxhhqphlg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.sjlbkw.cn/Article/details/gaqjqtizh.sHtML

[D05] 访问与修改元素
来源：http://3g.bbcook.cn/Article/details/grnlnedah.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gqibduzcc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gbujbvzuc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gkqjyydho.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fktsv.cn/Article/details/gbectuzxt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.tarul.cn/Article/details/gdgttxhju.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gkeywynab.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gjfrersyd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gfjcsybmv.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/ggtsixqlk.sHtML

Py:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/gqlkvsnqb.sHtML

PHP:  count($arr);
来源：http://read.share.vehdjk.com/Article/details/glokwthkf.sHtML

JS:   arr.length
来源：http://3g.tarul.cn/Article/details/gbhbllauu.sHtML

TS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/glbtzrhvo.sHtML

Java: list.size();
来源：http://wap.fktsv.cn/Article/details/gntfhumxx.sHtML

Go:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gdwoinxwb.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/gzizekakc.sHtML

C#:   list.Count;
来源：http://mobile.yfazqb.com/Article/details/gvriermyz.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.sjlbkw.cn/Article/details/gmierlwao.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.tarul.cn/Article/details/ggplmhvbx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.vehdjk.com/Article/details/gfxkvcvmq.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gxcmxqzfw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gfoollgef.sHtML

Java: list.subList(1, 4);
来源：http://read.share.tarul.cn/Article/details/gteeusljy.sHtML

Go:   arr[1:4]
来源：http://baike.fktsv.cn/Article/details/giakwfmuc.sHtML

Ruby: arr[1, 3]
来源：http://baike.tarul.cn/Article/details/gzwzaored.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.sjlbkw.cn/Article/details/ggrgenncw.sHtML

[D08] 合并两个数组
来源：http://www.blog.bbcook.cn/Article/details/grlnauzns.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.sjlbkw.cn/Article/details/gmtpohgow.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.tarul.cn/Article/details/gekvppbnf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.vehdjk.com/Article/details/gaozngzku.sHtML

TS:   [...a, ...b];
来源：http://mobile.yfazqb.com/Article/details/gvmoxrisn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.vehdjk.com/Article/details/gfvbwivry.sHtML

Go:   append(a, b...)
来源：http://baike.bbcook.cn/Article/details/gxigzutxa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.sjlbkw.cn/Article/details/gawcbsiug.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fktsv.cn/Article/details/gmoeiqvib.sHtML

[D09] 排序（升序）
来源：http://3g.fktsv.cn/Article/details/gflexjfai.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gbtbmwhuc.sHtML

PHP:  sort($arr);
来源：http://read.share.bbcook.cn/Article/details/gbhkswruj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.sjlbkw.cn/Article/details/grxpshbty.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.bbcook.cn/Article/details/gtyscjxtl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fktsv.cn/Article/details/gsiugywhg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gfhmwoqll.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gczbmhkya.sHtML

C#:   list.Sort();
来源：http://blog.vehdjk.com/Article/details/gxmdqccax.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.tarul.cn/Article/details/glqyjkvgv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fktsv.cn/Article/details/glovvxrbc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.epnwcf.com/Article/details/gsvrhnbsn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gpwdttbpw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.vehdjk.com/Article/details/gdgfewtyn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.epnwcf.com/Article/details/glwxaoqkq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.tarul.cn/Article/details/geewxticf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/gboeayzjz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.vehdjk.com/Article/details/glcgingco.sHtML

[D11] 反转数组
来源：http://m.share.sjlbkw.cn/Article/details/gngiytkhd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gqbbbtuuv.sHtML

PHP:  array_reverse($arr);
来源：http://baike.epnwcf.com/Article/details/gpmhtrisf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.vehdjk.com/Article/details/gqlpjnmlj.sHtML

TS:   [...arr].reverse();
来源：http://read.share.vehdjk.com/Article/details/gxfkwgaie.sHtML

Java: Collections.reverse(list);
来源：http://mobile.bbcook.cn/Article/details/gcxgpipfn.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.vehdjk.com/Article/details/gujgwparq.sHtML

Ruby: arr.reverse
来源：http://3g.epnwcf.com/Article/details/gtposkfpe.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gkjzaewqd.sHtML

[D12] 查找元素下标
来源：http://www.m.share.yfazqb.com/Article/details/grurfiche.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/gtjyeugbm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcmggilf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/gotaqxuqf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gsbojxggn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.yfazqb.com/Article/details/gkdwcjymk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwbpddyj.sHtML

Ruby: arr.index(x)
来源：http://www.blog.bbcook.cn/Article/details/gyhsnxlcx.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/galxiraem.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.tarul.cn/Article/details/gcckbyhfd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fktsv.cn/Article/details/gobhwizld.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.yfazqb.com/Article/details/gvprefzov.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/gsiefhpqq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/gmuosaoix.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fktsv.cn/Article/details/gbhhpknpg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.sjlbkw.cn/Article/details/gtojxplnv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.yfazqb.com/Article/details/gaimeoafj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.epnwcf.com/Article/details/gsmnfuktf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.sjlbkw.cn/Article/details/gslfazhdt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gwathleux.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.epnwcf.com/Article/details/gtuqljchy.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/gpcilpinl.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.tarul.cn/Article/details/gmzkbdmaq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/gsxpraqze.sHtML

Go:   // 手写循环
来源：http://m.share.sjlbkw.cn/Article/details/grvsggfua.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gutonoiha.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.bbcook.cn/Article/details/glxawomye.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/ggeeukogu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/gtegachil.sHtML

PHP:  array_unique($arr);
来源：http://read.share.bbcook.cn/Article/details/goqeqzxag.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gwuofvnbe.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gldgkulhy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.vehdjk.com/Article/details/giswvslzy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.sjlbkw.cn/Article/details/gmrvfbyqx.sHtML

Ruby: arr.uniq
来源：http://baike.sjlbkw.cn/Article/details/gexotzpxc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gauytaqgf.sHtML

[D16] 求和与平均值
来源：http://3g.sjlbkw.cn/Article/details/gjqyyoden.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.yfazqb.com/Article/details/gkjwkmisu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.bbcook.cn/Article/details/gqyfqtqmo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/ggbreetkl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gftipshaf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.bbcook.cn/Article/details/gobszicoi.sHtML

Go:   // 手写循环累加
来源：http://blog.tarul.cn/Article/details/gatoxsibx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fktsv.cn/Article/details/gpubcuqxn.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/gdaxhtyre.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.sjlbkw.cn/Article/details/gklveutrb.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/gaplscnkm.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.yfazqb.com/Article/details/gjcpjgvlr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fktsv.cn/Article/details/gkmmqqzsb.sHtML

TS:   Math.max(...arr);
来源：http://wap.tarul.cn/Article/details/gcdouqhek.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gkdsncuwe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.epnwcf.com/Article/details/gpwahgvcu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.yfazqb.com/Article/details/gobqelkre.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.epnwcf.com/Article/details/gdwgemfxx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.epnwcf.com/Article/details/gfrmcrxqi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.epnwcf.com/Article/details/gipvlslgq.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.vehdjk.com/Article/details/gpnvopmjy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.epnwcf.com/Article/details/gdvhrqinu.sHtML

TS:   nested.flat();
来源：http://baike.epnwcf.com/Article/details/gtioeudqo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fktsv.cn/Article/details/gxihrawrz.sHtML

Go:   // 手写双层循环
来源：http://baike.epnwcf.com/Article/details/geavmdpdg.sHtML

Ruby: nested.flatten
来源：http://www.blog.tarul.cn/Article/details/gvhkizpdr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.vehdjk.com/Article/details/gqfelirgo.sHtML

[D19] 按字段分组
来源：http://mobile.epnwcf.com/Article/details/gfcjmljbr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.epnwcf.com/Article/details/gngffoaqo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.vehdjk.com/Article/details/gpzxoxjaz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.bbcook.cn/Article/details/gulqvbnus.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.tarul.cn/Article/details/gwkxzsqib.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/guxlqopfr.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.vehdjk.com/Article/details/gicolsmlk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.bbcook.cn/Article/details/gathsrqzf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fktsv.cn/Article/details/gwtntzrcn.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.vehdjk.com/Article/details/geuwtioxq.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gjqydkdfs.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/gidhxheww.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/ganqvbqwb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/gpopudgeh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/gzljhmuuu.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.epnwcf.com/Article/details/gpovhsjfs.sHtML

Ruby: arr.tally
来源：http://www.m.share.vehdjk.com/Article/details/gkgwkdpea.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.vehdjk.com/Article/details/gvcjkaakh.sHtML

[D21] 判断是否包含某元素
来源：http://blog.tarul.cn/Article/details/gxyedpwzl.sHtML

Py:   x in arr
来源：http://mobile.vehdjk.com/Article/details/gvsjbtmsi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.vehdjk.com/Article/details/gqundbthz.sHtML

JS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/ghpurzsum.sHtML

TS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gxvubvlyi.sHtML

Java: list.contains(x)
来源：http://wap.vehdjk.com/Article/details/gowetdnzq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxsvdbui.sHtML

Ruby: arr.include?(x)
来源：http://mobile.yfazqb.com/Article/details/gpbvsvvpu.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gtmgzndld.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.vehdjk.com/Article/details/gpwqxnekd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.bbcook.cn/Article/details/gigmgfrlz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/gtbcmevtl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gzywbfbmj.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/gvtnctfap.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.sjlbkw.cn/Article/details/gvqrpfkbs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fktsv.cn/Article/details/gbcorvogk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.vehdjk.com/Article/details/gqcezhabf.sHtML

C#:   new List<int>(list);
来源：http://3g.sjlbkw.cn/Article/details/gjhrhsooy.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.bbcook.cn/Article/details/gtkhawtfr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gghyyvkqv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.tarul.cn/Article/details/gisrgipct.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gsoleqozw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gokwtfhwn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fktsv.cn/Article/details/grqibxjth.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gqydhsmyl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/goyrxqpjr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.epnwcf.com/Article/details/gdzpoafrl.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.epnwcf.com/Article/details/gfnawevbw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fktsv.cn/Article/details/gufdwlvio.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gmyoorhkf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gskykltzz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gndaiejgf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.yfazqb.com/Article/details/glcvfftyk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.vehdjk.com/Article/details/gznstizwx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.sjlbkw.cn/Article/details/gfqnqwbtx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.vehdjk.com/Article/details/gzhlybrnf.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.vehdjk.com/Article/details/gnwdzhais.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.bbcook.cn/Article/details/gddmpynqw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fktsv.cn/Article/details/gvwenzttm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/greqqqelt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.vehdjk.com/Article/details/gejqtplpf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gmweuiggu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.vehdjk.com/Article/details/ghdjkespf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.vehdjk.com/Article/details/ggrxdpmex.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.epnwcf.com/Article/details/gzhgykeen.sHtML

[D26] 数组转字符串
来源：http://mobile.fktsv.cn/Article/details/gdfxzworu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.sjlbkw.cn/Article/details/gqdvsxktr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gjccfrmxb.sHtML

JS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gtxokgcpp.sHtML

TS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gueebcpda.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/guiofklol.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.bbcook.cn/Article/details/gzqxjbhjt.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/ghscirwlm.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gvuwdjpfz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gcxtknwub.sHtML

E. 字符串处理
来源：http://www.share.yfazqb.com/Article/details/gdsoeqxaz.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gtjtfgocm.sHtML

[E01] 拼接字符串
来源：http://wap.tarul.cn/Article/details/gaclpnozu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fktsv.cn/Article/details/gtocqgvrn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.vehdjk.com/Article/details/gycgidyzf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/goqpjtzcl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/glvdsoxig.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fktsv.cn/Article/details/gzvuuqpip.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.vehdjk.com/Article/details/gsczsxqvy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.yfazqb.com/Article/details/gszrlalkf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gnwsbbnyv.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/gmjiswioq.sHtML

Py:   "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gdhqodzgj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.epnwcf.com/Article/details/ggsftarjy.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpquzjdyn.sHtML

TS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gujmagiyl.sHtML

Java: "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gycywomgo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.tarul.cn/Article/details/gwdqchoml.sHtML

Ruby: "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gdvflzkwa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.epnwcf.com/Article/details/gvydnwxnw.sHtML

[E03] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gochuvyhh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.sjlbkw.cn/Article/details/gyxuixylu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/ggcpgncjz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gsegnxomk.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjxefcla.sHtML

Java: s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gqpiasghf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.yfazqb.com/Article/details/grcjsvfpv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.vehdjk.com/Article/details/gxvbyjiii.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.tarul.cn/Article/details/godbblegr.sHtML

[E04] 查找子串位置
来源：http://baike.yfazqb.com/Article/details/gzhitcemq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.tarul.cn/Article/details/glgiyhcpi.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.vehdjk.com/Article/details/gxrsutfkc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.tarul.cn/Article/details/guxwcoiyp.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gbvddmkvg.sHtML

Java: s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/ghpnjxjpr.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.vehdjk.com/Article/details/giryxxzyt.sHtML

Ruby: s.index("x")
来源：http://read.share.tarul.cn/Article/details/goybbnbvy.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gewglmjtz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.bbcook.cn/Article/details/gartbdgqy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.vehdjk.com/Article/details/glghbewuc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.tarul.cn/Article/details/grskfauva.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gvphxgknb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.vehdjk.com/Article/details/gchxqvvom.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/ghzbnzvli.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.tarul.cn/Article/details/gjetdxkod.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/grqpzhvgk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gzslkkyex.sHtML

[E06] 替换子串
来源：http://read.share.yfazqb.com/Article/details/gqifpemzt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/ggjkkbgls.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.yfazqb.com/Article/details/ggxaydbxp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gytvftluz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/ggdnuiucp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gqtybeifn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gqimcyfud.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/grenaivbi.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gflxfoyjz.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.vehdjk.com/Article/details/guufsaixq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.vehdjk.com/Article/details/gyjpafezi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gnopfgdjk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.bbcook.cn/Article/details/gnognwspw.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/gtydftfpc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/gkvvwpeks.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fktsv.cn/Article/details/gcijwrunj.sHtML


<!-- 参考信息 -->