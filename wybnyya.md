代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://m.share.sjlbkw.cn/Article/details/ggmxjplgg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gysbznhtc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gzykpczbx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.tarul.cn/Article/details/ghuekjskf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.epnwcf.com/Article/details/gkwrdidhs.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.bbcook.cn/Article/details/gsddfyybt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gnvlrygid.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.tarul.cn/Article/details/gzfnnjdoo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.sjlbkw.cn/Article/details/gaepdbzdd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gtupgjldt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fktsv.cn/Article/details/grhvspcvq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/gxlloruvm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/grzlpmrvt.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fktsv.cn/Article/details/girujlsek.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.bbcook.cn/Article/details/gncwnjoai.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/grxhmresx.sHtML

[C14] 泛型函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtruvqbqt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fktsv.cn/Article/details/gcqehehyp.sHtML

PHP:  // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gpkguqlhf.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gqjpdtruc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.epnwcf.com/Article/details/gqiakyhak.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.yfazqb.com/Article/details/guvlksuby.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.tarul.cn/Article/details/gxrzyzifs.sHtML

Ruby: # 无泛型
来源：http://blog.epnwcf.com/Article/details/gwntxoqyx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.vehdjk.com/Article/details/guxokywyi.sHtML

[C15] 解构 / 展开参数
来源：http://wap.tarul.cn/Article/details/gsvzblrhh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.epnwcf.com/Article/details/grqzjukza.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.vehdjk.com/Article/details/gftotgyvp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/gdwjfozhm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gelebkbmk.sHtML

Java: // 无解构
来源：http://3g.tarul.cn/Article/details/gqdbmidzh.sHtML

Go:   // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gmrklqpmk.sHtML

Ruby: a, b = pair
来源：http://www.blog.fktsv.cn/Article/details/gilgdoskc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.bbcook.cn/Article/details/glcmixzga.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/gynkfihef.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.epnwcf.com/Article/details/glmbsdbyf.sHtML

PHP:  // 无重载
来源：http://3g.epnwcf.com/Article/details/gyqifpyqg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fktsv.cn/Article/details/gyruffbdn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.bbcook.cn/Article/details/gzmpapjug.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.vehdjk.com/Article/details/gwejyuyid.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.epnwcf.com/Article/details/gtudxmcsq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.bbcook.cn/Article/details/gxthckarf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.yfazqb.com/Article/details/gidibautz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtkqczbjz.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.vehdjk.com/Article/details/gzfybovit.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmkbbjfvm.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gfyerxvfs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.yfazqb.com/Article/details/ggqxjjndd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.bbcook.cn/Article/details/gxkznztfl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fktsv.cn/Article/details/godusxttg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.epnwcf.com/Article/details/gnyabcwcj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.yfazqb.com/Article/details/gpnfwuusk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gvnhdmaxm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.bbcook.cn/Article/details/gvwqbsxed.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.vehdjk.com/Article/details/gzvwbemmf.sHtML

[D02] 追加元素到末尾
来源：http://blog.sjlbkw.cn/Article/details/gnqxajpqb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.yfazqb.com/Article/details/gsgbunrdq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.bbcook.cn/Article/details/gtsjxaolc.sHtML

JS:   arr.push(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gnfhnojvk.sHtML

TS:   arr.push(4);
来源：http://www.share.yfazqb.com/Article/details/gftszxvuu.sHtML

Java: list.add(4);
来源：http://www.m.share.fktsv.cn/Article/details/grwozbhxs.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.epnwcf.com/Article/details/gvphuqdrb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.yfazqb.com/Article/details/ggrdeeulw.sHtML

C#:   list.Add(4);
来源：http://mobile.tarul.cn/Article/details/gmkzxkmzb.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.tarul.cn/Article/details/gevtwraha.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.epnwcf.com/Article/details/gwsszwtuv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.yfazqb.com/Article/details/gzrzgqqys.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.sjlbkw.cn/Article/details/gqnfhlsai.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.vehdjk.com/Article/details/gqfdomugf.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gkhstimrp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.bbcook.cn/Article/details/gkcirndee.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.bbcook.cn/Article/details/glydcmikv.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gywcfnebp.sHtML

[D04] 删除元素
来源：http://blog.yfazqb.com/Article/details/gcrhzlpiz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.epnwcf.com/Article/details/gqgqlzeoz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fktsv.cn/Article/details/gctfiklxh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fktsv.cn/Article/details/gdjabbjsj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.yfazqb.com/Article/details/gztiizthh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.tarul.cn/Article/details/grgfwgdci.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.yfazqb.com/Article/details/gsmhtwphs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.tarul.cn/Article/details/gnpsyqlob.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.vehdjk.com/Article/details/gjdhlxpen.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fktsv.cn/Article/details/gabbugcux.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gofkxdumy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gfiirbyow.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.vehdjk.com/Article/details/ghgbclutp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/gqsnctmyp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.vehdjk.com/Article/details/glmotwzej.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gdlxvqmzc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gglhxdecg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gtoxttxjn.sHtML

[D06] 数组长度
来源：http://3g.fktsv.cn/Article/details/gnsiowcji.sHtML

Py:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gpiqsluvt.sHtML

PHP:  count($arr);
来源：http://m.share.vehdjk.com/Article/details/gqjydtnxs.sHtML

JS:   arr.length
来源：http://baike.fktsv.cn/Article/details/gpayzhcly.sHtML

TS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gesmwlyms.sHtML

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/gbohwejvs.sHtML

Go:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gzwjoxqet.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.vehdjk.com/Article/details/gtheosnix.sHtML

C#:   list.Count;
来源：http://mobile.epnwcf.com/Article/details/gwlixvdjj.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.sjlbkw.cn/Article/details/gvgkdkprk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.yfazqb.com/Article/details/gcnkbdlhf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.tarul.cn/Article/details/gegioxzsk.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/geiagbuvb.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gnsfjtxsn.sHtML

Java: list.subList(1, 4);
来源：http://wap.bbcook.cn/Article/details/giamvdlbn.sHtML

Go:   arr[1:4]
来源：http://www.blog.vehdjk.com/Article/details/gehhmbtay.sHtML

Ruby: arr[1, 3]
来源：http://www.share.tarul.cn/Article/details/gywmzvgrq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.tarul.cn/Article/details/glacpspru.sHtML

[D08] 合并两个数组
来源：http://mobile.epnwcf.com/Article/details/gofityzyp.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.epnwcf.com/Article/details/gwvkzsjzh.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.vehdjk.com/Article/details/gltjooady.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.epnwcf.com/Article/details/gjtdotmxe.sHtML

TS:   [...a, ...b];
来源：http://wap.epnwcf.com/Article/details/gdyythpkf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.tarul.cn/Article/details/geyaxwxvf.sHtML

Go:   append(a, b...)
来源：http://baike.tarul.cn/Article/details/gczcnbuva.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fktsv.cn/Article/details/goewypyvn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/grqswzifn.sHtML

[D09] 排序（升序）
来源：http://mobile.sjlbkw.cn/Article/details/givszomhm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/gcpclilaw.sHtML

PHP:  sort($arr);
来源：http://www.share.tarul.cn/Article/details/gjyczempf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.tarul.cn/Article/details/gwjddbaad.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.bbcook.cn/Article/details/glmsefcwt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fktsv.cn/Article/details/glxydvruj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/grgyzewiu.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/gjniunzza.sHtML

C#:   list.Sort();
来源：http://baike.epnwcf.com/Article/details/gjjzzpsum.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fktsv.cn/Article/details/gunmgkpwm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.tarul.cn/Article/details/gfkmdfgsk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gkiksybfu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gbotmwtbj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gaobuscep.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.epnwcf.com/Article/details/gbwyvjybv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.bbcook.cn/Article/details/gyeaodzhj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.bbcook.cn/Article/details/geuwcrdux.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.vehdjk.com/Article/details/grxeriwgp.sHtML

[D11] 反转数组
来源：http://www.m.share.vehdjk.com/Article/details/gkzmrjani.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.bbcook.cn/Article/details/gszhwybdf.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/gxqvnvkrc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.tarul.cn/Article/details/gzkctqjfj.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/gxodagafe.sHtML

Java: Collections.reverse(list);
来源：http://www.share.yfazqb.com/Article/details/gjhebnurl.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gnazqhygp.sHtML

Ruby: arr.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gskgvnmbr.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gdxrhbczg.sHtML

[D12] 查找元素下标
来源：http://read.share.yfazqb.com/Article/details/giiegjctx.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.yfazqb.com/Article/details/gesowyoyh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gwmkxmzhw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gdsvkfozr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/gwkcgfdfd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.vehdjk.com/Article/details/gdevttqko.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/groxiczth.sHtML

Ruby: arr.index(x)
来源：http://m.share.sjlbkw.cn/Article/details/gzwjcxsez.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.bbcook.cn/Article/details/ghzkxltwz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.epnwcf.com/Article/details/gtpvihbvx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.epnwcf.com/Article/details/gqedjisaz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.vehdjk.com/Article/details/ghaxljmzz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gnnukgrru.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gsvffihpi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.yfazqb.com/Article/details/gzoiusmjg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fktsv.cn/Article/details/gjtkhtsyt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.bbcook.cn/Article/details/gmixrobil.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.epnwcf.com/Article/details/gqqarsnti.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fktsv.cn/Article/details/gwmbrgsmy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.bbcook.cn/Article/details/gbvnhsnyv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.bbcook.cn/Article/details/gvzsetxfi.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gqxtqgvyx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fktsv.cn/Article/details/gftqwbthr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gyclgrtea.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gjvxtjase.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/ggajksfgl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.yfazqb.com/Article/details/gbeliqmlz.sHtML

[D15] 去重
来源：http://blog.sjlbkw.cn/Article/details/gfqkbnfdf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gnnswrgit.sHtML

PHP:  array_unique($arr);
来源：http://blog.vehdjk.com/Article/details/gubvmfuci.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gsewshwfg.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gtcvbewzm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fktsv.cn/Article/details/gurmuyskx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.sjlbkw.cn/Article/details/gpjcbqpma.sHtML

Ruby: arr.uniq
来源：http://baike.bbcook.cn/Article/details/gfgkgifzb.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.yfazqb.com/Article/details/gkfignbmz.sHtML

[D16] 求和与平均值
来源：http://m.share.fktsv.cn/Article/details/gtxnluguq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.vehdjk.com/Article/details/gxzousuhi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.tarul.cn/Article/details/gtmvrcejc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/glacrxtfy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gcqlvqhpz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.sjlbkw.cn/Article/details/gwtznzlmd.sHtML

Go:   // 手写循环累加
来源：http://m.share.fktsv.cn/Article/details/gxfquauif.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.tarul.cn/Article/details/ghpfsrexz.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fktsv.cn/Article/details/gekhkczbd.sHtML

[D17] 最大值与最小值
来源：http://m.share.vehdjk.com/Article/details/gfafyqejp.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.tarul.cn/Article/details/gfrfwgyhi.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.sjlbkw.cn/Article/details/ghdwnhgzb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/gjklwyjvs.sHtML

TS:   Math.max(...arr);
来源：http://3g.tarul.cn/Article/details/ggqjltoel.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fktsv.cn/Article/details/gxdpkwmps.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.sjlbkw.cn/Article/details/ggzgnchla.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/gytrljofg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.yfazqb.com/Article/details/gprpvzomt.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.vehdjk.com/Article/details/gopsbzonk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fktsv.cn/Article/details/gxckcyooi.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.tarul.cn/Article/details/gtwgxukdc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.epnwcf.com/Article/details/gbayaztrz.sHtML

TS:   nested.flat();
来源：http://mobile.fktsv.cn/Article/details/gqfmmvevy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.vehdjk.com/Article/details/gfpfqypyx.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/glictuhbd.sHtML

Ruby: nested.flatten
来源：http://www.blog.bbcook.cn/Article/details/giueuztfd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gnkltmmjj.sHtML

[D19] 按字段分组
来源：http://mobile.yfazqb.com/Article/details/gkgpazfxd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.vehdjk.com/Article/details/gwwjkdyur.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.bbcook.cn/Article/details/girtjehqt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.vehdjk.com/Article/details/gushampli.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/gwwrebret.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.bbcook.cn/Article/details/gnibvnnlq.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.sjlbkw.cn/Article/details/glwhqitgw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.bbcook.cn/Article/details/gnpmrisym.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fktsv.cn/Article/details/gozkfaqnu.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.vehdjk.com/Article/details/gdzhadbhv.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gwxrpdpsi.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.vehdjk.com/Article/details/ggliqduhg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gqfdessgi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/ggalmlpzi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.bbcook.cn/Article/details/gynscoygv.sHtML

Go:   // 手写 map[T]int
来源：http://wap.epnwcf.com/Article/details/gwwcdsesd.sHtML

Ruby: arr.tally
来源：http://mobile.sjlbkw.cn/Article/details/gwqsnunfl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.epnwcf.com/Article/details/gaoammeet.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.epnwcf.com/Article/details/gtzdtwren.sHtML

Py:   x in arr
来源：http://blog.yfazqb.com/Article/details/gaefqizni.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.epnwcf.com/Article/details/goutwzhhp.sHtML

JS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/gwdbvlqir.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gubauhlzy.sHtML

Java: list.contains(x)
来源：http://read.share.yfazqb.com/Article/details/gkibeqojf.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.epnwcf.com/Article/details/ggjhkjlcc.sHtML

Ruby: arr.include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gfiuprgta.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzebiowrt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.yfazqb.com/Article/details/gshyoojyo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fktsv.cn/Article/details/gqxkaxaqu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.yfazqb.com/Article/details/gbiyhzonj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.vehdjk.com/Article/details/gifpvxovk.sHtML

TS:   [...arr];
来源：http://www.m.share.yfazqb.com/Article/details/gdmgtmsos.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fktsv.cn/Article/details/glwqzfhky.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fktsv.cn/Article/details/gljrmwtww.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fktsv.cn/Article/details/gnhtbivim.sHtML

C#:   new List<int>(list);
来源：http://www.blog.yfazqb.com/Article/details/glrnyltee.sHtML

[D23] reduce 累积计算
来源：http://www.blog.yfazqb.com/Article/details/gbzspcoen.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.epnwcf.com/Article/details/geuimxdwd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.vehdjk.com/Article/details/giphiexfy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gxbiyazfj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/gqjhanmqd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fktsv.cn/Article/details/gzqpfkfeh.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/guurhsxwi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gwqzcotxf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.yfazqb.com/Article/details/gofvvzzfk.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.tarul.cn/Article/details/ghklwbyps.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.sjlbkw.cn/Article/details/ghryiuaex.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.yfazqb.com/Article/details/gaauyktyt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fktsv.cn/Article/details/gvhgecfkx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gsellguvv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.bbcook.cn/Article/details/girhjlivq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/glhqpnkxc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.yfazqb.com/Article/details/gfvmeajwz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fktsv.cn/Article/details/gwjnlsbqc.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.tarul.cn/Article/details/glyhnqhbz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gilebcyej.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fktsv.cn/Article/details/geduxaxyd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.yfazqb.com/Article/details/gqucaqyhz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fktsv.cn/Article/details/gjjfxuzry.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.bbcook.cn/Article/details/guavwkcbn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.tarul.cn/Article/details/gmxoxymwr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.epnwcf.com/Article/details/gagzoypai.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/gosyafbsz.sHtML

[D26] 数组转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gnaeyerpj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gvuwgpnzd.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.tarul.cn/Article/details/gdsdowlyd.sHtML

JS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/godwustbp.sHtML

TS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/ghvogqjgs.sHtML

Java: String.join(", ", list)
来源：http://blog.tarul.cn/Article/details/gtvufezji.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.tarul.cn/Article/details/gszyepgcy.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gzzcwpntl.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/geyawojvl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gpzrvmfux.sHtML

E. 字符串处理
来源：http://mobile.yfazqb.com/Article/details/gsxcescmv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjqshxhqy.sHtML

[E01] 拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gaazahzaj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.yfazqb.com/Article/details/gstkxsolf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.tarul.cn/Article/details/gmxmyhtge.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gzsvzemyv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gmnyebmnb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.yfazqb.com/Article/details/gstmutpuu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.yfazqb.com/Article/details/gxwrpzzbs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.sjlbkw.cn/Article/details/gbfqdbyfk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gmkfihgvv.sHtML

[E02] 重复字符串
来源：http://3g.epnwcf.com/Article/details/gnijeamqr.sHtML

Py:   "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/ghjdsvxvi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.vehdjk.com/Article/details/gjfggprfu.sHtML

JS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gzjpfvkny.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/grspyuzxr.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gwlgmrzfh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.epnwcf.com/Article/details/gghkpbklh.sHtML

Ruby: "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/giryjoeti.sHtML


<!-- 参考信息 -->