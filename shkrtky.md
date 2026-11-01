代发 wailian999

Ruby: a, b = pair
来源：http://3g.tarul.cn/Article/details/gfscdbowx.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.yfazqb.com/Article/details/gqxqlecgu.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.tarul.cn/Article/details/gbknjupox.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.bbcook.cn/Article/details/gwyyenppl.sHtML

PHP:  // 无重载
来源：http://3g.epnwcf.com/Article/details/gznmwougw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.vehdjk.com/Article/details/ggrptlqth.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.epnwcf.com/Article/details/gahucurrn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fktsv.cn/Article/details/gpcbmhsnd.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.bbcook.cn/Article/details/gipjnyuyy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.yfazqb.com/Article/details/gzahrxwhp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.vehdjk.com/Article/details/grecipotq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmqvlzbvf.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.tarul.cn/Article/details/gdvqtvrka.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjzbnwyoi.sHtML

[D01] 创建数组 / 列表
来源：http://baike.sjlbkw.cn/Article/details/gkzvhyozy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fktsv.cn/Article/details/gmmopqfvn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.bbcook.cn/Article/details/gibxucbkk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.bbcook.cn/Article/details/gwpnpemca.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.bbcook.cn/Article/details/geditiign.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fktsv.cn/Article/details/gmlheuind.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.epnwcf.com/Article/details/gfkjfdrxh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.vehdjk.com/Article/details/gmclqatrq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.bbcook.cn/Article/details/gvtmkuwci.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fktsv.cn/Article/details/gcetsoiim.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.sjlbkw.cn/Article/details/ggchckeih.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/gbhrghnbq.sHtML

JS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gguovbjee.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gxgbktqma.sHtML

Java: list.add(4);
来源：http://blog.vehdjk.com/Article/details/gaoseyvtp.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.yfazqb.com/Article/details/gqwkrmpvh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.vehdjk.com/Article/details/giiiodpar.sHtML

C#:   list.Add(4);
来源：http://wap.fktsv.cn/Article/details/gledsdlot.sHtML

[D03] 在指定位置插入元素
来源：http://3g.sjlbkw.cn/Article/details/giwjksqgq.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.yfazqb.com/Article/details/gsnyiasqt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/gifxruvxq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fktsv.cn/Article/details/gzpncglix.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtaugejzt.sHtML

Java: list.add(0, 0);
来源：http://read.share.bbcook.cn/Article/details/germqlmgc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.epnwcf.com/Article/details/gjkzzrejp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.tarul.cn/Article/details/gkrwomnxg.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fktsv.cn/Article/details/gwyipgaxz.sHtML

[D04] 删除元素
来源：http://www.m.share.bbcook.cn/Article/details/gogprubie.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fktsv.cn/Article/details/gomctqnuc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gumxdbnkt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.bbcook.cn/Article/details/gwuusvbwn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.tarul.cn/Article/details/guwmktnfy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.tarul.cn/Article/details/gogtsxlsh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fktsv.cn/Article/details/govapwxid.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fktsv.cn/Article/details/gsrscyqen.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fktsv.cn/Article/details/ggaklhsel.sHtML

[D05] 访问与修改元素
来源：http://baike.vehdjk.com/Article/details/gxkdekrbl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gbdtllkvz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/ghzytuuiv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gsaaerxxd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fktsv.cn/Article/details/glaaybaac.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.epnwcf.com/Article/details/gptesgapi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gpuyhqrwh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gjpoevqzx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gryrcxbro.sHtML

[D06] 数组长度
来源：http://3g.epnwcf.com/Article/details/gmlzfogch.sHtML

Py:   len(arr)
来源：http://read.share.tarul.cn/Article/details/gpnypvuvo.sHtML

PHP:  count($arr);
来源：http://www.blog.yfazqb.com/Article/details/gavcoxrhz.sHtML

JS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gcmulivuc.sHtML

TS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/gahpbmsov.sHtML

Java: list.size();
来源：http://mobile.tarul.cn/Article/details/gmwhqzptm.sHtML

Go:   len(arr)
来源：http://baike.epnwcf.com/Article/details/goqhriufv.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fktsv.cn/Article/details/gdycciqql.sHtML

C#:   list.Count;
来源：http://blog.tarul.cn/Article/details/gopsarhob.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.yfazqb.com/Article/details/gzragfgem.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/gzhcduske.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/gpssndxil.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gtznrlsxu.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/ggnlmksda.sHtML

Java: list.subList(1, 4);
来源：http://3g.fktsv.cn/Article/details/gyoexeela.sHtML

Go:   arr[1:4]
来源：http://3g.epnwcf.com/Article/details/gmyzzlvul.sHtML

Ruby: arr[1, 3]
来源：http://blog.epnwcf.com/Article/details/gvuihukeq.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.bbcook.cn/Article/details/gfndlqiyy.sHtML

[D08] 合并两个数组
来源：http://www.share.fktsv.cn/Article/details/gjxlcxwyy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fktsv.cn/Article/details/gwqzumfcd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.epnwcf.com/Article/details/gitdkszdx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fktsv.cn/Article/details/gtqorpfzz.sHtML

TS:   [...a, ...b];
来源：http://www.share.epnwcf.com/Article/details/groqandgh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fktsv.cn/Article/details/gurdhebcu.sHtML

Go:   append(a, b...)
来源：http://wap.bbcook.cn/Article/details/gylfjhpjh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.yfazqb.com/Article/details/gftkdzguq.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/govnwdvbs.sHtML

[D09] 排序（升序）
来源：http://wap.epnwcf.com/Article/details/goxawvcac.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/guoaqufts.sHtML

PHP:  sort($arr);
来源：http://read.share.epnwcf.com/Article/details/gsxopvekn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.vehdjk.com/Article/details/gbvdobhef.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.sjlbkw.cn/Article/details/gjnmsosox.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.tarul.cn/Article/details/gfeqvfwxe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gkbbtgarm.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gkejvzred.sHtML

C#:   list.Sort();
来源：http://www.blog.sjlbkw.cn/Article/details/goapkjgym.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhkwhggr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.bbcook.cn/Article/details/gmtndvqtq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gbxgadpqr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gqexjlfuk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fktsv.cn/Article/details/gnnqchfok.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fktsv.cn/Article/details/gcugohutk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.sjlbkw.cn/Article/details/geukasynr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.yfazqb.com/Article/details/ghdxzdmsz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.bbcook.cn/Article/details/gzaijzqjb.sHtML

[D11] 反转数组
来源：http://wap.tarul.cn/Article/details/gldacukyh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.vehdjk.com/Article/details/gsmseoktu.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.yfazqb.com/Article/details/gcqxufylq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.vehdjk.com/Article/details/gtczmylnd.sHtML

TS:   [...arr].reverse();
来源：http://wap.sjlbkw.cn/Article/details/gfinlnxwt.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/ghjexwoxr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.epnwcf.com/Article/details/glcznrfnq.sHtML

Ruby: arr.reverse
来源：http://blog.sjlbkw.cn/Article/details/gboilzodf.sHtML

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/geeistwuf.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/guxnssemf.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.epnwcf.com/Article/details/grcpocxqn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.vehdjk.com/Article/details/gqlwkvihl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/gzrjjpoys.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.sjlbkw.cn/Article/details/gglndtgof.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.tarul.cn/Article/details/gckucpand.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gdefabjeh.sHtML

Ruby: arr.index(x)
来源：http://www.blog.tarul.cn/Article/details/gdptiirrr.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.vehdjk.com/Article/details/gskblgxcp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.epnwcf.com/Article/details/gkjzaodrt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/gqlmpcsqz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.bbcook.cn/Article/details/gdoqmtyki.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fktsv.cn/Article/details/gnhjhqwyu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/geomhgssh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/gvbjuvjlt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.yfazqb.com/Article/details/gxoyzfsyl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.vehdjk.com/Article/details/grziaqqvt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gyzjcbfeg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.tarul.cn/Article/details/gzgyxvwta.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gyidprase.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.vehdjk.com/Article/details/geqbvacbz.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gfrztxcpd.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.vehdjk.com/Article/details/gtanvampy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.tarul.cn/Article/details/grsqbynuu.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/gpobbtwqm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fktsv.cn/Article/details/gynrpntmq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gmucocjug.sHtML

[D15] 去重
来源：http://wap.yfazqb.com/Article/details/glijbvwux.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/gerexkstu.sHtML

PHP:  array_unique($arr);
来源：http://3g.sjlbkw.cn/Article/details/gjtwbqjkz.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gisnoqpzf.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/grduydkdi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.bbcook.cn/Article/details/gtxzelkpc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.epnwcf.com/Article/details/gnpthsdmx.sHtML

Ruby: arr.uniq
来源：http://m.share.sjlbkw.cn/Article/details/ghvuhcdsx.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fktsv.cn/Article/details/gmatdlqbb.sHtML

[D16] 求和与平均值
来源：http://www.blog.yfazqb.com/Article/details/gknvdeumu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.epnwcf.com/Article/details/gufrbvyik.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/grevidxzn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/gmipvptcd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gozcmwvhv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/gfmfohibo.sHtML

Go:   // 手写循环累加
来源：http://mobile.fktsv.cn/Article/details/gflvwpxqg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.epnwcf.com/Article/details/gmtkmgrwp.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.epnwcf.com/Article/details/gpxwpcjjw.sHtML

[D17] 最大值与最小值
来源：http://baike.tarul.cn/Article/details/gcudlmxwo.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.bbcook.cn/Article/details/ggntfrifm.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gpndvvegm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.vehdjk.com/Article/details/gibtwmgfc.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.tarul.cn/Article/details/gnauaihcc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.vehdjk.com/Article/details/gbxvdoymo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gcwaqrcem.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.yfazqb.com/Article/details/ggoxhbadc.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.bbcook.cn/Article/details/golpqtjrc.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.sjlbkw.cn/Article/details/gexiqaxyc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fktsv.cn/Article/details/ggpdgwkzq.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gxmyyvryg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fktsv.cn/Article/details/gaijqbuiy.sHtML

TS:   nested.flat();
来源：http://wap.tarul.cn/Article/details/gpswevugk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.bbcook.cn/Article/details/grikgsmtu.sHtML

Go:   // 手写双层循环
来源：http://baike.sjlbkw.cn/Article/details/gkyobcqvf.sHtML

Ruby: nested.flatten
来源：http://mobile.vehdjk.com/Article/details/gzytsxxsh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gvpjgzfux.sHtML

[D19] 按字段分组
来源：http://mobile.sjlbkw.cn/Article/details/gfuljpnoq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.yfazqb.com/Article/details/gvpdkpehr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.bbcook.cn/Article/details/gcikswglv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fktsv.cn/Article/details/grcjwaihm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/ggppdtqne.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.yfazqb.com/Article/details/grslpjfav.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/ghcnybiiq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.bbcook.cn/Article/details/gorygqfon.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.vehdjk.com/Article/details/gjabmtfxw.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.epnwcf.com/Article/details/gmmtskgcj.sHtML

Py:   Counter(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gqblxjqhh.sHtML

PHP:  array_count_values($arr);
来源：http://baike.sjlbkw.cn/Article/details/gfffdqxbv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gitzrxiwx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gejatecqk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.yfazqb.com/Article/details/gerkcaodu.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.epnwcf.com/Article/details/gzcqiblcc.sHtML

Ruby: arr.tally
来源：http://mobile.vehdjk.com/Article/details/gabgkekwd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.bbcook.cn/Article/details/gyyvubzvu.sHtML

[D21] 判断是否包含某元素
来源：http://blog.tarul.cn/Article/details/gdxruslpd.sHtML

Py:   x in arr
来源：http://read.share.yfazqb.com/Article/details/gwzqpsisa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.vehdjk.com/Article/details/gjbevzfwh.sHtML

JS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gnztjstui.sHtML

TS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/gtqnejmwc.sHtML

Java: list.contains(x)
来源：http://baike.vehdjk.com/Article/details/gvvuyfzze.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gmqwkebgw.sHtML

Ruby: arr.include?(x)
来源：http://baike.vehdjk.com/Article/details/gdmmvgqdp.sHtML

C#:   list.Contains(x)
来源：http://baike.yfazqb.com/Article/details/gpcbrbues.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.tarul.cn/Article/details/gukskazoo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.epnwcf.com/Article/details/gecbswtvs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.epnwcf.com/Article/details/gauaquvny.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gokqkcnna.sHtML

TS:   [...arr];
来源：http://www.blog.fktsv.cn/Article/details/grthvwcan.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.yfazqb.com/Article/details/guwpgnvyw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.vehdjk.com/Article/details/ghgiujokd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/gsscokvdg.sHtML

C#:   new List<int>(list);
来源：http://3g.sjlbkw.cn/Article/details/gmnoisqxe.sHtML

[D23] reduce 累积计算
来源：http://blog.yfazqb.com/Article/details/gufrwzazg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.yfazqb.com/Article/details/gtpjkbynv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gjlipahod.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.epnwcf.com/Article/details/gsrzxyodk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gypwtlble.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.epnwcf.com/Article/details/gokcpnxre.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/grsnjrpfn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.yfazqb.com/Article/details/gglzfzpki.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/gksrfujae.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.bbcook.cn/Article/details/ghilmconp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gaikpcqri.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.yfazqb.com/Article/details/gblwpphse.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.epnwcf.com/Article/details/gnpeqxxye.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gjcmkoxhr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.epnwcf.com/Article/details/gfnzdsmbg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.tarul.cn/Article/details/gtjpzfggt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.bbcook.cn/Article/details/gklcqpagm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.bbcook.cn/Article/details/govjbhozu.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/gvssjpchu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.tarul.cn/Article/details/gjnqeabjy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.bbcook.cn/Article/details/gfdizrijk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gyzvemnxm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.epnwcf.com/Article/details/gxgvrfhfd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/gzzwughyg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.bbcook.cn/Article/details/gluywxvow.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.vehdjk.com/Article/details/gkmvmtbut.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.vehdjk.com/Article/details/gxzgalbdv.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gepweawje.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.vehdjk.com/Article/details/ggktlpjip.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.vehdjk.com/Article/details/gouenkwfs.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gbwoptzqg.sHtML

TS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gitpykdtb.sHtML

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/ghbzipvkx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.tarul.cn/Article/details/grnbtqlbp.sHtML

Ruby: arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gplyzyonj.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/goscohuep.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ggxflkanu.sHtML

E. 字符串处理
来源：http://3g.fktsv.cn/Article/details/gajatiydf.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvvwbqmqg.sHtML

[E01] 拼接字符串
来源：http://blog.epnwcf.com/Article/details/gudbicagz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gsimddlse.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.epnwcf.com/Article/details/gsppewxhs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/gseqckleq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/glayoqfhx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.yfazqb.com/Article/details/gjuvckmdr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.vehdjk.com/Article/details/gifkveqpy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.epnwcf.com/Article/details/gxmvmgqlh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gwxwtozdv.sHtML

[E02] 重复字符串
来源：http://m.share.tarul.cn/Article/details/gnyqzyjmt.sHtML

Py:   "ab" * 3
来源：http://baike.tarul.cn/Article/details/gdtxazxsw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.sjlbkw.cn/Article/details/gnnixhzah.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/guqewmekv.sHtML

TS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gspixibbu.sHtML

Java: "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gfidphwdu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.sjlbkw.cn/Article/details/geyuvisev.sHtML

Ruby: "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gglryvkgm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.bbcook.cn/Article/details/gxuecmdmx.sHtML

[E03] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/ggregwwuj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gffjxdnkd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gshmpaxec.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gcumfhkxa.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gcmigpynu.sHtML

Java: s.substring(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gxqidvowf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gypytaxwh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.tarul.cn/Article/details/gvkmnxize.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.bbcook.cn/Article/details/guoyxutrb.sHtML

[E04] 查找子串位置
来源：http://www.m.share.tarul.cn/Article/details/gfizajusm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/grumphniu.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.tarul.cn/Article/details/gqenhifur.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.vehdjk.com/Article/details/gwuipnywx.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gjwmaygna.sHtML

Java: s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/ghvthyigh.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.bbcook.cn/Article/details/gmxjdslln.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gkxdmmfso.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/ggaohwgyl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/gmvbmsltm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.bbcook.cn/Article/details/gxqrpegiw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.sjlbkw.cn/Article/details/gbhnsayjy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gxntqfzgk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.vehdjk.com/Article/details/gokwgnnll.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gcwqlvwoy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.epnwcf.com/Article/details/gcvggokud.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.yfazqb.com/Article/details/gpdwpjact.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.epnwcf.com/Article/details/guzfdjspm.sHtML

[E06] 替换子串
来源：http://m.share.fktsv.cn/Article/details/gzxvmoqpu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/gzafulldu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/gzxaasvhh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gkxmahlbx.sHtML


<!-- 参考信息 -->