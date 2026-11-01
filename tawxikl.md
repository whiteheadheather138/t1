代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.share.epnwcf.com/Article/details/gccblfrgs.sHtML

C#:   using System.Text;
来源：http://m.share.epnwcf.com/Article/details/gnqjhxsdj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.epnwcf.com/Article/details/gkpjypeot.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.epnwcf.com/Article/details/gwzmacebs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.sjlbkw.cn/Article/details/gxqbmhbeg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gxqbjqmhh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gvvkjsdpx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.tarul.cn/Article/details/gytskoxkr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fktsv.cn/Article/details/gfaalayin.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.yfazqb.com/Article/details/grgqjdqwg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.yfazqb.com/Article/details/gvwhmczqt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.yfazqb.com/Article/details/gvdregstl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.yfazqb.com/Article/details/gtkrkydwo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/gtaeyrukb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.epnwcf.com/Article/details/gsjpvoyjy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/glntgozgh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gjoeotckz.sHtML

Go:   func add(a, b int) int
来源：http://www.share.tarul.cn/Article/details/ginqubnao.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.tarul.cn/Article/details/gkjoihhrq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.tarul.cn/Article/details/gijixfbfx.sHtML

[C14] 泛型函数
来源：http://wap.sjlbkw.cn/Article/details/giwovfmhh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fktsv.cn/Article/details/gmclcprgz.sHtML

PHP:  // 无泛型
来源：http://mobile.tarul.cn/Article/details/gzjrtuljy.sHtML

JS:   // 无泛型
来源：http://m.share.tarul.cn/Article/details/gpfbytweb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.tarul.cn/Article/details/gscsagvoo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.yfazqb.com/Article/details/gyfsulmgd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fktsv.cn/Article/details/giktngrfo.sHtML

Ruby: # 无泛型
来源：http://wap.vehdjk.com/Article/details/gfovjgucm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.epnwcf.com/Article/details/gtpsljibx.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/gplmxmeoc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fktsv.cn/Article/details/ggntqydla.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.bbcook.cn/Article/details/gjmhjpzcm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gyirxxesc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/goncauujc.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/grrtdanwe.sHtML

Go:   // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/gbdrqauea.sHtML

Ruby: a, b = pair
来源：http://baike.yfazqb.com/Article/details/glbuxsaqu.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.bbcook.cn/Article/details/gvjeuhdjv.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fktsv.cn/Article/details/guofkoodv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.vehdjk.com/Article/details/gqsqllvmb.sHtML

PHP:  // 无重载
来源：http://wap.vehdjk.com/Article/details/gdpavfoln.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.yfazqb.com/Article/details/gohgumvjj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fktsv.cn/Article/details/gvawkslfi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gxsdmpigb.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/grypgmyhx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fktsv.cn/Article/details/gpprywwtu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.vehdjk.com/Article/details/gtrenxvma.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gduixdozw.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.bbcook.cn/Article/details/gvxjzsqbo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gctnckgie.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.vehdjk.com/Article/details/gbnwlpsxa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.bbcook.cn/Article/details/gaapgqjvt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.bbcook.cn/Article/details/gdbjfdtum.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.vehdjk.com/Article/details/gschxtqxn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.sjlbkw.cn/Article/details/gpiznajcj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.tarul.cn/Article/details/giloikpya.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fktsv.cn/Article/details/gxtdrngkx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.vehdjk.com/Article/details/gqadzkfxa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.tarul.cn/Article/details/gvbelkglo.sHtML

[D02] 追加元素到末尾
来源：http://read.share.tarul.cn/Article/details/gikxddddx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.vehdjk.com/Article/details/gfhtkdrpv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.epnwcf.com/Article/details/gaalwsrqf.sHtML

JS:   arr.push(4);
来源：http://www.m.share.yfazqb.com/Article/details/ggtdywhqv.sHtML

TS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/glmzgwpyy.sHtML

Java: list.add(4);
来源：http://blog.sjlbkw.cn/Article/details/gszgbxlvf.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.bbcook.cn/Article/details/geuxennfn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.sjlbkw.cn/Article/details/ggxwsxubv.sHtML

C#:   list.Add(4);
来源：http://baike.vehdjk.com/Article/details/ggaoibvqh.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gifjlygwa.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.yfazqb.com/Article/details/gvmxqemlx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.tarul.cn/Article/details/gyepzrrmp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.epnwcf.com/Article/details/gczhqvcei.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.bbcook.cn/Article/details/gqxqqcerz.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gdtwrnhwz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.tarul.cn/Article/details/ggpjaqcpi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.epnwcf.com/Article/details/gosbjnylg.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.bbcook.cn/Article/details/gzcusjoxu.sHtML

[D04] 删除元素
来源：http://www.share.bbcook.cn/Article/details/gxicfiaqu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.bbcook.cn/Article/details/ghlftgsex.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fktsv.cn/Article/details/gtpwrtxkv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.bbcook.cn/Article/details/gfoposmgi.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.tarul.cn/Article/details/gurqboerv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.yfazqb.com/Article/details/ganbqenjk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.vehdjk.com/Article/details/gmshhyetz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.bbcook.cn/Article/details/gtrivzaqv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.sjlbkw.cn/Article/details/guiwcgsyp.sHtML

[D05] 访问与修改元素
来源：http://baike.fktsv.cn/Article/details/gcgaxnpax.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/ghrwneblr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gnupwpokd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gbbfdeadl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fktsv.cn/Article/details/glsvhowqi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.vehdjk.com/Article/details/guaodgnkp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gotayhumt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/ghyrprrwy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gsvukrheo.sHtML

[D06] 数组长度
来源：http://m.share.yfazqb.com/Article/details/gvfyjxbdp.sHtML

Py:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/glqiqrrjd.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gbalguqhl.sHtML

JS:   arr.length
来源：http://3g.bbcook.cn/Article/details/ghomxezrx.sHtML

TS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gfgestwic.sHtML

Java: list.size();
来源：http://www.blog.fktsv.cn/Article/details/gracctpdk.sHtML

Go:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gyvemkdck.sHtML

Ruby: arr.length; arr.size
来源：http://baike.sjlbkw.cn/Article/details/gtblkjvom.sHtML

C#:   list.Count;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkaugeql.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/gkggsiyph.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.bbcook.cn/Article/details/gmxzictdt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.yfazqb.com/Article/details/golhtmweg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/glpzkyokm.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.tarul.cn/Article/details/gfrmexwhb.sHtML

Java: list.subList(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gmqmhlytz.sHtML

Go:   arr[1:4]
来源：http://baike.fktsv.cn/Article/details/gcpyvkrcr.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.tarul.cn/Article/details/gmvogmudv.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.sjlbkw.cn/Article/details/gqbvxluiz.sHtML

[D08] 合并两个数组
来源：http://mobile.bbcook.cn/Article/details/gczojyjib.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.bbcook.cn/Article/details/gljnvezxg.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.tarul.cn/Article/details/gjgxxbfcl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.vehdjk.com/Article/details/gcypvzxgh.sHtML

TS:   [...a, ...b];
来源：http://blog.tarul.cn/Article/details/gzkyzjlsn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.bbcook.cn/Article/details/givcpygvt.sHtML

Go:   append(a, b...)
来源：http://www.m.share.bbcook.cn/Article/details/gyjhuawlg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.sjlbkw.cn/Article/details/grrtubqtu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.bbcook.cn/Article/details/glprxuxyb.sHtML

[D09] 排序（升序）
来源：http://blog.yfazqb.com/Article/details/gzgaticvx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gdhtonhjo.sHtML

PHP:  sort($arr);
来源：http://mobile.vehdjk.com/Article/details/gvvexduer.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.sjlbkw.cn/Article/details/gkvxxtgra.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.yfazqb.com/Article/details/grafdzrwu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fktsv.cn/Article/details/gzjvhdwbh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gaidzkzbe.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gppgsselo.sHtML

C#:   list.Sort();
来源：http://www.blog.sjlbkw.cn/Article/details/ggdaedmok.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.sjlbkw.cn/Article/details/gnfxwllcx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.epnwcf.com/Article/details/gptulllnl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.yfazqb.com/Article/details/gsrpqntib.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gucwidxql.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/ggqaanwpl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.yfazqb.com/Article/details/giylnupbi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.bbcook.cn/Article/details/gnqvwpqaf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.tarul.cn/Article/details/gdogiwuch.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.vehdjk.com/Article/details/gqrdbqker.sHtML

[D11] 反转数组
来源：http://read.share.bbcook.cn/Article/details/gniflland.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.sjlbkw.cn/Article/details/gtrlalpdf.sHtML

PHP:  array_reverse($arr);
来源：http://3g.yfazqb.com/Article/details/gqgzeladk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/gcinbtcrf.sHtML

TS:   [...arr].reverse();
来源：http://read.share.vehdjk.com/Article/details/gfpqcvhtj.sHtML

Java: Collections.reverse(list);
来源：http://blog.tarul.cn/Article/details/gheqthxsr.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.tarul.cn/Article/details/goyiklitv.sHtML

Ruby: arr.reverse
来源：http://wap.sjlbkw.cn/Article/details/givfjyqxm.sHtML

C#:   list.Reverse();
来源：http://www.blog.tarul.cn/Article/details/gdyerurwu.sHtML

[D12] 查找元素下标
来源：http://baike.sjlbkw.cn/Article/details/gdgrjnrbn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gkrxlssic.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gdhmccrwg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gektafcei.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/ghnvojujb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.tarul.cn/Article/details/gallppnwt.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/glhextyne.sHtML

Ruby: arr.index(x)
来源：http://m.share.fktsv.cn/Article/details/ggvjzytod.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.sjlbkw.cn/Article/details/goyddwntp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.bbcook.cn/Article/details/geczlhrvp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/ghipzxfkr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.tarul.cn/Article/details/ghokttxuy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/googzjriw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gmpjrrbrn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.sjlbkw.cn/Article/details/gepfqipdp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.epnwcf.com/Article/details/gnzllveld.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.sjlbkw.cn/Article/details/gtgznttut.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.epnwcf.com/Article/details/gpiitgxhk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.tarul.cn/Article/details/gyyxvjqmy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.tarul.cn/Article/details/gwtosuant.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gieyngaps.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/glyxqdkjg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gpettvehg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.sjlbkw.cn/Article/details/ghlrhlpek.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gfsprtwvh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.epnwcf.com/Article/details/gjvixfxqi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.tarul.cn/Article/details/grtvuthpe.sHtML

[D15] 去重
来源：http://blog.fktsv.cn/Article/details/gtkcolxpj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.bbcook.cn/Article/details/gykayumts.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.yfazqb.com/Article/details/gvdlfwipb.sHtML

JS:   [...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/gijozaxmo.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gbizrsgol.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.yfazqb.com/Article/details/gyceuhqmi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.bbcook.cn/Article/details/grtqvffkv.sHtML

Ruby: arr.uniq
来源：http://wap.bbcook.cn/Article/details/gxudokmhu.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.tarul.cn/Article/details/glkekhyyg.sHtML

[D16] 求和与平均值
来源：http://mobile.sjlbkw.cn/Article/details/gijahqiwz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/gjzvwpuhy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gmeqlomhu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gesctwjif.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gqzuftbhc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.tarul.cn/Article/details/gannsrcuq.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/gnsmdlacz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gebppqoth.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.sjlbkw.cn/Article/details/ghmluujrw.sHtML

[D17] 最大值与最小值
来源：http://3g.sjlbkw.cn/Article/details/gjzmzlxhd.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.bbcook.cn/Article/details/gtvojzbwa.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fktsv.cn/Article/details/gckymxrge.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.epnwcf.com/Article/details/gqxxeoezd.sHtML

TS:   Math.max(...arr);
来源：http://wap.fktsv.cn/Article/details/gydyztkgc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.bbcook.cn/Article/details/gcdieivmu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/ghpirmprb.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fktsv.cn/Article/details/gtksjtxqt.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.tarul.cn/Article/details/gririeceo.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.bbcook.cn/Article/details/gkjgpvdwc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.epnwcf.com/Article/details/gziqfvzip.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.tarul.cn/Article/details/gbcyxcwfv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.epnwcf.com/Article/details/gsivcblub.sHtML

TS:   nested.flat();
来源：http://www.share.fktsv.cn/Article/details/gzvvhbybx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gbuoangcg.sHtML

Go:   // 手写双层循环
来源：http://3g.vehdjk.com/Article/details/gmabzhkcw.sHtML

Ruby: nested.flatten
来源：http://blog.fktsv.cn/Article/details/gjvkeektj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fktsv.cn/Article/details/giumgckmw.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/gldkyougk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.vehdjk.com/Article/details/ggexnvizr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.epnwcf.com/Article/details/gqkfvakon.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gwjtsfylz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/ghdigxmcd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.sjlbkw.cn/Article/details/grdjmxnzj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.epnwcf.com/Article/details/ggozzjggm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.sjlbkw.cn/Article/details/geyvcmsgx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.sjlbkw.cn/Article/details/gqcrjnqjo.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.yfazqb.com/Article/details/grklvwboh.sHtML

Py:   Counter(arr)
来源：http://baike.yfazqb.com/Article/details/gddkfgzww.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/gityxbfyc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gwrtwcklj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gbuqdwcfp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.sjlbkw.cn/Article/details/gjnpxjxol.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.sjlbkw.cn/Article/details/gaadmlidj.sHtML

Ruby: arr.tally
来源：http://www.blog.fktsv.cn/Article/details/gugfectod.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gcpfdovks.sHtML

[D21] 判断是否包含某元素
来源：http://wap.yfazqb.com/Article/details/gmujlrbdy.sHtML

Py:   x in arr
来源：http://m.share.epnwcf.com/Article/details/gaaaeafkj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fktsv.cn/Article/details/gmreqhazz.sHtML

JS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gaauhpxaz.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/glxmuxfcw.sHtML

Java: list.contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gnyujtkdq.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.tarul.cn/Article/details/gukzbedep.sHtML

Ruby: arr.include?(x)
来源：http://baike.vehdjk.com/Article/details/gcmmekrlh.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gwjfbljgd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.yfazqb.com/Article/details/gxulmrfak.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fktsv.cn/Article/details/gfhqxztsq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/gerlspcun.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.bbcook.cn/Article/details/gbxdltxpb.sHtML

TS:   [...arr];
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkfbbuqy.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.epnwcf.com/Article/details/giomlykyh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gqicmtcix.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.tarul.cn/Article/details/gvcpihifo.sHtML

C#:   new List<int>(list);
来源：http://mobile.tarul.cn/Article/details/gkyllujch.sHtML

[D23] reduce 累积计算
来源：http://m.share.epnwcf.com/Article/details/gfnanimsr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.bbcook.cn/Article/details/gknbdjvmq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyeoghyp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gqqihdmfd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/gmfbnywkr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.tarul.cn/Article/details/gbqgtygji.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gmwioosnh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.vehdjk.com/Article/details/gjgogbalj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/gxfjiqqcd.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.sjlbkw.cn/Article/details/gxbhokrez.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.bbcook.cn/Article/details/gqkywhsyu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.vehdjk.com/Article/details/gpoxqraqx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.sjlbkw.cn/Article/details/gltjyfgce.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.yfazqb.com/Article/details/gniqcpeco.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.bbcook.cn/Article/details/gafggctlm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.sjlbkw.cn/Article/details/gnsytopyn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.bbcook.cn/Article/details/glcuqobef.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.yfazqb.com/Article/details/gmlkstezv.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.sjlbkw.cn/Article/details/gjieyzdwd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.bbcook.cn/Article/details/gjodfkmkb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/glclvsnws.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.vehdjk.com/Article/details/gerlsabgm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.bbcook.cn/Article/details/gwkqktkls.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.yfazqb.com/Article/details/geqooeufe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.sjlbkw.cn/Article/details/gfmjhdcvr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.bbcook.cn/Article/details/gkwrkbyuz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gukeztvwj.sHtML

[D26] 数组转字符串
来源：http://3g.vehdjk.com/Article/details/giysuitbv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.yfazqb.com/Article/details/gseagaxmn.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.tarul.cn/Article/details/gauupfkdz.sHtML

JS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gbkgpfdyh.sHtML

TS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gllwiwdvj.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gtoimzdrf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.bbcook.cn/Article/details/gukwhqhnk.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gpagbikvq.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gdcszkrwn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghddvzytm.sHtML

E. 字符串处理
来源：http://www.share.bbcook.cn/Article/details/guzxkpriz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqpmkvlgx.sHtML

[E01] 拼接字符串
来源：http://baike.fktsv.cn/Article/details/gaahffunc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.yfazqb.com/Article/details/gckudqdek.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.vehdjk.com/Article/details/gxqoavuva.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/geahscvvt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/ggozlqztq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.vehdjk.com/Article/details/gljnkhdya.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.sjlbkw.cn/Article/details/goyjtvifk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fktsv.cn/Article/details/grtnzkglt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.bbcook.cn/Article/details/geezgbgqf.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/gysxyrmwz.sHtML

Py:   "ab" * 3
来源：http://www.share.vehdjk.com/Article/details/gijrnjjdj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fktsv.cn/Article/details/gzyisepgk.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/ghvvtifjz.sHtML


<!-- 参考信息 -->