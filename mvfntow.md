代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://blog.yfazqb.com/Article/details/gnnjqpusf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.vehdjk.com/Article/details/gcodwoerb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gvtonqiib.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gdgygfgxu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.sjlbkw.cn/Article/details/gpagnvzqo.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.epnwcf.com/Article/details/glpvrvyjj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/gfxnyojjs.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.yfazqb.com/Article/details/grsszztne.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gioyctcgl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gotdhvlbn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.epnwcf.com/Article/details/grhtvekqs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gowfstyzn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gusmarssh.sHtML

Go:   func add(a, b int) int
来源：http://blog.vehdjk.com/Article/details/gpdliqtsy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.epnwcf.com/Article/details/gzzlbfiss.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.yfazqb.com/Article/details/gfvqkdero.sHtML

[C14] 泛型函数
来源：http://baike.fktsv.cn/Article/details/gyokptpgk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fktsv.cn/Article/details/gbrptydey.sHtML

PHP:  // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gurbbajnp.sHtML

JS:   // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gqqlebeuy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fktsv.cn/Article/details/gbcymfrpk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fktsv.cn/Article/details/gagdqbcaz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.sjlbkw.cn/Article/details/glrvwahoe.sHtML

Ruby: # 无泛型
来源：http://mobile.epnwcf.com/Article/details/gdimxcemg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.epnwcf.com/Article/details/gnuuvkadf.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/ghtyfhxnh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fktsv.cn/Article/details/gbzpwekhy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.vehdjk.com/Article/details/gacftrbux.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gqjkhbsto.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gqxfcxgqx.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gfbnrpchb.sHtML

Go:   // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/gursmgsqb.sHtML

Ruby: a, b = pair
来源：http://read.share.vehdjk.com/Article/details/guhnvapit.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.sjlbkw.cn/Article/details/glmrflaxh.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.sjlbkw.cn/Article/details/gdfackylz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.epnwcf.com/Article/details/gpquddksw.sHtML

PHP:  // 无重载
来源：http://mobile.yfazqb.com/Article/details/gkcdbyrvy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.bbcook.cn/Article/details/geyvomnec.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.tarul.cn/Article/details/gbxlmtjfm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fktsv.cn/Article/details/gijapsgoc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.yfazqb.com/Article/details/gfrscqhql.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.tarul.cn/Article/details/grfshxrpu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.yfazqb.com/Article/details/guzztkbpu.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grmdurfxt.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.yfazqb.com/Article/details/gvybdvflo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gcnqowgrc.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gddwrqhzf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.epnwcf.com/Article/details/geoevdwms.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gxxbeuvzk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gwvgdprkq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fktsv.cn/Article/details/glybaullc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fktsv.cn/Article/details/gixmmekgf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.epnwcf.com/Article/details/gpzgxbvhp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.tarul.cn/Article/details/grxciubvm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/ghcdpxiqb.sHtML

[D02] 追加元素到末尾
来源：http://www.share.sjlbkw.cn/Article/details/gdzmdltjs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.tarul.cn/Article/details/grdhvdpzl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.vehdjk.com/Article/details/gxlconxty.sHtML

JS:   arr.push(4);
来源：http://blog.sjlbkw.cn/Article/details/guffyyuit.sHtML

TS:   arr.push(4);
来源：http://www.blog.fktsv.cn/Article/details/goffkswvu.sHtML

Java: list.add(4);
来源：http://www.m.share.yfazqb.com/Article/details/grogfuvbg.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gqtthhxvt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.sjlbkw.cn/Article/details/gxafggpry.sHtML

C#:   list.Add(4);
来源：http://blog.sjlbkw.cn/Article/details/giwcrvgus.sHtML

[D03] 在指定位置插入元素
来源：http://blog.yfazqb.com/Article/details/gqbointvb.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.tarul.cn/Article/details/gamlxtbeb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fktsv.cn/Article/details/gujdnkgdv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fktsv.cn/Article/details/gtdpcqtig.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gfhsxortm.sHtML

Java: list.add(0, 0);
来源：http://baike.yfazqb.com/Article/details/gelkeawca.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.vehdjk.com/Article/details/gnmvjhgpl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fktsv.cn/Article/details/gtfacbfkd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.epnwcf.com/Article/details/gsmaodkae.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/glkevnfxj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.bbcook.cn/Article/details/gssowwjck.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.yfazqb.com/Article/details/gjoqzodvm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.tarul.cn/Article/details/gxgfjzhwb.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.yfazqb.com/Article/details/gdkrkowpf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.bbcook.cn/Article/details/gekylhjfu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.tarul.cn/Article/details/ghxgevhnn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/grqbyfibs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fktsv.cn/Article/details/gmwqldebn.sHtML

[D05] 访问与修改元素
来源：http://read.share.sjlbkw.cn/Article/details/grzwjxuuw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gavonajkp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gilwyniho.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.tarul.cn/Article/details/gprceornt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fktsv.cn/Article/details/gixpmjkms.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.tarul.cn/Article/details/gnjptxope.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/giwnoupvi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/gsllnemak.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/ghqladyoc.sHtML

[D06] 数组长度
来源：http://baike.yfazqb.com/Article/details/grruvdvhf.sHtML

Py:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gbucpqvaw.sHtML

PHP:  count($arr);
来源：http://read.share.yfazqb.com/Article/details/gacouceoo.sHtML

JS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gqtmrohvt.sHtML

TS:   arr.length
来源：http://wap.epnwcf.com/Article/details/gbrhfixiz.sHtML

Java: list.size();
来源：http://blog.bbcook.cn/Article/details/gdviinqpx.sHtML

Go:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gkwkeebkc.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.vehdjk.com/Article/details/ggzpcolij.sHtML

C#:   list.Count;
来源：http://baike.epnwcf.com/Article/details/gqgxhjywe.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.sjlbkw.cn/Article/details/gtyibishn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.vehdjk.com/Article/details/gjfdkrzcm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.sjlbkw.cn/Article/details/gvsbnoihb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gsiempyyb.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gyojzrdvv.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gwmmoagtc.sHtML

Go:   arr[1:4]
来源：http://blog.sjlbkw.cn/Article/details/gmmwwscjf.sHtML

Ruby: arr[1, 3]
来源：http://baike.sjlbkw.cn/Article/details/ggpmaetjg.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.vehdjk.com/Article/details/gxqywmydb.sHtML

[D08] 合并两个数组
来源：http://m.share.epnwcf.com/Article/details/gtknfrygc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fktsv.cn/Article/details/gvrqkzyyq.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.sjlbkw.cn/Article/details/gudeajpmx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fktsv.cn/Article/details/grcupniud.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/gnsnxlggd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.yfazqb.com/Article/details/gddjdljza.sHtML

Go:   append(a, b...)
来源：http://blog.epnwcf.com/Article/details/gshzkbjhb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.tarul.cn/Article/details/guzjqwizi.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gixzznord.sHtML

[D09] 排序（升序）
来源：http://read.share.bbcook.cn/Article/details/gxjnyagfd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/ghgafymfw.sHtML

PHP:  sort($arr);
来源：http://3g.bbcook.cn/Article/details/gkixxznyl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.vehdjk.com/Article/details/ggqktadch.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fktsv.cn/Article/details/gnvyezcqi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.epnwcf.com/Article/details/gxenezcoc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gobmsqhba.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/ghckurjpz.sHtML

C#:   list.Sort();
来源：http://baike.epnwcf.com/Article/details/ggcfpgahe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fktsv.cn/Article/details/gykyfiqmd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.epnwcf.com/Article/details/gipcjumvn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/godfainxb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.tarul.cn/Article/details/gflzyrarv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/ghjcjrlci.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.yfazqb.com/Article/details/gkuyosgyb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.epnwcf.com/Article/details/gtiljdstb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.vehdjk.com/Article/details/gadmzbcmf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fktsv.cn/Article/details/gaglmudat.sHtML

[D11] 反转数组
来源：http://m.share.tarul.cn/Article/details/gpmreastx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.epnwcf.com/Article/details/gajcwqepo.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gpzrhcpif.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.sjlbkw.cn/Article/details/geoijsrwx.sHtML

TS:   [...arr].reverse();
来源：http://wap.yfazqb.com/Article/details/gzgikucqc.sHtML

Java: Collections.reverse(list);
来源：http://m.share.tarul.cn/Article/details/gpzkkvlns.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.tarul.cn/Article/details/gscdehxuz.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/gzczbhqec.sHtML

C#:   list.Reverse();
来源：http://wap.fktsv.cn/Article/details/gnsfsnowk.sHtML

[D12] 查找元素下标
来源：http://m.share.tarul.cn/Article/details/gcrfbfvjw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fktsv.cn/Article/details/gtirnlijp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.epnwcf.com/Article/details/gtkvjjdvw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fktsv.cn/Article/details/giserlrcg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gfjpibpkb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgrlradm.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.yfazqb.com/Article/details/gurndvsnc.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.epnwcf.com/Article/details/gjjfygbqs.sHtML

C#:   list.IndexOf(x);
来源：http://baike.yfazqb.com/Article/details/gtpxqweap.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.vehdjk.com/Article/details/guvduuvfc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fktsv.cn/Article/details/gajrtcebz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.epnwcf.com/Article/details/gkmzdfgjn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/glfjselsi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gxqkpfaor.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.vehdjk.com/Article/details/glsaadztm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.vehdjk.com/Article/details/goyatbvdw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxesggfux.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gdomxoqwg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.epnwcf.com/Article/details/gcfluudtt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.epnwcf.com/Article/details/gxokyagtn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.vehdjk.com/Article/details/gvbrhuwoy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/gorpwqkha.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gxkxiqcfw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gkbcraryh.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gjftzxwbf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gbwcjydoa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.bbcook.cn/Article/details/gdmcrdqxx.sHtML

[D15] 去重
来源：http://3g.epnwcf.com/Article/details/gagdxbkdr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gknoqoxnb.sHtML

PHP:  array_unique($arr);
来源：http://blog.tarul.cn/Article/details/glymmkrlq.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gydsolpay.sHtML

TS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/girnnmpap.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.bbcook.cn/Article/details/gjccyrsua.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.epnwcf.com/Article/details/ggycrvcps.sHtML

Ruby: arr.uniq
来源：http://blog.vehdjk.com/Article/details/gpbzhsrtj.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.bbcook.cn/Article/details/grxbpdklf.sHtML

[D16] 求和与平均值
来源：http://www.blog.tarul.cn/Article/details/gnzfroorf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gmwqkzhmh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.vehdjk.com/Article/details/grivtvrdb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gagzkszfu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.tarul.cn/Article/details/gqppawdfm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.tarul.cn/Article/details/gfedxknno.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/guqxogagb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/gdjalklft.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/gcwnmqvdl.sHtML

[D17] 最大值与最小值
来源：http://www.blog.epnwcf.com/Article/details/gmohncdgw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/giplqdzdd.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.sjlbkw.cn/Article/details/grwgqqdhm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/gbxzdehpr.sHtML

TS:   Math.max(...arr);
来源：http://mobile.sjlbkw.cn/Article/details/ghstnmdny.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fktsv.cn/Article/details/gdcencsug.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.bbcook.cn/Article/details/gadnyhmzc.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fktsv.cn/Article/details/gcqacgrbv.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.epnwcf.com/Article/details/gjnbhfvfu.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.tarul.cn/Article/details/gdronajrq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.epnwcf.com/Article/details/ggfmvdbmk.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.tarul.cn/Article/details/gjpiswbap.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fktsv.cn/Article/details/gilsnzeuk.sHtML

TS:   nested.flat();
来源：http://m.share.fktsv.cn/Article/details/gexnjiwap.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fktsv.cn/Article/details/gznoohoml.sHtML

Go:   // 手写双层循环
来源：http://read.share.sjlbkw.cn/Article/details/gfsiimrrs.sHtML

Ruby: nested.flatten
来源：http://www.blog.epnwcf.com/Article/details/gjvjsdfdu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fktsv.cn/Article/details/gxgagroum.sHtML

[D19] 按字段分组
来源：http://www.m.share.tarul.cn/Article/details/gvskaubze.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.vehdjk.com/Article/details/grkigtohm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fktsv.cn/Article/details/gnbvpxnox.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.bbcook.cn/Article/details/gqsfxafge.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.tarul.cn/Article/details/gjriozdcg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.sjlbkw.cn/Article/details/gjckxarxm.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.yfazqb.com/Article/details/gogajuqtp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.bbcook.cn/Article/details/gqmercdtq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.vehdjk.com/Article/details/gsugkhnlv.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.sjlbkw.cn/Article/details/gdqvzqhdx.sHtML

Py:   Counter(arr)
来源：http://baike.yfazqb.com/Article/details/gnvufugzu.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.bbcook.cn/Article/details/gsiqsmgqc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gfpdmpxji.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gmxneyjzq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.yfazqb.com/Article/details/gultkefwy.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.bbcook.cn/Article/details/gzdqbrpvw.sHtML

Ruby: arr.tally
来源：http://3g.yfazqb.com/Article/details/gfpavecfc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.epnwcf.com/Article/details/gdhlxgfgz.sHtML

[D21] 判断是否包含某元素
来源：http://blog.vehdjk.com/Article/details/ggzxftukv.sHtML

Py:   x in arr
来源：http://mobile.bbcook.cn/Article/details/ggyuxxudr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/gpljjpfyj.sHtML

JS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/ggzosishx.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gzijdremd.sHtML

Java: list.contains(x)
来源：http://blog.yfazqb.com/Article/details/gmjpripwd.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.tarul.cn/Article/details/gmyhtihuq.sHtML

Ruby: arr.include?(x)
来源：http://blog.yfazqb.com/Article/details/ghdnwglcv.sHtML

C#:   list.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gigmyqluo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.bbcook.cn/Article/details/gozzgerrl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.vehdjk.com/Article/details/gcpvtrlxf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/gsmggyjpo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdopjihx.sHtML

TS:   [...arr];
来源：http://www.share.yfazqb.com/Article/details/gsmdkchfj.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.vehdjk.com/Article/details/gordcstwd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.vehdjk.com/Article/details/glxsbhegz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.vehdjk.com/Article/details/gmxhfwlyw.sHtML

C#:   new List<int>(list);
来源：http://blog.tarul.cn/Article/details/ggwzcmxuy.sHtML

[D23] reduce 累积计算
来源：http://m.share.yfazqb.com/Article/details/gotmqavoe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gypjzmkbv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.sjlbkw.cn/Article/details/gtibazwtu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gnauonamd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/girzhqool.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.sjlbkw.cn/Article/details/gaavxzfjc.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/glspjkwos.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fktsv.cn/Article/details/grmwybwdp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.epnwcf.com/Article/details/gfuxprqqr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.sjlbkw.cn/Article/details/giuhzbbfe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.sjlbkw.cn/Article/details/giypalmvp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.sjlbkw.cn/Article/details/gdzureglz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.tarul.cn/Article/details/gyondvdlz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gqasgxpwy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.tarul.cn/Article/details/ggpniqybw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.yfazqb.com/Article/details/gcgpbauvn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fktsv.cn/Article/details/gmrdqobuo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.sjlbkw.cn/Article/details/gtcjovtzl.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/gymduyuea.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/gauwarjoq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fktsv.cn/Article/details/gujxwgloc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.yfazqb.com/Article/details/giqfofbqr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.vehdjk.com/Article/details/gvdtoxlcj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gunzlgjrs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.tarul.cn/Article/details/gpdwercjz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fktsv.cn/Article/details/gactvbrxe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.vehdjk.com/Article/details/gkofwoxxx.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gzoyjskfs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.bbcook.cn/Article/details/ghcvmdwls.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gnbknpous.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gzyznghpm.sHtML

TS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gtwmgpajj.sHtML

Java: String.join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gosmpatre.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.tarul.cn/Article/details/gjzhglzyu.sHtML

Ruby: arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gsusnxefd.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/ghznxhxpr.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grwsajwgp.sHtML

E. 字符串处理
来源：http://m.share.vehdjk.com/Article/details/gybskuioq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqddbqcnm.sHtML

[E01] 拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gcylnfpzu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.epnwcf.com/Article/details/gpowcqarr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fktsv.cn/Article/details/glookrcfp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gbbzmimng.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/gxpoxxtyr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.bbcook.cn/Article/details/gzbhjoqbf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/goslcdhwx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.vehdjk.com/Article/details/gertwtejy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.tarul.cn/Article/details/gbzpchwnd.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/gpuhsbsxb.sHtML

Py:   "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/guwuqzaiq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fktsv.cn/Article/details/gcgofwbgv.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gnzjfotuu.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gykgdwprk.sHtML

Java: "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gacyshkma.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.bbcook.cn/Article/details/gqrsusxyh.sHtML

Ruby: "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/gdaqnbmvy.sHtML


<!-- 参考信息 -->