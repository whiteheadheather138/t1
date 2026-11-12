代发 wailian999

Py:   def add(a, b): return a + b
来源：http://wcz.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nio.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://fte.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jyw.xylfe.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://dxe.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://otj.xinyue.icu

Ruby: def add(a, b); a + b; end
来源：http://xgb.xylfe.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ytg.wangshuangyany.cn

[C02] 默认参数
来源：http://txz.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://rug.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dje.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://etg.xziqi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tcz.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://brm.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zsv.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://bgk.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://hhd.hysaishi.cn

[C03] 可变参数
来源：http://ecy.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://vox.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uov.nwbrower.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pyu.xingfuxueyuan.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bej.cqqwz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hsf.aizwys.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ymt.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://pcx.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zfm.zhoulong.xyz

[C04] 命名参数 / 关键字参数
来源：http://bnp.yuxming.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ttr.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kqb.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pks.tianlin.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://erh.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://jbr.chenjidiqi.icu

Go:   // 无：用配置结构体参数
来源：http://lmc.sjlbkw.cn

Ruby: f(a: 1, b: 2)
来源：http://wvm.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://eas.gogol.net.cn

[C05] 返回多个值
来源：http://bxv.fktsv.cn

Py:   return a, b
来源：http://ppb.hammf.cn

PHP:  return [$a, $b];
来源：http://eba.meibo888.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hwq.aibaodan.cn

TS:   return { a, b };
来源：http://nli.sufxvd.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cgn.zycfv.cn

Go:   return a, b
来源：http://bed.mhx1999.top

Ruby: return a, b
来源：http://wtu.yvedp.cn

C#:   return (a, b);              // ValueTuple
来源：http://elc.quarkkingdee.top

[C06] 匿名函数 / lambda
来源：http://pej.feifeiyinyue.top

Py:   square = lambda x: x * x
来源：http://msp.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rnm.tanke756.top

JS:   const square = x => x * x;
来源：http://nft.zhoulong.xyz

TS:   const square = (x: number): number => x * x;
来源：http://bov.xziqi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://aqd.tanke756.top

Go:   sq := func(x int) int { return x * x }
来源：http://dfy.zycfv.cn

Ruby: square = ->(x) { x * x }
来源：http://fps.haohaochexian.top

C#:   Func<int, int> square = x => x * x;
来源：http://lxc.daxiang520.top

[C07] 把函数作为参数传入
来源：http://hae.yj20258888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ubb.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kiv.52xcode.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ocj.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://cma.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tjl.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://veg.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://evu.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lzt.pengpengdd.cyou

[C08] 闭包
来源：http://kaq.dashuyun.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vie.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eig.zdqjudy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://upe.chenzaomai.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://oju.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ynz.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fat.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oak.jinyuanbaomall.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tph.shangyingyoupin.top

[C09] 递归
来源：http://wne.snrcjt.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dit.sjlbkw.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gcz.meibo888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bnm.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ogo.bjfxy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bpv.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qdr.sjlbkw.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sno.shzxlz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://erz.dashuyun.cn

[C10] 变量作用域
来源：http://xcz.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cnk.hfpthk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ncc.yj20258888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://txd.ivvv.top

TS:   同 JS
来源：http://ayx.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://gac.0kj1m.cn

Go:   花括号块级作用域
来源：http://wvx.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gmp.andypj.xyz

C#:   块级作用域
来源：http://mqz.chenjidiqi.icu

[C11] 模块导入与导出
来源：http://ewa.bbcook.cn

Py:   from module import func
来源：http://emp.snrcjt.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://njb.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://utf.jinqigufen.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xlf.sweek.top

Java: import java.util.List;
来源：http://zck.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vwq.chenjidiqi.icu

Ruby: require "json"; require_relative "./util"
来源：http://enh.yueranfly.top

C#:   using System.Text;
来源：http://hpv.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://jom.zhixingplan.top

Py:   (lambda: print("run"))()
来源：http://kgr.xylfe.cn

PHP:  (function () { echo "run"; })();
来源：http://hfu.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://sdz.ywan-chungtsiang.top

TS:   (() => { console.log("run"); })();
来源：http://blv.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qkw.xuetiantiany.cn

Go:   func() { fmt.Println("run") }()
来源：http://jey.9152youxi.cn

Ruby: -> { puts "run" }.call
来源：http://mlk.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zmo.hysaishi.cn

[C13] 类型声明 / 类型注解
来源：http://jaq.gogol.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vio.ppjwa.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lfi.yangfankeji.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mtj.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://edj.ybcxt.top

Java: int add(int a, int b) { return a + b; }
来源：http://vmj.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://bcy.gogol.net.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qib.hnxiangtu.top

C#:   int Add(int a, int b) => a + b;
来源：http://cln.xuetiantiany.cn

[C14] 泛型函数
来源：http://pam.chenzaomai.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://njc.hfpthk.cn

PHP:  // 无泛型
来源：http://ooi.bbcook.cn

JS:   // 无泛型
来源：http://kpz.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://znb.havefunace.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xyt.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kwe.nanxinkj.top

Ruby: # 无泛型
来源：http://gki.zhengqikj.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vfm.wangdashe.top

[C15] 解构 / 展开参数
来源：http://xya.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fht.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://mic.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://foe.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qsw.ydzc1.top

Java: // 无解构
来源：http://rhf.shangyingyoupin.top

Go:   // 无解构
来源：http://slk.hesvh.cn

Ruby: a, b = pair
来源：http://oqt.fanxiaobao.xyz

C#:   var (a, b) = pair;
来源：http://nxk.shanyushiyangtech.top

[C16] 函数 / 方法重载
来源：http://wqm.snrcjt.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://exb.aizwys.cn

PHP:  // 无重载
来源：http://vtr.hnqzz.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jnq.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://dmy.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qim.hysaishi.cn

Go:   // 无重载：用不同函数名
来源：http://ivy.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://qyp.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tnp.jinyuanbaomall.cn

================================================================================
来源：http://tdp.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://qyt.hywenlv.cn

================================================================================
来源：http://bpf.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://udx.ywan-chungtsiang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://sfx.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mie.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iir.xziqi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tqb.yueranfly.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zqw.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://jiu.zhaomingkeji.xyz

Ruby: arr = [1, 2, 3]
来源：http://ihn.hcnkem.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://trg.vqdsnc.cn

[D02] 追加元素到末尾
来源：http://nmh.hfpthk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://vxe.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zkj.xziqi.cn

JS:   arr.push(4);
来源：http://bfk.shzxlz.cn

TS:   arr.push(4);
来源：http://gzi.tian-w.cn

Java: list.add(4);
来源：http://tlj.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://kdx.ppjwa.cn

Ruby: arr << 4; arr.push(5)
来源：http://tmu.zdqjudy.top

C#:   list.Add(4);
来源：http://rpo.sxryk.cn

[D03] 在指定位置插入元素
来源：http://zfx.havefunace.top

Py:   arr.insert(0, 0)
来源：http://dxp.yonumen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hev.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wii.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://fgp.hysaishi.cn

Java: list.add(0, 0);
来源：http://xqe.316326.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://cho.yuxming.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wrm.jyoumei.cn

C#:   list.Insert(0, 0);
来源：http://pmh.zhongyouzk.top

[D04] 删除元素
来源：http://gej.tianlin.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://brw.52xcode.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rba.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sxr.hesvh.cn

TS:   arr.splice(0, 1);
来源：http://mtg.yj202588.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://akf.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ids.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nzz.zhengqikj.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hpm.cdnleiting.top

[D05] 访问与修改元素
来源：http://wuc.gotoacloud.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sph.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vyi.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rox.zhijiandao.cn

TS:   arr[0]; arr.at(-1);
来源：http://liz.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://vqi.xingfuxueyuan.xyz

Go:   arr[0]; arr[0] = 9
来源：http://vpf.hesvh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kgp.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mjw.tarul.cn

[D06] 数组长度
来源：http://rlc.vehdjk.com

Py:   len(arr)
来源：http://ufs.fktsv.cn

PHP:  count($arr);
来源：http://ymg.sxryk.cn

JS:   arr.length
来源：http://slt.fktsv.cn

TS:   arr.length
来源：http://nrt.tian-w.cn

Java: list.size();
来源：http://uvw.yj202588.top

Go:   len(arr)
来源：http://nay.bjfxy.top

Ruby: arr.length; arr.size
来源：http://num.xylfe.cn

C#:   list.Count;
来源：http://vtj.316326.xyz

[D07] 切片 / 取子数组
来源：http://bgk.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://doh.epnwcf.com

PHP:  array_slice($arr, 1, 3);
来源：http://acr.shanyushiyangtech.top

JS:   arr.slice(1, 4);
来源：http://qie.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://qzy.yuxming.cn

Java: list.subList(1, 4);
来源：http://yzi.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://moz.hnqzz.top

Ruby: arr[1, 3]
来源：http://fpd.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://rmm.fengsongda.top

[D08] 合并两个数组
来源：http://lqv.jinyuanbaomall.cn

Py:   a + b;  a.extend(b)
来源：http://iva.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://ccu.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://acp.iojbl.cn

TS:   [...a, ...b];
来源：http://xvz.xinyue.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kvw.nanxinkj.top

Go:   append(a, b...)
来源：http://ffb.guannengcc.top

Ruby: a + b;  a.concat(b)
来源：http://sui.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://pew.haohaochexian.top

[D09] 排序（升序）
来源：http://ntd.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://ieu.aibaodan.cn

PHP:  sort($arr);
来源：http://grw.meibo888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://afv.redwolf501.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yug.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qhv.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hwh.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://tsb.guowangkeji.top

C#:   list.Sort();
来源：http://rwm.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sjd.yanxiufei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rkr.gaohongyu789.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lku.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nro.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ntz.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sqp.sxryk.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lvj.9152youxi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jau.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qgg.cqqwz.cn

[D11] 反转数组
来源：http://cmp.jiagoushi.top

Py:   arr[::-1];  arr.reverse()
来源：http://jnr.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://qma.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vzc.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://xov.zdqjudy.top

Java: Collections.reverse(list);
来源：http://lqv.xuanzx.com

Go:   slices.Reverse(arr)
来源：http://oxk.sweek.top

Ruby: arr.reverse
来源：http://kzz.ydzc1.top

C#:   list.Reverse();
来源：http://cyf.shanyushiyangkeji.top

[D12] 查找元素下标
来源：http://wkj.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://gsl.yonumen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iic.sjlbkw.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sac.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oxa.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ark.fanxiaobao.xyz

Go:   slices.Index(arr, x)
来源：http://jpa.zhoulong.xyz

Ruby: arr.index(x)
来源：http://owm.redwolf501.top

C#:   list.IndexOf(x);
来源：http://mjx.gotoacloud.top

[D13] 过滤（保留满足条件的）
来源：http://woq.sweek.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zsa.zdqjudy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rgs.zhaomingkeji.xyz

JS:   arr.filter(x => x > 3)
来源：http://iww.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://kcl.ctjpmb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zqx.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ywq.sxryk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://urf.zhongyouzk.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dfy.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://gla.yj20258888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ecq.yj20258888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hmq.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://rpm.snrcjt.cn

TS:   arr.map(x => x * 2)
来源：http://nur.yj20258.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lck.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://ktx.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://vun.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ebr.tianlin.xyz

[D15] 去重
来源：http://mxx.meibo888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fdk.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://yvl.shzxlz.cn

JS:   [...new Set(arr)]
来源：http://yvm.fktsv.cn

TS:   [...new Set(arr)]
来源：http://tnf.wangdashe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ezh.fanxiaobao.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://vrh.ivvv.top

Ruby: arr.uniq
来源：http://gam.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://nvs.hfpthk.cn

[D16] 求和与平均值
来源：http://hcg.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zke.shanyushiyangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wkf.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ntx.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hkw.yonumen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pux.zhijiandao.cn

Go:   // 手写循环累加
来源：http://sbx.52xcode.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tfi.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://xie.chenlongwang.top

[D17] 最大值与最小值
来源：http://lmp.sweek.top

Py:   max(arr);  min(arr)
来源：http://xat.tarul.cn

PHP:  max($arr);  min($arr);
来源：http://wsj.bbcook.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lkb.guowangkeji.top

TS:   Math.max(...arr);
来源：http://unj.gzhubu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kug.epnwcf.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gmz.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://oqo.fktsv.cn

C#:   list.Max();  list.Min()
来源：http://acr.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://xbr.ybcxt.top


<!-- 参考信息 -->