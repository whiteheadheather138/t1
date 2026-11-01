代发 wailian999

[C14] 泛型函数
来源：http://wap.tarul.cn/Article/details/gjfhdqvcj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.tarul.cn/Article/details/gnplobayw.sHtML

PHP:  // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/ghjsbvxdl.sHtML

JS:   // 无泛型
来源：http://baike.yfazqb.com/Article/details/grcgrcasv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.vehdjk.com/Article/details/ggznuyomh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/ghqisnqez.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/gunjldxkv.sHtML

Ruby: # 无泛型
来源：http://mobile.yfazqb.com/Article/details/gnpvqzccp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.sjlbkw.cn/Article/details/gexixfttb.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.epnwcf.com/Article/details/ghkrpempd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.vehdjk.com/Article/details/gnspptocz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/gcdklvrpv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gjckvkvmb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/gjyiiwwxh.sHtML

Java: // 无解构
来源：http://mobile.vehdjk.com/Article/details/glvsddtxq.sHtML

Go:   // 无解构
来源：http://www.blog.sjlbkw.cn/Article/details/gpboiqlyp.sHtML

Ruby: a, b = pair
来源：http://www.m.share.epnwcf.com/Article/details/gchxyygqe.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fktsv.cn/Article/details/gnlyilzke.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.tarul.cn/Article/details/gslugqngy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.vehdjk.com/Article/details/gsesrrclr.sHtML

PHP:  // 无重载
来源：http://www.m.share.tarul.cn/Article/details/gesaljfpj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.sjlbkw.cn/Article/details/ggeumcbiv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.yfazqb.com/Article/details/gplxxqlad.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.epnwcf.com/Article/details/gazimslsj.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fktsv.cn/Article/details/gfazftgen.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fktsv.cn/Article/details/guxkclgmw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.yfazqb.com/Article/details/gftlcdtrx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwxxzssyi.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.vehdjk.com/Article/details/gqiurnklb.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwiqpmbgi.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gxapektrk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.epnwcf.com/Article/details/gelpsucnu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.tarul.cn/Article/details/gzksmqrhm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.vehdjk.com/Article/details/gibovbbxx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.tarul.cn/Article/details/gjxtmlnhe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.bbcook.cn/Article/details/gcndertlc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.yfazqb.com/Article/details/gmpsilwgt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.sjlbkw.cn/Article/details/grzcjwxsx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.yfazqb.com/Article/details/gmxpanudr.sHtML

[D02] 追加元素到末尾
来源：http://3g.bbcook.cn/Article/details/giffwowxb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.vehdjk.com/Article/details/gyycoecxc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fktsv.cn/Article/details/grxcvudgc.sHtML

JS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/gsobjlczp.sHtML

TS:   arr.push(4);
来源：http://baike.yfazqb.com/Article/details/gkdjaybew.sHtML

Java: list.add(4);
来源：http://blog.epnwcf.com/Article/details/gphsrhuym.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.tarul.cn/Article/details/gcruqvwox.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.bbcook.cn/Article/details/gesjtpaao.sHtML

C#:   list.Add(4);
来源：http://blog.vehdjk.com/Article/details/gdjbrojtf.sHtML

[D03] 在指定位置插入元素
来源：http://3g.sjlbkw.cn/Article/details/gznthdree.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.yfazqb.com/Article/details/gvdycdxrq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.tarul.cn/Article/details/gtkcdtjem.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.yfazqb.com/Article/details/gzeroujnr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.bbcook.cn/Article/details/gijexhkto.sHtML

Java: list.add(0, 0);
来源：http://read.share.fktsv.cn/Article/details/glwlxwkqb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.vehdjk.com/Article/details/gtpniyico.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.sjlbkw.cn/Article/details/grqpznkrf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/glqsqyvqr.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/gojcueimp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.yfazqb.com/Article/details/gxjstljpm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.vehdjk.com/Article/details/gxenbndpv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.sjlbkw.cn/Article/details/geogimsay.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.epnwcf.com/Article/details/gxzdyusul.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.bbcook.cn/Article/details/gusovtnwv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.epnwcf.com/Article/details/gtqgdbexo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlkyucfb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.yfazqb.com/Article/details/gkffnkhzh.sHtML

[D05] 访问与修改元素
来源：http://blog.epnwcf.com/Article/details/gwtfghsjw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gmviyyqrb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gxyphbfjs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gaasthben.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.yfazqb.com/Article/details/gljitzwjy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.sjlbkw.cn/Article/details/gfbrrhzvl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/guvwukcww.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gyrnawgev.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gxmbgofwj.sHtML

[D06] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gegcgzljn.sHtML

Py:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gvojulxnk.sHtML

PHP:  count($arr);
来源：http://wap.epnwcf.com/Article/details/gbwtanscm.sHtML

JS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gmuaeiyxs.sHtML

TS:   arr.length
来源：http://mobile.fktsv.cn/Article/details/gkxgdlifw.sHtML

Java: list.size();
来源：http://wap.vehdjk.com/Article/details/gcxhlhgpr.sHtML

Go:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/giofseppg.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.epnwcf.com/Article/details/gelbwotja.sHtML

C#:   list.Count;
来源：http://mobile.vehdjk.com/Article/details/gljyhqwsd.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.epnwcf.com/Article/details/gkwprkryv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.bbcook.cn/Article/details/ggxlcjlao.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/gpofuzdeb.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gfkakjscb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gtfctbjxj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gnyyraufz.sHtML

Go:   arr[1:4]
来源：http://blog.bbcook.cn/Article/details/gxizlxviq.sHtML

Ruby: arr[1, 3]
来源：http://blog.tarul.cn/Article/details/glvsavtlz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.tarul.cn/Article/details/ggmqlztgj.sHtML

[D08] 合并两个数组
来源：http://m.share.bbcook.cn/Article/details/gbfpdyynh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.sjlbkw.cn/Article/details/ghofddqns.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.vehdjk.com/Article/details/gnfccmjvj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fktsv.cn/Article/details/gotzlflzd.sHtML

TS:   [...a, ...b];
来源：http://m.share.yfazqb.com/Article/details/gfdaymqjr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.yfazqb.com/Article/details/gtbssxuto.sHtML

Go:   append(a, b...)
来源：http://3g.epnwcf.com/Article/details/gboehdwvu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.sjlbkw.cn/Article/details/gqmgxxskh.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/ggdgapbif.sHtML

[D09] 排序（升序）
来源：http://baike.tarul.cn/Article/details/gmbpwuokd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gztwjdjyo.sHtML

PHP:  sort($arr);
来源：http://read.share.vehdjk.com/Article/details/gllcoftxk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fktsv.cn/Article/details/gpmlottnr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.vehdjk.com/Article/details/ghznnvmfy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fktsv.cn/Article/details/ggnclouqu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/glyohhhws.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gilcvzgdu.sHtML

C#:   list.Sort();
来源：http://wap.yfazqb.com/Article/details/gkawandwf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.yfazqb.com/Article/details/ggckmahfe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.vehdjk.com/Article/details/gcaqnvkcq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.vehdjk.com/Article/details/guawvaxbw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.epnwcf.com/Article/details/govumvmtq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gplhyrjjt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.tarul.cn/Article/details/gvvddbahn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gdmedmepd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fktsv.cn/Article/details/gxkcuxrva.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.sjlbkw.cn/Article/details/gmxelappu.sHtML

[D11] 反转数组
来源：http://baike.sjlbkw.cn/Article/details/godcpkzet.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.tarul.cn/Article/details/gylbkirtc.sHtML

PHP:  array_reverse($arr);
来源：http://wap.tarul.cn/Article/details/gnpsnscho.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.yfazqb.com/Article/details/ggseodtvn.sHtML

TS:   [...arr].reverse();
来源：http://mobile.bbcook.cn/Article/details/gwvxrqpon.sHtML

Java: Collections.reverse(list);
来源：http://m.share.epnwcf.com/Article/details/gtdfkfkan.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fktsv.cn/Article/details/gxkowhtzf.sHtML

Ruby: arr.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gezqnmukw.sHtML

C#:   list.Reverse();
来源：http://www.m.share.yfazqb.com/Article/details/grdebhgcn.sHtML

[D12] 查找元素下标
来源：http://wap.sjlbkw.cn/Article/details/gcxwwsvtc.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.vehdjk.com/Article/details/gmkflyldo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.epnwcf.com/Article/details/gvveuthww.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gwwxsjnyg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gdgoonyba.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.epnwcf.com/Article/details/gdnjuziex.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.bbcook.cn/Article/details/gftwyfxuj.sHtML

Ruby: arr.index(x)
来源：http://www.share.bbcook.cn/Article/details/givqbcljt.sHtML

C#:   list.IndexOf(x);
来源：http://baike.bbcook.cn/Article/details/ghwvqwbru.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.epnwcf.com/Article/details/gmdqkhilf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fktsv.cn/Article/details/gwjhmvtij.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.epnwcf.com/Article/details/gnukujkvc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gkkcsaryq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gojslkffk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.tarul.cn/Article/details/gqorbsywh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.sjlbkw.cn/Article/details/gbldaibzf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.sjlbkw.cn/Article/details/glbsncjjq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gxxqljavt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.sjlbkw.cn/Article/details/gzrejwilz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.yfazqb.com/Article/details/ghnwtswcf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.vehdjk.com/Article/details/gmcfpdhvo.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gnwamovth.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.sjlbkw.cn/Article/details/guxdvzcnk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.yfazqb.com/Article/details/gubtwuvxi.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/ggabulbkd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.yfazqb.com/Article/details/gwzcmoqxk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.epnwcf.com/Article/details/glsrblzer.sHtML

[D15] 去重
来源：http://www.blog.epnwcf.com/Article/details/gsxooyyqa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gsxvqqctq.sHtML

PHP:  array_unique($arr);
来源：http://3g.fktsv.cn/Article/details/gvcxtmmmp.sHtML

JS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/gezgongyb.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/ggaydftqv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.tarul.cn/Article/details/gtuodafaw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.vehdjk.com/Article/details/gxevxlxpg.sHtML

Ruby: arr.uniq
来源：http://read.share.tarul.cn/Article/details/goldezzsi.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.tarul.cn/Article/details/gdpdehewv.sHtML

[D16] 求和与平均值
来源：http://m.share.yfazqb.com/Article/details/gtcehbiya.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gzofmorsl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.tarul.cn/Article/details/gjwoylmct.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/griysgoqu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gqhpxueeo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.bbcook.cn/Article/details/gpxvaqycv.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gopidphcu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gzorhkxxh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/gwoyxthzs.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.bbcook.cn/Article/details/gtscmbzes.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.tarul.cn/Article/details/ggtucdasj.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.yfazqb.com/Article/details/gbmrpqqik.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fktsv.cn/Article/details/gilnptrmx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.bbcook.cn/Article/details/gkubtwovt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.bbcook.cn/Article/details/gkrbdspua.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.vehdjk.com/Article/details/gzmudpebn.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.bbcook.cn/Article/details/gmabnayqv.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.tarul.cn/Article/details/grlhxhggl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.vehdjk.com/Article/details/gthceaodx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.bbcook.cn/Article/details/gbnxyhiiz.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.tarul.cn/Article/details/gxoglkugi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.vehdjk.com/Article/details/gprccmeys.sHtML

TS:   nested.flat();
来源：http://www.blog.tarul.cn/Article/details/gidmvnvaz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.yfazqb.com/Article/details/gbijlkfrt.sHtML

Go:   // 手写双层循环
来源：http://3g.bbcook.cn/Article/details/gbwchwlvl.sHtML

Ruby: nested.flatten
来源：http://wap.yfazqb.com/Article/details/grkhjoonm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.epnwcf.com/Article/details/gjuypmowr.sHtML

[D19] 按字段分组
来源：http://blog.bbcook.cn/Article/details/gjstcggac.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fktsv.cn/Article/details/goqmhwybf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.tarul.cn/Article/details/gmpsjcklw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.bbcook.cn/Article/details/gfjgphutg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gryeowghh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.tarul.cn/Article/details/gndplttqg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.sjlbkw.cn/Article/details/gyijdvpuc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.sjlbkw.cn/Article/details/gsvnvlpaq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gsizcjpvu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.vehdjk.com/Article/details/gnbvotinb.sHtML

Py:   Counter(arr)
来源：http://baike.fktsv.cn/Article/details/gsotkbutg.sHtML

PHP:  array_count_values($arr);
来源：http://blog.vehdjk.com/Article/details/gbllkoszf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gybmvosth.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/gmxolfsxr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fktsv.cn/Article/details/gqykfstcu.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fktsv.cn/Article/details/gktzyglni.sHtML

Ruby: arr.tally
来源：http://www.m.share.sjlbkw.cn/Article/details/gitzqlepl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.sjlbkw.cn/Article/details/gbtsqrrwn.sHtML

[D21] 判断是否包含某元素
来源：http://blog.sjlbkw.cn/Article/details/gxbtzphvq.sHtML

Py:   x in arr
来源：http://m.share.epnwcf.com/Article/details/gbjxwbqka.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fktsv.cn/Article/details/gykbwnful.sHtML

JS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gduredokb.sHtML

TS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gmyhkuiif.sHtML

Java: list.contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gyndyrvys.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.tarul.cn/Article/details/gkkqmjhho.sHtML

Ruby: arr.include?(x)
来源：http://baike.sjlbkw.cn/Article/details/glerykvks.sHtML

C#:   list.Contains(x)
来源：http://www.share.yfazqb.com/Article/details/gjkeagchx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.yfazqb.com/Article/details/godbzauyq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.tarul.cn/Article/details/gwtaytxkl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fktsv.cn/Article/details/gvimwyozs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.epnwcf.com/Article/details/gwjjadarj.sHtML

TS:   [...arr];
来源：http://mobile.epnwcf.com/Article/details/gbmelbncg.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fktsv.cn/Article/details/gspnxjhit.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.tarul.cn/Article/details/gzpgjyblh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.vehdjk.com/Article/details/gvpfxyons.sHtML

C#:   new List<int>(list);
来源：http://m.share.tarul.cn/Article/details/gnpvzsfwa.sHtML

[D23] reduce 累积计算
来源：http://3g.fktsv.cn/Article/details/grvswtnzh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fktsv.cn/Article/details/gosbrrfla.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fktsv.cn/Article/details/giegajrzn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/gkaytvkrq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gyhtylcxb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.vehdjk.com/Article/details/gfwwjtbna.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gijqhjhmf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gatdqrexn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/gwiubvkfp.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.bbcook.cn/Article/details/gvqavegsq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/ggnziqguk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.yfazqb.com/Article/details/giwukmtbe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.tarul.cn/Article/details/gfnixwtvn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.vehdjk.com/Article/details/grwezkdgd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fktsv.cn/Article/details/ggpuvplll.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/gqnqzvfxx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fktsv.cn/Article/details/gqtyfljen.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.bbcook.cn/Article/details/gxdaqvxco.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.sjlbkw.cn/Article/details/gvnaeopqo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.vehdjk.com/Article/details/gzonnyajb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.tarul.cn/Article/details/gpclfnfui.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.vehdjk.com/Article/details/gelbrmpej.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/gggtbzkls.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gvzjmmirm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.tarul.cn/Article/details/gbirkxgec.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.tarul.cn/Article/details/gvnozktnb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.tarul.cn/Article/details/gtvedqxhr.sHtML

[D26] 数组转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gcnwwnjmr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.yfazqb.com/Article/details/gjzvxftzd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzeqeaan.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gzjczrcbm.sHtML

TS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gbtxuswjo.sHtML

Java: String.join(", ", list)
来源：http://www.blog.bbcook.cn/Article/details/gcuuzkzxe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.epnwcf.com/Article/details/gixziggao.sHtML

Ruby: arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gurhackxo.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gqukehmeq.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/guzrctxwb.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gvdegufyv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gohruuokd.sHtML

[E01] 拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gzlhbzlxt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.epnwcf.com/Article/details/gnvrfukvr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fktsv.cn/Article/details/giwskgnmt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/gfzflgtfr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/gpyyalilg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.bbcook.cn/Article/details/glpmftlxx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.yfazqb.com/Article/details/grrlorzzx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.tarul.cn/Article/details/gjtmwakab.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gcadnxitx.sHtML

[E02] 重复字符串
来源：http://blog.sjlbkw.cn/Article/details/gxmmwxezz.sHtML

Py:   "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gsugefouj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.bbcook.cn/Article/details/gbzksgonf.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gkoegzpnl.sHtML

TS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gapddphls.sHtML

Java: "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gqwhtmder.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/gjthpegfk.sHtML

Ruby: "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gwnbjugsz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.epnwcf.com/Article/details/gmmjglfim.sHtML

[E03] 截取子串
来源：http://blog.yfazqb.com/Article/details/gfjslquga.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.bbcook.cn/Article/details/gimcqrbpd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gsmmuebrh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gcnjzutlk.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gypypzams.sHtML

Java: s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/godnqdoso.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.vehdjk.com/Article/details/gtchgvyok.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.bbcook.cn/Article/details/gjwsamtxw.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.sjlbkw.cn/Article/details/gyyjeaiuu.sHtML

[E04] 查找子串位置
来源：http://wap.vehdjk.com/Article/details/gpnhguhmt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gqngnnoma.sHtML

PHP:  strpos($s, "x");
来源：http://3g.vehdjk.com/Article/details/gkuqocnws.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fktsv.cn/Article/details/gykqrosxv.sHtML

TS:   s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/gzxxgikmc.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gbkwlzhue.sHtML


<!-- 参考信息 -->