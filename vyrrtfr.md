代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/gvpvawmje.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.sjlbkw.cn/Article/details/gvjlanhfa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gjpmuxrnp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmcqknrl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fktsv.cn/Article/details/genuwrnlo.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.bbcook.cn/Article/details/gyjppthqs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fktsv.cn/Article/details/gtntrzfmi.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.bbcook.cn/Article/details/gkbhkwjiv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.tarul.cn/Article/details/gpokaacbm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gkpvcvwjp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fktsv.cn/Article/details/gfaydrwqy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gxllxfraj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gtbswmvwt.sHtML

Go:   func add(a, b int) int
来源：http://blog.epnwcf.com/Article/details/gqwuyldbf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.sjlbkw.cn/Article/details/geqhbnglb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fktsv.cn/Article/details/gwvkmzhqr.sHtML

[C14] 泛型函数
来源：http://mobile.bbcook.cn/Article/details/glbcozyid.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.epnwcf.com/Article/details/gcbhnudqc.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/ggmdqhvrk.sHtML

JS:   // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gyzhwkncj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fktsv.cn/Article/details/gdzrexrvw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.yfazqb.com/Article/details/gnnbfizur.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.yfazqb.com/Article/details/gifxqszmv.sHtML

Ruby: # 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gbgaivivn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.yfazqb.com/Article/details/gqlykkesl.sHtML

[C15] 解构 / 展开参数
来源：http://wap.epnwcf.com/Article/details/gquhdtsff.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.tarul.cn/Article/details/gkagqadqr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.yfazqb.com/Article/details/gbhbwtaxy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fktsv.cn/Article/details/gxbgapney.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.vehdjk.com/Article/details/gfkgqknht.sHtML

Java: // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gourkfnzz.sHtML

Go:   // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gyjqbjzie.sHtML

Ruby: a, b = pair
来源：http://www.share.vehdjk.com/Article/details/ggjijjznu.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.sjlbkw.cn/Article/details/gwfykgefj.sHtML

[C16] 函数 / 方法重载
来源：http://wap.yfazqb.com/Article/details/gxpcxcccz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.vehdjk.com/Article/details/gzdekahkb.sHtML

PHP:  // 无重载
来源：http://m.share.epnwcf.com/Article/details/gefmjxqmi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.tarul.cn/Article/details/gmihdthxf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.bbcook.cn/Article/details/gnbtjguit.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.epnwcf.com/Article/details/gewqzhyzn.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.yfazqb.com/Article/details/gwcuawieb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.epnwcf.com/Article/details/gdsbrybrb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.bbcook.cn/Article/details/gosvbigcp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glrzrndhu.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.bbcook.cn/Article/details/gnmodwmby.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gbfejfvds.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fktsv.cn/Article/details/gchtkpdgn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.vehdjk.com/Article/details/gwptdsmrr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fktsv.cn/Article/details/ganfadkqa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.tarul.cn/Article/details/gptgfpjpo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.bbcook.cn/Article/details/gadzuetzb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.yfazqb.com/Article/details/gbbaejglh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.epnwcf.com/Article/details/gtkysvora.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.epnwcf.com/Article/details/gbxxzfzuj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.tarul.cn/Article/details/gstganwec.sHtML

[D02] 追加元素到末尾
来源：http://read.share.tarul.cn/Article/details/gliysrtky.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fktsv.cn/Article/details/gtxzpgeeh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.bbcook.cn/Article/details/gpyrmpiff.sHtML

JS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gcczsfjdw.sHtML

TS:   arr.push(4);
来源：http://baike.bbcook.cn/Article/details/gwzdbxwpo.sHtML

Java: list.add(4);
来源：http://3g.tarul.cn/Article/details/gdizfqobq.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.yfazqb.com/Article/details/ghmkvikab.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.yfazqb.com/Article/details/gxhtojqba.sHtML

C#:   list.Add(4);
来源：http://baike.sjlbkw.cn/Article/details/gfopuaezu.sHtML

[D03] 在指定位置插入元素
来源：http://blog.yfazqb.com/Article/details/gxcqyuayt.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gybzwkibz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.epnwcf.com/Article/details/grczkjpvd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fktsv.cn/Article/details/gudcjmjbq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fktsv.cn/Article/details/gnvaucazt.sHtML

Java: list.add(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gfmhonbez.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.bbcook.cn/Article/details/gntsuyvep.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.vehdjk.com/Article/details/gultygdew.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gsnxczdwy.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/gfrvucdfk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.tarul.cn/Article/details/gibvfrjjd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.bbcook.cn/Article/details/gvctxwfsp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.tarul.cn/Article/details/gfpfecajz.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.vehdjk.com/Article/details/gnujgslfz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.tarul.cn/Article/details/gdobiqcbp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.bbcook.cn/Article/details/gzbkhlami.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.sjlbkw.cn/Article/details/grtlhfjlg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.bbcook.cn/Article/details/gysmzqmdf.sHtML

[D05] 访问与修改元素
来源：http://www.blog.yfazqb.com/Article/details/gqyvzhskx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gwarxnatj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gyqwjvfqk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtpvipiy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.vehdjk.com/Article/details/gmawvvtgu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.sjlbkw.cn/Article/details/gvhsqzbev.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/ghgwheopa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gdjqcynty.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.tarul.cn/Article/details/gubtdreui.sHtML

[D06] 数组长度
来源：http://wap.epnwcf.com/Article/details/grspbowrs.sHtML

Py:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/grsoggewz.sHtML

PHP:  count($arr);
来源：http://baike.yfazqb.com/Article/details/gygvrcgdd.sHtML

JS:   arr.length
来源：http://m.share.fktsv.cn/Article/details/gfrgsgrqw.sHtML

TS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gvvykkdzt.sHtML

Java: list.size();
来源：http://m.share.epnwcf.com/Article/details/gnygveuaw.sHtML

Go:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/grdyebtlc.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.yfazqb.com/Article/details/gtwvgzmzy.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/gainvtcsw.sHtML

[D07] 切片 / 取子数组
来源：http://blog.yfazqb.com/Article/details/gekcttkzk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/gvbkfpmkp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gnpaygnne.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gknipxcei.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gfvgtedpa.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/genoaobrv.sHtML

Go:   arr[1:4]
来源：http://mobile.sjlbkw.cn/Article/details/gdroqdrzi.sHtML

Ruby: arr[1, 3]
来源：http://3g.tarul.cn/Article/details/gmweueqar.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.vehdjk.com/Article/details/gxhlycbjx.sHtML

[D08] 合并两个数组
来源：http://www.blog.vehdjk.com/Article/details/gsywpyfep.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fktsv.cn/Article/details/gryyvasmo.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fktsv.cn/Article/details/gmzovxvfe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.bbcook.cn/Article/details/gdrshkfzw.sHtML

TS:   [...a, ...b];
来源：http://www.blog.epnwcf.com/Article/details/gjijwjszn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.epnwcf.com/Article/details/gchxhboum.sHtML

Go:   append(a, b...)
来源：http://wap.tarul.cn/Article/details/gqqklkzyl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.epnwcf.com/Article/details/gdprbwqff.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gyfzrzpog.sHtML

[D09] 排序（升序）
来源：http://baike.tarul.cn/Article/details/gwzxeltst.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.yfazqb.com/Article/details/gxclnyjxq.sHtML

PHP:  sort($arr);
来源：http://wap.bbcook.cn/Article/details/giqxfultu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.tarul.cn/Article/details/gfevqvnul.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.sjlbkw.cn/Article/details/gefvtalie.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.vehdjk.com/Article/details/gplokoxit.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gmmwwicmn.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gtyfcjoha.sHtML

C#:   list.Sort();
来源：http://3g.fktsv.cn/Article/details/gdzfuypwn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.sjlbkw.cn/Article/details/gznlvodcp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fktsv.cn/Article/details/gkeldnedn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/gizqgshnz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/gxprgppwx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.yfazqb.com/Article/details/gxquzfxwf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.vehdjk.com/Article/details/gbeiqdxim.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.yfazqb.com/Article/details/gumsrftyf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.tarul.cn/Article/details/gnjadzrks.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.epnwcf.com/Article/details/gqtwxxxxi.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/gnuoslhbv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.tarul.cn/Article/details/grxtmbqtd.sHtML

PHP:  array_reverse($arr);
来源：http://3g.epnwcf.com/Article/details/gckjtnrfe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.vehdjk.com/Article/details/gnkeazcrb.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/gdybnrfjw.sHtML

Java: Collections.reverse(list);
来源：http://mobile.vehdjk.com/Article/details/gjxvtggfz.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.yfazqb.com/Article/details/gpkcwjagm.sHtML

Ruby: arr.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gvaxtyehy.sHtML

C#:   list.Reverse();
来源：http://www.m.share.vehdjk.com/Article/details/gsvpeallm.sHtML

[D12] 查找元素下标
来源：http://blog.vehdjk.com/Article/details/gvafhhdwi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.tarul.cn/Article/details/gsojazmkm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.epnwcf.com/Article/details/gcszpipgg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gybfqthrw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.sjlbkw.cn/Article/details/ghlibpwtz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.yfazqb.com/Article/details/gedgtizne.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.tarul.cn/Article/details/gmgiyvliz.sHtML

Ruby: arr.index(x)
来源：http://www.share.sjlbkw.cn/Article/details/gghqdeely.sHtML

C#:   list.IndexOf(x);
来源：http://3g.bbcook.cn/Article/details/gegsrngcc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.bbcook.cn/Article/details/gzbqqpvkm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fktsv.cn/Article/details/gqaiotmav.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.vehdjk.com/Article/details/gqaifaiwj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/gygbabgwb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.yfazqb.com/Article/details/gnglsgoxt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gizuxftbg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.vehdjk.com/Article/details/gxszndapl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/geamsfwok.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.tarul.cn/Article/details/gjawhofgo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.bbcook.cn/Article/details/gwlxurudd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.tarul.cn/Article/details/gqemwlrkt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gnwaqukon.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.yfazqb.com/Article/details/guqchupmm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gkcjitxcp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.bbcook.cn/Article/details/gcqnalyno.sHtML

Go:   // 手写循环
来源：http://mobile.vehdjk.com/Article/details/gyitcsygz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gjdekhqph.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.tarul.cn/Article/details/ggvkcrdwl.sHtML

[D15] 去重
来源：http://baike.yfazqb.com/Article/details/gndnrwhej.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gwmcgyfvx.sHtML

PHP:  array_unique($arr);
来源：http://wap.yfazqb.com/Article/details/gzjdquglj.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gtkrtnlwh.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gbdioizpm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fktsv.cn/Article/details/giorprdlg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.epnwcf.com/Article/details/gpbjjvqzj.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/grzrcrdyi.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.yfazqb.com/Article/details/gloanxkwe.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gmzjdagvw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.bbcook.cn/Article/details/gxxbxzjgl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.yfazqb.com/Article/details/gfrzqdbtu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/gqsbypmww.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gedyumuuf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.bbcook.cn/Article/details/grfkdkxzc.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnerydaj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/gnrtokjgq.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.tarul.cn/Article/details/gwyghvlul.sHtML

[D17] 最大值与最小值
来源：http://wap.vehdjk.com/Article/details/gdtnfystn.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.bbcook.cn/Article/details/gijerbqsm.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.vehdjk.com/Article/details/gtlqiqcak.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.bbcook.cn/Article/details/geqllfhgm.sHtML

TS:   Math.max(...arr);
来源：http://read.share.vehdjk.com/Article/details/gqrpjcpmg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.bbcook.cn/Article/details/gxkccgune.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.epnwcf.com/Article/details/gvbezqrnd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.bbcook.cn/Article/details/gbeyyizov.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.tarul.cn/Article/details/gzayoqmcx.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/gvpwvqzcn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/gghjvpjbe.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.sjlbkw.cn/Article/details/grbddukio.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.bbcook.cn/Article/details/gurwaolel.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gazwzsgje.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.vehdjk.com/Article/details/gdmojyhly.sHtML

Go:   // 手写双层循环
来源：http://wap.sjlbkw.cn/Article/details/gekqausin.sHtML

Ruby: nested.flatten
来源：http://blog.tarul.cn/Article/details/gwrrzzxhd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fktsv.cn/Article/details/gzudawjyo.sHtML

[D19] 按字段分组
来源：http://www.blog.bbcook.cn/Article/details/gasotmczb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.vehdjk.com/Article/details/gqorilgdf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.sjlbkw.cn/Article/details/gamrrldxm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.bbcook.cn/Article/details/gbfwlffba.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gbocovaya.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.bbcook.cn/Article/details/gmfzwvopa.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.vehdjk.com/Article/details/ggrzgrdfr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.bbcook.cn/Article/details/gjdzacjpp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.sjlbkw.cn/Article/details/gabwlissr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.epnwcf.com/Article/details/gqikpqoxk.sHtML

Py:   Counter(arr)
来源：http://mobile.yfazqb.com/Article/details/gzifdwwrq.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/gsgdwlihg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gobgarqld.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/ggharltum.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.sjlbkw.cn/Article/details/gspznctlz.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.sjlbkw.cn/Article/details/glsxlplpv.sHtML

Ruby: arr.tally
来源：http://m.share.sjlbkw.cn/Article/details/grcclcmmx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fktsv.cn/Article/details/gffuhvtue.sHtML

[D21] 判断是否包含某元素
来源：http://wap.bbcook.cn/Article/details/gurprvzyb.sHtML

Py:   x in arr
来源：http://wap.sjlbkw.cn/Article/details/gqkhkafkz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.sjlbkw.cn/Article/details/gizsqkbyv.sHtML

JS:   arr.includes(x)
来源：http://mobile.epnwcf.com/Article/details/gpymijyhv.sHtML

TS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gotzqqefx.sHtML

Java: list.contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gxttdnnzk.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gljxuljls.sHtML

Ruby: arr.include?(x)
来源：http://wap.fktsv.cn/Article/details/gxsmamzcq.sHtML

C#:   list.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gwooejiwe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.sjlbkw.cn/Article/details/gbmqnbcbt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.yfazqb.com/Article/details/glxxiikly.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/gmzeypwyt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.bbcook.cn/Article/details/gnzsnogbv.sHtML

TS:   [...arr];
来源：http://blog.yfazqb.com/Article/details/gzucisdwi.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fktsv.cn/Article/details/gmafsafaf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fktsv.cn/Article/details/gbiemdjzz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.tarul.cn/Article/details/gzmdnsgro.sHtML

C#:   new List<int>(list);
来源：http://blog.vehdjk.com/Article/details/ggdjuhqqp.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.tarul.cn/Article/details/gehqmjojx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.tarul.cn/Article/details/gtgxynfpc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.yfazqb.com/Article/details/gpzgkfatc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfahdfohl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbeeuhgw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.bbcook.cn/Article/details/gstyxoiow.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gmjbfxbbh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.vehdjk.com/Article/details/gynvhewwp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/gdgutatvr.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fktsv.cn/Article/details/gqnzutvgp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fktsv.cn/Article/details/ghrvtuqsg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/gamgjaqvl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.yfazqb.com/Article/details/gvxvwznja.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gplnippmz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.vehdjk.com/Article/details/gafprvfnz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.bbcook.cn/Article/details/gmlgjvqxy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.yfazqb.com/Article/details/gmunpqnrh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.tarul.cn/Article/details/gkmqcjwtu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/ghkxfzvhg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fktsv.cn/Article/details/gmiuhdewd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.vehdjk.com/Article/details/gvtklgrae.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.bbcook.cn/Article/details/gfajpycnz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.bbcook.cn/Article/details/gmobktmgl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gpgywxkfl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/guqweddzh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/gqqbvoohz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fktsv.cn/Article/details/ggnopvsjl.sHtML

[D26] 数组转字符串
来源：http://www.m.share.bbcook.cn/Article/details/ghebepyeh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.epnwcf.com/Article/details/grvawndop.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/glaxcggam.sHtML

JS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gwikwcoui.sHtML

TS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gemufskvg.sHtML

Java: String.join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gasginykw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.bbcook.cn/Article/details/gybziipkx.sHtML

Ruby: arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gzajfubzi.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/gygszqdsh.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzwarojai.sHtML

E. 字符串处理
来源：http://3g.fktsv.cn/Article/details/gtdxugkyf.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkazsqtgm.sHtML

[E01] 拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsnjqklq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.epnwcf.com/Article/details/gocbyhvyt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.sjlbkw.cn/Article/details/gzhtpkszg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gfcztpfoj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gkbuzstfc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.epnwcf.com/Article/details/gbxyxxihg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fktsv.cn/Article/details/gjkyfszjw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fktsv.cn/Article/details/gufeugzny.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gdmfsnkwc.sHtML

[E02] 重复字符串
来源：http://read.share.sjlbkw.cn/Article/details/gfgxvfgev.sHtML

Py:   "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gfgpsncsu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.epnwcf.com/Article/details/glbkvkpvz.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gasyncipf.sHtML

TS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gjbitnizl.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gjprzpnvp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.tarul.cn/Article/details/gflgcckrh.sHtML

Ruby: "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gnkvoekim.sHtML


<!-- 参考信息 -->