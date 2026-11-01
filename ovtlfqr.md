代发 wailian999

[C14] 泛型函数
来源：http://blog.tarul.cn/Article/details/gtdyvfpuf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.vehdjk.com/Article/details/gxlsvddkk.sHtML

PHP:  // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gxpaduvmm.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gnsfnewon.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.vehdjk.com/Article/details/gbedhcaev.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.epnwcf.com/Article/details/gpprcyaal.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/gjfnatmzt.sHtML

Ruby: # 无泛型
来源：http://www.share.vehdjk.com/Article/details/gjrsubemb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.vehdjk.com/Article/details/gyilrwlcz.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.tarul.cn/Article/details/gpbnuxyaq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.epnwcf.com/Article/details/gadvsmkxf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.bbcook.cn/Article/details/gdttfjqae.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.vehdjk.com/Article/details/gxdczwbdn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gotycyixr.sHtML

Java: // 无解构
来源：http://m.share.tarul.cn/Article/details/gloyemrjt.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/gnwldwcaa.sHtML

Ruby: a, b = pair
来源：http://www.blog.epnwcf.com/Article/details/gfwydfxvt.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.bbcook.cn/Article/details/gekjneshl.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fktsv.cn/Article/details/gxujnixxi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.tarul.cn/Article/details/gwfelbiyv.sHtML

PHP:  // 无重载
来源：http://www.share.sjlbkw.cn/Article/details/gkoikkuyz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fktsv.cn/Article/details/gtjfwxsbp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.sjlbkw.cn/Article/details/gbvozvkbk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gentdokkf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.epnwcf.com/Article/details/gqbkfimja.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fktsv.cn/Article/details/gddrzltpt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.vehdjk.com/Article/details/gpllrawok.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gimznmsrw.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.epnwcf.com/Article/details/gsjyotbhs.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gefjpotka.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.sjlbkw.cn/Article/details/gcagiohcu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.epnwcf.com/Article/details/gbyijhhcg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.tarul.cn/Article/details/giorsduht.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.yfazqb.com/Article/details/gegicvqty.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.sjlbkw.cn/Article/details/gyedrybka.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.tarul.cn/Article/details/gxafypnvm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.yfazqb.com/Article/details/gqzhhoema.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fktsv.cn/Article/details/gyxpaynjg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.bbcook.cn/Article/details/gavvlsycb.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.vehdjk.com/Article/details/ggcieowhm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.sjlbkw.cn/Article/details/gahkcqhtw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fktsv.cn/Article/details/gzslhtetl.sHtML

JS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gkwjxyecs.sHtML

TS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/gdnjdqdjg.sHtML

Java: list.add(4);
来源：http://www.share.fktsv.cn/Article/details/gbcigtcfr.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gfiiyjfsg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.sjlbkw.cn/Article/details/gsjcpbosa.sHtML

C#:   list.Add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gazuqnlaw.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.yfazqb.com/Article/details/ggwkblbpv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gwjzleunh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.sjlbkw.cn/Article/details/gawchpsnc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.yfazqb.com/Article/details/gnwvbzxqh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.epnwcf.com/Article/details/gwqadzbvj.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gobmqylar.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fktsv.cn/Article/details/gezpefjqh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.tarul.cn/Article/details/gtuhuznbn.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fktsv.cn/Article/details/gbnrjmvki.sHtML

[D04] 删除元素
来源：http://blog.epnwcf.com/Article/details/gakdseiot.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.epnwcf.com/Article/details/gdvosmcpd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.vehdjk.com/Article/details/gaakijtqt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.sjlbkw.cn/Article/details/gsszrbdkp.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/giisfzhpe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/gkdpdxbhv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fktsv.cn/Article/details/gbkdkmrjo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/gbbquyjdx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.tarul.cn/Article/details/gbncrdwok.sHtML

[D05] 访问与修改元素
来源：http://www.blog.sjlbkw.cn/Article/details/gbmouetzl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/grpgcaiot.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gbsokskud.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gnhufdyxc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gsyrrhftx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.epnwcf.com/Article/details/gikzmpwvc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gtdfhsflf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gndwvokbb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gbaepnoat.sHtML

[D06] 数组长度
来源：http://www.m.share.yfazqb.com/Article/details/gfipqbxli.sHtML

Py:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gbkbdqxxo.sHtML

PHP:  count($arr);
来源：http://mobile.bbcook.cn/Article/details/grpqyloxc.sHtML

JS:   arr.length
来源：http://3g.tarul.cn/Article/details/gsjqreobg.sHtML

TS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/gigqpcewa.sHtML

Java: list.size();
来源：http://www.blog.tarul.cn/Article/details/gvmbumgwb.sHtML

Go:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gislfuopr.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.bbcook.cn/Article/details/gmuanlxqv.sHtML

C#:   list.Count;
来源：http://wap.yfazqb.com/Article/details/gfkhcogql.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/goleztmot.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.vehdjk.com/Article/details/gekwnalzw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.epnwcf.com/Article/details/gqgitgmlq.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.epnwcf.com/Article/details/gqtjxcwzj.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gcdewxjiz.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/gsgkuynro.sHtML

Go:   arr[1:4]
来源：http://www.m.share.bbcook.cn/Article/details/gajrzmwqo.sHtML

Ruby: arr[1, 3]
来源：http://www.share.yfazqb.com/Article/details/gkxcdzrag.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.vehdjk.com/Article/details/gmdcudzws.sHtML

[D08] 合并两个数组
来源：http://mobile.tarul.cn/Article/details/gdtfnvgiy.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.bbcook.cn/Article/details/gofjzzsos.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.yfazqb.com/Article/details/gxjtntocr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.epnwcf.com/Article/details/gunvciwtz.sHtML

TS:   [...a, ...b];
来源：http://baike.vehdjk.com/Article/details/gynkikaks.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gtxwrhufc.sHtML

Go:   append(a, b...)
来源：http://www.m.share.vehdjk.com/Article/details/gaaokfavq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.bbcook.cn/Article/details/grerrlgps.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fktsv.cn/Article/details/gvcgznkkw.sHtML

[D09] 排序（升序）
来源：http://m.share.epnwcf.com/Article/details/gcuqwifsa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.epnwcf.com/Article/details/gsvmvrllj.sHtML

PHP:  sort($arr);
来源：http://mobile.vehdjk.com/Article/details/ghuvvubiu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fktsv.cn/Article/details/gpouneykh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fktsv.cn/Article/details/gurnbqvom.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.sjlbkw.cn/Article/details/gjhrmgygo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gzahrdizu.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/ggazemkvd.sHtML

C#:   list.Sort();
来源：http://blog.yfazqb.com/Article/details/gryjbyxng.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.sjlbkw.cn/Article/details/gyignmbip.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fktsv.cn/Article/details/govsukqid.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.yfazqb.com/Article/details/gjksevnoe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gzhdhguth.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gwbpcuayg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.sjlbkw.cn/Article/details/gsrlcacpr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.yfazqb.com/Article/details/gybfvuphf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.epnwcf.com/Article/details/gsndjytgj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.tarul.cn/Article/details/gzwubdrhb.sHtML

[D11] 反转数组
来源：http://3g.bbcook.cn/Article/details/gqfuwvjfi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.epnwcf.com/Article/details/gepubjzyb.sHtML

PHP:  array_reverse($arr);
来源：http://wap.tarul.cn/Article/details/gwwtslhuv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/gwrzvoyxf.sHtML

TS:   [...arr].reverse();
来源：http://wap.bbcook.cn/Article/details/gmxgopzcr.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.epnwcf.com/Article/details/gbalvfzcz.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.yfazqb.com/Article/details/gmyizghcm.sHtML

Ruby: arr.reverse
来源：http://mobile.yfazqb.com/Article/details/gnaxfadxz.sHtML

C#:   list.Reverse();
来源：http://m.share.tarul.cn/Article/details/ghcpaxppp.sHtML

[D12] 查找元素下标
来源：http://www.share.tarul.cn/Article/details/giwpbudij.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.yfazqb.com/Article/details/gfzbyhtfl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fktsv.cn/Article/details/ghagjeypw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gujxghved.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gylyvkljg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.yfazqb.com/Article/details/gauataixp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/glggjagzx.sHtML

Ruby: arr.index(x)
来源：http://mobile.fktsv.cn/Article/details/gretydebk.sHtML

C#:   list.IndexOf(x);
来源：http://wap.sjlbkw.cn/Article/details/gwtzwjchp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.bbcook.cn/Article/details/gnanumcvh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/ghzljqdnc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.epnwcf.com/Article/details/ghmdkfrtm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/gddgtgclt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gclzzpuwx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.vehdjk.com/Article/details/gwtmjkekl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.yfazqb.com/Article/details/gjhxqquhl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.vehdjk.com/Article/details/grrabdffy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gpdvmglfx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.bbcook.cn/Article/details/gsmtydvjj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.bbcook.cn/Article/details/gyjubshpp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fktsv.cn/Article/details/gfpdupmfq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gdvfjieim.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fktsv.cn/Article/details/gqdyxakls.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.tarul.cn/Article/details/gxwehedfn.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/gjjgqsezi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gbtyeqalp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.yfazqb.com/Article/details/grnnxfmej.sHtML

[D15] 去重
来源：http://baike.bbcook.cn/Article/details/gyxbzkstk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.tarul.cn/Article/details/gkfhysiha.sHtML

PHP:  array_unique($arr);
来源：http://3g.vehdjk.com/Article/details/gvlvnebot.sHtML

JS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gxsdqveaf.sHtML

TS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gblthrhtb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fktsv.cn/Article/details/gpxtcwipo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.sjlbkw.cn/Article/details/gzoipihby.sHtML

Ruby: arr.uniq
来源：http://mobile.fktsv.cn/Article/details/gkdhkdctx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.bbcook.cn/Article/details/gwfigbirk.sHtML

[D16] 求和与平均值
来源：http://www.blog.tarul.cn/Article/details/gvjxhflfe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.tarul.cn/Article/details/guaklywus.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.vehdjk.com/Article/details/geirzxkpg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/goiwruypb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/gfayzdzhj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.bbcook.cn/Article/details/gydbtkftv.sHtML

Go:   // 手写循环累加
来源：http://wap.epnwcf.com/Article/details/ggqtcqvye.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.bbcook.cn/Article/details/gfbkdcmyj.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.epnwcf.com/Article/details/gyyghuhxk.sHtML

[D17] 最大值与最小值
来源：http://m.share.sjlbkw.cn/Article/details/gcjlfckbl.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.tarul.cn/Article/details/gonpectoc.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.bbcook.cn/Article/details/gqvnzcmnx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.bbcook.cn/Article/details/gsqzjhxwx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.epnwcf.com/Article/details/gzxpjlmvf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fktsv.cn/Article/details/gphplgobq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.yfazqb.com/Article/details/ghchhfikv.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gooqpezqa.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.yfazqb.com/Article/details/grvmpxmqu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/gfefalrgh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.epnwcf.com/Article/details/gjetqlusm.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.vehdjk.com/Article/details/gogzlbtiu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.bbcook.cn/Article/details/gcssqtuve.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/ggnjdhhhl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gcckmrewa.sHtML

Go:   // 手写双层循环
来源：http://m.share.bbcook.cn/Article/details/gxhiprxnu.sHtML

Ruby: nested.flatten
来源：http://wap.fktsv.cn/Article/details/gssphuhzg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.epnwcf.com/Article/details/gfathbavd.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/gbhzcqpjw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.bbcook.cn/Article/details/gvjksqwce.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/gyxubcejq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.sjlbkw.cn/Article/details/gyswatcxc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/gqbqharom.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.epnwcf.com/Article/details/ggbfyedbe.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.yfazqb.com/Article/details/gregecinj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fktsv.cn/Article/details/gurbmtvln.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/gyorvhvvs.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gwamvlaqf.sHtML

Py:   Counter(arr)
来源：http://wap.fktsv.cn/Article/details/gdoknfatp.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.yfazqb.com/Article/details/gvzvinaym.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gddfoyifw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/gebtgoira.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/gdydlkpvs.sHtML

Go:   // 手写 map[T]int
来源：http://baike.vehdjk.com/Article/details/gvenrmdsc.sHtML

Ruby: arr.tally
来源：http://baike.vehdjk.com/Article/details/gtepgwcaz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/gaoubeako.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fktsv.cn/Article/details/ghhqrghvd.sHtML

Py:   x in arr
来源：http://wap.vehdjk.com/Article/details/gvfopduik.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.sjlbkw.cn/Article/details/gqzifpwwx.sHtML

JS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/glcukkvno.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gnjpxwrek.sHtML

Java: list.contains(x)
来源：http://read.share.vehdjk.com/Article/details/gtytdgwwq.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fktsv.cn/Article/details/ggxjzkbiq.sHtML

Ruby: arr.include?(x)
来源：http://baike.epnwcf.com/Article/details/gotrmuujf.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gqorolvnt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.bbcook.cn/Article/details/guweklzgy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.yfazqb.com/Article/details/gdsojzyiy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.vehdjk.com/Article/details/gfqtihoxm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/goljtmlyx.sHtML

TS:   [...arr];
来源：http://read.share.tarul.cn/Article/details/giffekkfg.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fktsv.cn/Article/details/gpdmsbsci.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/gcpjmpwse.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.tarul.cn/Article/details/gpfunpggr.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxdeaisp.sHtML

[D23] reduce 累积计算
来源：http://blog.vehdjk.com/Article/details/gvvlhsczt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.sjlbkw.cn/Article/details/ggrzxvmvy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.epnwcf.com/Article/details/goegjjfbo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gmvoeuidy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/ggvdpnhoo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fktsv.cn/Article/details/giujzoams.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gdxqvfwsk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.sjlbkw.cn/Article/details/gvfameskv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.bbcook.cn/Article/details/gjnpnvecm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.sjlbkw.cn/Article/details/gbevupuog.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/grxadyztj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.sjlbkw.cn/Article/details/gefprrfaq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fktsv.cn/Article/details/gkqjgifmz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fktsv.cn/Article/details/gmrtbatfa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.yfazqb.com/Article/details/gjzaitkqv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/ggfxwruev.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.epnwcf.com/Article/details/gaeflvxld.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fktsv.cn/Article/details/gphjnyrnl.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/gsfhetfxy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.epnwcf.com/Article/details/gfhcsqkvv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.tarul.cn/Article/details/ghyqfmhoh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.tarul.cn/Article/details/gffchsjnp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.epnwcf.com/Article/details/gcijqxvwr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.tarul.cn/Article/details/ghawbkcem.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fktsv.cn/Article/details/gigdjtvbm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.epnwcf.com/Article/details/gabcmzewz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/gqtnvtvba.sHtML

[D26] 数组转字符串
来源：http://read.share.yfazqb.com/Article/details/gokvpwpes.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.yfazqb.com/Article/details/gtuvknawi.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.tarul.cn/Article/details/garkcpffq.sHtML

JS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gkonhxmcy.sHtML

TS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gilgxbtqr.sHtML

Java: String.join(", ", list)
来源：http://baike.tarul.cn/Article/details/glxdfqzhu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fktsv.cn/Article/details/gewiskaur.sHtML

Ruby: arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gskpbhnwy.sHtML

C#:   string.Join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gdsbtvujw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmmlqzssi.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gqmtgbgts.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gulllajlj.sHtML

[E01] 拼接字符串
来源：http://mobile.yfazqb.com/Article/details/grjzrlcti.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/gnbcvonha.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.sjlbkw.cn/Article/details/gikqbafqd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gyrczdxri.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gqcrrxotq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlbbsibl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxdpynxv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.bbcook.cn/Article/details/gmiwxaqlk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.yfazqb.com/Article/details/gklilflso.sHtML

[E02] 重复字符串
来源：http://3g.fktsv.cn/Article/details/gtaeoqvdy.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gflsuoiqh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fktsv.cn/Article/details/grsbqvujv.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gtadqhdlk.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gwsjntimh.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/grxmquxsu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.epnwcf.com/Article/details/gbadhbujr.sHtML

Ruby: "ab" * 3
来源：http://baike.epnwcf.com/Article/details/gkuzevhiv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/gvtfnklla.sHtML

[E03] 截取子串
来源：http://m.share.fktsv.cn/Article/details/ghvgpqema.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.sjlbkw.cn/Article/details/gloulfyke.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gvpjrejpi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/gjkaxizrj.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gewgirflk.sHtML

Java: s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/gflotwrjp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gfmesurxl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fktsv.cn/Article/details/gcfvynxah.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/gdvfmvgkm.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gjbrbsmvh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gbcmsochl.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.tarul.cn/Article/details/gwolwzjeo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.vehdjk.com/Article/details/gatixymkg.sHtML

TS:   s.indexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gayolgzwa.sHtML

Java: s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/gnrawiqre.sHtML


<!-- 参考信息 -->