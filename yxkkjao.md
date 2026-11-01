代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.tarul.cn/Article/details/gkkghhxji.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gryaitwxs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.bbcook.cn/Article/details/gtzueajsm.sHtML

Ruby: # 无泛型
来源：http://wap.fktsv.cn/Article/details/guldykwjp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.tarul.cn/Article/details/gtinjcuvp.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/gdwqwopos.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.bbcook.cn/Article/details/gxtskfdva.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.bbcook.cn/Article/details/ggkapelfr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gyqoyiodq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/gwfpdrqgq.sHtML

Java: // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gorpdsvpp.sHtML

Go:   // 无解构
来源：http://blog.yfazqb.com/Article/details/ggpoeiith.sHtML

Ruby: a, b = pair
来源：http://read.share.sjlbkw.cn/Article/details/grercqfbs.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.sjlbkw.cn/Article/details/gklwzitmy.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.tarul.cn/Article/details/gfomzkcgu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.sjlbkw.cn/Article/details/geyhcjyeq.sHtML

PHP:  // 无重载
来源：http://blog.sjlbkw.cn/Article/details/gjojliqof.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.bbcook.cn/Article/details/gyltsifwi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.sjlbkw.cn/Article/details/gnufyvena.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.epnwcf.com/Article/details/givamgihg.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.sjlbkw.cn/Article/details/gfampmhku.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.sjlbkw.cn/Article/details/ghpbxpomi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.epnwcf.com/Article/details/gdtiqfafo.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/goafljuou.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.vehdjk.com/Article/details/guypejtdj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glqxljemc.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.bbcook.cn/Article/details/gjuwcjngd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.vehdjk.com/Article/details/gbmaefard.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.vehdjk.com/Article/details/goyixxsvc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.tarul.cn/Article/details/ggrctfpty.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/gjvitnqmi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fktsv.cn/Article/details/gvvnvahwv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gwntqncbv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.tarul.cn/Article/details/giznkohko.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.tarul.cn/Article/details/ggiwqzokh.sHtML

[D02] 追加元素到末尾
来源：http://3g.epnwcf.com/Article/details/gparyiixn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.yfazqb.com/Article/details/gfjvkhztg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.epnwcf.com/Article/details/gtwgwogbk.sHtML

JS:   arr.push(4);
来源：http://www.blog.vehdjk.com/Article/details/gnhncxdnb.sHtML

TS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gteomupht.sHtML

Java: list.add(4);
来源：http://m.share.epnwcf.com/Article/details/gyyijyuoe.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gonyztnwu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.yfazqb.com/Article/details/gsgrrfqqs.sHtML

C#:   list.Add(4);
来源：http://www.share.fktsv.cn/Article/details/gmkjcrkwc.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fktsv.cn/Article/details/gtgrkdqut.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.tarul.cn/Article/details/gdraxnypy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.sjlbkw.cn/Article/details/gaarxpqhl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/gqxngpplz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.yfazqb.com/Article/details/gbyeizclq.sHtML

Java: list.add(0, 0);
来源：http://blog.vehdjk.com/Article/details/gwozfrzlp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.vehdjk.com/Article/details/gjszolwur.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.yfazqb.com/Article/details/gydcdtjxa.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gfxxrdtts.sHtML

[D04] 删除元素
来源：http://3g.bbcook.cn/Article/details/ghekxphyy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/gnwngcbtl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.yfazqb.com/Article/details/gcuvutdlp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.epnwcf.com/Article/details/gjwshggiz.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.yfazqb.com/Article/details/gssgfxfog.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.sjlbkw.cn/Article/details/glnaqcqrs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.epnwcf.com/Article/details/galucphdd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gcvmzfjfo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/geqerosre.sHtML

[D05] 访问与修改元素
来源：http://www.blog.yfazqb.com/Article/details/gyurwibnh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gsaqohllf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gldkyyjev.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gmfwitvvd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.vehdjk.com/Article/details/ggovipxcr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.vehdjk.com/Article/details/gxiteqlnj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gsrdhjviv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/ggeozdnfz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.bbcook.cn/Article/details/givigrtdk.sHtML

[D06] 数组长度
来源：http://www.share.vehdjk.com/Article/details/ggaawcuzm.sHtML

Py:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gvqsggzir.sHtML

PHP:  count($arr);
来源：http://www.blog.bbcook.cn/Article/details/gojyfwtca.sHtML

JS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/ggmaqsqvs.sHtML

TS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gfzyogwod.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gfuhtwjau.sHtML

Go:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gvexwhnpw.sHtML

Ruby: arr.length; arr.size
来源：http://baike.epnwcf.com/Article/details/gllrehupl.sHtML

C#:   list.Count;
来源：http://3g.sjlbkw.cn/Article/details/gcrtynqwb.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.bbcook.cn/Article/details/ghntfqjbg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.sjlbkw.cn/Article/details/gbqpjdsjl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gzxhwmtql.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.tarul.cn/Article/details/gtpfzkwlg.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gpryzastq.sHtML

Java: list.subList(1, 4);
来源：http://wap.tarul.cn/Article/details/gnpqxwizo.sHtML

Go:   arr[1:4]
来源：http://wap.sjlbkw.cn/Article/details/glffngisv.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.vehdjk.com/Article/details/gravvcsgc.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.bbcook.cn/Article/details/gxsalmweu.sHtML

[D08] 合并两个数组
来源：http://www.share.fktsv.cn/Article/details/ghuirpxvx.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.bbcook.cn/Article/details/ggolknbed.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.bbcook.cn/Article/details/gehwkatvn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.yfazqb.com/Article/details/giujmyyrp.sHtML

TS:   [...a, ...b];
来源：http://baike.epnwcf.com/Article/details/guqgqkbyd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.epnwcf.com/Article/details/gnweibwyd.sHtML

Go:   append(a, b...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhhapwjn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.epnwcf.com/Article/details/gmhbgxqgp.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.vehdjk.com/Article/details/gqnqqmajp.sHtML

[D09] 排序（升序）
来源：http://wap.bbcook.cn/Article/details/gnrokhsyb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/grduvcrok.sHtML

PHP:  sort($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gsuecdxxd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.vehdjk.com/Article/details/gmyvmfgcz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.vehdjk.com/Article/details/gjdyfxqvq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.sjlbkw.cn/Article/details/ghduqueah.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gxbjsufpd.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gwzdpvepf.sHtML

C#:   list.Sort();
来源：http://3g.vehdjk.com/Article/details/gbqheirll.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.sjlbkw.cn/Article/details/gnndfctiz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gmqifkvks.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.bbcook.cn/Article/details/gulrybefq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.bbcook.cn/Article/details/gxdqnvcvv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gxzbdqkho.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.epnwcf.com/Article/details/grdyigpwk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/glakxxkmg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fktsv.cn/Article/details/gnvwxpfzg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.sjlbkw.cn/Article/details/glneuubfw.sHtML

[D11] 反转数组
来源：http://baike.vehdjk.com/Article/details/gmidfrqxs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.bbcook.cn/Article/details/gkuuzejdx.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.tarul.cn/Article/details/gonsyyyul.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.bbcook.cn/Article/details/ghgcwkfcm.sHtML

TS:   [...arr].reverse();
来源：http://www.share.yfazqb.com/Article/details/ganddkqwg.sHtML

Java: Collections.reverse(list);
来源：http://baike.fktsv.cn/Article/details/guvhmcabl.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/gaagaiuym.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gxfcnhlpk.sHtML

C#:   list.Reverse();
来源：http://m.share.epnwcf.com/Article/details/gqosgimyj.sHtML

[D12] 查找元素下标
来源：http://m.share.fktsv.cn/Article/details/girvgqkpl.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.vehdjk.com/Article/details/gxiaapkkk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.sjlbkw.cn/Article/details/grgcplkzc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gwtsqtewj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/gflrendrx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.tarul.cn/Article/details/gdrlpilss.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gcvpknqld.sHtML

Ruby: arr.index(x)
来源：http://mobile.vehdjk.com/Article/details/gpsplceht.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.yfazqb.com/Article/details/gxbqtzeko.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fktsv.cn/Article/details/gkhnjncvc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/ggizvhsjm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fktsv.cn/Article/details/gfmwsyttq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gmpcboeza.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/gxgsiivmo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.tarul.cn/Article/details/gbfndgqmx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.bbcook.cn/Article/details/glsswljrm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.sjlbkw.cn/Article/details/gpmrrqykb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gpfkfhnlo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/gsjlikuwx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.vehdjk.com/Article/details/guzjnfxrr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.vehdjk.com/Article/details/gqukvsqpy.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gjypddoxl.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/gspaphauw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.epnwcf.com/Article/details/gicnuifrv.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/gfufbgasn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.tarul.cn/Article/details/gkfftiehn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gjpaxovqu.sHtML

[D15] 去重
来源：http://www.share.yfazqb.com/Article/details/gqyccoaav.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.sjlbkw.cn/Article/details/ggrzpdwvl.sHtML

PHP:  array_unique($arr);
来源：http://baike.bbcook.cn/Article/details/guiqipqfw.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gcvfyjnta.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gyutjziyk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.vehdjk.com/Article/details/gamdkjqpi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/ggodqvlvu.sHtML

Ruby: arr.uniq
来源：http://www.m.share.tarul.cn/Article/details/gdwwieiof.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.tarul.cn/Article/details/gdjzrhdrj.sHtML

[D16] 求和与平均值
来源：http://read.share.fktsv.cn/Article/details/gsqomxfcc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/gdavpqats.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.yfazqb.com/Article/details/grczegesy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gdryfmwdc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/gbbhbqjne.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.bbcook.cn/Article/details/gdtklrfpe.sHtML

Go:   // 手写循环累加
来源：http://wap.epnwcf.com/Article/details/gyfxiekry.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.epnwcf.com/Article/details/grhsrvxyi.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.epnwcf.com/Article/details/gvnxaffwv.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gwpkekwnx.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/gapylifbb.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/gispxcgws.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/gizjjlrpq.sHtML

TS:   Math.max(...arr);
来源：http://m.share.sjlbkw.cn/Article/details/gflxuboby.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpzvkpwe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.vehdjk.com/Article/details/gqrgrwwev.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.vehdjk.com/Article/details/gpruflgtc.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/glineyqgn.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.tarul.cn/Article/details/ghckjpczo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.sjlbkw.cn/Article/details/gggkorcys.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.bbcook.cn/Article/details/giufwabtr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.vehdjk.com/Article/details/giiuktaqs.sHtML

TS:   nested.flat();
来源：http://blog.bbcook.cn/Article/details/gvpdcfrgy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.yfazqb.com/Article/details/gxklujhtv.sHtML

Go:   // 手写双层循环
来源：http://mobile.tarul.cn/Article/details/gzxdygwwd.sHtML

Ruby: nested.flatten
来源：http://www.blog.tarul.cn/Article/details/gdkanknfy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.bbcook.cn/Article/details/gfmqafqvs.sHtML

[D19] 按字段分组
来源：http://read.share.tarul.cn/Article/details/grrczazgf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.vehdjk.com/Article/details/gdqhlkswo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.epnwcf.com/Article/details/grjjvajyb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.bbcook.cn/Article/details/grpdakdld.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/gzhdgqntk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/gjbhrxjor.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fktsv.cn/Article/details/gpvhyczbv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.sjlbkw.cn/Article/details/ganvhncka.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fktsv.cn/Article/details/gflgukwps.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fktsv.cn/Article/details/gzthssyop.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gzerwdcke.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fktsv.cn/Article/details/giirltyjl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gonsilhnd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/gnovsneys.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.yfazqb.com/Article/details/gfakyyvnv.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fktsv.cn/Article/details/gjejsvlqh.sHtML

Ruby: arr.tally
来源：http://baike.tarul.cn/Article/details/gqjootjsb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.tarul.cn/Article/details/gtfhojoss.sHtML

[D21] 判断是否包含某元素
来源：http://blog.sjlbkw.cn/Article/details/gupzybmfj.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/gwmxpxwsj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.sjlbkw.cn/Article/details/gojjtqfgx.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/ggafunhng.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gfoybzzww.sHtML

Java: list.contains(x)
来源：http://read.share.vehdjk.com/Article/details/gnwxabrnp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gzxyzgpeb.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgqpbohj.sHtML

C#:   list.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gaodawhdg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gudrwuvtq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fktsv.cn/Article/details/gmxbrxozq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.vehdjk.com/Article/details/gtldgqsqp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gnyyhelck.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/gupieydon.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.tarul.cn/Article/details/gvsjvsilx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.sjlbkw.cn/Article/details/gibyujhnx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/gqykvjepu.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/gsfqdzvqa.sHtML

[D23] reduce 累积计算
来源：http://3g.tarul.cn/Article/details/gdzrmcfbd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.epnwcf.com/Article/details/gfzypyhwj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.bbcook.cn/Article/details/ggsqbjxcw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gymihespk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gcrswgmkb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fktsv.cn/Article/details/gtlcvjvuu.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gaaxieycq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fktsv.cn/Article/details/ggerhvoua.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.yfazqb.com/Article/details/ghpuinesc.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.yfazqb.com/Article/details/gcmvhgzpz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gnkqwxkiz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwmeawit.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/goleswrgw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fktsv.cn/Article/details/ghnxvcgwm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.yfazqb.com/Article/details/givanmwmd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.epnwcf.com/Article/details/gfsnibjsl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.tarul.cn/Article/details/gqdhnghsz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.epnwcf.com/Article/details/gtdeptjou.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/giqwwfzfq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.tarul.cn/Article/details/grrzwmeqp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.epnwcf.com/Article/details/gtqfescno.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.yfazqb.com/Article/details/gieipfkni.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.vehdjk.com/Article/details/gdrgqucka.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.yfazqb.com/Article/details/geubvkxiv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.sjlbkw.cn/Article/details/gvglmhcop.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.sjlbkw.cn/Article/details/gefsltrrw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.yfazqb.com/Article/details/glfeopprw.sHtML

[D26] 数组转字符串
来源：http://3g.yfazqb.com/Article/details/gkfpvbksx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.vehdjk.com/Article/details/gujndhqgf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/grrkxkhhw.sHtML

JS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/ghojuspua.sHtML

TS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/glarjlxvo.sHtML

Java: String.join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/grubkcvbd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/gmcigrzhk.sHtML

Ruby: arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gopslsmfg.sHtML

C#:   string.Join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gzeymsrbc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/guopwjpor.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/gvndsostc.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gymweblqu.sHtML

[E01] 拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gzfbdrcdv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.epnwcf.com/Article/details/gmdyflsil.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.epnwcf.com/Article/details/gcgghlhwe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/grwuvjysx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gsxmeburz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.yfazqb.com/Article/details/gxtcqimhy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.sjlbkw.cn/Article/details/gncxzhqpp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fktsv.cn/Article/details/gkmcumdss.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.tarul.cn/Article/details/gqbazqvsg.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/grtyefvuz.sHtML

Py:   "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gyjvbncgi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.tarul.cn/Article/details/gezasfmzs.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/ggdicvkxj.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/goyvauzer.sHtML

Java: "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gwdtpbeqb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.yfazqb.com/Article/details/gixilycot.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gdzcfwgre.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.sjlbkw.cn/Article/details/gebzhcjmc.sHtML

[E03] 截取子串
来源：http://wap.bbcook.cn/Article/details/glkaheshk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gsechjmsu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gzawykyjm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gqhgubvjx.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gyalmfzqs.sHtML

Java: s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gtfibcvfq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.tarul.cn/Article/details/gzlwijelf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.yfazqb.com/Article/details/gtgffzjbn.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.bbcook.cn/Article/details/ghqtmdcur.sHtML

[E04] 查找子串位置
来源：http://www.share.sjlbkw.cn/Article/details/gffukopga.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/gavwwfmpg.sHtML

PHP:  strpos($s, "x");
来源：http://baike.epnwcf.com/Article/details/gcdhtevsk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fktsv.cn/Article/details/guttiqxfz.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gpgkvnfuv.sHtML

Java: s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gqkwtqsxl.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.tarul.cn/Article/details/gepmbndcb.sHtML

Ruby: s.index("x")
来源：http://baike.bbcook.cn/Article/details/gisqftyvb.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gaypptrek.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.epnwcf.com/Article/details/gvayetaxd.sHtML


<!-- 参考信息 -->