代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://read.share.tarul.cn/Article/details/gozabslxq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gmfokdyin.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gjzzlzzol.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.tarul.cn/Article/details/gkhyniryl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/gafjsjvmy.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.yfazqb.com/Article/details/grfcpafwq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/ggnmcvmev.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.tarul.cn/Article/details/ggsqwklhg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/gocewsbnv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gfypwqdxf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.epnwcf.com/Article/details/glsagxvik.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gryyswkpi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gxfcloncr.sHtML

Go:   func add(a, b int) int
来源：http://wap.sjlbkw.cn/Article/details/gptgeabxu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.sjlbkw.cn/Article/details/gsmmnbprr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.vehdjk.com/Article/details/ghtlqcvsl.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/gazfjxbvr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.epnwcf.com/Article/details/gzfggexal.sHtML

PHP:  // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gphdvrtkb.sHtML

JS:   // 无泛型
来源：http://3g.bbcook.cn/Article/details/gjsutodls.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/guyylonli.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fktsv.cn/Article/details/gbzxqzhpx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fktsv.cn/Article/details/gjhfvytws.sHtML

Ruby: # 无泛型
来源：http://read.share.vehdjk.com/Article/details/geirmubuc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.tarul.cn/Article/details/gdzwyimzx.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.yfazqb.com/Article/details/gdjytutwj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fktsv.cn/Article/details/gruqbyqgb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.sjlbkw.cn/Article/details/gtrircyzm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/gwnkygteu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gednzktsx.sHtML

Java: // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/geypswmkw.sHtML

Go:   // 无解构
来源：http://wap.epnwcf.com/Article/details/glwemizlq.sHtML

Ruby: a, b = pair
来源：http://blog.sjlbkw.cn/Article/details/gqeoessoy.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.tarul.cn/Article/details/gterlttta.sHtML

[C16] 函数 / 方法重载
来源：http://3g.sjlbkw.cn/Article/details/gsuyncbco.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fktsv.cn/Article/details/gxwhpaatk.sHtML

PHP:  // 无重载
来源：http://3g.fktsv.cn/Article/details/gnwyxflbl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.vehdjk.com/Article/details/gfjufxkni.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.tarul.cn/Article/details/gpfkrjdge.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.yfazqb.com/Article/details/gtrbrettt.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.sjlbkw.cn/Article/details/gyywckscr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.bbcook.cn/Article/details/gkzmyrnqy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gggukohgt.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdpxbmobc.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.vehdjk.com/Article/details/gevzchyca.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnqcrgdzx.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.bbcook.cn/Article/details/ggykmiuej.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.yfazqb.com/Article/details/gyvjagxvs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.epnwcf.com/Article/details/gtskyvicn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.bbcook.cn/Article/details/gxdkpugud.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.epnwcf.com/Article/details/gndrvjoow.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.sjlbkw.cn/Article/details/gpcgotvvx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxiyywuo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.epnwcf.com/Article/details/gpkgwescg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.tarul.cn/Article/details/ggrkfblwq.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.sjlbkw.cn/Article/details/gczbnzztr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.tarul.cn/Article/details/gmqaihbwz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.tarul.cn/Article/details/gunbtduzm.sHtML

JS:   arr.push(4);
来源：http://wap.bbcook.cn/Article/details/gwtvqcvhq.sHtML

TS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gejjbctsc.sHtML

Java: list.add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gdmiwxlqf.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.epnwcf.com/Article/details/glfxfsdek.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fktsv.cn/Article/details/gdpripjrl.sHtML

C#:   list.Add(4);
来源：http://3g.fktsv.cn/Article/details/gxzweqrjg.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.sjlbkw.cn/Article/details/gkkahllbi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/grdszrwdk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.yfazqb.com/Article/details/gvgmzyrqe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fktsv.cn/Article/details/ghwcinwwx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fktsv.cn/Article/details/gcwhuwqot.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/ggqfszrkf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.yfazqb.com/Article/details/gxfifnksk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.yfazqb.com/Article/details/gswxaxduk.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.vehdjk.com/Article/details/gbwdkrscc.sHtML

[D04] 删除元素
来源：http://mobile.tarul.cn/Article/details/ghqpjagvv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.sjlbkw.cn/Article/details/gbwfbobry.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/gmmvhkrfd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.tarul.cn/Article/details/gpdjyxpgx.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.vehdjk.com/Article/details/guiffmsau.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.sjlbkw.cn/Article/details/guxsuoccl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.epnwcf.com/Article/details/gupiejpna.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fktsv.cn/Article/details/gdwdpcuql.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fktsv.cn/Article/details/gmaxfptge.sHtML

[D05] 访问与修改元素
来源：http://3g.vehdjk.com/Article/details/guexoiggr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gsqkjjres.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gibrbwnqv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gbyhawqfr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fktsv.cn/Article/details/gdhoqmjhs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.yfazqb.com/Article/details/gimgzzszp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gldktymib.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gqavgiuir.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gffqufjpq.sHtML

[D06] 数组长度
来源：http://mobile.vehdjk.com/Article/details/geqsbxdie.sHtML

Py:   len(arr)
来源：http://wap.bbcook.cn/Article/details/ggvkujqhq.sHtML

PHP:  count($arr);
来源：http://3g.sjlbkw.cn/Article/details/gmqwzmpeb.sHtML

JS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdvoujlt.sHtML

TS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/gctpbzndd.sHtML

Java: list.size();
来源：http://www.blog.sjlbkw.cn/Article/details/gbfqocjhi.sHtML

Go:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/goxxrynde.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.vehdjk.com/Article/details/gzzgrbarp.sHtML

C#:   list.Count;
来源：http://wap.vehdjk.com/Article/details/gmbrbkmol.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/glcwmdtfr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.sjlbkw.cn/Article/details/gymncdnmg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.epnwcf.com/Article/details/gjkjslzwp.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fktsv.cn/Article/details/giqhdboms.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gilqxahsx.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gldsfaluz.sHtML

Go:   arr[1:4]
来源：http://3g.sjlbkw.cn/Article/details/gfpfwmttp.sHtML

Ruby: arr[1, 3]
来源：http://wap.fktsv.cn/Article/details/gnhtltswh.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.tarul.cn/Article/details/gsttqkqem.sHtML

[D08] 合并两个数组
来源：http://blog.sjlbkw.cn/Article/details/gjknxfwwk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.yfazqb.com/Article/details/gyqsydbgx.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.sjlbkw.cn/Article/details/gryliirha.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.vehdjk.com/Article/details/ghmdnlzxx.sHtML

TS:   [...a, ...b];
来源：http://read.share.tarul.cn/Article/details/gsleutpqm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.sjlbkw.cn/Article/details/ghqsnovtx.sHtML

Go:   append(a, b...)
来源：http://m.share.sjlbkw.cn/Article/details/glzfawydj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fktsv.cn/Article/details/guvyumwkl.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.vehdjk.com/Article/details/gsclgxzmb.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/giutdlbxm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gufnyarws.sHtML

PHP:  sort($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gofaxzudw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.bbcook.cn/Article/details/ggkwfqegw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.tarul.cn/Article/details/gtetlamqv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.yfazqb.com/Article/details/gxihfwouy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/ginxeuwsa.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gyikbutwl.sHtML

C#:   list.Sort();
来源：http://www.share.epnwcf.com/Article/details/gnvkayzph.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.yfazqb.com/Article/details/gbuvvvqbx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.bbcook.cn/Article/details/gocboddte.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.yfazqb.com/Article/details/gaevpeiwe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fktsv.cn/Article/details/ghnlllrnc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gxvlqhxoq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.tarul.cn/Article/details/gosfcesmc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/gvstuirvs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.bbcook.cn/Article/details/gpeejcsaa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fktsv.cn/Article/details/gtrqgqfgb.sHtML

[D11] 反转数组
来源：http://www.blog.fktsv.cn/Article/details/ghpvazyjn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.vehdjk.com/Article/details/gltqdteni.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.tarul.cn/Article/details/gpmbgdutc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.epnwcf.com/Article/details/gsftjgois.sHtML

TS:   [...arr].reverse();
来源：http://baike.epnwcf.com/Article/details/ghcliqqoo.sHtML

Java: Collections.reverse(list);
来源：http://m.share.epnwcf.com/Article/details/gozjrsmnc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/gtsxzqadr.sHtML

Ruby: arr.reverse
来源：http://3g.sjlbkw.cn/Article/details/grcmxqkjr.sHtML

C#:   list.Reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gnsmqitux.sHtML

[D12] 查找元素下标
来源：http://wap.tarul.cn/Article/details/gyxikeijf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.bbcook.cn/Article/details/getflyqtw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.sjlbkw.cn/Article/details/glvolpwiq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/gghgzprqx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.bbcook.cn/Article/details/gxdbpdeyl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.yfazqb.com/Article/details/gzdwbkrzk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gefrpgrlq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmzwfkyj.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.tarul.cn/Article/details/grpdjzeee.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.vehdjk.com/Article/details/gkezlbbuk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gwoxpwssv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.vehdjk.com/Article/details/gelpjhfbe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.vehdjk.com/Article/details/gvoajfgfm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gvjlpnjop.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.epnwcf.com/Article/details/gjqgjbuqd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.tarul.cn/Article/details/gslcbgoko.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.vehdjk.com/Article/details/goquffczp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gnsyvlmaz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.tarul.cn/Article/details/gdyoqzofe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fktsv.cn/Article/details/ggvyfiays.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gfklkndhx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.tarul.cn/Article/details/gwqvawrcg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gulgoqdyl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/gzsriodyh.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/gsdljhqpu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gmhfxzfvf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.vehdjk.com/Article/details/gejdlzeaa.sHtML

[D15] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gcvgnbynv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.sjlbkw.cn/Article/details/gdwxyrwcd.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.bbcook.cn/Article/details/gltmgahvi.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gqmcztcdf.sHtML

TS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gdmouahil.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.tarul.cn/Article/details/glgozyqti.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.epnwcf.com/Article/details/gblktrlco.sHtML

Ruby: arr.uniq
来源：http://read.share.yfazqb.com/Article/details/gqjdpynxv.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.bbcook.cn/Article/details/gvoittchl.sHtML

[D16] 求和与平均值
来源：http://m.share.epnwcf.com/Article/details/gracjfrim.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/gombhevdo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.vehdjk.com/Article/details/ghxygfffk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fktsv.cn/Article/details/gokbnkdad.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.vehdjk.com/Article/details/gbchbkugs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fktsv.cn/Article/details/grzxrbycs.sHtML

Go:   // 手写循环累加
来源：http://wap.bbcook.cn/Article/details/gmfavbvmk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gwewfosmz.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.epnwcf.com/Article/details/gjxfblzqi.sHtML

[D17] 最大值与最小值
来源：http://m.share.fktsv.cn/Article/details/gblflarwx.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/gmiluwapy.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.yfazqb.com/Article/details/gxcpvtndh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fktsv.cn/Article/details/ggfwrbiky.sHtML

TS:   Math.max(...arr);
来源：http://3g.fktsv.cn/Article/details/gdxkilxpo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.bbcook.cn/Article/details/gbgxjipel.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/ginxwktno.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.vehdjk.com/Article/details/guexilnrs.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.bbcook.cn/Article/details/ggfbetgxl.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.bbcook.cn/Article/details/goqnmvjna.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.sjlbkw.cn/Article/details/gykeivofr.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.bbcook.cn/Article/details/gavrnljcq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.epnwcf.com/Article/details/gdlblfxop.sHtML

TS:   nested.flat();
来源：http://wap.epnwcf.com/Article/details/gjyzyznwi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.yfazqb.com/Article/details/gfobxgpru.sHtML

Go:   // 手写双层循环
来源：http://wap.yfazqb.com/Article/details/gxaqhmwtl.sHtML

Ruby: nested.flatten
来源：http://blog.vehdjk.com/Article/details/gpexzijuf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.vehdjk.com/Article/details/gjjgcncmg.sHtML

[D19] 按字段分组
来源：http://www.blog.tarul.cn/Article/details/grhbeiluu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.yfazqb.com/Article/details/gdvnuuutp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/gkfmjguan.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.epnwcf.com/Article/details/gdsvrjinl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/grebepihj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/gsonsizhg.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.tarul.cn/Article/details/gdvfxixdb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fktsv.cn/Article/details/gsrtawcoo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.vehdjk.com/Article/details/goakmraan.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gfzrxvgia.sHtML

Py:   Counter(arr)
来源：http://www.share.epnwcf.com/Article/details/gjyvdecdk.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gtqawtzwy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.epnwcf.com/Article/details/gsdfqjrgd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gwgacgdyy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.bbcook.cn/Article/details/gxhpjbodz.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.epnwcf.com/Article/details/gdnftbkbl.sHtML

Ruby: arr.tally
来源：http://www.m.share.tarul.cn/Article/details/gtpohcyrk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.vehdjk.com/Article/details/gltdgrjoe.sHtML

[D21] 判断是否包含某元素
来源：http://blog.bbcook.cn/Article/details/gwbkglhlm.sHtML

Py:   x in arr
来源：http://www.blog.fktsv.cn/Article/details/gvdscbsma.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fktsv.cn/Article/details/gmgupwkgm.sHtML

JS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gknsgrujf.sHtML

TS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gspxgytwo.sHtML

Java: list.contains(x)
来源：http://www.share.epnwcf.com/Article/details/gqsvxayzx.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.bbcook.cn/Article/details/gcvzzsjqb.sHtML

Ruby: arr.include?(x)
来源：http://wap.vehdjk.com/Article/details/gguhlrgpn.sHtML

C#:   list.Contains(x)
来源：http://wap.tarul.cn/Article/details/gelnwcctq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.bbcook.cn/Article/details/gkitiqhoe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.vehdjk.com/Article/details/galidndux.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.bbcook.cn/Article/details/gghlbhgul.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fktsv.cn/Article/details/gtswwfycj.sHtML

TS:   [...arr];
来源：http://www.blog.sjlbkw.cn/Article/details/gpcmqsfie.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.epnwcf.com/Article/details/gsxtwuyhk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fktsv.cn/Article/details/gtnmcvuwo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.yfazqb.com/Article/details/gmhpqkmac.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/gfkipzdtq.sHtML

[D23] reduce 累积计算
来源：http://mobile.yfazqb.com/Article/details/gvmpxdmdv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.epnwcf.com/Article/details/gejsogrhx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gfckvomrl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/geeqmkdpw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gfjsbthss.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.vehdjk.com/Article/details/gsolelzht.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gdgqlneax.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fktsv.cn/Article/details/gnoucacwm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.bbcook.cn/Article/details/gutcdxuif.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.bbcook.cn/Article/details/gbpmrpngp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.sjlbkw.cn/Article/details/ggmqilgsa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.tarul.cn/Article/details/gkifgegdj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gghtzjyjh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gegxnutyf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.sjlbkw.cn/Article/details/grndvztoi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/gwtutoqme.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.sjlbkw.cn/Article/details/gncnekvyk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.bbcook.cn/Article/details/gxatexcln.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.sjlbkw.cn/Article/details/ghagefzrc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/gtugwmczt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.yfazqb.com/Article/details/gqgmsqyue.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.epnwcf.com/Article/details/gxjgaravz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.epnwcf.com/Article/details/grszmoqfi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.yfazqb.com/Article/details/gqnrvmhke.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.sjlbkw.cn/Article/details/gyiunwhbc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.epnwcf.com/Article/details/glpaowqps.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.tarul.cn/Article/details/gqfrqpodr.sHtML

[D26] 数组转字符串
来源：http://3g.yfazqb.com/Article/details/gafqkimrg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.epnwcf.com/Article/details/gnpzifvph.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/goqmhsegd.sHtML

JS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gvelkcwor.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gpraqvauh.sHtML

Java: String.join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gdjyvxhom.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.tarul.cn/Article/details/gommlsbxe.sHtML

Ruby: arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gidrqoknl.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gztomumqw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glpsbspmx.sHtML

E. 字符串处理
来源：http://read.share.bbcook.cn/Article/details/ggjfqahxa.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkhtechtc.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gdukwyilh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.sjlbkw.cn/Article/details/gfqcutcwl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.sjlbkw.cn/Article/details/gsivaxiek.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/gmtanayhg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gflyamjsn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.bbcook.cn/Article/details/gebtoiumn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.epnwcf.com/Article/details/gkmousouk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/ghvyoyons.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.tarul.cn/Article/details/gyhjqzzgs.sHtML

[E02] 重复字符串
来源：http://m.share.bbcook.cn/Article/details/gyvptlgno.sHtML

Py:   "ab" * 3
来源：http://baike.fktsv.cn/Article/details/glprhapgd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/gltuwebti.sHtML

JS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gshawiopx.sHtML

TS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/glzblhvqt.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gnxydxlex.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.sjlbkw.cn/Article/details/gsrexeihj.sHtML

Ruby: "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/geercgjkq.sHtML


<!-- 参考信息 -->