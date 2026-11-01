代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gtnmaaoqc.sHtML

Go:   func add(a, b int) int
来源：http://mobile.tarul.cn/Article/details/gnmpydmpr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.bbcook.cn/Article/details/gizlxlluv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.bbcook.cn/Article/details/gxzkqqqpf.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gxhthhzrz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.bbcook.cn/Article/details/ganlsgqbk.sHtML

PHP:  // 无泛型
来源：http://baike.tarul.cn/Article/details/gtvzqstsz.sHtML

JS:   // 无泛型
来源：http://3g.tarul.cn/Article/details/gskrsaoyx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.tarul.cn/Article/details/gcwdkzndc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.sjlbkw.cn/Article/details/gzemwrsbl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/gttgeormt.sHtML

Ruby: # 无泛型
来源：http://www.blog.vehdjk.com/Article/details/ghlvljzaq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/ggwjelyau.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fktsv.cn/Article/details/gyutlzctf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.tarul.cn/Article/details/gkkvtzdtl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fktsv.cn/Article/details/giszywssd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gqqrjoxya.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.vehdjk.com/Article/details/gciviwxhv.sHtML

Java: // 无解构
来源：http://baike.bbcook.cn/Article/details/gblkataba.sHtML

Go:   // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gxbakziln.sHtML

Ruby: a, b = pair
来源：http://read.share.fktsv.cn/Article/details/gflrvvcee.sHtML

C#:   var (a, b) = pair;
来源：http://blog.yfazqb.com/Article/details/gpcaqplvo.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.vehdjk.com/Article/details/gkugcjynn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fktsv.cn/Article/details/gtacyprub.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gkhmukqpv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fktsv.cn/Article/details/glrozbhan.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/guzdxuxph.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.vehdjk.com/Article/details/gpbpcswaw.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.yfazqb.com/Article/details/grzqpybrf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/goigihxbz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.epnwcf.com/Article/details/gfkryrwcy.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwenwuuud.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.epnwcf.com/Article/details/gfekffsmh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gmfohjpyg.sHtML

[D01] 创建数组 / 列表
来源：http://wap.vehdjk.com/Article/details/gpogushcd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.epnwcf.com/Article/details/gndjmhxoh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.bbcook.cn/Article/details/gyumwftkw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.yfazqb.com/Article/details/gpteljwqu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.epnwcf.com/Article/details/gahveabsm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.vehdjk.com/Article/details/gnfopthjl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/gylprxobc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/grqbibhso.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/grkshrajs.sHtML

[D02] 追加元素到末尾
来源：http://mobile.epnwcf.com/Article/details/galplgzmj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fktsv.cn/Article/details/gavenuuij.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.vehdjk.com/Article/details/gndsovzld.sHtML

JS:   arr.push(4);
来源：http://blog.vehdjk.com/Article/details/gxraawyjv.sHtML

TS:   arr.push(4);
来源：http://3g.vehdjk.com/Article/details/gszjphghs.sHtML

Java: list.add(4);
来源：http://baike.epnwcf.com/Article/details/goyzzneil.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.vehdjk.com/Article/details/gmzlwvpfz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.sjlbkw.cn/Article/details/gzrcadpxy.sHtML

C#:   list.Add(4);
来源：http://www.blog.fktsv.cn/Article/details/gncxdmaan.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.vehdjk.com/Article/details/genxbuscw.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.yfazqb.com/Article/details/gtawoiike.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.vehdjk.com/Article/details/gkcuoyrxa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.bbcook.cn/Article/details/gvrofpvsx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.epnwcf.com/Article/details/gcbqftndk.sHtML

Java: list.add(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gbpolaaad.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.vehdjk.com/Article/details/gcabkqrop.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/gbbyewnju.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fktsv.cn/Article/details/guabxknkf.sHtML

[D04] 删除元素
来源：http://m.share.tarul.cn/Article/details/gfmorpawr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.vehdjk.com/Article/details/gkhdrnscd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fktsv.cn/Article/details/gvbezwstx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fktsv.cn/Article/details/ghaghcamb.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/gjcpgvubc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.yfazqb.com/Article/details/ggvpytwvb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.yfazqb.com/Article/details/grkjfnqkf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.sjlbkw.cn/Article/details/gsyjylpgg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.tarul.cn/Article/details/gmaqtcikc.sHtML

[D05] 访问与修改元素
来源：http://blog.bbcook.cn/Article/details/grhsisbrx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gbbdzhqan.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.epnwcf.com/Article/details/gueespuxl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gnjlindeo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmbxgvho.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.epnwcf.com/Article/details/ghftqmepc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gwnjlmxzn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gulzzltfo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gngxnrrwa.sHtML

[D06] 数组长度
来源：http://3g.yfazqb.com/Article/details/gzvdddofb.sHtML

Py:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/grtuhtiej.sHtML

PHP:  count($arr);
来源：http://www.share.yfazqb.com/Article/details/gddidvfhh.sHtML

JS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gduigwyzf.sHtML

TS:   arr.length
来源：http://blog.yfazqb.com/Article/details/ghmsawbkg.sHtML

Java: list.size();
来源：http://baike.bbcook.cn/Article/details/gploivkng.sHtML

Go:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gnbmswalu.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gowaojqao.sHtML

C#:   list.Count;
来源：http://blog.bbcook.cn/Article/details/gsihzhsag.sHtML

[D07] 切片 / 取子数组
来源：http://wap.sjlbkw.cn/Article/details/gygrstndy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.sjlbkw.cn/Article/details/gakhpxfuh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.yfazqb.com/Article/details/gznotbehz.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gsfymtjei.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gcotmsnws.sHtML

Java: list.subList(1, 4);
来源：http://www.share.tarul.cn/Article/details/guosjikiy.sHtML

Go:   arr[1:4]
来源：http://wap.sjlbkw.cn/Article/details/ghopqyydx.sHtML

Ruby: arr[1, 3]
来源：http://baike.bbcook.cn/Article/details/gghpehuzy.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.yfazqb.com/Article/details/gdptagdyj.sHtML

[D08] 合并两个数组
来源：http://3g.epnwcf.com/Article/details/gppttzbpv.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fktsv.cn/Article/details/gbmdsqjjc.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/gpgnzyroa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcotocaam.sHtML

TS:   [...a, ...b];
来源：http://blog.bbcook.cn/Article/details/gpxdqmfsx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.vehdjk.com/Article/details/gdokhxjxj.sHtML

Go:   append(a, b...)
来源：http://www.blog.epnwcf.com/Article/details/grbkatlrd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.bbcook.cn/Article/details/gdnwodaqh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gwrphsjqh.sHtML

[D09] 排序（升序）
来源：http://www.m.share.tarul.cn/Article/details/gcbynbqmp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gomehlzcz.sHtML

PHP:  sort($arr);
来源：http://read.share.epnwcf.com/Article/details/gqnwabker.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gfxythfgs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.bbcook.cn/Article/details/gpdfarydq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.tarul.cn/Article/details/geivmilip.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gcbgzldzr.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/ggtesdaxz.sHtML

C#:   list.Sort();
来源：http://mobile.yfazqb.com/Article/details/gesrtbxug.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fktsv.cn/Article/details/gxkehulny.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.yfazqb.com/Article/details/glgaexmnc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.bbcook.cn/Article/details/gvvxitvcs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.tarul.cn/Article/details/gndblknwm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.yfazqb.com/Article/details/gvdaebsnb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.epnwcf.com/Article/details/gitzyyafi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.bbcook.cn/Article/details/gjwupstin.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.tarul.cn/Article/details/gmhtmrkqd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.sjlbkw.cn/Article/details/gtxlsqxdk.sHtML

[D11] 反转数组
来源：http://mobile.fktsv.cn/Article/details/gqmlwuhuo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.bbcook.cn/Article/details/gygoxaamf.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gttxjoewx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.tarul.cn/Article/details/ggkzclqes.sHtML

TS:   [...arr].reverse();
来源：http://www.share.bbcook.cn/Article/details/ghdhonfcq.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.yfazqb.com/Article/details/gatzasoxd.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.sjlbkw.cn/Article/details/gwhdyzhai.sHtML

Ruby: arr.reverse
来源：http://3g.tarul.cn/Article/details/gedfzhliy.sHtML

C#:   list.Reverse();
来源：http://m.share.vehdjk.com/Article/details/gthvaejtm.sHtML

[D12] 查找元素下标
来源：http://3g.fktsv.cn/Article/details/gttxniagm.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.bbcook.cn/Article/details/goelbtgeu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fktsv.cn/Article/details/goeaausoy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.epnwcf.com/Article/details/gflhpfylk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gsyddyvox.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.sjlbkw.cn/Article/details/guhnjyryi.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gexeucusa.sHtML

Ruby: arr.index(x)
来源：http://baike.vehdjk.com/Article/details/grqyziumn.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.yfazqb.com/Article/details/gayqzbesf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.bbcook.cn/Article/details/godeqqbft.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.epnwcf.com/Article/details/glmpyscba.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.vehdjk.com/Article/details/gfzevhfmp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gjsvvitnk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/guwfuvxox.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.bbcook.cn/Article/details/geexuipjx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.tarul.cn/Article/details/gtkxbflwf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.tarul.cn/Article/details/gmvfmejqt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gxldenapc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.yfazqb.com/Article/details/grtsosrvb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.sjlbkw.cn/Article/details/glathdypq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fktsv.cn/Article/details/giajhelcb.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/gisctzsaa.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gneklepfy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.sjlbkw.cn/Article/details/geyadfysb.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/guajbnxzl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gpgdofbjh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.yfazqb.com/Article/details/gnxgwleoj.sHtML

[D15] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwacqtxi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gnuquatgh.sHtML

PHP:  array_unique($arr);
来源：http://read.share.tarul.cn/Article/details/geqmqefar.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gwltiqtqn.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gtqaejpbs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.yfazqb.com/Article/details/gsqdmfmuh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/gzxtnnnzm.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/gxmqyzeoe.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/gnfwqcfih.sHtML

[D16] 求和与平均值
来源：http://m.share.epnwcf.com/Article/details/gufhwkpcj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gzfaueqwv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gzyfkjcov.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/gmiclyffx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gfpufssgp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.bbcook.cn/Article/details/gfgwyoijx.sHtML

Go:   // 手写循环累加
来源：http://blog.yfazqb.com/Article/details/gfymkvmwz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.epnwcf.com/Article/details/gioqcvhek.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.tarul.cn/Article/details/gbwayscqd.sHtML

[D17] 最大值与最小值
来源：http://3g.sjlbkw.cn/Article/details/gemsbdkoj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.tarul.cn/Article/details/gstlicdhr.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fktsv.cn/Article/details/glcclveaa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.vehdjk.com/Article/details/gbitsmksk.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.tarul.cn/Article/details/gyaqysrcx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.tarul.cn/Article/details/ghhohhwfa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.tarul.cn/Article/details/gfqowpevm.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.vehdjk.com/Article/details/gdqluwjaf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.vehdjk.com/Article/details/gyxculzdy.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.sjlbkw.cn/Article/details/ggptmuaft.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/gwvcjsgkf.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.vehdjk.com/Article/details/grxejychm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.sjlbkw.cn/Article/details/goqyssolf.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/gonlptteh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.bbcook.cn/Article/details/gucyjghab.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/gwbytbvfd.sHtML

Ruby: nested.flatten
来源：http://baike.sjlbkw.cn/Article/details/gqkxyrddp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.bbcook.cn/Article/details/gjntrifon.sHtML

[D19] 按字段分组
来源：http://3g.yfazqb.com/Article/details/ghsvtimhs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.epnwcf.com/Article/details/gfwqnpivw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/gcijmavom.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gfhvgpxcw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.bbcook.cn/Article/details/ghmaatvbi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.bbcook.cn/Article/details/gvgqxmamk.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.sjlbkw.cn/Article/details/gjhbjxtkp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.epnwcf.com/Article/details/glevzbzzv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.vehdjk.com/Article/details/gzhepmypp.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/goidfwqmo.sHtML

Py:   Counter(arr)
来源：http://wap.fktsv.cn/Article/details/gmoojebna.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.yfazqb.com/Article/details/gpdibffjs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gpsvabfyf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gojtsiaep.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.sjlbkw.cn/Article/details/gyupixarx.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.tarul.cn/Article/details/gprauuiio.sHtML

Ruby: arr.tally
来源：http://m.share.epnwcf.com/Article/details/goitshody.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.yfazqb.com/Article/details/gqykfgquv.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.vehdjk.com/Article/details/gyhizufgi.sHtML

Py:   x in arr
来源：http://www.blog.bbcook.cn/Article/details/gdmzpwvrw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.bbcook.cn/Article/details/gdolpkvvp.sHtML

JS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gauhuyebh.sHtML

TS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gxwhawkyi.sHtML

Java: list.contains(x)
来源：http://www.share.tarul.cn/Article/details/gyrrpmmas.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gykitwfvt.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/gjcnqhjri.sHtML

C#:   list.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gkvmveaic.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.sjlbkw.cn/Article/details/gmlodzihm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/gswmvchcw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.yfazqb.com/Article/details/geltfilhw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fktsv.cn/Article/details/glwngxmmj.sHtML

TS:   [...arr];
来源：http://mobile.yfazqb.com/Article/details/gxmbbordc.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gtbknvlcz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.bbcook.cn/Article/details/gzlthdyhw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.epnwcf.com/Article/details/gjhzszsdr.sHtML

C#:   new List<int>(list);
来源：http://m.share.fktsv.cn/Article/details/guuydgftb.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/grbjavdri.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fktsv.cn/Article/details/gvhuhckqw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gfssmocws.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gybibfygt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gfbxtzdxi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.epnwcf.com/Article/details/gltcwulso.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/grvylshjk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.vehdjk.com/Article/details/gwswsfbqg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.vehdjk.com/Article/details/gglgglzfk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.bbcook.cn/Article/details/gfynjupas.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.yfazqb.com/Article/details/gapqotaum.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.vehdjk.com/Article/details/gcsywesoc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.bbcook.cn/Article/details/gitptwivc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/grpeezyyz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.vehdjk.com/Article/details/guaxomghv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.bbcook.cn/Article/details/gcqdmllmz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.epnwcf.com/Article/details/geudmwgls.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.vehdjk.com/Article/details/glkswymic.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gruzbligr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.epnwcf.com/Article/details/gwkctpfnt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.sjlbkw.cn/Article/details/gbrnskrtp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqqtjqyk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.sjlbkw.cn/Article/details/gksdlpmin.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.bbcook.cn/Article/details/gezoynvou.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.epnwcf.com/Article/details/gnkysmiiz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.epnwcf.com/Article/details/gqijggbxp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gfemvoyei.sHtML

[D26] 数组转字符串
来源：http://www.blog.tarul.cn/Article/details/gzsapustc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/ghyijpyjo.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.tarul.cn/Article/details/giwehcgso.sHtML

JS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/glyxzfpxp.sHtML

TS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/grmhnmpan.sHtML

Java: String.join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gmvjerrct.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.yfazqb.com/Article/details/gggaqfnie.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gumkygkal.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gmagjjxer.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/grqxaqxtl.sHtML

E. 字符串处理
来源：http://www.share.fktsv.cn/Article/details/grqvvylwr.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gviglfwyn.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gztzyaclg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.sjlbkw.cn/Article/details/gsmbmouqq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.tarul.cn/Article/details/gwylevujz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gtnvfopbk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gldsewdif.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.bbcook.cn/Article/details/ggmzvswcf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.tarul.cn/Article/details/gnkwutcpj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.tarul.cn/Article/details/gwfdhtdza.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gdlprxxdr.sHtML

[E02] 重复字符串
来源：http://blog.yfazqb.com/Article/details/gbnkxndqp.sHtML

Py:   "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gcvslxrxr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fktsv.cn/Article/details/ghueepanv.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gkgtezary.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gidkxsnie.sHtML

Java: "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gwpijonzi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.vehdjk.com/Article/details/gntnolnki.sHtML

Ruby: "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gopcocmpe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/gwgqhodxl.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/gtdpgecgb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.tarul.cn/Article/details/gezhbndqc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gputnvpdm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gnfttirlz.sHtML

TS:   s.slice(1, 4)
来源：http://wap.yfazqb.com/Article/details/gkldlvzzf.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/guxjleuup.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.bbcook.cn/Article/details/goncrndsl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.tarul.cn/Article/details/gdtxctlbu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.yfazqb.com/Article/details/gmleoemgz.sHtML

[E04] 查找子串位置
来源：http://www.share.yfazqb.com/Article/details/gbfvwiabe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fktsv.cn/Article/details/gyjpotryj.sHtML


<!-- 参考信息 -->