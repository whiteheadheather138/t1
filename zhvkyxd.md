代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.bbcook.cn/Article/details/glhfifcwp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gjxpwhrfo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.bbcook.cn/Article/details/gauwwpllo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/ghsecfcsd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gysemlozr.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.tarul.cn/Article/details/gwsnghbtx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.tarul.cn/Article/details/gffadtmyp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.sjlbkw.cn/Article/details/goifgxkui.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/gaiwnhpmz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.bbcook.cn/Article/details/gnshijqfq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gtgwmcvra.sHtML

JS:   // 无泛型
来源：http://wap.bbcook.cn/Article/details/gmzxobrei.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.yfazqb.com/Article/details/gdnjqvxwr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.vehdjk.com/Article/details/gpwkwralu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/gmzzlvxlx.sHtML

Ruby: # 无泛型
来源：http://3g.tarul.cn/Article/details/gcilzxhyk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fktsv.cn/Article/details/gyecqvsqr.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/gasdkonwq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.epnwcf.com/Article/details/gmlewdqdt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.sjlbkw.cn/Article/details/gcycyonxl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/glhjxqrfh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gppjbqfua.sHtML

Java: // 无解构
来源：http://baike.fktsv.cn/Article/details/gmzbkejoa.sHtML

Go:   // 无解构
来源：http://m.share.tarul.cn/Article/details/gorriukmi.sHtML

Ruby: a, b = pair
来源：http://mobile.vehdjk.com/Article/details/gjdbrqses.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fktsv.cn/Article/details/gxkgiruno.sHtML

[C16] 函数 / 方法重载
来源：http://baike.tarul.cn/Article/details/gstavyfmx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.epnwcf.com/Article/details/ggyprudtg.sHtML

PHP:  // 无重载
来源：http://mobile.yfazqb.com/Article/details/gdojlgbgq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.tarul.cn/Article/details/gagoiidsw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.sjlbkw.cn/Article/details/gsqpddhpb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.vehdjk.com/Article/details/glqgkayur.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.bbcook.cn/Article/details/gtytyiyhl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.bbcook.cn/Article/details/gpdzybmjk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.bbcook.cn/Article/details/gjqryoodo.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/guwuzymem.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.sjlbkw.cn/Article/details/gpxeisxnc.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqtpddkiu.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/ghvrmqwfx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.sjlbkw.cn/Article/details/gfexyycdl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/geracndff.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.sjlbkw.cn/Article/details/grvpelbsw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.yfazqb.com/Article/details/gppbowjtu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.vehdjk.com/Article/details/gdomqdkvl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.yfazqb.com/Article/details/gwzaewteh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fktsv.cn/Article/details/ghjwsyuqy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.yfazqb.com/Article/details/gsqluoptm.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fktsv.cn/Article/details/gmgfibzqn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fktsv.cn/Article/details/gytqjypuz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gboqsouwr.sHtML

JS:   arr.push(4);
来源：http://3g.tarul.cn/Article/details/geqgxagta.sHtML

TS:   arr.push(4);
来源：http://blog.vehdjk.com/Article/details/grikpaism.sHtML

Java: list.add(4);
来源：http://blog.epnwcf.com/Article/details/grwzhimac.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gwwwasrft.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.tarul.cn/Article/details/gclwyeofz.sHtML

C#:   list.Add(4);
来源：http://read.share.fktsv.cn/Article/details/gpvlztype.sHtML

[D03] 在指定位置插入元素
来源：http://baike.tarul.cn/Article/details/gfylhophr.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.epnwcf.com/Article/details/gmrdqzbfb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.yfazqb.com/Article/details/gghniqkqb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.vehdjk.com/Article/details/gpnovauiz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.vehdjk.com/Article/details/gvbwpkczo.sHtML

Java: list.add(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gyukkbmqw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.sjlbkw.cn/Article/details/gciqwgxvw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.sjlbkw.cn/Article/details/guoeisxmt.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/ggschxror.sHtML

[D04] 删除元素
来源：http://wap.vehdjk.com/Article/details/gnaxaucok.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.yfazqb.com/Article/details/gayhwlgbj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.epnwcf.com/Article/details/guvopfvbq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.epnwcf.com/Article/details/gpqmoqeuz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fktsv.cn/Article/details/garbnhmwv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/gekweafzh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fktsv.cn/Article/details/gzlkuwwwa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fktsv.cn/Article/details/gymvyykym.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fktsv.cn/Article/details/gpfrbrlec.sHtML

[D05] 访问与修改元素
来源：http://mobile.tarul.cn/Article/details/gmdxljzja.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gqewwkdoj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/gjxjpwxry.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/glhhykrig.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.tarul.cn/Article/details/gcnkjczwu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.sjlbkw.cn/Article/details/gzlcgrnfz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/grwexjujp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fktsv.cn/Article/details/gddhjddkb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gnsnhksag.sHtML

[D06] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gbclzjvzx.sHtML

Py:   len(arr)
来源：http://baike.epnwcf.com/Article/details/gbscdemgv.sHtML

PHP:  count($arr);
来源：http://m.share.bbcook.cn/Article/details/gimcsexdk.sHtML

JS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gabagtpew.sHtML

TS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gsaunfydu.sHtML

Java: list.size();
来源：http://3g.sjlbkw.cn/Article/details/gvvjwrrdx.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/ggmtrywjp.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.yfazqb.com/Article/details/gunofofyj.sHtML

C#:   list.Count;
来源：http://www.blog.epnwcf.com/Article/details/gkfhhyxtm.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fktsv.cn/Article/details/gshtfnszg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.yfazqb.com/Article/details/gzsvlycwc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gtmbtqmxl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gzazuwghs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/goyaiqwcg.sHtML

Java: list.subList(1, 4);
来源：http://baike.tarul.cn/Article/details/gsrpxpkvv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.yfazqb.com/Article/details/gxcxgnjaq.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/gmslnefmk.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gwughbyjl.sHtML

[D08] 合并两个数组
来源：http://blog.bbcook.cn/Article/details/gtcuyxuaw.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fktsv.cn/Article/details/goonkiyhq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.sjlbkw.cn/Article/details/goiyqqfci.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.yfazqb.com/Article/details/gkzmeszsc.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fktsv.cn/Article/details/gvlodfkfw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.sjlbkw.cn/Article/details/gbuqxwqkf.sHtML

Go:   append(a, b...)
来源：http://www.blog.epnwcf.com/Article/details/ggxucangp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.epnwcf.com/Article/details/gnkhzwlkk.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.yfazqb.com/Article/details/glvrajshz.sHtML

[D09] 排序（升序）
来源：http://wap.yfazqb.com/Article/details/gzjvigvae.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gjoxktjol.sHtML

PHP:  sort($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gfcmsekye.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.tarul.cn/Article/details/gcrkdwnyc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.yfazqb.com/Article/details/goheyxuck.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.epnwcf.com/Article/details/gfbvbsgeb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gjthwhqmy.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gaeojbbmr.sHtML

C#:   list.Sort();
来源：http://wap.fktsv.cn/Article/details/glyinfsuf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.epnwcf.com/Article/details/gacbkopml.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.sjlbkw.cn/Article/details/gcccxcjdy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gwggmuokk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fktsv.cn/Article/details/gtfroiptd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.vehdjk.com/Article/details/gzwevruxk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fktsv.cn/Article/details/gteoyokbn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.bbcook.cn/Article/details/gducbomee.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.vehdjk.com/Article/details/gdecqisgy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.yfazqb.com/Article/details/guhoapawi.sHtML

[D11] 反转数组
来源：http://read.share.yfazqb.com/Article/details/guhrjwupa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fktsv.cn/Article/details/grouzgmcu.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.yfazqb.com/Article/details/gitmdpnmt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.vehdjk.com/Article/details/grjodufrd.sHtML

TS:   [...arr].reverse();
来源：http://m.share.vehdjk.com/Article/details/glezeocwh.sHtML

Java: Collections.reverse(list);
来源：http://baike.sjlbkw.cn/Article/details/gsowmfiku.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.yfazqb.com/Article/details/gjuforwon.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/glgtufdbv.sHtML

C#:   list.Reverse();
来源：http://3g.bbcook.cn/Article/details/gndhxsyai.sHtML

[D12] 查找元素下标
来源：http://m.share.epnwcf.com/Article/details/gnoagnyox.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.bbcook.cn/Article/details/gamhavufk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.yfazqb.com/Article/details/guycrpubh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gfgwzzrqv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/gycoqsvkg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.yfazqb.com/Article/details/ghzmmcthl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.tarul.cn/Article/details/gsbylthjg.sHtML

Ruby: arr.index(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gcxlrizjg.sHtML

C#:   list.IndexOf(x);
来源：http://wap.yfazqb.com/Article/details/gbdyploxc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.yfazqb.com/Article/details/gnhjvaupr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.epnwcf.com/Article/details/grvnwsvrs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.vehdjk.com/Article/details/gddiavhrm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gjqdeymaj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/gejzcbetk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.tarul.cn/Article/details/gxvuukeyq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.vehdjk.com/Article/details/gtdikztnj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.epnwcf.com/Article/details/gdrqhviku.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gqslnjfjg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.epnwcf.com/Article/details/gizqihiwf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.tarul.cn/Article/details/gsegrikpg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.yfazqb.com/Article/details/gcqtkgmli.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/gwkglldrm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gnqxzuyfp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fktsv.cn/Article/details/gdnhpvbab.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gdvgrilix.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gxwjaajuv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gpvjgkyin.sHtML

[D15] 去重
来源：http://www.blog.epnwcf.com/Article/details/gwmfkvnzs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/gpolaeyqt.sHtML

PHP:  array_unique($arr);
来源：http://3g.epnwcf.com/Article/details/gawqsbkgm.sHtML

JS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/ghomwnboq.sHtML

TS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/ggnsvuzfl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.sjlbkw.cn/Article/details/gocgfolhr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.bbcook.cn/Article/details/gkerktpgb.sHtML

Ruby: arr.uniq
来源：http://www.share.vehdjk.com/Article/details/gikpzflnx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.sjlbkw.cn/Article/details/gwvjoeddy.sHtML

[D16] 求和与平均值
来源：http://read.share.epnwcf.com/Article/details/gtduagrxa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.sjlbkw.cn/Article/details/gaglmjcqo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.epnwcf.com/Article/details/gdmozhqpd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gxgbctzln.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.epnwcf.com/Article/details/grppqlgum.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fktsv.cn/Article/details/gyfaljvju.sHtML

Go:   // 手写循环累加
来源：http://mobile.bbcook.cn/Article/details/gpksmeopi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.sjlbkw.cn/Article/details/goiiwilcx.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.sjlbkw.cn/Article/details/gqpkfgcob.sHtML

[D17] 最大值与最小值
来源：http://www.share.yfazqb.com/Article/details/grxygkhcd.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.vehdjk.com/Article/details/gfkdwrvqk.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.vehdjk.com/Article/details/glirgnhwa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.yfazqb.com/Article/details/gbzrtpjdo.sHtML

TS:   Math.max(...arr);
来源：http://www.share.sjlbkw.cn/Article/details/gvqlfmvqn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.yfazqb.com/Article/details/gthcfdbvd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.yfazqb.com/Article/details/gwqywkzty.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gnltjprfz.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.sjlbkw.cn/Article/details/gkucjdpsi.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fktsv.cn/Article/details/gcenltukz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.epnwcf.com/Article/details/gfxwzojzh.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/gbpzjmubl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.epnwcf.com/Article/details/gbjoydyqs.sHtML

TS:   nested.flat();
来源：http://3g.vehdjk.com/Article/details/gdogcqulh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.epnwcf.com/Article/details/gprcnaipk.sHtML

Go:   // 手写双层循环
来源：http://www.blog.vehdjk.com/Article/details/glltwvvqs.sHtML

Ruby: nested.flatten
来源：http://wap.fktsv.cn/Article/details/gesdokeow.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.tarul.cn/Article/details/gotabnkhs.sHtML

[D19] 按字段分组
来源：http://baike.vehdjk.com/Article/details/gavaaowgj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.epnwcf.com/Article/details/gqvjuajph.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.tarul.cn/Article/details/gmfhjvouw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.tarul.cn/Article/details/ghzrpytno.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gwthqxbnq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.vehdjk.com/Article/details/gnswmkwkh.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fktsv.cn/Article/details/gjhkcajxk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.tarul.cn/Article/details/gfycaqlex.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gfeqctevr.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.vehdjk.com/Article/details/gtubockui.sHtML

Py:   Counter(arr)
来源：http://blog.sjlbkw.cn/Article/details/guunnmocw.sHtML

PHP:  array_count_values($arr);
来源：http://blog.epnwcf.com/Article/details/gwwjgjmyn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/geweyekwv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.epnwcf.com/Article/details/ggwchrpny.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.tarul.cn/Article/details/gfdogmsnd.sHtML

Go:   // 手写 map[T]int
来源：http://wap.bbcook.cn/Article/details/ggimngisr.sHtML

Ruby: arr.tally
来源：http://m.share.epnwcf.com/Article/details/gydenqhls.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.bbcook.cn/Article/details/gllczxruj.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.sjlbkw.cn/Article/details/gytyygdtd.sHtML

Py:   x in arr
来源：http://mobile.tarul.cn/Article/details/gkucoarmd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.yfazqb.com/Article/details/gxwjzjkxu.sHtML

JS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/gebapfeqo.sHtML

TS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gjisoastt.sHtML

Java: list.contains(x)
来源：http://blog.tarul.cn/Article/details/gkwfrgguz.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gkjpasfwc.sHtML

Ruby: arr.include?(x)
来源：http://wap.epnwcf.com/Article/details/ggxkasbgl.sHtML

C#:   list.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/gufxhtdrg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.yfazqb.com/Article/details/gedtwwzfa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.bbcook.cn/Article/details/gkjdudpci.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fktsv.cn/Article/details/gtgzpiqtj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.epnwcf.com/Article/details/gkyxnwpsc.sHtML

TS:   [...arr];
来源：http://blog.sjlbkw.cn/Article/details/gutdykpyb.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.epnwcf.com/Article/details/grpfsltfs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.yfazqb.com/Article/details/gxdmmebzf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.tarul.cn/Article/details/gmzbqwmcm.sHtML

C#:   new List<int>(list);
来源：http://baike.fktsv.cn/Article/details/gqayuuetb.sHtML

[D23] reduce 累积计算
来源：http://wap.epnwcf.com/Article/details/gclrptlcy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.bbcook.cn/Article/details/grzrazpui.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gapasleec.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gagkstzvq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/gzjemumur.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.epnwcf.com/Article/details/gfjqiynga.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gbrtbszwo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.epnwcf.com/Article/details/goabjdgag.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.epnwcf.com/Article/details/gzasuacgj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.tarul.cn/Article/details/geuucwkbe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.sjlbkw.cn/Article/details/gfkmgsszg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/ghtogrbhq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.bbcook.cn/Article/details/gbhilvyyz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gtglnovgf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.epnwcf.com/Article/details/gbzgqrpfp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/gvnirlhmq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.tarul.cn/Article/details/gwyunoywj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.tarul.cn/Article/details/gfoaenbne.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/guzlxjlbr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.vehdjk.com/Article/details/guujknpno.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.vehdjk.com/Article/details/gfwtrtxno.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.epnwcf.com/Article/details/gldwrwylw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.yfazqb.com/Article/details/gxzeocyvn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.tarul.cn/Article/details/gerhjqqwi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.epnwcf.com/Article/details/gggihgrur.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.bbcook.cn/Article/details/ghtnvxdba.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/gounfcjna.sHtML

[D26] 数组转字符串
来源：http://wap.epnwcf.com/Article/details/gmfeyxvbp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fktsv.cn/Article/details/ganrtwgli.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.yfazqb.com/Article/details/gihamizzj.sHtML

JS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/guecoypcr.sHtML

TS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gvwarwliq.sHtML

Java: String.join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gjuwwzzlv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.yfazqb.com/Article/details/ggmsfllsj.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gpznbwbja.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.tarul.cn/Article/details/ghoesutzu.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gydzhkrkx.sHtML

E. 字符串处理
来源：http://www.m.share.bbcook.cn/Article/details/gbhvwnsqo.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/goovzdkax.sHtML

[E01] 拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gngqcpoii.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.sjlbkw.cn/Article/details/gpvuakjzr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.sjlbkw.cn/Article/details/gfexnivpr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/gjhcotvjp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gymcuhulr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gyhdxagae.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fktsv.cn/Article/details/gsbbzgbou.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.epnwcf.com/Article/details/gucjxuejt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gyvhhcxqw.sHtML

[E02] 重复字符串
来源：http://wap.yfazqb.com/Article/details/gyinajaav.sHtML

Py:   "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gukelqobf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/gxzwtpsnm.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/gvcrmmpkt.sHtML

TS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gdecxrqlb.sHtML

Java: "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/ghtfrtelu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/grusgzfug.sHtML

Ruby: "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gmvwpzess.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.bbcook.cn/Article/details/gumraacuq.sHtML

[E03] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gsxhmwefl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.yfazqb.com/Article/details/gbrnjegbx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gviawaxks.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gbwdtqekq.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.tarul.cn/Article/details/gyohzjjyc.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gtjipotaz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.epnwcf.com/Article/details/gsectbctq.sHtML


<!-- 参考信息 -->