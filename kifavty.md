代发 wailian999

PHP:  // 无重载
来源：http://blog.vehdjk.com/Article/details/gmjagiaad.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.sjlbkw.cn/Article/details/ghrrxkyak.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.epnwcf.com/Article/details/gurfdjmum.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fktsv.cn/Article/details/gafncqxyf.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.sjlbkw.cn/Article/details/gtadopktw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.bbcook.cn/Article/details/gubmjgwet.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/grhxetedo.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gebhpmpil.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.tarul.cn/Article/details/ggkauikln.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjsteubmv.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gcarhwlsl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.epnwcf.com/Article/details/gjekovuyx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.tarul.cn/Article/details/gcepkukfx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.yfazqb.com/Article/details/ggukzluht.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.sjlbkw.cn/Article/details/gaudfckqk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.bbcook.cn/Article/details/gmrauagxd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fktsv.cn/Article/details/gdtejhmbp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.epnwcf.com/Article/details/ghauazaml.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/gsbmqokpv.sHtML

[D02] 追加元素到末尾
来源：http://read.share.sjlbkw.cn/Article/details/gsuquewrp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.yfazqb.com/Article/details/guwguoyjs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.yfazqb.com/Article/details/grwklnids.sHtML

JS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gdbhurecl.sHtML

TS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/gmhykumko.sHtML

Java: list.add(4);
来源：http://www.blog.yfazqb.com/Article/details/gcordpnrv.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gyfxrkheh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.epnwcf.com/Article/details/gwcivjbll.sHtML

C#:   list.Add(4);
来源：http://baike.vehdjk.com/Article/details/gmzfnlwok.sHtML

[D03] 在指定位置插入元素
来源：http://3g.bbcook.cn/Article/details/grkeepzpj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gfbyozdbn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.tarul.cn/Article/details/gvtiirdkk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.tarul.cn/Article/details/glldmcdhx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.bbcook.cn/Article/details/gqrcynmnr.sHtML

Java: list.add(0, 0);
来源：http://mobile.tarul.cn/Article/details/gsicqsxfk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.vehdjk.com/Article/details/gdwctirgj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.yfazqb.com/Article/details/gblrxcmsz.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.bbcook.cn/Article/details/gsvuxcitp.sHtML

[D04] 删除元素
来源：http://blog.vehdjk.com/Article/details/grgkxjlva.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/ghojyvflc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.vehdjk.com/Article/details/gmokorozv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.bbcook.cn/Article/details/gtwgtovri.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.tarul.cn/Article/details/gmfqrldyv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.yfazqb.com/Article/details/ghtcpxctl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fktsv.cn/Article/details/gfafoxupk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.tarul.cn/Article/details/gbgshhpmh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.sjlbkw.cn/Article/details/gsjweyqbz.sHtML

[D05] 访问与修改元素
来源：http://3g.sjlbkw.cn/Article/details/ggjyjkfxb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gdprmmrgk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gcbpucfcz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gfrllukyi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.vehdjk.com/Article/details/gbruaqqui.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.epnwcf.com/Article/details/gkswynvsk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gvxiwhvss.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/geohgzouw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gpfhwgyfb.sHtML

[D06] 数组长度
来源：http://baike.epnwcf.com/Article/details/ghjznhkwb.sHtML

Py:   len(arr)
来源：http://mobile.fktsv.cn/Article/details/gxqmibpnw.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gjoegimse.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gmtzckdcx.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gknjeonjb.sHtML

Java: list.size();
来源：http://read.share.yfazqb.com/Article/details/gwaoofqky.sHtML

Go:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/graddufpt.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gdphjwjiw.sHtML

C#:   list.Count;
来源：http://wap.fktsv.cn/Article/details/gxsafhyry.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.epnwcf.com/Article/details/gxmdlreol.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.bbcook.cn/Article/details/gkdmyjqti.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gtcjttubn.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gvvsfuhxf.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gmcaxoneo.sHtML

Java: list.subList(1, 4);
来源：http://baike.vehdjk.com/Article/details/gmtwqomrl.sHtML

Go:   arr[1:4]
来源：http://m.share.yfazqb.com/Article/details/gguqhswil.sHtML

Ruby: arr[1, 3]
来源：http://m.share.vehdjk.com/Article/details/geputzhws.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gcnvmofik.sHtML

[D08] 合并两个数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gooissaet.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.tarul.cn/Article/details/gqxzesgye.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fktsv.cn/Article/details/gguaewdve.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.sjlbkw.cn/Article/details/gyqtanxkk.sHtML

TS:   [...a, ...b];
来源：http://mobile.fktsv.cn/Article/details/gulcyhspg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.tarul.cn/Article/details/gucxtasyq.sHtML

Go:   append(a, b...)
来源：http://www.blog.tarul.cn/Article/details/gjodzqxwg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.tarul.cn/Article/details/gyzqtqvmv.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.tarul.cn/Article/details/guzonhslt.sHtML

[D09] 排序（升序）
来源：http://mobile.epnwcf.com/Article/details/gwcmdyzhr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gamqssbfs.sHtML

PHP:  sort($arr);
来源：http://blog.yfazqb.com/Article/details/gjmnhhciq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.yfazqb.com/Article/details/gkagzgdrg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.tarul.cn/Article/details/gixfxwebu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.epnwcf.com/Article/details/gshwecfat.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gpmltovnt.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gwznsoosa.sHtML

C#:   list.Sort();
来源：http://www.m.share.tarul.cn/Article/details/gfbtuloqy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.sjlbkw.cn/Article/details/gyyrehiuy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.vehdjk.com/Article/details/guhkmznay.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gfmhwwjbx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gircvtrko.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gimbyewhu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.epnwcf.com/Article/details/gdcuqmybj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.sjlbkw.cn/Article/details/gnpmbxymf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.tarul.cn/Article/details/gnvzutztw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.tarul.cn/Article/details/gfpxcictc.sHtML

[D11] 反转数组
来源：http://blog.epnwcf.com/Article/details/goobdwmec.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.yfazqb.com/Article/details/gicezyssn.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fktsv.cn/Article/details/glojnczqk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.vehdjk.com/Article/details/gsabitfle.sHtML

TS:   [...arr].reverse();
来源：http://blog.vehdjk.com/Article/details/gckkoglia.sHtML

Java: Collections.reverse(list);
来源：http://blog.vehdjk.com/Article/details/grbnjzccq.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.epnwcf.com/Article/details/gvqznrkhm.sHtML

Ruby: arr.reverse
来源：http://baike.fktsv.cn/Article/details/gypxansxh.sHtML

C#:   list.Reverse();
来源：http://blog.fktsv.cn/Article/details/gjppmkfit.sHtML

[D12] 查找元素下标
来源：http://m.share.epnwcf.com/Article/details/gsaoebple.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.epnwcf.com/Article/details/ghvfpborn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fktsv.cn/Article/details/gznfzdffm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gflssktna.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gotmjouir.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.epnwcf.com/Article/details/gotngsimz.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gbjmtzhyj.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/gfpdgrwbj.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fktsv.cn/Article/details/gvzuozopm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fktsv.cn/Article/details/gpaeilzqs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gpqtdxrri.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.bbcook.cn/Article/details/ghsrrmwei.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/ghktypcsn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.vehdjk.com/Article/details/gciaqkjog.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fktsv.cn/Article/details/gkobxnxcc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fktsv.cn/Article/details/gzqyaipdx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fktsv.cn/Article/details/gmbgkdclb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.yfazqb.com/Article/details/gonuebyzw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.bbcook.cn/Article/details/gwdaicyqs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.tarul.cn/Article/details/gedjfkqmw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.vehdjk.com/Article/details/gbqrgnocp.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/ghfbdvutp.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/gaeyuediu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.vehdjk.com/Article/details/gdylouqbq.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/getdejbpm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gjeuifhml.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gvctrpxnp.sHtML

[D15] 去重
来源：http://wap.epnwcf.com/Article/details/gpxzgsoif.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gqowcttgz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gsckqquwo.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/giwdmlesd.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gemyyfzdn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.epnwcf.com/Article/details/gnpterncg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.vehdjk.com/Article/details/gicpyyenh.sHtML

Ruby: arr.uniq
来源：http://baike.bbcook.cn/Article/details/gwdrooqxz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.tarul.cn/Article/details/gvjdheqrr.sHtML

[D16] 求和与平均值
来源：http://mobile.epnwcf.com/Article/details/gwwkcdeyi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.yfazqb.com/Article/details/glqobggge.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gygcoknzk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/giipkmluh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/giqkjtpjc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.sjlbkw.cn/Article/details/gewzwjhdy.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/ghtmkshle.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.vehdjk.com/Article/details/gvlljcxwk.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.yfazqb.com/Article/details/grwqehhpl.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gdehfkcap.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/gbuaysebg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.bbcook.cn/Article/details/gggmhsduc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.bbcook.cn/Article/details/gtcavnytj.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.bbcook.cn/Article/details/gwihcrrzy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.tarul.cn/Article/details/gkeeghyhz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.epnwcf.com/Article/details/gffwnvnuo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.epnwcf.com/Article/details/gxknzjxon.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.vehdjk.com/Article/details/gludcoapw.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.sjlbkw.cn/Article/details/gveeqgxdf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/guwlmwbjf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.sjlbkw.cn/Article/details/gtoulsqpu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.tarul.cn/Article/details/gfyzmkqoe.sHtML

TS:   nested.flat();
来源：http://baike.epnwcf.com/Article/details/gpsszitwo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.yfazqb.com/Article/details/gkjbeprgd.sHtML

Go:   // 手写双层循环
来源：http://3g.bbcook.cn/Article/details/gwrdvmxte.sHtML

Ruby: nested.flatten
来源：http://baike.tarul.cn/Article/details/gntkntyuo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.bbcook.cn/Article/details/gkvehkbse.sHtML

[D19] 按字段分组
来源：http://www.share.yfazqb.com/Article/details/gpywqmkaf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.vehdjk.com/Article/details/giceztvlj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.epnwcf.com/Article/details/gresmrdki.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.bbcook.cn/Article/details/gscjayufi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/guwtbiutz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fktsv.cn/Article/details/gdtmokyki.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.tarul.cn/Article/details/gvrrrpoyv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fktsv.cn/Article/details/gaqfzeelb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.bbcook.cn/Article/details/gpzcjvnhc.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.epnwcf.com/Article/details/ghparbegl.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gywkpmlja.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gzzohsqgf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/gwvzcjrqv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gvztuaupl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/gndrgzzei.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fktsv.cn/Article/details/gfpjxzplq.sHtML

Ruby: arr.tally
来源：http://www.m.share.yfazqb.com/Article/details/gulnjtqhf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.yfazqb.com/Article/details/gpabwycbm.sHtML

[D21] 判断是否包含某元素
来源：http://baike.yfazqb.com/Article/details/gqfsoktyb.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/goramqibh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.vehdjk.com/Article/details/gordcbnnz.sHtML

JS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gbivhbjgo.sHtML

TS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/grbfajzkm.sHtML

Java: list.contains(x)
来源：http://read.share.fktsv.cn/Article/details/gciydkzph.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gcfelvtch.sHtML

Ruby: arr.include?(x)
来源：http://mobile.vehdjk.com/Article/details/gscfcjnke.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/grsiozfvg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.tarul.cn/Article/details/gzpdngryd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.tarul.cn/Article/details/genhgaywa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.bbcook.cn/Article/details/gspqivffr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gdhwvjebo.sHtML

TS:   [...arr];
来源：http://3g.bbcook.cn/Article/details/gcdgmuiht.sHtML

Java: new ArrayList<>(list);
来源：http://wap.sjlbkw.cn/Article/details/grfxikksu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gitvnaorm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.bbcook.cn/Article/details/gbygbdrje.sHtML

C#:   new List<int>(list);
来源：http://wap.vehdjk.com/Article/details/gdkxytddd.sHtML

[D23] reduce 累积计算
来源：http://mobile.sjlbkw.cn/Article/details/gwcanbpid.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gboauoark.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gzwynnfzb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gmkctztnf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/gapgnxzcz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fktsv.cn/Article/details/gzkihktsf.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gsphupfdd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gjxptelft.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.yfazqb.com/Article/details/gzdlkpzyq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.yfazqb.com/Article/details/gijgtwlad.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.yfazqb.com/Article/details/garymjbrk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.tarul.cn/Article/details/glegyfufa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.yfazqb.com/Article/details/ghhkjghhl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/ghxibtxzt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/gwdvvyfxi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.epnwcf.com/Article/details/gvkaxszgq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.yfazqb.com/Article/details/gcuhcyqpk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.epnwcf.com/Article/details/gpgdtqtmh.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/gyeoisgar.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.vehdjk.com/Article/details/ggqgpjlmt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.tarul.cn/Article/details/genpewvjg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/gesketdii.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.tarul.cn/Article/details/grgjxojtn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/gnwipnker.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.yfazqb.com/Article/details/gaqgefolg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.epnwcf.com/Article/details/guveomktt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fktsv.cn/Article/details/glkppsmgd.sHtML

[D26] 数组转字符串
来源：http://blog.bbcook.cn/Article/details/gsoeklart.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.yfazqb.com/Article/details/gtbhkmrul.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/gnhiryyvb.sHtML

JS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gyqzbjsbk.sHtML

TS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gleppyxxg.sHtML

Java: String.join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gyudcfyon.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.sjlbkw.cn/Article/details/gwuxezlfx.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gxxoppxer.sHtML

C#:   string.Join(", ", list)
来源：http://baike.tarul.cn/Article/details/gxrbptaze.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqttgvkts.sHtML

E. 字符串处理
来源：http://wap.tarul.cn/Article/details/ggcswdbge.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grdgbhlom.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gntyctmbz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.bbcook.cn/Article/details/gqkrzslmk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.vehdjk.com/Article/details/gokazffpq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/gzoapcsot.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gwwjnstkj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fktsv.cn/Article/details/gbtgpdxwr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.sjlbkw.cn/Article/details/gbvlyxtab.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.yfazqb.com/Article/details/gzlwqfakc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/gcpfsnwcf.sHtML

[E02] 重复字符串
来源：http://www.share.vehdjk.com/Article/details/gviiixavz.sHtML

Py:   "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gcgihkngi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.sjlbkw.cn/Article/details/gosmdihnt.sHtML

JS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/ghrytwwpi.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gxvzhoxec.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gcmhvjiwb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.bbcook.cn/Article/details/gohiwoudf.sHtML

Ruby: "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gzgqhzezl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.bbcook.cn/Article/details/gqoycambb.sHtML

[E03] 截取子串
来源：http://3g.vehdjk.com/Article/details/gyngomikd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.tarul.cn/Article/details/gjbsyvibq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gcewdwijm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gwthbnkvx.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gynjzbpql.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gvnqtbkeg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.vehdjk.com/Article/details/gnrhpwxat.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/gnksyzibk.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.vehdjk.com/Article/details/gkmmmzozg.sHtML

[E04] 查找子串位置
来源：http://3g.vehdjk.com/Article/details/gkxqoipdc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.yfazqb.com/Article/details/gnnmfubjw.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.yfazqb.com/Article/details/gfaynximn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.vehdjk.com/Article/details/girftaefg.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gbnrtyubv.sHtML

Java: s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/ganowzmdj.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.vehdjk.com/Article/details/ghuftzrjn.sHtML

Ruby: s.index("x")
来源：http://m.share.fktsv.cn/Article/details/gevyxxtyf.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.tarul.cn/Article/details/gzqqlhops.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.vehdjk.com/Article/details/gwnpkvymu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.bbcook.cn/Article/details/gmwbxzroz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fktsv.cn/Article/details/gbvzbcoau.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/glnpsodjh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.bbcook.cn/Article/details/ghonxuvew.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gxspwiqnd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.yfazqb.com/Article/details/grhqqcjrw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gufhmapub.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gasvtkjir.sHtML

[E06] 替换子串
来源：http://www.m.share.yfazqb.com/Article/details/gdwdchpzy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/ghbddnaol.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.epnwcf.com/Article/details/gcjiwcvyi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gwxhaxgst.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gpdspbrxx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gfoozrype.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gujxmagne.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/guqdjmorv.sHtML


<!-- 参考信息 -->