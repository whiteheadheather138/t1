代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://eip.tianlin.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://ndi.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jdn.epnwcf.com

Ruby: def greet(name = "World") = name
来源：http://ryi.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://uun.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://cmk.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://apj.nanxinkj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xpl.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tax.jinyuanbaomall.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bhx.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mto.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pbn.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://kwb.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ztd.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://ixs.ydzc1.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mxv.gogol.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gnf.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lmn.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://iwi.ybcxt.top

Java: // 无：用 Builder 模式或 record
来源：http://dsn.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://sza.havefunace.top

Ruby: f(a: 1, b: 2)
来源：http://byg.fzhhl.top

C#:   f(a: 1, b: 2)
来源：http://hgp.zdbjq.cn

[C05] 返回多个值
来源：http://ifj.xinyue.icu

Py:   return a, b
来源：http://hln.shanyushiyangtech.top

PHP:  return [$a, $b];
来源：http://euu.jlsjyb.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://omh.shanyushiyangkeji.top

TS:   return { a, b };
来源：http://ufx.aibaodan.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vsc.yueranfly.top

Go:   return a, b
来源：http://gnt.dashuyun.cn

Ruby: return a, b
来源：http://xok.xziqi.cn

C#:   return (a, b);              // ValueTuple
来源：http://rit.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://kpm.meibo888.top

Py:   square = lambda x: x * x
来源：http://cpl.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://zyk.mhx1999.top

JS:   const square = x => x * x;
来源：http://kgm.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://pdv.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hxw.zdqjudy.top

Go:   sq := func(x int) int { return x * x }
来源：http://def.sysykeji.top

Ruby: square = ->(x) { x * x }
来源：http://ich.ydzc1.top

C#:   Func<int, int> square = x => x * x;
来源：http://new.fehbvm.com

[C07] 把函数作为参数传入
来源：http://prf.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rrf.ydzc1.top

PHP:  array_map("strtoupper", $arr);
来源：http://uyw.sxryk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lwo.ydjk.org.cn

TS:   arr.map(String)
来源：http://pnr.cqqwz.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qkc.yj20258.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zmx.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://ydd.yfazqb.com

C#:   arr.Select(s => s.ToUpper())
来源：http://qoe.svipenyu.cn

[C08] 闭包
来源：http://ffl.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xtu.ctjpmb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yqu.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://htc.epnwcf.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tmy.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://btl.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://peu.c1oappe.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://deg.zhengqikj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://liy.jqgufenzy.top

[C09] 递归
来源：http://jvm.shangyingyoupin.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ood.ydzc1.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rpd.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://drg.yueranfly.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qvv.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nop.aibaodan.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tft.jqgfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ifi.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dge.haohaochexian.top

[C10] 变量作用域
来源：http://rdw.bbcook.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xdn.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iia.ivvv.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://idz.pengpengdd.cyou

TS:   同 JS
来源：http://inc.zhixingplan.top

Java: 方法内为块级作用域
来源：http://tzi.shuidangran.top

Go:   花括号块级作用域
来源：http://vpp.fehbvm.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://lbp.ppjwa.cn

C#:   块级作用域
来源：http://lws.sjlbkw.cn

[C11] 模块导入与导出
来源：http://sdh.jinqigufen.top

Py:   from module import func
来源：http://rju.jinqigfzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://eyi.aibaodan.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://flj.yangfankeji.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://twm.tianlin.xyz

Java: import java.util.List;
来源：http://wyj.andypj.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jcd.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://ooj.xingfuxueyuan.xyz

C#:   using System.Text;
来源：http://kam.tanke756.top

[C12] 立即执行函数 IIFE
来源：http://avt.svipenyu.cn

Py:   (lambda: print("run"))()
来源：http://kuz.xylfe.cn

PHP:  (function () { echo "run"; })();
来源：http://ets.vqdsnc.cn

JS:   (() => { console.log("run"); })();
来源：http://uqb.tarul.cn

TS:   (() => { console.log("run"); })();
来源：http://uwh.meibo888.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dkg.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://xjc.hnxiangtu.top

Ruby: -> { puts "run" }.call
来源：http://asd.9152youxi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gvh.dashuyun.cn

[C13] 类型声明 / 类型注解
来源：http://lvh.yfazqb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bfa.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gyq.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xhr.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lgf.tianlin.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://woy.dianchejie.cn

Go:   func add(a, b int) int
来源：http://vyq.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qqq.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://inv.jlsjyb.cn

[C14] 泛型函数
来源：http://hou.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xse.vqdsnc.cn

PHP:  // 无泛型
来源：http://pgb.jinyuanbaomall.cn

JS:   // 无泛型
来源：http://ssv.9152youxi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ate.tian-w.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lbp.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jpq.birdmap.top

Ruby: # 无泛型
来源：http://uzj.cucudq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sjp.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://wrh.tarul.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uhy.yuxming.cn

PHP:  [$a, $b] = $pair;
来源：http://qgp.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ish.dianchejie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oqw.shzxlz.cn

Java: // 无解构
来源：http://tgi.zhijiandao.cn

Go:   // 无解构
来源：http://iro.zdbjq.cn

Ruby: a, b = pair
来源：http://dav.aibaodan.cn

C#:   var (a, b) = pair;
来源：http://jvc.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://ltr.fengsongda.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pqt.ydzc1.top

PHP:  // 无重载
来源：http://fld.zhiwuduotai.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ezq.pengpengdd.cyou

TS:   // 用联合类型或重载签名声明
来源：http://kex.zhiwuduotai.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wws.shuidangran.top

Go:   // 无重载：用不同函数名
来源：http://zbo.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://ykh.jinyuanbaomall.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mzc.jinqigufen.top

================================================================================
来源：http://ktk.52xcode.cn

D. 数组 / 列表 / 集合
来源：http://vrb.316326.xyz

================================================================================
来源：http://kts.ydjk.org.cn

[D01] 创建数组 / 列表
来源：http://nah.yangfankeji.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://tou.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://olg.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://apu.zhoulong.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://bbc.chenzaomai.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hxe.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://nih.birdmap.top

Ruby: arr = [1, 2, 3]
来源：http://hke.yj202588.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wqx.nanxinkj.top

[D02] 追加元素到末尾
来源：http://waz.shangyingyoupin.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vrl.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://goh.yj20258.top

JS:   arr.push(4);
来源：http://bzv.hammf.cn

TS:   arr.push(4);
来源：http://xyi.andypj.xyz

Java: list.add(4);
来源：http://cxh.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://hgz.bbcook.cn

Ruby: arr << 4; arr.push(5)
来源：http://mrk.fehbvm.com

C#:   list.Add(4);
来源：http://gnu.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://zcs.ctjpmb.com

Py:   arr.insert(0, 0)
来源：http://jlg.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ooz.redwolf501.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ayw.vehdjk.com

TS:   arr.splice(0, 0, 0);
来源：http://lfs.nwbrower.top

Java: list.add(0, 0);
来源：http://xhm.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://bvn.aizwys.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ixt.tarul.cn

C#:   list.Insert(0, 0);
来源：http://kxw.birdmap.top

[D04] 删除元素
来源：http://eiy.bbcook.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gqt.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bii.ywan-chungtsiang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hzy.yj20258.top

TS:   arr.splice(0, 1);
来源：http://hnr.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://byt.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dna.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gcg.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zvx.9152youxi.cn

[D05] 访问与修改元素
来源：http://onw.nanxinkj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tpj.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gcd.yueranfly.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mvk.gotoacloud.top

TS:   arr[0]; arr.at(-1);
来源：http://obh.chenlongwang.top

Java: list.get(0); list.set(0, 9);
来源：http://wqf.yuanzhike.top

Go:   arr[0]; arr[0] = 9
来源：http://iit.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bps.sufxvd.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mua.kuanghao11.cn

[D06] 数组长度
来源：http://gky.fanxiaobao.xyz

Py:   len(arr)
来源：http://aaz.yangfankeji.com

PHP:  count($arr);
来源：http://asa.nanxuanxn.top

JS:   arr.length
来源：http://aan.ctjpmb.com

TS:   arr.length
来源：http://mla.52xcode.cn

Java: list.size();
来源：http://tff.zhaomingkeji.xyz

Go:   len(arr)
来源：http://sdz.iojbl.cn

Ruby: arr.length; arr.size
来源：http://eia.yueranfly.top

C#:   list.Count;
来源：http://cab.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://dyz.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vjf.fengsongda.top

PHP:  array_slice($arr, 1, 3);
来源：http://dqh.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://egw.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://qqh.yongpay.top

Java: list.subList(1, 4);
来源：http://kqa.ydzc1.top

Go:   arr[1:4]
来源：http://vrd.daxiang520.top

Ruby: arr[1, 3]
来源：http://scy.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://pdb.yueranfly.top

[D08] 合并两个数组
来源：http://tbk.dianchejie.cn

Py:   a + b;  a.extend(b)
来源：http://sit.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://ugk.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ijs.hongshengwenyu.top

TS:   [...a, ...b];
来源：http://iqe.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ctf.xuanzx.com

Go:   append(a, b...)
来源：http://hip.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://oiw.xinyue.icu

C#:   a.Concat(b).ToList()
来源：http://jsi.cucudq.cn

[D09] 排序（升序）
来源：http://unu.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://itf.xylfe.cn

PHP:  sort($arr);
来源：http://qgj.sysykeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bar.havefunace.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wyh.jqgfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gvn.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zow.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://uzv.yj20258.top

C#:   list.Sort();
来源：http://npu.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pyu.yj20258888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wav.uphjek.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lxv.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wqs.yj20258888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ihn.birdmap.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yaz.zhixingplan.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qbv.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wxc.nanxuanxn.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lkw.gaohongyu789.top

[D11] 反转数组
来源：http://qur.guannengcc.top

Py:   arr[::-1];  arr.reverse()
来源：http://fws.ivvv.top

PHP:  array_reverse($arr);
来源：http://uhw.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://szv.dianchejie.cn

TS:   [...arr].reverse();
来源：http://vng.hysaishi.cn

Java: Collections.reverse(list);
来源：http://jrx.ehwqpu.com

Go:   slices.Reverse(arr)
来源：http://mhm.yuanzhike.top

Ruby: arr.reverse
来源：http://kln.yangfankeji.com

C#:   list.Reverse();
来源：http://wco.zhoulong.xyz

[D12] 查找元素下标
来源：http://jgo.ivvv.top

Py:   arr.index(x);  x in arr
来源：http://int.haohaochexian.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ais.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wve.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://buw.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://glm.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://rqu.yfazqb.com

Ruby: arr.index(x)
来源：http://mfn.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://ftb.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://kwj.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://due.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dgu.ctjpmb.com

JS:   arr.filter(x => x > 3)
来源：http://wml.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://jif.zhoulong.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jud.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ans.havefunace.top

Ruby: arr.select { |x| x > 3 }
来源：http://rrx.xingfuxueyuan.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://jzz.meibo888.top

[D14] 映射转换（每个元素变形）
来源：http://kna.hywenlv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cwh.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rsf.hywenlv.cn

JS:   arr.map(x => x * 2)
来源：http://oso.dashuyun.cn

TS:   arr.map(x => x * 2)
来源：http://xpg.guannengcc.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://nhr.birdmap.top

Go:   // 手写循环
来源：http://fox.dianchejie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xiz.xingfuxueyuan.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://mzt.xuetiantiany.cn

[D15] 去重
来源：http://zmw.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gmo.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://sph.zhoulong.xyz

JS:   [...new Set(arr)]
来源：http://ewe.pycfn.com

TS:   [...new Set(arr)]
来源：http://wpe.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cae.chenlongwang.top

Go:   // 用 map[T]struct{} 手写
来源：http://yzg.yj202588.top

Ruby: arr.uniq
来源：http://mnt.birdmap.top

C#:   list.Distinct().ToList()
来源：http://sok.chenzaomai.com

[D16] 求和与平均值
来源：http://fqo.epnwcf.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xvv.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qju.daxiang520.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ofq.hcnkem.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gkg.yangfankeji.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kau.zhongyouzk.top

Go:   // 手写循环累加
来源：http://pdn.wangshuangyany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ffl.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://bft.jinyuanbaomall.cn

[D17] 最大值与最小值
来源：http://itn.jiagoushi.top

Py:   max(arr);  min(arr)
来源：http://kdv.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://xua.guowangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eeh.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://rru.haohaochexian.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ohe.daxiang520.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ckx.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://wmg.gotoacloud.top

C#:   list.Max();  list.Min()
来源：http://wlr.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://meg.feifeiyinyue.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fwh.ybcxt.top

PHP:  array_merge(...$nested);
来源：http://zoe.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ocj.yongpay.top

TS:   nested.flat();
来源：http://htp.tanke756.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fes.uphjek.com

Go:   // 手写双层循环
来源：http://crl.quarkkingdee.top

Ruby: nested.flatten
来源：http://jqc.smart0.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://kib.jianghu66.top

[D19] 按字段分组
来源：http://ini.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jsj.tanke756.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://naf.gogol.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kuc.shuidangran.top


<!-- 参考信息 -->