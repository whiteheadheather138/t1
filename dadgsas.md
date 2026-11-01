代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/gyutcaglw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fktsv.cn/Article/details/gakdqfyhm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.bbcook.cn/Article/details/gtlvszaoi.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/grhzewxtu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.vehdjk.com/Article/details/ggpphcpfw.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/gwayydkks.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.yfazqb.com/Article/details/geffuxyyf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.yfazqb.com/Article/details/gdkgvpyac.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gmmwsylrq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.vehdjk.com/Article/details/ghfqqowmc.sHtML

Java: // 无解构
来源：http://blog.tarul.cn/Article/details/gcwnwxfzu.sHtML

Go:   // 无解构
来源：http://m.share.tarul.cn/Article/details/gvpqwlpof.sHtML

Ruby: a, b = pair
来源：http://www.m.share.bbcook.cn/Article/details/gklgxvswb.sHtML

C#:   var (a, b) = pair;
来源：http://3g.yfazqb.com/Article/details/gtyfrnvac.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fktsv.cn/Article/details/gujhtaddt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.vehdjk.com/Article/details/gkefkashs.sHtML

PHP:  // 无重载
来源：http://baike.yfazqb.com/Article/details/gsdllsqaz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.bbcook.cn/Article/details/ggjtmhmdf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.bbcook.cn/Article/details/gdxdcshxm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.tarul.cn/Article/details/gsgjatups.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.vehdjk.com/Article/details/gywxxnxad.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.epnwcf.com/Article/details/gconzbzte.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.tarul.cn/Article/details/gnvoblejj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gitigxgjb.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fktsv.cn/Article/details/gxasavrwg.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gigoqqpfi.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.tarul.cn/Article/details/gcldertbf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fktsv.cn/Article/details/gtluurozh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.bbcook.cn/Article/details/ghvbdeyrm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fktsv.cn/Article/details/gtowrfqqc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fktsv.cn/Article/details/gpjwxpsdd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/gjvsfvpir.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.bbcook.cn/Article/details/gvusttlxp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.vehdjk.com/Article/details/gsqofaeft.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.vehdjk.com/Article/details/gksvlziwr.sHtML

[D02] 追加元素到末尾
来源：http://read.share.vehdjk.com/Article/details/gmlmiring.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.tarul.cn/Article/details/gciorgrmx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.tarul.cn/Article/details/ghtzxbnuz.sHtML

JS:   arr.push(4);
来源：http://3g.fktsv.cn/Article/details/gixwtiqcz.sHtML

TS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/gefroxjtj.sHtML

Java: list.add(4);
来源：http://baike.bbcook.cn/Article/details/gzsvzlzin.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fktsv.cn/Article/details/gcdlhcntx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.yfazqb.com/Article/details/gvzghzxpu.sHtML

C#:   list.Add(4);
来源：http://blog.vehdjk.com/Article/details/ghqvifpnr.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.epnwcf.com/Article/details/gnxokpiic.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.tarul.cn/Article/details/gndrpftge.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.tarul.cn/Article/details/gjnnxwzwm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.tarul.cn/Article/details/gsslmgrjk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.vehdjk.com/Article/details/gyqrczjly.sHtML

Java: list.add(0, 0);
来源：http://baike.fktsv.cn/Article/details/ghlelxlda.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.bbcook.cn/Article/details/gfdtsphzd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.epnwcf.com/Article/details/giapiutfc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gxwhnxfzz.sHtML

[D04] 删除元素
来源：http://mobile.epnwcf.com/Article/details/geifepvfg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.epnwcf.com/Article/details/glopmcbbo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.vehdjk.com/Article/details/gaznsslas.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.vehdjk.com/Article/details/ghpssjwld.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/giopcwpdw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.vehdjk.com/Article/details/gemeuaptx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.bbcook.cn/Article/details/gtudbjcfk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.yfazqb.com/Article/details/gcjrpvvhb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.bbcook.cn/Article/details/gdhjoqapd.sHtML

[D05] 访问与修改元素
来源：http://www.share.tarul.cn/Article/details/gmbikupar.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gzqwoylww.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gstfyhlov.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gdoprqcjr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.tarul.cn/Article/details/gkcgbwcgm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.epnwcf.com/Article/details/gxtypffup.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gexqryvvc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.epnwcf.com/Article/details/guwcuirqe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gicbnozae.sHtML

[D06] 数组长度
来源：http://blog.tarul.cn/Article/details/gsrbtuelw.sHtML

Py:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gwlipilvz.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gxkdypvtd.sHtML

JS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gdovbpywa.sHtML

TS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gvmongdll.sHtML

Java: list.size();
来源：http://www.m.share.bbcook.cn/Article/details/grxyemsti.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/goznajkxt.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.bbcook.cn/Article/details/gnxoktkzq.sHtML

C#:   list.Count;
来源：http://3g.yfazqb.com/Article/details/ggrpanpor.sHtML

[D07] 切片 / 取子数组
来源：http://blog.epnwcf.com/Article/details/gxvmavcog.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.bbcook.cn/Article/details/grdigiwda.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.bbcook.cn/Article/details/gvrlsfsps.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gzlawefzy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gprvumwxp.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gutfkjfom.sHtML

Go:   arr[1:4]
来源：http://wap.fktsv.cn/Article/details/gualqojec.sHtML

Ruby: arr[1, 3]
来源：http://baike.fktsv.cn/Article/details/gmrshqavq.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fktsv.cn/Article/details/gricugkhm.sHtML

[D08] 合并两个数组
来源：http://wap.vehdjk.com/Article/details/gfwnlnrtz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.tarul.cn/Article/details/gpubegqjk.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.yfazqb.com/Article/details/glpbfewjn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fktsv.cn/Article/details/grystfeeb.sHtML

TS:   [...a, ...b];
来源：http://www.blog.bbcook.cn/Article/details/gyezjgozp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.epnwcf.com/Article/details/gjwtsqydm.sHtML

Go:   append(a, b...)
来源：http://3g.sjlbkw.cn/Article/details/gnwxfdnce.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.sjlbkw.cn/Article/details/gfeouxzln.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.vehdjk.com/Article/details/gvotrnwfp.sHtML

[D09] 排序（升序）
来源：http://blog.bbcook.cn/Article/details/gbcurnpks.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gwnqfejdc.sHtML

PHP:  sort($arr);
来源：http://baike.bbcook.cn/Article/details/glgbxrrde.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.sjlbkw.cn/Article/details/gkbvlyfbc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.bbcook.cn/Article/details/gcogeptow.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.epnwcf.com/Article/details/gbuprnzmk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gwqbxfngi.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gpzsmhdno.sHtML

C#:   list.Sort();
来源：http://baike.epnwcf.com/Article/details/gknzpehiy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.sjlbkw.cn/Article/details/gwnysjiya.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.yfazqb.com/Article/details/godlrmupj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.vehdjk.com/Article/details/ghkmuqwej.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gkmxukkuu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/gmebdjuvv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.tarul.cn/Article/details/gudrjbbrj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.epnwcf.com/Article/details/gjvlldylu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.vehdjk.com/Article/details/geqhupadv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.sjlbkw.cn/Article/details/gbjmgmavr.sHtML

[D11] 反转数组
来源：http://www.blog.vehdjk.com/Article/details/gbwzorevs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.bbcook.cn/Article/details/gkcgpitcb.sHtML

PHP:  array_reverse($arr);
来源：http://blog.bbcook.cn/Article/details/gajvyjcrp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.epnwcf.com/Article/details/gwdwbqiyj.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gfghpmtpj.sHtML

Java: Collections.reverse(list);
来源：http://blog.fktsv.cn/Article/details/gxjywoqyg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fktsv.cn/Article/details/gurzrhfrt.sHtML

Ruby: arr.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gnjhzmtjb.sHtML

C#:   list.Reverse();
来源：http://3g.yfazqb.com/Article/details/gjqqcwqfm.sHtML

[D12] 查找元素下标
来源：http://m.share.tarul.cn/Article/details/glpsvmzlm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/goebskgfd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.vehdjk.com/Article/details/geictqzay.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.bbcook.cn/Article/details/gekvfmuhy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.bbcook.cn/Article/details/gonhsdyzc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.yfazqb.com/Article/details/gifysdfva.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fktsv.cn/Article/details/gqidehcwr.sHtML

Ruby: arr.index(x)
来源：http://3g.vehdjk.com/Article/details/gqnbwqmsn.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.tarul.cn/Article/details/gynbrpkhq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.bbcook.cn/Article/details/grtkkpwlc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.epnwcf.com/Article/details/ghzlmvrau.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.yfazqb.com/Article/details/gbjusxjtq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gcpammojn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/gtorsmtgd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.vehdjk.com/Article/details/glwqnkxkg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fktsv.cn/Article/details/gbjchwqbr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.tarul.cn/Article/details/gocsdlqgw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.epnwcf.com/Article/details/gvbynqbqk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fktsv.cn/Article/details/ghwfxornq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.epnwcf.com/Article/details/gvcuxpzpv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gorerucfw.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.sjlbkw.cn/Article/details/grmdozdvn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gcuntphfe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fktsv.cn/Article/details/gxyrignln.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gprbjlmgl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gekdaabdy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gxibyszxl.sHtML

[D15] 去重
来源：http://baike.fktsv.cn/Article/details/gxgiidwev.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gcqjqqbjx.sHtML

PHP:  array_unique($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gmxxbnjef.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gssvhhgqx.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gogdsnvvf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.bbcook.cn/Article/details/gdfecodpo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.yfazqb.com/Article/details/gqqpystge.sHtML

Ruby: arr.uniq
来源：http://www.m.share.epnwcf.com/Article/details/galfeeknq.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fktsv.cn/Article/details/gkjjvregb.sHtML

[D16] 求和与平均值
来源：http://baike.tarul.cn/Article/details/gzztktmxa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.bbcook.cn/Article/details/gorbsyleu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.tarul.cn/Article/details/gfkexwrdm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/goxfgxbvs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.tarul.cn/Article/details/ggwztzpwc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.epnwcf.com/Article/details/gsrawxkyc.sHtML

Go:   // 手写循环累加
来源：http://wap.yfazqb.com/Article/details/gddlaqcun.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.epnwcf.com/Article/details/gafwczftj.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.bbcook.cn/Article/details/gawepknhb.sHtML

[D17] 最大值与最小值
来源：http://3g.tarul.cn/Article/details/gcdgnmrpr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gnqhnlzvn.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.tarul.cn/Article/details/gzmwnvczo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpqreavl.sHtML

TS:   Math.max(...arr);
来源：http://baike.sjlbkw.cn/Article/details/gryapdgzb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.bbcook.cn/Article/details/gwhsmivvm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.yfazqb.com/Article/details/ggzaqhhbd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fktsv.cn/Article/details/gkjsucmhl.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.tarul.cn/Article/details/gczxlvwla.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.epnwcf.com/Article/details/gdteqdyzq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fktsv.cn/Article/details/glqqlcpea.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/gcmqczvwi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/gmlrevhfb.sHtML

TS:   nested.flat();
来源：http://www.blog.tarul.cn/Article/details/gwclpgmlh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gpaszuehc.sHtML

Go:   // 手写双层循环
来源：http://3g.sjlbkw.cn/Article/details/gtsoxmnlb.sHtML

Ruby: nested.flatten
来源：http://www.m.share.yfazqb.com/Article/details/gfrjwgkvv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.vehdjk.com/Article/details/gzsmqddwf.sHtML

[D19] 按字段分组
来源：http://mobile.sjlbkw.cn/Article/details/gdjmyoupi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.epnwcf.com/Article/details/gcdfqvyft.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/ghavutyne.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.epnwcf.com/Article/details/gqciicuuj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gnozzwzmu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.bbcook.cn/Article/details/gwaptjrfz.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.vehdjk.com/Article/details/gofgcnzsz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.sjlbkw.cn/Article/details/gktdjiafw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.yfazqb.com/Article/details/gauqtelli.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.vehdjk.com/Article/details/gizmztgsb.sHtML

Py:   Counter(arr)
来源：http://blog.tarul.cn/Article/details/gfsbqmtke.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/gkueksrul.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/grligqioe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/gqqxpvxsz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.epnwcf.com/Article/details/gfsaoqjip.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/gqhfjejcr.sHtML

Ruby: arr.tally
来源：http://blog.yfazqb.com/Article/details/gcuutbcwc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/gqzruhjyq.sHtML

[D21] 判断是否包含某元素
来源：http://wap.bbcook.cn/Article/details/glhkgndxm.sHtML

Py:   x in arr
来源：http://wap.epnwcf.com/Article/details/gqgczfopt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.epnwcf.com/Article/details/gtxslmxkc.sHtML

JS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/gxyavrvxs.sHtML

TS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/ghglvuttr.sHtML

Java: list.contains(x)
来源：http://m.share.epnwcf.com/Article/details/gnrouvxat.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.vehdjk.com/Article/details/gkffogjct.sHtML

Ruby: arr.include?(x)
来源：http://blog.yfazqb.com/Article/details/gzalcuhzf.sHtML

C#:   list.Contains(x)
来源：http://baike.vehdjk.com/Article/details/galadjkcl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.vehdjk.com/Article/details/gpuzaicid.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.bbcook.cn/Article/details/gznhtgtvo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.tarul.cn/Article/details/gxigyzvaa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fktsv.cn/Article/details/gmakttsge.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/gauvmtfmr.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.bbcook.cn/Article/details/gqaearuyj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.tarul.cn/Article/details/gumbjqmyc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.vehdjk.com/Article/details/gxmljjhfp.sHtML

C#:   new List<int>(list);
来源：http://m.share.tarul.cn/Article/details/gwuwtxaiv.sHtML

[D23] reduce 累积计算
来源：http://baike.yfazqb.com/Article/details/gfhphtlhj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.tarul.cn/Article/details/gfqvjwpff.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gxfenfwxp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/grcjvkeqx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gloaacfuo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.bbcook.cn/Article/details/gcpgmuvtx.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gohihhhuh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.bbcook.cn/Article/details/gwpxlqqrp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.tarul.cn/Article/details/gplacnfoy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.bbcook.cn/Article/details/ghopsewcn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.bbcook.cn/Article/details/gqsddshuw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.vehdjk.com/Article/details/gvawaheih.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.sjlbkw.cn/Article/details/ggivlapqz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gcbmduueg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.tarul.cn/Article/details/guxsfmagv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.tarul.cn/Article/details/gsidlsezu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gkxgdwhzw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.vehdjk.com/Article/details/gtzmnrwjv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.tarul.cn/Article/details/gbokzwdnz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.vehdjk.com/Article/details/gbpmiycfb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.epnwcf.com/Article/details/gqanpugnq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.vehdjk.com/Article/details/gjarfbpqp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.vehdjk.com/Article/details/ghoreogjy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxugztaz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/gboulkyrb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.sjlbkw.cn/Article/details/ghhhkadro.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gyvahetub.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gkkivipfz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gtwzconkn.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.epnwcf.com/Article/details/grpeulwhz.sHtML

JS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gqlixpjcc.sHtML

TS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gshmnmsil.sHtML

Java: String.join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gpjjlsmag.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.tarul.cn/Article/details/gkxwlkdxk.sHtML

Ruby: arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gayhbwpxw.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gjjtraoqt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gkmdvkqoh.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/gqjzdxiuu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjmjrgovk.sHtML

[E01] 拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/goonhoomv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fktsv.cn/Article/details/gnmkreyux.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.vehdjk.com/Article/details/gabafklsb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/ggzjjbpqx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/gvhqkauay.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.vehdjk.com/Article/details/gowvgxqnj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fktsv.cn/Article/details/gfqanoawe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.sjlbkw.cn/Article/details/gllgickte.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.bbcook.cn/Article/details/gbaycdrwu.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/gfimgxjdm.sHtML

Py:   "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gxbuwyyey.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.epnwcf.com/Article/details/gshjcazgr.sHtML

JS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/goozohwoi.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gusrzhtir.sHtML

Java: "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gcyowbixm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.epnwcf.com/Article/details/giafrgahq.sHtML

Ruby: "ab" * 3
来源：http://blog.yfazqb.com/Article/details/gyxdrnsqc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/ghwiegimd.sHtML

[E03] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gpzssvmjs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gcckxwevx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gdrjrahom.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/grnjxwwkj.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gybpytgof.sHtML

Java: s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gucwpywgp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.vehdjk.com/Article/details/gatsgswit.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.sjlbkw.cn/Article/details/glxlkxvtb.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.yfazqb.com/Article/details/gmzzietnt.sHtML

[E04] 查找子串位置
来源：http://wap.sjlbkw.cn/Article/details/gbpzoszvc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/gmalmdqqy.sHtML

PHP:  strpos($s, "x");
来源：http://baike.epnwcf.com/Article/details/gitvgjmri.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.bbcook.cn/Article/details/gxykjhtas.sHtML

TS:   s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/gdexsbncv.sHtML

Java: s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gkuvmovvw.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.sjlbkw.cn/Article/details/gahxwpzfr.sHtML

Ruby: s.index("x")
来源：http://blog.tarul.cn/Article/details/ghnklaiby.sHtML

C#:   s.IndexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gsepwefgt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.sjlbkw.cn/Article/details/gqtrjorzu.sHtML


<!-- 参考信息 -->