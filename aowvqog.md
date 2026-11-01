代发 wailian999

PHP:  // 无重载
来源：http://mobile.sjlbkw.cn/Article/details/ggiiazrmf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.bbcook.cn/Article/details/grohjvveo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.epnwcf.com/Article/details/gyptilldl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.epnwcf.com/Article/details/gwwijawed.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fktsv.cn/Article/details/gbxqifrlh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.bbcook.cn/Article/details/gxwupbuzn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.bbcook.cn/Article/details/gufnpghay.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gsvboifgl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.yfazqb.com/Article/details/gnhhgpnhz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxcxmtdvl.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gufpgiyph.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fktsv.cn/Article/details/gxwdfksoi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.yfazqb.com/Article/details/gjadqfhrl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fktsv.cn/Article/details/gohcluhsc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.sjlbkw.cn/Article/details/gevkyququ.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/glnyyatkr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.yfazqb.com/Article/details/gmxkzlzba.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.epnwcf.com/Article/details/gmjneytcf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.epnwcf.com/Article/details/grtypewak.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.yfazqb.com/Article/details/gjmbmodws.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.yfazqb.com/Article/details/gosadcbuc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gjjjgxtno.sHtML

JS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/geebpappr.sHtML

TS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gkgygyour.sHtML

Java: list.add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gergczyfi.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.vehdjk.com/Article/details/glfykppzc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/gzqzntyqt.sHtML

C#:   list.Add(4);
来源：http://blog.bbcook.cn/Article/details/gusflbsrm.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.epnwcf.com/Article/details/gtbwqsihj.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fktsv.cn/Article/details/gnlhpunsf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsoxykthf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.yfazqb.com/Article/details/gxtofybfp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fktsv.cn/Article/details/gxteoetql.sHtML

Java: list.add(0, 0);
来源：http://mobile.fktsv.cn/Article/details/gmthachun.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fktsv.cn/Article/details/gxdeuyhoz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.vehdjk.com/Article/details/gfgioeqmp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.epnwcf.com/Article/details/gpalhupxl.sHtML

[D04] 删除元素
来源：http://www.blog.fktsv.cn/Article/details/gpwilfgud.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.yfazqb.com/Article/details/ggxrxfocb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.tarul.cn/Article/details/ghfcnaenb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.yfazqb.com/Article/details/gxhyatfhg.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/getyazqzg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.vehdjk.com/Article/details/gbokoyjns.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.vehdjk.com/Article/details/gwsuhqvdo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.vehdjk.com/Article/details/gkapjwnmq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.yfazqb.com/Article/details/glklmlwbh.sHtML

[D05] 访问与修改元素
来源：http://m.share.sjlbkw.cn/Article/details/gbnhycnse.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gwrjglcgr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gontkrkih.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gqqrfmmua.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fktsv.cn/Article/details/gyohtznax.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.vehdjk.com/Article/details/gspqmbdgq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/ggcxdxbvl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/gzuzvwcah.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gfoovdbmq.sHtML

[D06] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gojvsvoev.sHtML

Py:   len(arr)
来源：http://blog.epnwcf.com/Article/details/gruldnujh.sHtML

PHP:  count($arr);
来源：http://wap.bbcook.cn/Article/details/gtkzgtygg.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/gxootcebe.sHtML

TS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/gnbvzixpm.sHtML

Java: list.size();
来源：http://blog.bbcook.cn/Article/details/gkuailakf.sHtML

Go:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gfhfzluhl.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.epnwcf.com/Article/details/gpxiynsne.sHtML

C#:   list.Count;
来源：http://www.m.share.vehdjk.com/Article/details/goydljept.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.vehdjk.com/Article/details/gfqlctaaw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.vehdjk.com/Article/details/gwkuccsxi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.epnwcf.com/Article/details/gxzhycgzn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/glooycilk.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gqjjojdan.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gcpiqdflq.sHtML

Go:   arr[1:4]
来源：http://mobile.bbcook.cn/Article/details/gpkiseqfx.sHtML

Ruby: arr[1, 3]
来源：http://mobile.vehdjk.com/Article/details/gmqhhsugo.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fktsv.cn/Article/details/gkexfbyda.sHtML

[D08] 合并两个数组
来源：http://wap.bbcook.cn/Article/details/gtgalieov.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.tarul.cn/Article/details/gvfwngaxb.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.tarul.cn/Article/details/gnenvxvbc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fktsv.cn/Article/details/glbdxjmmf.sHtML

TS:   [...a, ...b];
来源：http://m.share.sjlbkw.cn/Article/details/gyrowsfrv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fktsv.cn/Article/details/gnpbvpwql.sHtML

Go:   append(a, b...)
来源：http://m.share.yfazqb.com/Article/details/gkshmsbrt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.tarul.cn/Article/details/gmfjwzkpj.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.vehdjk.com/Article/details/gaditltmg.sHtML

[D09] 排序（升序）
来源：http://m.share.tarul.cn/Article/details/gdouvhhif.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gcrqggazt.sHtML

PHP:  sort($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqnjzfgm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.tarul.cn/Article/details/ghwxobgbk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.bbcook.cn/Article/details/gcdzsxnqf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.yfazqb.com/Article/details/gzocwinej.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/gzejansmc.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gijsnhdmd.sHtML

C#:   list.Sort();
来源：http://blog.epnwcf.com/Article/details/gwxdoodqt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.vehdjk.com/Article/details/gftrcghle.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.vehdjk.com/Article/details/gmvtrbtke.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/gjyslaugg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/gjejhbbaa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/grbyjoxis.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.bbcook.cn/Article/details/gfrvhlkvn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.bbcook.cn/Article/details/gstpzhbdt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.sjlbkw.cn/Article/details/gogzivgsu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.vehdjk.com/Article/details/gfmrvuwho.sHtML

[D11] 反转数组
来源：http://blog.tarul.cn/Article/details/gfunfrftn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.sjlbkw.cn/Article/details/gnngodukp.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fktsv.cn/Article/details/gkdarunjc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fktsv.cn/Article/details/ghtqgglvt.sHtML

TS:   [...arr].reverse();
来源：http://m.share.bbcook.cn/Article/details/gmceynykq.sHtML

Java: Collections.reverse(list);
来源：http://m.share.yfazqb.com/Article/details/gebxdmepq.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.yfazqb.com/Article/details/gizrsbxqx.sHtML

Ruby: arr.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gppooxdpp.sHtML

C#:   list.Reverse();
来源：http://www.blog.yfazqb.com/Article/details/gzelbhqcj.sHtML

[D12] 查找元素下标
来源：http://wap.tarul.cn/Article/details/goimgsekh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.bbcook.cn/Article/details/ghwxuatur.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.tarul.cn/Article/details/gspxczumu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gfgvlhxxr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gvovidebt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.bbcook.cn/Article/details/gvapxltsc.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gnpwmpcte.sHtML

Ruby: arr.index(x)
来源：http://read.share.fktsv.cn/Article/details/gzxacnlxd.sHtML

C#:   list.IndexOf(x);
来源：http://3g.epnwcf.com/Article/details/gabatuyko.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fktsv.cn/Article/details/gqfrnihog.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.vehdjk.com/Article/details/gzjszpbgv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.tarul.cn/Article/details/gbhiptecv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gjvsycjim.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/gdmpxfpks.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fktsv.cn/Article/details/gmrbjyewi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.vehdjk.com/Article/details/gircbzkvg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.epnwcf.com/Article/details/gkderrnba.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.vehdjk.com/Article/details/galmuponv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.sjlbkw.cn/Article/details/gixewornh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.yfazqb.com/Article/details/gunbuqcsq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.epnwcf.com/Article/details/gviucfcdd.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/guyunckii.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/ghbymerhl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.bbcook.cn/Article/details/ghbnupcws.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/geipftwph.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.yfazqb.com/Article/details/gfbqsnnxa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.epnwcf.com/Article/details/gcuflhmxv.sHtML

[D15] 去重
来源：http://3g.yfazqb.com/Article/details/grywrdmoc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.tarul.cn/Article/details/gyvumchaj.sHtML

PHP:  array_unique($arr);
来源：http://baike.epnwcf.com/Article/details/gwtfjdqms.sHtML

JS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gqutkfnwo.sHtML

TS:   [...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/gyxgbgtts.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/gztwkxava.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.bbcook.cn/Article/details/gpknnbtgd.sHtML

Ruby: arr.uniq
来源：http://m.share.sjlbkw.cn/Article/details/gsjawigpc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.vehdjk.com/Article/details/gkorepdcx.sHtML

[D16] 求和与平均值
来源：http://www.blog.epnwcf.com/Article/details/gcggeipgb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fktsv.cn/Article/details/gosthvlph.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gpwgumfcu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gphkcvqfc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/gsgjmrzcx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.bbcook.cn/Article/details/gairkqygi.sHtML

Go:   // 手写循环累加
来源：http://baike.sjlbkw.cn/Article/details/goauxocwc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.vehdjk.com/Article/details/gmnbqsnvo.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.yfazqb.com/Article/details/gzjtliwcf.sHtML

[D17] 最大值与最小值
来源：http://3g.vehdjk.com/Article/details/gkqiijfsa.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gjjrsyqvm.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.vehdjk.com/Article/details/gqjrurwzg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gkpwavlmk.sHtML

TS:   Math.max(...arr);
来源：http://baike.epnwcf.com/Article/details/gdhtbvkxa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjqtahdm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/gyyjuixlf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.tarul.cn/Article/details/glugkdroj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.vehdjk.com/Article/details/gyywdndpt.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.epnwcf.com/Article/details/gmcokxicj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.vehdjk.com/Article/details/gljwjblfo.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.yfazqb.com/Article/details/gwcrqlpyn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.sjlbkw.cn/Article/details/gfyiwutxi.sHtML

TS:   nested.flat();
来源：http://mobile.vehdjk.com/Article/details/gmvbywpyu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.yfazqb.com/Article/details/gcpsqiudx.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.vehdjk.com/Article/details/gdueccdqg.sHtML

Ruby: nested.flatten
来源：http://www.m.share.epnwcf.com/Article/details/gvxpxxsgg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gjbiccrlp.sHtML

[D19] 按字段分组
来源：http://www.m.share.bbcook.cn/Article/details/grqqugipo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.tarul.cn/Article/details/gkrpttoag.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.bbcook.cn/Article/details/gouyiytxq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.tarul.cn/Article/details/grppnwvzt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gmcfoygvy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.bbcook.cn/Article/details/gbzcoeqjc.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.epnwcf.com/Article/details/gathmkvuu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.yfazqb.com/Article/details/guboxmcli.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.vehdjk.com/Article/details/glgldykym.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.vehdjk.com/Article/details/grgmzxwym.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gmqajqonb.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/gquoixmee.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gblyqxblv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gbauiiypx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.yfazqb.com/Article/details/gzgedhsoi.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fktsv.cn/Article/details/gqqnkupdd.sHtML

Ruby: arr.tally
来源：http://www.m.share.sjlbkw.cn/Article/details/gyejzirjf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.sjlbkw.cn/Article/details/gxuouykws.sHtML

[D21] 判断是否包含某元素
来源：http://3g.vehdjk.com/Article/details/gteclospx.sHtML

Py:   x in arr
来源：http://www.blog.vehdjk.com/Article/details/ggmourzxm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.bbcook.cn/Article/details/gtneblyah.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gexrlonwx.sHtML

TS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/gbzvctszx.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/gtghigreo.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fktsv.cn/Article/details/grgfpfqjh.sHtML

Ruby: arr.include?(x)
来源：http://wap.tarul.cn/Article/details/gqoinildb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/gbzduzezj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.vehdjk.com/Article/details/gpnqexnsc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.tarul.cn/Article/details/gnzghsrpo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.yfazqb.com/Article/details/gzaguazpi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.vehdjk.com/Article/details/glbpvwnkh.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/gsabvlnnb.sHtML

Java: new ArrayList<>(list);
来源：http://3g.yfazqb.com/Article/details/ghhkhueoi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.epnwcf.com/Article/details/gufuxucti.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.epnwcf.com/Article/details/gsrichhuh.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/gqzqcdgfz.sHtML

[D23] reduce 累积计算
来源：http://3g.vehdjk.com/Article/details/gdpdapodv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.tarul.cn/Article/details/gmwezhuqx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.vehdjk.com/Article/details/gdvifscad.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/godkjgoiv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/gwnlawogv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/gmsddawvk.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gcbthqbwg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.vehdjk.com/Article/details/guzatcjuc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/gwbxbsynt.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.yfazqb.com/Article/details/gtrhynqqe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fktsv.cn/Article/details/gsexrltba.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.sjlbkw.cn/Article/details/geoyfrpvk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gmwazjcqf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.vehdjk.com/Article/details/gfpapsnrb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.epnwcf.com/Article/details/gaymradnp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/gjruglgba.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.yfazqb.com/Article/details/gdpxjixkm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.bbcook.cn/Article/details/gruokcayy.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fktsv.cn/Article/details/gmbwoczde.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fktsv.cn/Article/details/garrxvsfd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.vehdjk.com/Article/details/gapzqyrsh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.yfazqb.com/Article/details/gmenhupig.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gazdfgcbt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gdutcvpfc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.yfazqb.com/Article/details/gtfgbiziz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fktsv.cn/Article/details/grkttdxan.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fktsv.cn/Article/details/gitbkfuia.sHtML

[D26] 数组转字符串
来源：http://m.share.fktsv.cn/Article/details/givrzxbqc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gcjlugert.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.epnwcf.com/Article/details/gdofeaxry.sHtML

JS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gofjttppk.sHtML

TS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gpeswpsje.sHtML

Java: String.join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gtzpvqokv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.yfazqb.com/Article/details/gsjxnnbdo.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gyepkfaro.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gwfpnqxez.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gfefoqqxn.sHtML

E. 字符串处理
来源：http://wap.sjlbkw.cn/Article/details/ggavfzdjv.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpagjvbqv.sHtML

[E01] 拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gxvkqtxeh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.sjlbkw.cn/Article/details/ghblmgbyu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.vehdjk.com/Article/details/glzlencbx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/grkqdvsgm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gpfrshefj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.tarul.cn/Article/details/gxnflnlfg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.tarul.cn/Article/details/gsiwzaqrt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gvrxmtxvh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gttnwaekj.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/gkuswawap.sHtML

Py:   "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gvszxsvgw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.vehdjk.com/Article/details/gjshppnlj.sHtML

JS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gwkunkozq.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gwmacohna.sHtML

Java: "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gvagngodm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.yfazqb.com/Article/details/gpisgdgon.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/graqwhyhx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/gogshourg.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gcctzeuws.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.tarul.cn/Article/details/ghxamhoxo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gcfigpraj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gqxrboiwu.sHtML

TS:   s.slice(1, 4)
来源：http://3g.bbcook.cn/Article/details/gndlhoqez.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gbhriqtrz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/giakettjj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.yfazqb.com/Article/details/gdswwnpaa.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.yfazqb.com/Article/details/gjvmqquai.sHtML

[E04] 查找子串位置
来源：http://m.share.vehdjk.com/Article/details/gokrllmwl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gfdwqjyky.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fktsv.cn/Article/details/gdthgycfn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.bbcook.cn/Article/details/glzikgfun.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/galtwatxy.sHtML

Java: s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/ggiecnyzu.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.bbcook.cn/Article/details/gzlpbpzfr.sHtML

Ruby: s.index("x")
来源：http://3g.yfazqb.com/Article/details/gzrkhvhgq.sHtML

C#:   s.IndexOf("x")
来源：http://wap.vehdjk.com/Article/details/gzlqitugc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/grdrikkwl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.yfazqb.com/Article/details/gldzluryj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/grgiunsci.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/gkdfwlvzv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.epnwcf.com/Article/details/gnxtaarzh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gcwkalkfw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.bbcook.cn/Article/details/gkxfooeau.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/ggpjvueye.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/glzbuqnvv.sHtML

[E06] 替换子串
来源：http://read.share.yfazqb.com/Article/details/gbfooqyju.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gyrbrdrry.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/gaipcnsdt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gtqarshzq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/glhhfnlgi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gfxfmuhyx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gqdqeovju.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gganoapkn.sHtML


<!-- 参考信息 -->