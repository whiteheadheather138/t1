代发 wailian999

Py:   def add(a, b): return a + b
来源：http://qqp.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nnr.52xcode.cn

JS:   function add(a, b) { return a + b; }
来源：http://jew.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gtp.hnqzz.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jxg.cdnleiting.top

Go:   func add(a, b int) int { return a + b }
来源：http://atf.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://pae.yanxiufei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ino.gaohongyu789.top

[C02] 默认参数
来源：http://dwe.xuanzx.com

Py:   def greet(name="World"): return name
来源：http://mur.0kj1m.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xui.vehdjk.com

JS:   function greet(name = "World") { return name; }
来源：http://fae.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tvn.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://cxk.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uph.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://qwn.c1oappe.top

C#:   string Greet(string name = "World") => name;
来源：http://qej.wangshuangyany.cn

[C03] 可变参数
来源：http://wof.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://cbj.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tfy.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://exm.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bfe.shanyushiyangtech.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://war.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hiw.hammf.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xui.xuanzx.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://utu.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://izd.aibaodan.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pze.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pvm.tarul.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gji.zhoulong.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://coh.gogol.net.cn

Java: // 无：用 Builder 模式或 record
来源：http://zxa.havefunace.top

Go:   // 无：用配置结构体参数
来源：http://zro.vqdsnc.cn

Ruby: f(a: 1, b: 2)
来源：http://orv.gogol.net.cn

C#:   f(a: 1, b: 2)
来源：http://rfv.tianlin.xyz

[C05] 返回多个值
来源：http://byq.zdqjudy.top

Py:   return a, b
来源：http://qdu.uphjek.com

PHP:  return [$a, $b];
来源：http://hlf.meibo888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://owv.chenlongwang.top

TS:   return { a, b };
来源：http://ebr.zhixingplan.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xtj.yuxming.cn

Go:   return a, b
来源：http://aae.shanyushiyangtech.top

Ruby: return a, b
来源：http://agv.shanyushiyangtech.top

C#:   return (a, b);              // ValueTuple
来源：http://hgk.ydzc1.top

[C06] 匿名函数 / lambda
来源：http://wkq.jyoumei.cn

Py:   square = lambda x: x * x
来源：http://deh.meibo888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vdf.fengsongda.top

JS:   const square = x => x * x;
来源：http://lmj.jianghu66.top

TS:   const square = (x: number): number => x * x;
来源：http://vle.guannengcc.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cki.jinqigufen.top

Go:   sq := func(x int) int { return x * x }
来源：http://drt.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://ofb.ydzc1.top

C#:   Func<int, int> square = x => x * x;
来源：http://bhd.hywenlv.cn

[C07] 把函数作为参数传入
来源：http://nmp.jqgfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lxt.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://iyj.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dan.ywan-chungtsiang.top

TS:   arr.map(String)
来源：http://gry.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mcs.jinyuanbaomall.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zcs.meibo888.top

Ruby: arr.map(&:upcase)
来源：http://ffq.zhongyouzk.top

C#:   arr.Select(s => s.ToUpper())
来源：http://boz.dianchejie.cn

[C08] 闭包
来源：http://vmb.ydzc1.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vko.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://myc.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rac.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mxv.gaohongyu789.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cri.tanke756.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://naf.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://htl.sjlbkw.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nqd.bjfxy.top

[C09] 递归
来源：http://euk.nanxinkj.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hak.yj20258888.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://alb.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eiz.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yfo.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yde.c1oappe.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hsn.vehdjk.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://raf.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pmu.shzxlz.cn

[C10] 变量作用域
来源：http://uqd.quarkkingdee.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jpc.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://edv.cucudq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xsp.bbcook.cn

TS:   同 JS
来源：http://jvx.svipenyu.cn

Java: 方法内为块级作用域
来源：http://met.zhijiandao.cn

Go:   花括号块级作用域
来源：http://rhv.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://uoi.chenjidiqi.icu

C#:   块级作用域
来源：http://gty.xuanzx.com

[C11] 模块导入与导出
来源：http://uod.hongshengwenyu.top

Py:   from module import func
来源：http://lfo.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lte.zhoulong.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://gxr.dianchejie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nnz.yueranfly.top

Java: import java.util.List;
来源：http://ojo.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zrd.zhaomingkeji.xyz

Ruby: require "json"; require_relative "./util"
来源：http://ofc.sufxvd.cn

C#:   using System.Text;
来源：http://oqf.shanyushiyangtech.top

[C12] 立即执行函数 IIFE
来源：http://dmr.hcnkem.com

Py:   (lambda: print("run"))()
来源：http://lcf.cdnleiting.top

PHP:  (function () { echo "run"; })();
来源：http://sds.gzhubu.top

JS:   (() => { console.log("run"); })();
来源：http://jie.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://pak.sxryk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://oxh.gaohongyu789.top

Go:   func() { fmt.Println("run") }()
来源：http://mze.xuetiantiany.cn

Ruby: -> { puts "run" }.call
来源：http://tnn.hfpthk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://phe.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://ayn.zycfv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rja.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ogh.uphjek.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jjl.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uzr.havefunace.top

Java: int add(int a, int b) { return a + b; }
来源：http://ylb.iojbl.cn

Go:   func add(a, b int) int
来源：http://bcv.quarkkingdee.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://uqc.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://fyx.zhoulong.xyz

[C14] 泛型函数
来源：http://zut.fengsongda.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ggo.ydzc1.top

PHP:  // 无泛型
来源：http://xiz.birdmap.top

JS:   // 无泛型
来源：http://orh.zhiwuduotai.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nlu.zhixingplan.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qkl.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cur.c1oappe.top

Ruby: # 无泛型
来源：http://xkx.yuanzhike.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nul.sysykeji.top

[C15] 解构 / 展开参数
来源：http://kqt.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nns.hammf.cn

PHP:  [$a, $b] = $pair;
来源：http://xdk.gotoacloud.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jmw.vqdsnc.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://edm.cqqwz.cn

Java: // 无解构
来源：http://hjm.cheryme.top

Go:   // 无解构
来源：http://bxa.zdbjq.cn

Ruby: a, b = pair
来源：http://smx.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://aev.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://aon.feifeiyinyue.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lkb.nanxuanxn.top

PHP:  // 无重载
来源：http://dwb.hnxiangtu.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://pde.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://hik.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://wfr.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://ftz.xziqi.cn

Ruby: # 无重载：靠动态参数
来源：http://eof.xuetiantiany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kyd.shanyushiyangtech.top

================================================================================
来源：http://rnb.hongshengwenyu.top

D. 数组 / 列表 / 集合
来源：http://pdr.shanyushiyangkeji.top

================================================================================
来源：http://mmv.shuidangran.top

[D01] 创建数组 / 列表
来源：http://dkd.zhengqikj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://nzx.jinghuilouyu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ksx.bjfxy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zvc.dianchejie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hbu.cucudq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xon.bbcook.cn

Go:   arr := []int{1, 2, 3}
来源：http://fna.fengsongda.top

Ruby: arr = [1, 2, 3]
来源：http://kkx.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qjp.guowangkeji.top

[D02] 追加元素到末尾
来源：http://why.sysykeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hro.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fgq.tian-w.cn

JS:   arr.push(4);
来源：http://slv.yvedp.cn

TS:   arr.push(4);
来源：http://gig.daxiang520.top

Java: list.add(4);
来源：http://ybd.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://amd.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://zmp.bjfxy.top

C#:   list.Add(4);
来源：http://vve.zycfv.cn

[D03] 在指定位置插入元素
来源：http://xvn.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://bps.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aty.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dhf.shuidangran.top

TS:   arr.splice(0, 0, 0);
来源：http://nmm.fktsv.cn

Java: list.add(0, 0);
来源：http://vlc.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://tbv.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://njv.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://yuk.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://rpc.dianchejie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://noj.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rnw.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://icb.cheryme.top

TS:   arr.splice(0, 1);
来源：http://hsm.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rmw.hongshengwenyu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xjp.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ict.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mxu.tianlin.xyz

[D05] 访问与修改元素
来源：http://dlp.yuanzhike.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ouo.wangshuangyany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bii.xylfe.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kxg.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://eiv.hnqzz.top

Java: list.get(0); list.set(0, 9);
来源：http://abo.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://uvm.shangyingyoupin.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fak.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nlf.jqgufenzy.top

[D06] 数组长度
来源：http://csf.shanyushiyangtech.top

Py:   len(arr)
来源：http://qum.9152youxi.cn

PHP:  count($arr);
来源：http://dnu.jqgufenzy.top

JS:   arr.length
来源：http://tpw.shanyushiyangtech.top

TS:   arr.length
来源：http://dri.yj20258.top

Java: list.size();
来源：http://qsd.mhx1999.top

Go:   len(arr)
来源：http://lao.nanxinkj.top

Ruby: arr.length; arr.size
来源：http://sjd.jyoumei.cn

C#:   list.Count;
来源：http://nud.yonumen.top

[D07] 切片 / 取子数组
来源：http://aqr.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nsr.yfazqb.com

PHP:  array_slice($arr, 1, 3);
来源：http://zwv.tian-w.cn

JS:   arr.slice(1, 4);
来源：http://bet.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://ljk.haohaochexian.top

Java: list.subList(1, 4);
来源：http://yvv.shangyingyoupin.top

Go:   arr[1:4]
来源：http://sea.xziqi.cn

Ruby: arr[1, 3]
来源：http://jkc.yanxiufei.cn

C#:   list.GetRange(1, 3);
来源：http://zck.tian-w.cn

[D08] 合并两个数组
来源：http://xis.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://xsl.yanxiufei.cn

PHP:  array_merge($a, $b);
来源：http://cum.dashuyun.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pkv.xuetiantiany.cn

TS:   [...a, ...b];
来源：http://ela.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bxd.epnwcf.com

Go:   append(a, b...)
来源：http://jax.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://osk.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://mal.yongpay.top

[D09] 排序（升序）
来源：http://dkv.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://sid.hysaishi.cn

PHP:  sort($arr);
来源：http://kwh.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qnb.c1oappe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nmi.xingfuxueyuan.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://ohr.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://olh.fktsv.cn

Ruby: arr.sort
来源：http://kog.sjlbkw.cn

C#:   list.Sort();
来源：http://jgl.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ccp.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bdd.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aym.cheryme.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://toa.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jfc.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wvr.sufxvd.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jau.xylfe.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kav.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://znn.vqdsnc.cn

[D11] 反转数组
来源：http://kjg.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://pll.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://vix.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jwp.redwolf501.top

TS:   [...arr].reverse();
来源：http://bev.cqqwz.cn

Java: Collections.reverse(list);
来源：http://wrv.guowangkeji.top

Go:   slices.Reverse(arr)
来源：http://djh.bjfxy.top

Ruby: arr.reverse
来源：http://dhq.hongshengwenyu.top

C#:   list.Reverse();
来源：http://lvn.fengsongda.top

[D12] 查找元素下标
来源：http://qdd.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://hct.zhiwuduotai.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lid.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lux.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lpf.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fia.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://sne.zhengqikj.top

Ruby: arr.index(x)
来源：http://vdf.jqgfzy.top

C#:   list.IndexOf(x);
来源：http://dxd.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://goi.ydjk.org.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ami.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blr.cdnleiting.top

JS:   arr.filter(x => x > 3)
来源：http://qyr.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://fqv.yj202588.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jju.meibo888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gpj.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://lzr.yangfankeji.com

C#:   list.Where(x => x > 3).ToList()
来源：http://dip.yangfankeji.com

[D14] 映射转换（每个元素变形）
来源：http://dmz.9152youxi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ewx.tian-w.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jad.yfazqb.com

JS:   arr.map(x => x * 2)
来源：http://aoi.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://xgh.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ltd.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://wfw.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://lhi.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://roy.ehwqpu.com

[D15] 去重
来源：http://pdx.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gjr.aibaodan.cn

PHP:  array_unique($arr);
来源：http://buu.pengpengdd.cyou

JS:   [...new Set(arr)]
来源：http://rni.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://sdf.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sbh.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://ssx.daxiang520.top

Ruby: arr.uniq
来源：http://deu.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://tbo.aibaodan.cn

[D16] 求和与平均值
来源：http://hnw.nanxuanxn.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://plt.ydjk.org.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rzu.tian-w.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fcd.yuxming.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kzf.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yvb.zhixingplan.top

Go:   // 手写循环累加
来源：http://voj.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cqz.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://xuw.yj20258888.top

[D17] 最大值与最小值
来源：http://sbg.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://kba.xingfuxueyuan.xyz

PHP:  max($arr);  min($arr);
来源：http://xbd.yfazqb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://spe.gogol.net.cn

TS:   Math.max(...arr);
来源：http://vha.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jmj.dianchejie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dmu.havefunace.top

Ruby: arr.max;  arr.min
来源：http://roy.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://jun.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://nwj.aibaodan.cn


<!-- 参考信息 -->