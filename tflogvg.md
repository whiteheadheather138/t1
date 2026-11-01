代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.yfazqb.com/Article/details/goosqbgur.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.vehdjk.com/Article/details/ghlswerps.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/guvfjbvrg.sHtML

Ruby: # 无泛型
来源：http://mobile.fktsv.cn/Article/details/gxalnklxm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/gjxomkzpm.sHtML

[C15] 解构 / 展开参数
来源：http://3g.epnwcf.com/Article/details/gdazjudod.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.sjlbkw.cn/Article/details/glnoiuzux.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.sjlbkw.cn/Article/details/gxxggtqmu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.vehdjk.com/Article/details/gwtmsskst.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/gthaqfwrj.sHtML

Java: // 无解构
来源：http://m.share.epnwcf.com/Article/details/gubpacnxo.sHtML

Go:   // 无解构
来源：http://3g.vehdjk.com/Article/details/gxjeolrwo.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/guchzoqdf.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.yfazqb.com/Article/details/gcmiwmotx.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.vehdjk.com/Article/details/geefvyepz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fktsv.cn/Article/details/gizhfhuza.sHtML

PHP:  // 无重载
来源：http://3g.tarul.cn/Article/details/gtezkppyj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.bbcook.cn/Article/details/gvncirofp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.vehdjk.com/Article/details/gxsblpmrx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fktsv.cn/Article/details/goqxawlwy.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fktsv.cn/Article/details/glvtirvzc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fktsv.cn/Article/details/groublugk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.tarul.cn/Article/details/grjvhxamz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxwcybeen.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.bbcook.cn/Article/details/ggzcfckzv.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbwcjorsz.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.epnwcf.com/Article/details/gelkansca.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/gnvzogakq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fktsv.cn/Article/details/gqflozutj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.yfazqb.com/Article/details/gvbslpiil.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fktsv.cn/Article/details/gxyztzfxt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.bbcook.cn/Article/details/gbhylupwx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.tarul.cn/Article/details/gnhdoomyv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.tarul.cn/Article/details/gqlkltjoi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.epnwcf.com/Article/details/gfnyawbay.sHtML

[D02] 追加元素到末尾
来源：http://wap.tarul.cn/Article/details/gmhitjxxb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fktsv.cn/Article/details/ghlsgrijb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.tarul.cn/Article/details/gosyxyyxp.sHtML

JS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/gtgwtqlar.sHtML

TS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/grpbdlgml.sHtML

Java: list.add(4);
来源：http://www.m.share.bbcook.cn/Article/details/gboymuivu.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.yfazqb.com/Article/details/gknruftng.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.tarul.cn/Article/details/gngctqmut.sHtML

C#:   list.Add(4);
来源：http://m.share.yfazqb.com/Article/details/gxemewurm.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.vehdjk.com/Article/details/gdlmspmje.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.epnwcf.com/Article/details/gfalogdww.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.vehdjk.com/Article/details/gdktkvuoj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.epnwcf.com/Article/details/gkcedzgdz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.yfazqb.com/Article/details/gtwvyrykk.sHtML

Java: list.add(0, 0);
来源：http://baike.vehdjk.com/Article/details/gfymkcciv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fktsv.cn/Article/details/gcvzbtygx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.sjlbkw.cn/Article/details/glcaqpztp.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gzrcvrryw.sHtML

[D04] 删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gksaansha.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.yfazqb.com/Article/details/gxvvxwzoz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.epnwcf.com/Article/details/gzuupbohj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.vehdjk.com/Article/details/gkjbuojlw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gwuqaljhd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.tarul.cn/Article/details/gbwotzloc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.epnwcf.com/Article/details/grmxjnunk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fktsv.cn/Article/details/gjqhdwcya.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.epnwcf.com/Article/details/gwzqlmbrw.sHtML

[D05] 访问与修改元素
来源：http://blog.epnwcf.com/Article/details/gqzzfwfly.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/ghxabwuif.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gpirvlylf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gsdvcghgu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fktsv.cn/Article/details/gcaswrrhn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.yfazqb.com/Article/details/gzwjvlhqe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gzxtpkgof.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gepxaioxw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gjfcjjefg.sHtML

[D06] 数组长度
来源：http://blog.sjlbkw.cn/Article/details/gweunzdfv.sHtML

Py:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gccfkxffa.sHtML

PHP:  count($arr);
来源：http://wap.yfazqb.com/Article/details/gtbhxqfir.sHtML

JS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gwlchfbje.sHtML

TS:   arr.length
来源：http://3g.yfazqb.com/Article/details/gygmssorn.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/gczaxpnni.sHtML

Go:   len(arr)
来源：http://3g.yfazqb.com/Article/details/gmmbcgqot.sHtML

Ruby: arr.length; arr.size
来源：http://blog.sjlbkw.cn/Article/details/gghzkwlcb.sHtML

C#:   list.Count;
来源：http://wap.bbcook.cn/Article/details/gkjeacvfd.sHtML

[D07] 切片 / 取子数组
来源：http://wap.bbcook.cn/Article/details/goajvyspt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.yfazqb.com/Article/details/gcvynlfrn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/gigzqqtux.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gamdulixm.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/grdmfsota.sHtML

Java: list.subList(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gejhmborn.sHtML

Go:   arr[1:4]
来源：http://baike.yfazqb.com/Article/details/gfmdrwwjj.sHtML

Ruby: arr[1, 3]
来源：http://baike.epnwcf.com/Article/details/gnekkfomg.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gspffmqgn.sHtML

[D08] 合并两个数组
来源：http://wap.epnwcf.com/Article/details/gdbkhwkay.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.epnwcf.com/Article/details/gvgaoyamz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.tarul.cn/Article/details/gxzzxekmd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.tarul.cn/Article/details/gkryxkjxi.sHtML

TS:   [...a, ...b];
来源：http://www.share.bbcook.cn/Article/details/ggacefcyk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.epnwcf.com/Article/details/galzfobfx.sHtML

Go:   append(a, b...)
来源：http://read.share.tarul.cn/Article/details/gwlrrlnmb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.tarul.cn/Article/details/gjgpklwhg.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/gknbsqlcx.sHtML

[D09] 排序（升序）
来源：http://mobile.sjlbkw.cn/Article/details/gvffggzil.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gnclroanw.sHtML

PHP:  sort($arr);
来源：http://m.share.tarul.cn/Article/details/gnatbjltm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.tarul.cn/Article/details/geybeskrv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.epnwcf.com/Article/details/gzbvafhss.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.bbcook.cn/Article/details/gmkdneuih.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnvoecns.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/glcscnffa.sHtML

C#:   list.Sort();
来源：http://www.blog.sjlbkw.cn/Article/details/ghrvwjdal.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.epnwcf.com/Article/details/gtadoumch.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fktsv.cn/Article/details/gkfhhzkzv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.bbcook.cn/Article/details/gvevyjkda.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.sjlbkw.cn/Article/details/gpkwbcrob.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/gchjylinp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.tarul.cn/Article/details/gtrqbqmbu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.sjlbkw.cn/Article/details/griozjukc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.vehdjk.com/Article/details/gvsozhlct.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.epnwcf.com/Article/details/gugwmhfia.sHtML

[D11] 反转数组
来源：http://baike.sjlbkw.cn/Article/details/gboywsrix.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.sjlbkw.cn/Article/details/gbkabbzni.sHtML

PHP:  array_reverse($arr);
来源：http://baike.yfazqb.com/Article/details/gshmvyxvv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.tarul.cn/Article/details/gygzgekzf.sHtML

TS:   [...arr].reverse();
来源：http://blog.sjlbkw.cn/Article/details/galzxojib.sHtML

Java: Collections.reverse(list);
来源：http://m.share.tarul.cn/Article/details/gvpdxfuni.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.yfazqb.com/Article/details/gtqtdhill.sHtML

Ruby: arr.reverse
来源：http://mobile.bbcook.cn/Article/details/gbdqnliyv.sHtML

C#:   list.Reverse();
来源：http://3g.sjlbkw.cn/Article/details/ggcopxkhz.sHtML

[D12] 查找元素下标
来源：http://3g.yfazqb.com/Article/details/gdjujeqql.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/gmgupqzdy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.yfazqb.com/Article/details/giteckgmm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gnvjqixbk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.sjlbkw.cn/Article/details/gsamxjccp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fktsv.cn/Article/details/gktaaklea.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.tarul.cn/Article/details/gjtwxfrwz.sHtML

Ruby: arr.index(x)
来源：http://3g.bbcook.cn/Article/details/gydxjmjre.sHtML

C#:   list.IndexOf(x);
来源：http://baike.vehdjk.com/Article/details/gudaigsft.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.sjlbkw.cn/Article/details/gmfkteuwg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.epnwcf.com/Article/details/goodminkm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.bbcook.cn/Article/details/gqyiakwew.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gdtpsqshl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gepqxedwh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.epnwcf.com/Article/details/gnjyjlbzj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.epnwcf.com/Article/details/gwibkudnf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.vehdjk.com/Article/details/gxfkpfedf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.yfazqb.com/Article/details/gvbdxjzlk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gvclbgakv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.tarul.cn/Article/details/gkwnbblci.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gohmvutyg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/glyfpadpy.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gjferixsn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gotvkndvv.sHtML

Go:   // 手写循环
来源：http://blog.yfazqb.com/Article/details/gzifcljfg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.bbcook.cn/Article/details/ggcacwjdc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fktsv.cn/Article/details/gngvhsian.sHtML

[D15] 去重
来源：http://read.share.vehdjk.com/Article/details/gsdauqjst.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.bbcook.cn/Article/details/gmsqkuzik.sHtML

PHP:  array_unique($arr);
来源：http://m.share.epnwcf.com/Article/details/gduwmvvjo.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gksjfqduh.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gllucapyn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.yfazqb.com/Article/details/gkxsguxgb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.vehdjk.com/Article/details/gtzkkhymb.sHtML

Ruby: arr.uniq
来源：http://read.share.bbcook.cn/Article/details/gtilxjsru.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.yfazqb.com/Article/details/gqaczkrzj.sHtML

[D16] 求和与平均值
来源：http://read.share.epnwcf.com/Article/details/gdcnyqucr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/gakwmaoho.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fktsv.cn/Article/details/gmsochiid.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gwvwjwssr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gtmdbxevz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.yfazqb.com/Article/details/gpoqbwlga.sHtML

Go:   // 手写循环累加
来源：http://read.share.epnwcf.com/Article/details/glpjkwewh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.vehdjk.com/Article/details/gpsghnjzj.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/glboxejmf.sHtML

[D17] 最大值与最小值
来源：http://baike.yfazqb.com/Article/details/givsdmcue.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/gafkhhzrq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fktsv.cn/Article/details/gjhwlbsgt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.vehdjk.com/Article/details/gycijvcsk.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.tarul.cn/Article/details/ghtmhxkmy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fktsv.cn/Article/details/gqnsujyrv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.vehdjk.com/Article/details/gebhdnbdy.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.sjlbkw.cn/Article/details/gemrkiaqm.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fktsv.cn/Article/details/ggrnasmhq.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.sjlbkw.cn/Article/details/gnwgktxev.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.yfazqb.com/Article/details/gwojxqbyz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.epnwcf.com/Article/details/guwctkqxv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fktsv.cn/Article/details/gsjyefchf.sHtML

TS:   nested.flat();
来源：http://read.share.vehdjk.com/Article/details/ghhmdxsvw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.yfazqb.com/Article/details/gvpjagecq.sHtML

Go:   // 手写双层循环
来源：http://mobile.epnwcf.com/Article/details/gjmztxmow.sHtML

Ruby: nested.flatten
来源：http://baike.sjlbkw.cn/Article/details/gzlgtxrkr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.tarul.cn/Article/details/gdyqbceal.sHtML

[D19] 按字段分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gwaqwuflw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.sjlbkw.cn/Article/details/gpyrjeean.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.bbcook.cn/Article/details/grfwanvom.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/gapxhjfsa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gbfpkbcjm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fktsv.cn/Article/details/gaoumtntv.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.yfazqb.com/Article/details/ghoezpsnq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.sjlbkw.cn/Article/details/ggyzecrht.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.bbcook.cn/Article/details/ghvpygsya.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.sjlbkw.cn/Article/details/ggmsrnbov.sHtML

Py:   Counter(arr)
来源：http://www.blog.fktsv.cn/Article/details/gljmvunsi.sHtML

PHP:  array_count_values($arr);
来源：http://blog.vehdjk.com/Article/details/ggpusjlds.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gtwlwfcwf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.bbcook.cn/Article/details/ghimfsivu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.vehdjk.com/Article/details/gyxnigzzu.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fktsv.cn/Article/details/giyuuzwjn.sHtML

Ruby: arr.tally
来源：http://read.share.bbcook.cn/Article/details/gxmtzbfpu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.yfazqb.com/Article/details/gjqvnzsyb.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.sjlbkw.cn/Article/details/godcukbsy.sHtML

Py:   x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gqyihczdp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.bbcook.cn/Article/details/giheqexzt.sHtML

JS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/gtphjbwov.sHtML

TS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gnyyrsgxf.sHtML

Java: list.contains(x)
来源：http://baike.bbcook.cn/Article/details/gfxcztwmg.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.yfazqb.com/Article/details/gltzcwqyu.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/gfcmjloyf.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gyrvpgolp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.epnwcf.com/Article/details/gbogqlwee.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhqsbcbf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/gjtadafxt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gmaaywgmj.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/gpxktduhd.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.tarul.cn/Article/details/ghsqtsbvt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.yfazqb.com/Article/details/gxapubzmp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fktsv.cn/Article/details/gsdyfxirl.sHtML

C#:   new List<int>(list);
来源：http://www.share.tarul.cn/Article/details/gjopxcdyo.sHtML

[D23] reduce 累积计算
来源：http://blog.sjlbkw.cn/Article/details/gzqnltiqt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.epnwcf.com/Article/details/gpadxbpas.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.epnwcf.com/Article/details/gnlfxikok.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gvbfwylag.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/glvediblg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.yfazqb.com/Article/details/gstlnraex.sHtML

Go:   // 手写循环
来源：http://www.m.share.bbcook.cn/Article/details/gceppedgt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.tarul.cn/Article/details/ggmfxuubx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.tarul.cn/Article/details/gqpbscodz.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.tarul.cn/Article/details/gbhbfstbz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fktsv.cn/Article/details/gauluoffj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fktsv.cn/Article/details/giefonggg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gpgtkxyhx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gqwnnymje.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.sjlbkw.cn/Article/details/gkmemkncn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fktsv.cn/Article/details/ghgzymrch.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.sjlbkw.cn/Article/details/gtxhehwkn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.yfazqb.com/Article/details/gkpsiphwb.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.sjlbkw.cn/Article/details/gendmqklf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.bbcook.cn/Article/details/gmiatbytj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.epnwcf.com/Article/details/gajhcqrdn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.yfazqb.com/Article/details/gtxnvdhub.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.vehdjk.com/Article/details/gtgvwosku.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gyylmkmps.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fktsv.cn/Article/details/guucahzxs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.vehdjk.com/Article/details/gaygvvijs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.vehdjk.com/Article/details/grkgkxvui.sHtML

[D26] 数组转字符串
来源：http://baike.vehdjk.com/Article/details/gohkeoxui.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fktsv.cn/Article/details/gmnigjdnp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.yfazqb.com/Article/details/gmvgyejal.sHtML

JS:   arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/glbcbolrv.sHtML

TS:   arr.join(", ")
来源：http://www.blog.bbcook.cn/Article/details/gddplepds.sHtML

Java: String.join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gmhdeabyp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.epnwcf.com/Article/details/gpaeifrgg.sHtML

Ruby: arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gpifgqhqz.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/gcwphbezh.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gyryxctzr.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gbjimlawd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/giyhepwpb.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/grluifels.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.bbcook.cn/Article/details/genpekigm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.epnwcf.com/Article/details/glwlvjcll.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gvmvuoiqc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.sjlbkw.cn/Article/details/gyoulfdxs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.epnwcf.com/Article/details/gwperpzoo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/gtjaacfvo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fktsv.cn/Article/details/giuaixkmn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.yfazqb.com/Article/details/gzbewanis.sHtML

[E02] 重复字符串
来源：http://m.share.bbcook.cn/Article/details/gnhtmnjmj.sHtML

Py:   "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gukoutjuu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.tarul.cn/Article/details/gvhkzqfpj.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gwnhzfeeq.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gapjsckkq.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gqcwygnyk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gmdbjxoio.sHtML

Ruby: "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gqalrywvp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fktsv.cn/Article/details/gjranebcc.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gejlgiino.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.yfazqb.com/Article/details/glezwwjrv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gwwlphceu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gjfmumpez.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gamdnixgv.sHtML

Java: s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/glncthfkx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.sjlbkw.cn/Article/details/grcwrqoyv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.sjlbkw.cn/Article/details/grhwaldfu.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.bbcook.cn/Article/details/gptisvrxu.sHtML

[E04] 查找子串位置
来源：http://blog.epnwcf.com/Article/details/gqgrcssgx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gyudsxnyq.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.sjlbkw.cn/Article/details/gdxphuffi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/gctxmskqc.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gbuboiwjo.sHtML

Java: s.indexOf("x")
来源：http://3g.tarul.cn/Article/details/gojrvkiyz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.yfazqb.com/Article/details/gbqvolyva.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gmfmwcuty.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gaqsfnzgr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.epnwcf.com/Article/details/gfhoqiisv.sHtML


<!-- 参考信息 -->