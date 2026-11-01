代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.yfazqb.com/Article/details/gvkaicnsd.sHtML

C#:   using System.Text;
来源：http://mobile.vehdjk.com/Article/details/gtpmjdtzc.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.tarul.cn/Article/details/gyxhaavfa.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.epnwcf.com/Article/details/ggfrhnbdc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fktsv.cn/Article/details/grtfikjyt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.bbcook.cn/Article/details/gikcbhnsn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/gnzimabjm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fktsv.cn/Article/details/gqkkiskdn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.yfazqb.com/Article/details/gyigziddc.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.epnwcf.com/Article/details/gcjhgpmlj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.epnwcf.com/Article/details/gygmrzsfd.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/gjqaexrza.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.sjlbkw.cn/Article/details/gmyqezsvb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gzxrvqfow.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.sjlbkw.cn/Article/details/gzlhbuomt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gsmvadidq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/ggnrpaizw.sHtML

Go:   func add(a, b int) int
来源：http://www.share.sjlbkw.cn/Article/details/gbnmnqjnp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.epnwcf.com/Article/details/gudwvrfeh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.yfazqb.com/Article/details/gvvnglirs.sHtML

[C14] 泛型函数
来源：http://www.share.vehdjk.com/Article/details/gcrnjohjx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.sjlbkw.cn/Article/details/gzrigizvz.sHtML

PHP:  // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gtqrgpdvr.sHtML

JS:   // 无泛型
来源：http://wap.epnwcf.com/Article/details/groukuezg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gejrxnxyr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.epnwcf.com/Article/details/gookzhcis.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fktsv.cn/Article/details/gggohmhcm.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fktsv.cn/Article/details/gbjwuizfa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.epnwcf.com/Article/details/gzsjahshh.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.tarul.cn/Article/details/gespwxkje.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.tarul.cn/Article/details/grgaamsxh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.bbcook.cn/Article/details/gnxkdqjgy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/gfmdqrsac.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fktsv.cn/Article/details/glnorrfol.sHtML

Java: // 无解构
来源：http://read.share.bbcook.cn/Article/details/gnfdfpnen.sHtML

Go:   // 无解构
来源：http://mobile.fktsv.cn/Article/details/gdwmmojsv.sHtML

Ruby: a, b = pair
来源：http://www.m.share.vehdjk.com/Article/details/gpfnumdzn.sHtML

C#:   var (a, b) = pair;
来源：http://baike.sjlbkw.cn/Article/details/gddstzbir.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.bbcook.cn/Article/details/gmecqeixg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fktsv.cn/Article/details/gizufnhos.sHtML

PHP:  // 无重载
来源：http://3g.tarul.cn/Article/details/gcfvitcgd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.bbcook.cn/Article/details/gvcfeyojd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.tarul.cn/Article/details/gsusjrxgt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fktsv.cn/Article/details/gxzbyqmlt.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.sjlbkw.cn/Article/details/gnexpetso.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.vehdjk.com/Article/details/geplthcjk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/glsldadmn.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gahrafant.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/gqeytnmgy.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gxhlppccf.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/giatpnexp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.bbcook.cn/Article/details/gxvzuxqdd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.tarul.cn/Article/details/gzuflyllp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.bbcook.cn/Article/details/gmvxoepbi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.sjlbkw.cn/Article/details/grzmjtkaz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.vehdjk.com/Article/details/gannmeaop.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.sjlbkw.cn/Article/details/glnixedtq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.sjlbkw.cn/Article/details/guaabfsdm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/glqcqpyzc.sHtML

[D02] 追加元素到末尾
来源：http://3g.sjlbkw.cn/Article/details/gcoetzmqj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.yfazqb.com/Article/details/gbgdtyhpx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gbomvwjbd.sHtML

JS:   arr.push(4);
来源：http://blog.sjlbkw.cn/Article/details/grqqopezf.sHtML

TS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gwvoivrox.sHtML

Java: list.add(4);
来源：http://blog.fktsv.cn/Article/details/gdsvzeefc.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.vehdjk.com/Article/details/gyohizial.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.epnwcf.com/Article/details/gcnenwwzw.sHtML

C#:   list.Add(4);
来源：http://m.share.vehdjk.com/Article/details/gylfecnyb.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.bbcook.cn/Article/details/galtesvcs.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fktsv.cn/Article/details/gjogkwcbc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/gfdbqepoj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fktsv.cn/Article/details/gkefghskx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.vehdjk.com/Article/details/gasgsyjbv.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gavmhluqe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fktsv.cn/Article/details/gwwlgkrff.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpujrzczj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.epnwcf.com/Article/details/gwdadbrht.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/garqbaroj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fktsv.cn/Article/details/gyaqhnqiz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/gtklavuvb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.sjlbkw.cn/Article/details/ghklcryly.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.sjlbkw.cn/Article/details/glrcuydtw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.yfazqb.com/Article/details/gzggklavb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/gpnblmfpm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.sjlbkw.cn/Article/details/gniwlypjj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.vehdjk.com/Article/details/gsqejnwgz.sHtML

[D05] 访问与修改元素
来源：http://www.share.vehdjk.com/Article/details/gezptxhkl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/goofsuynj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.epnwcf.com/Article/details/grhvsthsm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/glerirmiz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.tarul.cn/Article/details/gcnzobnln.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fktsv.cn/Article/details/gxuadzgjb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gmxiswzot.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gyutklfna.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.tarul.cn/Article/details/gpanubtmr.sHtML

[D06] 数组长度
来源：http://blog.tarul.cn/Article/details/gyfhtjuhp.sHtML

Py:   len(arr)
来源：http://baike.tarul.cn/Article/details/gsjuuurlj.sHtML

PHP:  count($arr);
来源：http://blog.fktsv.cn/Article/details/guupkacpj.sHtML

JS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/grzgptukj.sHtML

TS:   arr.length
来源：http://m.share.sjlbkw.cn/Article/details/geputwwhp.sHtML

Java: list.size();
来源：http://www.share.yfazqb.com/Article/details/gtmwlirma.sHtML

Go:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gaeleuioc.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.tarul.cn/Article/details/gyhkuxina.sHtML

C#:   list.Count;
来源：http://wap.vehdjk.com/Article/details/glrajrhot.sHtML

[D07] 切片 / 取子数组
来源：http://3g.vehdjk.com/Article/details/gjdjcmilv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.vehdjk.com/Article/details/gxdvtygip.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.vehdjk.com/Article/details/gdlijbesn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gqxznxmhi.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gkhtrbjrj.sHtML

Java: list.subList(1, 4);
来源：http://wap.fktsv.cn/Article/details/gcrrkvfcn.sHtML

Go:   arr[1:4]
来源：http://mobile.tarul.cn/Article/details/gwhsljuci.sHtML

Ruby: arr[1, 3]
来源：http://www.share.tarul.cn/Article/details/gwdzysvvs.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.tarul.cn/Article/details/gnilgicer.sHtML

[D08] 合并两个数组
来源：http://mobile.sjlbkw.cn/Article/details/gqcfrdoaz.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.yfazqb.com/Article/details/gljyeibae.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.tarul.cn/Article/details/geatlpzvt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.vehdjk.com/Article/details/glgxbofpf.sHtML

TS:   [...a, ...b];
来源：http://3g.epnwcf.com/Article/details/gqrelqulb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fktsv.cn/Article/details/ggqjtsytj.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/gpbfjnvsj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.bbcook.cn/Article/details/gulwgprjl.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.vehdjk.com/Article/details/glwgfqulb.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/ghqtzikup.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gnxgopojk.sHtML

PHP:  sort($arr);
来源：http://m.share.tarul.cn/Article/details/gycuwkihi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fktsv.cn/Article/details/gtnqumgux.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.vehdjk.com/Article/details/ghfkayeuw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.bbcook.cn/Article/details/gpppjtbho.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/gfttpijwu.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/guoanzhme.sHtML

C#:   list.Sort();
来源：http://baike.fktsv.cn/Article/details/gobfgrftx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.vehdjk.com/Article/details/gegfcvbjt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.sjlbkw.cn/Article/details/gpbdqdofw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.yfazqb.com/Article/details/grhzwjzjm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.sjlbkw.cn/Article/details/gedmgcxgm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.sjlbkw.cn/Article/details/gkpkstykd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fktsv.cn/Article/details/gkgyoqjmu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.tarul.cn/Article/details/guwstfvjy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.vehdjk.com/Article/details/gmmtwchvp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fktsv.cn/Article/details/gbmxnadcd.sHtML

[D11] 反转数组
来源：http://3g.bbcook.cn/Article/details/grwvbbdox.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.bbcook.cn/Article/details/gueskpwhq.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.epnwcf.com/Article/details/grvetsobz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.yfazqb.com/Article/details/gewwcitjl.sHtML

TS:   [...arr].reverse();
来源：http://baike.yfazqb.com/Article/details/gzgyyfnof.sHtML

Java: Collections.reverse(list);
来源：http://3g.tarul.cn/Article/details/gszspsfsu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.epnwcf.com/Article/details/gvbauvgmt.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/gsqobzfze.sHtML

C#:   list.Reverse();
来源：http://wap.bbcook.cn/Article/details/gaxueevab.sHtML

[D12] 查找元素下标
来源：http://read.share.tarul.cn/Article/details/giutlrsyo.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.vehdjk.com/Article/details/gzkyixtmt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.epnwcf.com/Article/details/gexmujsad.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.sjlbkw.cn/Article/details/gokknzsml.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gnquwnaxt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.bbcook.cn/Article/details/grzwkpnoi.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.epnwcf.com/Article/details/gksijkpzs.sHtML

Ruby: arr.index(x)
来源：http://blog.yfazqb.com/Article/details/gegoxlkon.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.bbcook.cn/Article/details/gblvztois.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.yfazqb.com/Article/details/gifmyowca.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.tarul.cn/Article/details/gicbbydiv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.vehdjk.com/Article/details/gsfxgvktj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/gzpophqib.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gnnoxaeoi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.epnwcf.com/Article/details/grbkgkzxx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.yfazqb.com/Article/details/gccbuxklq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fktsv.cn/Article/details/gaordbora.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.epnwcf.com/Article/details/guvytgqow.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.vehdjk.com/Article/details/gdizhltzu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.yfazqb.com/Article/details/gumabbuxh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gvuxqwzka.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gziuqhiqk.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gknqhffpl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.sjlbkw.cn/Article/details/gknuoozox.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gwmnbdabf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.epnwcf.com/Article/details/glwgrcqla.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.tarul.cn/Article/details/giugnkljo.sHtML

[D15] 去重
来源：http://mobile.yfazqb.com/Article/details/gxbdezzye.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gyewztmlc.sHtML

PHP:  array_unique($arr);
来源：http://baike.sjlbkw.cn/Article/details/gvujiddkc.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.tarul.cn/Article/details/gsasdpjvk.sHtML

TS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gnntcxoqn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.tarul.cn/Article/details/gapqzzloa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.vehdjk.com/Article/details/gbajlxcpi.sHtML

Ruby: arr.uniq
来源：http://www.blog.tarul.cn/Article/details/gqzcuaqbg.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.bbcook.cn/Article/details/gxdgvdyjx.sHtML

[D16] 求和与平均值
来源：http://baike.bbcook.cn/Article/details/gdjcdyztx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fktsv.cn/Article/details/gcdctdqaf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/gcobqxvqo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gnppqnsya.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gigbkrxdv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.yfazqb.com/Article/details/gqcsqpndz.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcrynent.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.yfazqb.com/Article/details/guszjjgdd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fktsv.cn/Article/details/gqjndzcqj.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gsbfqwiws.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.sjlbkw.cn/Article/details/gpznylkmh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gtdxtdfgh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.vehdjk.com/Article/details/gjymcquuy.sHtML

TS:   Math.max(...arr);
来源：http://baike.bbcook.cn/Article/details/glfntxlps.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.sjlbkw.cn/Article/details/gyuwsnuqt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gxxlfjjeo.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gwhgrshui.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fktsv.cn/Article/details/getxkhgfu.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.yfazqb.com/Article/details/gmrgqfznz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fktsv.cn/Article/details/gyzslweiq.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fktsv.cn/Article/details/gsqbzrkdp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.yfazqb.com/Article/details/gucixudlt.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/gywddgifw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.bbcook.cn/Article/details/gmklgmpdf.sHtML

Go:   // 手写双层循环
来源：http://blog.tarul.cn/Article/details/gqpzhpesz.sHtML

Ruby: nested.flatten
来源：http://3g.fktsv.cn/Article/details/grhmphcbb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gthzraggu.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/glfdlytzb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.vehdjk.com/Article/details/gdcbatzfa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.sjlbkw.cn/Article/details/gfqqdgilv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.bbcook.cn/Article/details/gphpaolms.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gmgxnvwbc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.tarul.cn/Article/details/gjfyvkzxm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fktsv.cn/Article/details/gdlcbppwf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.vehdjk.com/Article/details/giyzcsegt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.bbcook.cn/Article/details/gagpmdohq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.tarul.cn/Article/details/gcpjkuzxl.sHtML

Py:   Counter(arr)
来源：http://baike.vehdjk.com/Article/details/gyzonkvil.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.tarul.cn/Article/details/gcwikbrzo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gxnitpagd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gprfdhxhr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.tarul.cn/Article/details/gyvaxamjm.sHtML

Go:   // 手写 map[T]int
来源：http://baike.bbcook.cn/Article/details/gtnlomtjd.sHtML

Ruby: arr.tally
来源：http://www.share.tarul.cn/Article/details/gspvshrqi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.sjlbkw.cn/Article/details/grynilhii.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fktsv.cn/Article/details/giebtswok.sHtML

Py:   x in arr
来源：http://read.share.epnwcf.com/Article/details/grhgiuozj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/genuletor.sHtML

JS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gyyjkdrkm.sHtML

TS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/gsqrldoxw.sHtML

Java: list.contains(x)
来源：http://mobile.tarul.cn/Article/details/ghplijtid.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.tarul.cn/Article/details/gueiplrns.sHtML

Ruby: arr.include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gppladnql.sHtML

C#:   list.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gppgcknow.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.bbcook.cn/Article/details/gvqktkaxz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fktsv.cn/Article/details/galczebzc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/gquduepuw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqijpotg.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/gnzofimaf.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gyonxdpwv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.vehdjk.com/Article/details/gnrclhxvt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.yfazqb.com/Article/details/gapkmzhdz.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/ggnflvgyv.sHtML

[D23] reduce 累积计算
来源：http://www.share.yfazqb.com/Article/details/gwoklcsyi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gdnjtorhj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.tarul.cn/Article/details/gtfzbftbp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gknjnbgai.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/glpqcsoip.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.epnwcf.com/Article/details/gpldrkduq.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gohbokjgd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.sjlbkw.cn/Article/details/gjpqnlrjn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.sjlbkw.cn/Article/details/gwfiswnvi.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/gffggcfez.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.vehdjk.com/Article/details/gzvlgvdws.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.tarul.cn/Article/details/gwsdrbkui.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.epnwcf.com/Article/details/gyobpesqm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.yfazqb.com/Article/details/ghaqoaxmq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/gxsuhajhm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.tarul.cn/Article/details/gniyvxtip.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.tarul.cn/Article/details/givzcqxmh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fktsv.cn/Article/details/grpwjrmms.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.bbcook.cn/Article/details/gspufaebt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gmurpjjdy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.epnwcf.com/Article/details/gpzobvfre.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.bbcook.cn/Article/details/gxxrsbffr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.bbcook.cn/Article/details/gpcscuuan.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/guigihcru.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gkkhbngvk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.vehdjk.com/Article/details/gakfsrzxz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gskepnkis.sHtML

[D26] 数组转字符串
来源：http://baike.tarul.cn/Article/details/gcezunmld.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.tarul.cn/Article/details/gnkzigkmc.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gzlyjmxqn.sHtML

JS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gefhhzjhx.sHtML

TS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gxxmbujmj.sHtML

Java: String.join(", ", list)
来源：http://baike.tarul.cn/Article/details/giwwptcqa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/gfrpsqrep.sHtML

Ruby: arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gbfgtiyhg.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gtjtsajqm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnegetmec.sHtML

E. 字符串处理
来源：http://m.share.fktsv.cn/Article/details/gncppnlvg.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gzzvakbhm.sHtML

[E01] 拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gybahhggl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fktsv.cn/Article/details/grxevuqzx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.tarul.cn/Article/details/gtvdktgaw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gdldswupy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/guwjuvvnq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gvrralfpq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/gcvdxqsia.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.vehdjk.com/Article/details/gjfghnafv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gmdozvbcx.sHtML

[E02] 重复字符串
来源：http://mobile.yfazqb.com/Article/details/gdoupflai.sHtML

Py:   "ab" * 3
来源：http://wap.vehdjk.com/Article/details/ggoomogbb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.sjlbkw.cn/Article/details/gsrmlicqo.sHtML

JS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gyemqoqkc.sHtML


<!-- 参考信息 -->