代发 wailian999

Py:   def add(a, b): return a + b
来源：http://ieq.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rqr.52xcode.cn

JS:   function add(a, b) { return a + b; }
来源：http://lwp.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hwc.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yip.ywan-chungtsiang.top

Go:   func add(a, b int) int { return a + b }
来源：http://xrw.wangshuangyany.cn

Ruby: def add(a, b); a + b; end
来源：http://lcj.nanxinkj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sqa.sjlbkw.cn

[C02] 默认参数
来源：http://gvh.jqgufenzy.top

Py:   def greet(name="World"): return name
来源：http://oir.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rcz.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://zwj.zdbjq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://kfi.yj202588.top

Java: // 无默认参数：方法重载或 Optional
来源：http://aik.hongshengwenyu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tad.ywan-chungtsiang.top

Ruby: def greet(name = "World") = name
来源：http://ubl.bjfxy.top

C#:   string Greet(string name = "World") => name;
来源：http://gue.ehwqpu.com

[C03] 可变参数
来源：http://diq.cashguo.top

Py:   def total(*args): return sum(args)
来源：http://lae.fanxiaobao.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nsb.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dzd.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://sgo.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jvq.aibaodan.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dxu.pycfn.com

Ruby: def total(*nums); nums.sum; end
来源：http://kjx.aibaodan.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zko.jyoumei.cn

[C04] 命名参数 / 关键字参数
来源：http://ifn.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zyo.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tvu.yfazqb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hpw.xingfuxueyuan.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jnq.yuxming.cn

Java: // 无：用 Builder 模式或 record
来源：http://iyg.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://jon.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://ebq.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://hip.zhiwuduotai.top

[C05] 返回多个值
来源：http://jpx.pycfn.com

Py:   return a, b
来源：http://fgv.ctjpmb.com

PHP:  return [$a, $b];
来源：http://ilo.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hsj.gzhubu.top

TS:   return { a, b };
来源：http://zqj.hfpthk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zjv.fanxiaobao.xyz

Go:   return a, b
来源：http://xkq.hywenlv.cn

Ruby: return a, b
来源：http://khr.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://suv.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://rvu.dianchejie.cn

Py:   square = lambda x: x * x
来源：http://nyt.gaohongyu789.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sig.ivvv.top

JS:   const square = x => x * x;
来源：http://pyu.feifeiyinyue.top

TS:   const square = (x: number): number => x * x;
来源：http://kwh.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fae.guowangkeji.top

Go:   sq := func(x int) int { return x * x }
来源：http://hxf.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://acd.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://wks.shuidangran.top

[C07] 把函数作为参数传入
来源：http://gfk.ctjpmb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://obz.cqqwz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://flm.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://diw.yuanzhike.top

TS:   arr.map(String)
来源：http://geo.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kwq.gzhubu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://izt.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://qwb.yangfankeji.com

C#:   arr.Select(s => s.ToUpper())
来源：http://zsr.shanyushiyangkeji.top

[C08] 闭包
来源：http://dog.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ert.vqdsnc.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ifn.aibaodan.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wxs.xuanzx.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tep.jqgufenzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ckw.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nuc.sysykeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jtz.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jpz.cheryme.top

[C09] 递归
来源：http://lfm.guowangkeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qgr.daxiang520.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://klt.ppjwa.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://win.jlsjyb.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wft.dashuyun.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wva.shanyushiyangtech.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fvq.yonumen.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zqf.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sax.tian-w.cn

[C10] 变量作用域
来源：http://qlf.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://liq.zhixingplan.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xlf.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ppo.epnwcf.com

TS:   同 JS
来源：http://qtp.jyoumei.cn

Java: 方法内为块级作用域
来源：http://wwy.jianghu66.top

Go:   花括号块级作用域
来源：http://rpv.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kuj.pengpengdd.cyou

C#:   块级作用域
来源：http://iux.jinghuilouyu.cn

[C11] 模块导入与导出
来源：http://def.gaohongyu789.top

Py:   from module import func
来源：http://uvz.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://oih.redwolf501.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://myy.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zjn.iojbl.cn

Java: import java.util.List;
来源：http://ovl.hnqzz.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zso.tanke756.top

Ruby: require "json"; require_relative "./util"
来源：http://uxn.hnxiangtu.top

C#:   using System.Text;
来源：http://ctt.ivvv.top

[C12] 立即执行函数 IIFE
来源：http://jih.xuetiantiany.cn

Py:   (lambda: print("run"))()
来源：http://cat.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://tzk.svipenyu.cn

JS:   (() => { console.log("run"); })();
来源：http://hsj.kuanghao11.cn

TS:   (() => { console.log("run"); })();
来源：http://abw.zdbjq.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://npd.vehdjk.com

Go:   func() { fmt.Println("run") }()
来源：http://hmt.316326.xyz

Ruby: -> { puts "run" }.call
来源：http://ixl.nwbrower.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nka.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://niu.guowangkeji.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xwk.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ndm.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pwk.hongshengwenyu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oak.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://exk.tarul.cn

Go:   func add(a, b int) int
来源：http://ofv.52xcode.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bmj.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://pbz.yueranfly.top

[C14] 泛型函数
来源：http://cmc.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hmq.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://xfn.xuanzx.com

JS:   // 无泛型
来源：http://fhi.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vvj.vehdjk.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blx.fzhhl.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lhe.jlsjyb.cn

Ruby: # 无泛型
来源：http://xae.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://thb.ppjwa.cn

[C15] 解构 / 展开参数
来源：http://cww.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mwt.cqqwz.cn

PHP:  [$a, $b] = $pair;
来源：http://qtj.fengsongda.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ekz.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wuo.cucudq.cn

Java: // 无解构
来源：http://ifq.cashguo.top

Go:   // 无解构
来源：http://gwo.cheryme.top

Ruby: a, b = pair
来源：http://hai.nwbrower.top

C#:   var (a, b) = pair;
来源：http://jqo.quarkkingdee.top

[C16] 函数 / 方法重载
来源：http://nux.sxryk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rlf.zycfv.cn

PHP:  // 无重载
来源：http://ntg.hysaishi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lov.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://syn.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vsb.hammf.cn

Go:   // 无重载：用不同函数名
来源：http://ybp.zhijiandao.cn

Ruby: # 无重载：靠动态参数
来源：http://mha.pycfn.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://dlq.daria6918.cn

================================================================================
来源：http://kzm.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://wwb.hongshengwenyu.top

================================================================================
来源：http://slv.zhongyouzk.top

[D01] 创建数组 / 列表
来源：http://afz.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nfb.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ihb.bjfxy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ymo.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pwm.ydjk.org.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://imd.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://vtz.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://pwm.yvedp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hjl.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://oru.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cvc.daxiang520.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qhy.xuanzx.com

JS:   arr.push(4);
来源：http://hio.tian-w.cn

TS:   arr.push(4);
来源：http://znn.yangfankeji.com

Java: list.add(4);
来源：http://zbd.ywan-chungtsiang.top

Go:   arr = append(arr, 4)
来源：http://tkr.xylfe.cn

Ruby: arr << 4; arr.push(5)
来源：http://qra.yueranfly.top

C#:   list.Add(4);
来源：http://psz.jqgfzy.top

[D03] 在指定位置插入元素
来源：http://iyv.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://zov.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fqa.ppjwa.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://isb.dianchejie.cn

TS:   arr.splice(0, 0, 0);
来源：http://zsr.vehdjk.com

Java: list.add(0, 0);
来源：http://tse.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://fcz.nanxinkj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zet.ywan-chungtsiang.top

C#:   list.Insert(0, 0);
来源：http://bbr.zhaomingkeji.xyz

[D04] 删除元素
来源：http://qed.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://icq.guowangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jdt.zhoulong.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xez.gzhubu.top

TS:   arr.splice(0, 1);
来源：http://rkd.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yqe.ppjwa.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jvw.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://evw.yangfankeji.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://adl.vqdsnc.cn

[D05] 访问与修改元素
来源：http://jwf.aibaodan.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://spq.cashguo.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cit.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oug.bjfxy.top

TS:   arr[0]; arr.at(-1);
来源：http://tua.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://xms.gaohongyu789.top

Go:   arr[0]; arr[0] = 9
来源：http://iwj.uphjek.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kzw.sxryk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dcp.havefunace.top

[D06] 数组长度
来源：http://uei.hywenlv.cn

Py:   len(arr)
来源：http://hwm.epnwcf.com

PHP:  count($arr);
来源：http://tvn.nanxinkj.top

JS:   arr.length
来源：http://vth.andypj.xyz

TS:   arr.length
来源：http://ivg.gotoacloud.top

Java: list.size();
来源：http://pze.shuidangran.top

Go:   len(arr)
来源：http://czg.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://oaj.xziqi.cn

C#:   list.Count;
来源：http://nit.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://eed.shangyingyoupin.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://isy.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lcs.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://kig.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://arh.dashuyun.cn

Java: list.subList(1, 4);
来源：http://qwl.vqdsnc.cn

Go:   arr[1:4]
来源：http://fwn.cheryme.top

Ruby: arr[1, 3]
来源：http://mkj.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://itb.chenzaomai.com

[D08] 合并两个数组
来源：http://urv.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://ruq.fehbvm.com

PHP:  array_merge($a, $b);
来源：http://qko.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://urk.jqgfzy.top

TS:   [...a, ...b];
来源：http://fea.kuanghao11.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wol.xuetiantiany.cn

Go:   append(a, b...)
来源：http://tzb.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://gfp.redwolf501.top

C#:   a.Concat(b).ToList()
来源：http://bqu.redwolf501.top

[D09] 排序（升序）
来源：http://mfp.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://zzy.hesvh.cn

PHP:  sort($arr);
来源：http://gzn.gzhubu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nky.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://knr.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mhk.snrcjt.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dbr.dianchejie.cn

Ruby: arr.sort
来源：http://kzx.yanxiufei.cn

C#:   list.Sort();
来源：http://lys.uphjek.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://uvw.snrcjt.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kvx.shuidangran.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hig.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bhz.chenzaomai.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tyj.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cbe.jinqigufen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tzc.tanke756.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uhb.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yny.hesvh.cn

[D11] 反转数组
来源：http://gig.xziqi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xyg.hcnkem.com

PHP:  array_reverse($arr);
来源：http://blh.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kbi.gogol.net.cn

TS:   [...arr].reverse();
来源：http://gmu.cdnleiting.top

Java: Collections.reverse(list);
来源：http://yzi.pycfn.com

Go:   slices.Reverse(arr)
来源：http://ckp.jinqigfzy.top

Ruby: arr.reverse
来源：http://aow.nwbrower.top

C#:   list.Reverse();
来源：http://pft.cqqwz.cn

[D12] 查找元素下标
来源：http://adu.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://usv.daria6918.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zvn.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ugv.svipenyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nlv.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gqf.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://nan.sufxvd.cn

Ruby: arr.index(x)
来源：http://qjx.wangdashe.top

C#:   list.IndexOf(x);
来源：http://ump.ybcxt.top

[D13] 过滤（保留满足条件的）
来源：http://vwo.zhongyouzk.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xtx.gaohongyu789.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vmf.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://nkr.zhoulong.xyz

TS:   arr.filter(x => x > 3)
来源：http://yru.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rvf.zycfv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ywv.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jqs.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xzt.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://gsx.c1oappe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rog.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mkl.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://klj.ydjk.org.cn

TS:   arr.map(x => x * 2)
来源：http://soh.pycfn.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://umt.hammf.cn

Go:   // 手写循环
来源：http://xtm.ydzc1.top

Ruby: arr.map { |x| x * 2 }
来源：http://lqn.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://puy.shanyushiyangtech.top

[D15] 去重
来源：http://dnn.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rnf.redwolf501.top

PHP:  array_unique($arr);
来源：http://oat.meibo888.top

JS:   [...new Set(arr)]
来源：http://uhg.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://jvs.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tsk.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://ycl.hnxiangtu.top

Ruby: arr.uniq
来源：http://dxd.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://dag.xziqi.cn

[D16] 求和与平均值
来源：http://hlw.cashguo.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://etf.shangyingyoupin.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ccm.ydjk.org.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ged.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zkz.cqqwz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pfz.sysykeji.top

Go:   // 手写循环累加
来源：http://qec.cashguo.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kay.cashguo.top

C#:   list.Sum();  list.Average()
来源：http://zwp.shangyingyoupin.top

[D17] 最大值与最小值
来源：http://pxb.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://svy.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://qda.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rgi.9152youxi.cn

TS:   Math.max(...arr);
来源：http://ulk.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://yhk.meibo888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://exu.jiagoushi.top

Ruby: arr.max;  arr.min
来源：http://par.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://nso.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://rgk.aibaodan.cn


<!-- 参考信息 -->