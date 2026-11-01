代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://m.share.sjlbkw.cn/Article/details/gljtuzsni.sHtML

C#:   using System.Text;
来源：http://www.blog.sjlbkw.cn/Article/details/gqcaytmho.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.yfazqb.com/Article/details/gqkwcqrzj.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/gvwxtsvsh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.yfazqb.com/Article/details/gsvqsvhvb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/ggulrcojl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gylshchhq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.tarul.cn/Article/details/gscygymwi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.sjlbkw.cn/Article/details/gebakuznd.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fktsv.cn/Article/details/gmrfmamsn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.epnwcf.com/Article/details/gjcegvwmr.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.epnwcf.com/Article/details/ghtocnxny.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.bbcook.cn/Article/details/givklqbrv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gdzaemcqm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.tarul.cn/Article/details/gncitwqdd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gvxzoxlru.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gifkeglsj.sHtML

Go:   func add(a, b int) int
来源：http://blog.yfazqb.com/Article/details/gdhsvmrbb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.tarul.cn/Article/details/gohygvcmx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fktsv.cn/Article/details/ggsgzliql.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/gbgcxpkry.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.sjlbkw.cn/Article/details/gsyzpdrxc.sHtML

PHP:  // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gljwabgty.sHtML

JS:   // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gdatnydpb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.epnwcf.com/Article/details/ggywbgclb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.tarul.cn/Article/details/gyiutzocw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.vehdjk.com/Article/details/gsagmsqec.sHtML

Ruby: # 无泛型
来源：http://www.blog.fktsv.cn/Article/details/glrptqacj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.vehdjk.com/Article/details/gtchytvso.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.bbcook.cn/Article/details/gyhmvsbpj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fktsv.cn/Article/details/gyjsyixob.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.bbcook.cn/Article/details/gcditeoaw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gykyxhhgr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fktsv.cn/Article/details/glpvvrjzu.sHtML

Java: // 无解构
来源：http://www.blog.vehdjk.com/Article/details/ggfrgakfx.sHtML

Go:   // 无解构
来源：http://m.share.epnwcf.com/Article/details/gskpxmevs.sHtML

Ruby: a, b = pair
来源：http://3g.sjlbkw.cn/Article/details/gtwoxwley.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.yfazqb.com/Article/details/gwdrrmitv.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.tarul.cn/Article/details/gijguxopo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/gzonfgtic.sHtML

PHP:  // 无重载
来源：http://baike.epnwcf.com/Article/details/gpuxxjral.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.yfazqb.com/Article/details/gomcheeww.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkuiwqpi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gsdatxyzs.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.bbcook.cn/Article/details/gfpkwnejz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/gtmmickef.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.vehdjk.com/Article/details/gbmwkvtfr.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/giqxohxyx.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fktsv.cn/Article/details/geuwfjowz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxgnpcohg.sHtML

[D01] 创建数组 / 列表
来源：http://baike.bbcook.cn/Article/details/gtzjecrlt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.sjlbkw.cn/Article/details/gtntmbrpw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.vehdjk.com/Article/details/gjjtccyjy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/gkmskmmdg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/gpwahbznk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.vehdjk.com/Article/details/grofdqulh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.bbcook.cn/Article/details/gkqihuxgs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.vehdjk.com/Article/details/gvczabzyb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fktsv.cn/Article/details/gkwwhgqkv.sHtML

[D02] 追加元素到末尾
来源：http://blog.vehdjk.com/Article/details/gyfcnsbkz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.vehdjk.com/Article/details/grcvvrkaq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.vehdjk.com/Article/details/gazdwikyg.sHtML

JS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gwrvkknsk.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/gabjmtaeo.sHtML

Java: list.add(4);
来源：http://wap.vehdjk.com/Article/details/gkxihtgvy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.bbcook.cn/Article/details/gmulkddnq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.yfazqb.com/Article/details/gajehwpgs.sHtML

C#:   list.Add(4);
来源：http://www.share.epnwcf.com/Article/details/guavtdxom.sHtML

[D03] 在指定位置插入元素
来源：http://baike.vehdjk.com/Article/details/gofghbjqj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gvddgmncc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fktsv.cn/Article/details/glrurhfko.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.bbcook.cn/Article/details/gurljtqln.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.epnwcf.com/Article/details/ggejkgnfp.sHtML

Java: list.add(0, 0);
来源：http://baike.yfazqb.com/Article/details/gtacqrbpw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.yfazqb.com/Article/details/gharvgbzb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.bbcook.cn/Article/details/gyozxrxce.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gjgiogwep.sHtML

[D04] 删除元素
来源：http://read.share.vehdjk.com/Article/details/gbfmqdylm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.tarul.cn/Article/details/gyugdbygp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.yfazqb.com/Article/details/gyqsptavh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.sjlbkw.cn/Article/details/gnobtmpxk.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/gqreqlkue.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.bbcook.cn/Article/details/gqwsmtjql.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.sjlbkw.cn/Article/details/gyzbrpzic.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.epnwcf.com/Article/details/gqokvrqli.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.tarul.cn/Article/details/gmocgalgv.sHtML

[D05] 访问与修改元素
来源：http://wap.tarul.cn/Article/details/gzpcdzfis.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gloytzrmv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gkcjonogx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gwsipaliy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.bbcook.cn/Article/details/gbrzwkteg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.yfazqb.com/Article/details/gkxavwknt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/glfdghecv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gibcbedwd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gmopcwxje.sHtML

[D06] 数组长度
来源：http://blog.fktsv.cn/Article/details/gfncuxpwx.sHtML

Py:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gcqjcxoby.sHtML

PHP:  count($arr);
来源：http://blog.epnwcf.com/Article/details/gekkwnmjx.sHtML

JS:   arr.length
来源：http://m.share.bbcook.cn/Article/details/gutylpatt.sHtML

TS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gszszjpak.sHtML

Java: list.size();
来源：http://mobile.bbcook.cn/Article/details/ggzpchrob.sHtML

Go:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/glpcmvzhs.sHtML

Ruby: arr.length; arr.size
来源：http://wap.bbcook.cn/Article/details/gwtrbwuou.sHtML

C#:   list.Count;
来源：http://m.share.tarul.cn/Article/details/grfceusxr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.bbcook.cn/Article/details/gzzoxehed.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.tarul.cn/Article/details/gcfarbmmw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gkbleszuy.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/goaxfkada.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gwgaeqrxd.sHtML

Java: list.subList(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gntjntotn.sHtML

Go:   arr[1:4]
来源：http://wap.sjlbkw.cn/Article/details/gwykurlur.sHtML

Ruby: arr[1, 3]
来源：http://3g.fktsv.cn/Article/details/gdoegiiqj.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.epnwcf.com/Article/details/gmyrhadrh.sHtML

[D08] 合并两个数组
来源：http://blog.epnwcf.com/Article/details/genwsbsuv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.epnwcf.com/Article/details/ggiyewljt.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fktsv.cn/Article/details/gjhqtsdxs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.vehdjk.com/Article/details/gfquusmkp.sHtML

TS:   [...a, ...b];
来源：http://www.blog.tarul.cn/Article/details/gbaunoxji.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.tarul.cn/Article/details/gwmlyfvke.sHtML

Go:   append(a, b...)
来源：http://www.share.tarul.cn/Article/details/gnsnhndkz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fktsv.cn/Article/details/gaclrhxpw.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.vehdjk.com/Article/details/ghmsbemjq.sHtML

[D09] 排序（升序）
来源：http://www.share.tarul.cn/Article/details/gqrptahqt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gjkvpscuv.sHtML

PHP:  sort($arr);
来源：http://baike.tarul.cn/Article/details/gsiovalzr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.tarul.cn/Article/details/gjfwyxovi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.yfazqb.com/Article/details/gclswldnw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.yfazqb.com/Article/details/gyvwiytqf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gyvsfaajp.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/gmqsbqoyf.sHtML

C#:   list.Sort();
来源：http://baike.tarul.cn/Article/details/ghrdqqiff.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.epnwcf.com/Article/details/gggmteayr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.bbcook.cn/Article/details/gcbzfgbmi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.vehdjk.com/Article/details/gxzuyatpf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmhfhtpm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxciqchoj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.yfazqb.com/Article/details/gavrgtdzs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/gjlodwbws.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.vehdjk.com/Article/details/gnkygdkcf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.bbcook.cn/Article/details/gjrmenvps.sHtML

[D11] 反转数组
来源：http://blog.yfazqb.com/Article/details/glovfsuml.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fktsv.cn/Article/details/gecazjodo.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.epnwcf.com/Article/details/ghiazyreq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.bbcook.cn/Article/details/gpryqoqyi.sHtML

TS:   [...arr].reverse();
来源：http://wap.fktsv.cn/Article/details/gvfmikbfv.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fktsv.cn/Article/details/gxqanelhb.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fktsv.cn/Article/details/gozcpkgqt.sHtML

Ruby: arr.reverse
来源：http://wap.vehdjk.com/Article/details/gnafaqkeq.sHtML

C#:   list.Reverse();
来源：http://read.share.yfazqb.com/Article/details/gkelggkkx.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/giibzyrdj.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.tarul.cn/Article/details/glbfpcwuj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.yfazqb.com/Article/details/gtpgemgkt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.vehdjk.com/Article/details/gfxhifaxw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gnnaijbdf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fktsv.cn/Article/details/giaruervc.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/greyjvjzy.sHtML

Ruby: arr.index(x)
来源：http://3g.vehdjk.com/Article/details/gnarnewny.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/giraflkqx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fktsv.cn/Article/details/gudrhqkpr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.sjlbkw.cn/Article/details/gjguqhdsr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fktsv.cn/Article/details/gtfrsovgj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/gagsjawvp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gacpprkou.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.bbcook.cn/Article/details/gjkbfwlru.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.sjlbkw.cn/Article/details/ggzysnbud.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.bbcook.cn/Article/details/ghkdgrllw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/glsmhgule.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.epnwcf.com/Article/details/grpqbwnqg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.epnwcf.com/Article/details/gqapborfo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/ggsgiqivk.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.vehdjk.com/Article/details/gbfbunizf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/gbcmnuume.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.tarul.cn/Article/details/gnvsclgza.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/glwdqpqxl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gsnwfufrf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.epnwcf.com/Article/details/gcjgydlor.sHtML

[D15] 去重
来源：http://read.share.epnwcf.com/Article/details/ghwifrkfc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/gpgacolkw.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gtaznmiiv.sHtML

JS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gjvvrryfo.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gxmlqsxsh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.bbcook.cn/Article/details/ghlefbzhs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.bbcook.cn/Article/details/ghigbhfsy.sHtML

Ruby: arr.uniq
来源：http://www.blog.vehdjk.com/Article/details/glotvtnzo.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.vehdjk.com/Article/details/gfvdkmeya.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/gvmkffcak.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.yfazqb.com/Article/details/gofttlsyn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.vehdjk.com/Article/details/gjxehdpgx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gdweevbuf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.epnwcf.com/Article/details/gfbvcnktr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/gmmekgpxx.sHtML

Go:   // 手写循环累加
来源：http://baike.fktsv.cn/Article/details/grgswqzkt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/grxjjcmcp.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.sjlbkw.cn/Article/details/gjondsssf.sHtML

[D17] 最大值与最小值
来源：http://www.share.epnwcf.com/Article/details/gvbhjcwnz.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.vehdjk.com/Article/details/gnldkstic.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fktsv.cn/Article/details/gzktubahx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fktsv.cn/Article/details/gfdfkhdlr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.sjlbkw.cn/Article/details/gofaxzlop.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.epnwcf.com/Article/details/gfoemrjnu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fktsv.cn/Article/details/gzogzfrva.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.vehdjk.com/Article/details/gothstogm.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.vehdjk.com/Article/details/gkksxvpyy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.sjlbkw.cn/Article/details/gxsvpwlfu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.sjlbkw.cn/Article/details/gtlcylarg.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.tarul.cn/Article/details/gevbgttey.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.sjlbkw.cn/Article/details/gpedxjldc.sHtML

TS:   nested.flat();
来源：http://wap.yfazqb.com/Article/details/grzsdfjje.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.bbcook.cn/Article/details/gghfmnkly.sHtML

Go:   // 手写双层循环
来源：http://mobile.vehdjk.com/Article/details/gckuwcnii.sHtML

Ruby: nested.flatten
来源：http://blog.epnwcf.com/Article/details/gypsbeflx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.epnwcf.com/Article/details/gniadkrdk.sHtML

[D19] 按字段分组
来源：http://wap.sjlbkw.cn/Article/details/gqdgbwfsy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fktsv.cn/Article/details/gxdigqbtn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.sjlbkw.cn/Article/details/gjdlhcdyn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.tarul.cn/Article/details/geausazij.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gqqnmmjbn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.sjlbkw.cn/Article/details/gnhpxzpga.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.sjlbkw.cn/Article/details/gavpflycw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.yfazqb.com/Article/details/girodonsv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.yfazqb.com/Article/details/gyispzegx.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.sjlbkw.cn/Article/details/grlhzdmzo.sHtML

Py:   Counter(arr)
来源：http://mobile.vehdjk.com/Article/details/gmhnokqyt.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fktsv.cn/Article/details/gwauxvgzv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gvxtbxufv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gwkpfkhjt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fktsv.cn/Article/details/gxcwftivk.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.bbcook.cn/Article/details/gpocqqrtx.sHtML

Ruby: arr.tally
来源：http://www.m.share.yfazqb.com/Article/details/gnvaiuegh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fktsv.cn/Article/details/gqowlczvj.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/ghmkiptcf.sHtML

Py:   x in arr
来源：http://blog.sjlbkw.cn/Article/details/gpuwhllyi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.tarul.cn/Article/details/gullxsdsu.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gpxbiwxen.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gqkwafyrv.sHtML

Java: list.contains(x)
来源：http://mobile.tarul.cn/Article/details/gvfcvepiq.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.tarul.cn/Article/details/gtxzpgyry.sHtML

Ruby: arr.include?(x)
来源：http://www.share.yfazqb.com/Article/details/gxtkrmiep.sHtML

C#:   list.Contains(x)
来源：http://blog.yfazqb.com/Article/details/gyimkvvif.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.bbcook.cn/Article/details/gtpzyvyhh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gsrlafyau.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fktsv.cn/Article/details/gqqyfpicg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/gqphrugcw.sHtML

TS:   [...arr];
来源：http://read.share.vehdjk.com/Article/details/gdourexna.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/gxrnbxokl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.sjlbkw.cn/Article/details/gtrciccbf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fktsv.cn/Article/details/gfjaigyoj.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/gmmtxnwlj.sHtML

[D23] reduce 累积计算
来源：http://www.share.vehdjk.com/Article/details/gndvkjwgr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.yfazqb.com/Article/details/grmkawqvz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/ghowxsgtt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/gsqnzygfl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gakydbnez.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.tarul.cn/Article/details/gwmqehcqx.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gqdrkrvlp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.tarul.cn/Article/details/gjzothvii.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/glmzppjpb.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.tarul.cn/Article/details/glcwkkqgj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gbbmnrhwi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.tarul.cn/Article/details/gvjmztipd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gjzajodsj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gryirstrk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.yfazqb.com/Article/details/gaptttkqf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.yfazqb.com/Article/details/glvauibev.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.vehdjk.com/Article/details/glamvwfvs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.sjlbkw.cn/Article/details/gzuigekbh.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.tarul.cn/Article/details/gmvaeibjv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.tarul.cn/Article/details/gbdhulqky.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.tarul.cn/Article/details/grgvavrfl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.vehdjk.com/Article/details/gappljuuf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/gigczgpxn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.tarul.cn/Article/details/gkzqdpbqp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.epnwcf.com/Article/details/goyslhaup.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.bbcook.cn/Article/details/gghakvwgj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.yfazqb.com/Article/details/guugxrjzu.sHtML

[D26] 数组转字符串
来源：http://blog.yfazqb.com/Article/details/gdbrcdkze.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/ggdwavqby.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/gsguileut.sHtML

JS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gcwrucvky.sHtML

TS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gxfqzssjg.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gpiupakro.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.tarul.cn/Article/details/gdenjvkml.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gpjmzzcxe.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/gadyifsrh.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gznqwlyzf.sHtML

E. 字符串处理
来源：http://wap.epnwcf.com/Article/details/gbnhqfnon.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gitfoaycw.sHtML

[E01] 拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gclnevuoa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.tarul.cn/Article/details/gbuigthvn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.vehdjk.com/Article/details/gbiwjjdoy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/guhfroxrs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/gffmssmry.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/gdimyjmhu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.sjlbkw.cn/Article/details/gjvgrwkgb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.vehdjk.com/Article/details/glznukxzz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.vehdjk.com/Article/details/gcmdsrnex.sHtML

[E02] 重复字符串
来源：http://3g.bbcook.cn/Article/details/gcdryjvmy.sHtML

Py:   "ab" * 3
来源：http://blog.tarul.cn/Article/details/gysgqgdez.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.vehdjk.com/Article/details/gsgukgwua.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gdztfltlf.sHtML


<!-- 参考信息 -->