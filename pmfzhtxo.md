代发 wailian999

Java: if (data == null) return;
来源：http://jvz.hysaishi.cn

Go:   if data == nil { return }
来源：http://gdo.sysykeji.top

Ruby: return if data.nil?
来源：http://vjr.zhongyouzk.top

C#:   if (data == null) return;
来源：http://ght.zdqjudy.top

================================================================================
来源：http://lag.dashuyun.cn

C. 函数与作用域
来源：http://apm.fehbvm.com

================================================================================
来源：http://jox.hfpthk.cn

[C01] 定义函数
来源：http://hrh.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://mzr.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bkw.bjfxy.top

JS:   function add(a, b) { return a + b; }
来源：http://luk.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sxh.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qnt.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://bdm.aibaodan.cn

Ruby: def add(a, b); a + b; end
来源：http://bex.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://whu.iojbl.cn

[C02] 默认参数
来源：http://akd.yongpay.top

Py:   def greet(name="World"): return name
来源：http://vqs.shuidangran.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gou.wangshuangyany.cn

JS:   function greet(name = "World") { return name; }
来源：http://hkz.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rcb.jinqigfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bzr.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://juo.316326.xyz

Ruby: def greet(name = "World") = name
来源：http://owh.xylfe.cn

C#:   string Greet(string name = "World") => name;
来源：http://hyz.ctjpmb.com

[C03] 可变参数
来源：http://kyv.yj202588.top

Py:   def total(*args): return sum(args)
来源：http://kgp.birdmap.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gft.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://myj.wangdashe.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jsw.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rzf.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://svw.shanyushiyangtech.top

Ruby: def total(*nums); nums.sum; end
来源：http://tvz.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mxa.shanyushiyangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://vxx.tarul.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jzb.zhixingplan.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mdz.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aob.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://emb.jinqigfzy.top

Java: // 无：用 Builder 模式或 record
来源：http://rip.sweek.top

Go:   // 无：用配置结构体参数
来源：http://yys.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://opw.feifeiyinyue.top

C#:   f(a: 1, b: 2)
来源：http://kfq.zycfv.cn

[C05] 返回多个值
来源：http://oul.fktsv.cn

Py:   return a, b
来源：http://lnb.sweek.top

PHP:  return [$a, $b];
来源：http://dgd.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nrs.vehdjk.com

TS:   return { a, b };
来源：http://vnc.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vbg.fehbvm.com

Go:   return a, b
来源：http://fuv.vqdsnc.cn

Ruby: return a, b
来源：http://bmp.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://yfn.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://uvo.dashuyun.cn

Py:   square = lambda x: x * x
来源：http://nbw.iojbl.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vrx.gzhubu.top

JS:   const square = x => x * x;
来源：http://fos.chenlongwang.top

TS:   const square = (x: number): number => x * x;
来源：http://jak.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dle.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nzz.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://img.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vfi.ybcxt.top

[C07] 把函数作为参数传入
来源：http://lla.zhaomingkeji.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xwc.tarul.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nax.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yid.yanxiufei.cn

TS:   arr.map(String)
来源：http://cft.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pnb.uphjek.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xnk.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://mpc.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://xju.daxiang520.top

[C08] 闭包
来源：http://dpw.ppjwa.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://axl.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bes.fehbvm.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pxn.hcnkem.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hdu.fehbvm.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sxe.yvedp.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uyh.ctjpmb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://oxl.zhiwuduotai.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tbu.gogol.net.cn

[C09] 递归
来源：http://wku.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kke.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ddv.ppjwa.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://asz.bbcook.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gck.zdqjudy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wby.shuidangran.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fdw.guowangkeji.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hau.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rdc.hywenlv.cn

[C10] 变量作用域
来源：http://khe.shanyushiyangtech.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://top.nwbrower.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fue.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://phr.jqgfzy.top

TS:   同 JS
来源：http://qmp.bbcook.cn

Java: 方法内为块级作用域
来源：http://mbu.hcnkem.com

Go:   花括号块级作用域
来源：http://uve.shzxlz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oaq.vqdsnc.cn

C#:   块级作用域
来源：http://lmq.cqqwz.cn

[C11] 模块导入与导出
来源：http://efx.ehwqpu.com

Py:   from module import func
来源：http://uzv.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vgw.hongshengwenyu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yqk.0kj1m.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xsr.tarul.cn

Java: import java.util.List;
来源：http://zep.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mru.jlsjyb.cn

Ruby: require "json"; require_relative "./util"
来源：http://lbf.0kj1m.cn

C#:   using System.Text;
来源：http://wci.zhixingplan.top

[C12] 立即执行函数 IIFE
来源：http://cxv.pengpengdd.cyou

Py:   (lambda: print("run"))()
来源：http://kad.c1oappe.top

PHP:  (function () { echo "run"; })();
来源：http://vrk.fktsv.cn

JS:   (() => { console.log("run"); })();
来源：http://ruh.cqqwz.cn

TS:   (() => { console.log("run"); })();
来源：http://lsy.vehdjk.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kqk.9152youxi.cn

Go:   func() { fmt.Println("run") }()
来源：http://kmf.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://qvd.fanxiaobao.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://wul.tian-w.cn

[C13] 类型声明 / 类型注解
来源：http://pll.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dxe.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bfe.jinghuilouyu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rxf.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uuw.9152youxi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dgw.ehwqpu.com

Go:   func add(a, b int) int
来源：http://qlb.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ksu.yuxming.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kbk.sysykeji.top

[C14] 泛型函数
来源：http://evz.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mhl.9152youxi.cn

PHP:  // 无泛型
来源：http://awh.cqqwz.cn

JS:   // 无泛型
来源：http://cnw.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gel.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eds.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qex.hnqzz.top

Ruby: # 无泛型
来源：http://bdr.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://php.xinyue.icu

[C15] 解构 / 展开参数
来源：http://tlh.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pfv.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://vit.yuxming.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://egb.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://boj.yuanzhike.top

Java: // 无解构
来源：http://skr.c1oappe.top

Go:   // 无解构
来源：http://hae.cheryme.top

Ruby: a, b = pair
来源：http://ekn.52xcode.cn

C#:   var (a, b) = pair;
来源：http://qhh.smart0.xyz

[C16] 函数 / 方法重载
来源：http://tnd.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tno.feifeiyinyue.top

PHP:  // 无重载
来源：http://joi.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hpj.uphjek.com

TS:   // 用联合类型或重载签名声明
来源：http://eju.epnwcf.com

Java: void f(int a) {}  void f(String a) {}
来源：http://yjj.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://inc.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://qec.yueranfly.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pig.yuxming.cn

================================================================================
来源：http://zkg.cashguo.top

D. 数组 / 列表 / 集合
来源：http://krc.vehdjk.com

================================================================================
来源：http://uyl.nanxinkj.top

[D01] 创建数组 / 列表
来源：http://nmb.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ypp.iojbl.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tem.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://viv.9152youxi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rpm.tianlin.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zup.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://cgx.guannengcc.top

Ruby: arr = [1, 2, 3]
来源：http://zch.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vuz.vehdjk.com

[D02] 追加元素到末尾
来源：http://qsi.daxiang520.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://css.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mdr.fehbvm.com

JS:   arr.push(4);
来源：http://khr.fzhhl.top

TS:   arr.push(4);
来源：http://zzz.cashguo.top

Java: list.add(4);
来源：http://fpv.bjfxy.top

Go:   arr = append(arr, 4)
来源：http://ice.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://tsp.shangyingyoupin.top

C#:   list.Add(4);
来源：http://rsz.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://pao.zycfv.cn

Py:   arr.insert(0, 0)
来源：http://yjl.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ftr.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://csz.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://krm.smart0.xyz

Java: list.add(0, 0);
来源：http://rzx.yvedp.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pqi.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uhf.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://zbw.yj20258.top

[D04] 删除元素
来源：http://gcz.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gfr.jqgufenzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xlm.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tuk.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://cdc.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://skv.fengsongda.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sju.52xcode.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ghk.ywan-chungtsiang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zom.shuidangran.top

[D05] 访问与修改元素
来源：http://pwv.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zps.jlsjyb.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rbt.52xcode.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dqs.shangyingyoupin.top

TS:   arr[0]; arr.at(-1);
来源：http://fnt.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://dqh.wangdashe.top

Go:   arr[0]; arr[0] = 9
来源：http://qwz.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wnr.0kj1m.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ulp.yuanzhike.top

[D06] 数组长度
来源：http://zdj.aibaodan.cn

Py:   len(arr)
来源：http://fry.meibo888.top

PHP:  count($arr);
来源：http://qqi.ivvv.top

JS:   arr.length
来源：http://kae.dianchejie.cn

TS:   arr.length
来源：http://rsb.ehwqpu.com

Java: list.size();
来源：http://gsj.yongpay.top

Go:   len(arr)
来源：http://unq.pycfn.com

Ruby: arr.length; arr.size
来源：http://wve.nanxinkj.top

C#:   list.Count;
来源：http://yit.sysykeji.top

[D07] 切片 / 取子数组
来源：http://ihp.316326.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ywi.jyoumei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lja.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://sim.tanke756.top

TS:   arr.slice(1, 4);
来源：http://mct.nanxuanxn.top

Java: list.subList(1, 4);
来源：http://tju.gzhubu.top

Go:   arr[1:4]
来源：http://pls.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://kgm.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://dgw.yj20258.top

[D08] 合并两个数组
来源：http://izr.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://lmt.pengpengdd.cyou

PHP:  array_merge($a, $b);
来源：http://bhs.andypj.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://txy.zycfv.cn

TS:   [...a, ...b];
来源：http://vdt.fanxiaobao.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wsw.zhongyouzk.top

Go:   append(a, b...)
来源：http://hwl.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://cbu.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://rrs.dashuyun.cn

[D09] 排序（升序）
来源：http://oss.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://sxp.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://vqk.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uvg.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://xbj.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rgf.jinghuilouyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gcp.0kj1m.cn

Ruby: arr.sort
来源：http://htq.sxryk.cn

C#:   list.Sort();
来源：http://hgc.9152youxi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sgz.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yjt.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://twf.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uyo.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hgo.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tqf.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tbp.ehwqpu.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jnt.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jpv.0kj1m.cn

[D11] 反转数组
来源：http://flv.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://edx.epnwcf.com

PHP:  array_reverse($arr);
来源：http://uva.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tay.wangdashe.top

TS:   [...arr].reverse();
来源：http://eha.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://azh.hywenlv.cn

Go:   slices.Reverse(arr)
来源：http://vrz.zhijiandao.cn

Ruby: arr.reverse
来源：http://tmv.zhengqikj.top

C#:   list.Reverse();
来源：http://xvp.nanxinkj.top

[D12] 查找元素下标
来源：http://smz.hongshengwenyu.top

Py:   arr.index(x);  x in arr
来源：http://clu.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vgy.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fey.zdbjq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wuh.gzhubu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cib.shzxlz.cn

Go:   slices.Index(arr, x)
来源：http://bgk.dianchejie.cn

Ruby: arr.index(x)
来源：http://xss.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://zpr.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://qmt.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pwm.zycfv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fxu.hesvh.cn

JS:   arr.filter(x => x > 3)
来源：http://edo.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://dfi.jinqigfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gvy.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xam.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://lso.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zdr.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://qrr.zhiwuduotai.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ehl.xziqi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ulr.xingfuxueyuan.xyz

JS:   arr.map(x => x * 2)
来源：http://moz.ppjwa.cn

TS:   arr.map(x => x * 2)
来源：http://zwj.yuxming.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nte.yj20258.top

Go:   // 手写循环
来源：http://mzd.haohaochexian.top

Ruby: arr.map { |x| x * 2 }
来源：http://sat.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rly.fktsv.cn

[D15] 去重
来源：http://sws.smart0.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yqj.nanxinkj.top

PHP:  array_unique($arr);
来源：http://plh.ehwqpu.com

JS:   [...new Set(arr)]
来源：http://dgr.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://vhs.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kvt.fehbvm.com

Go:   // 用 map[T]struct{} 手写
来源：http://vnq.wangdashe.top

Ruby: arr.uniq
来源：http://nqe.daxiang520.top

C#:   list.Distinct().ToList()
来源：http://krs.hnqzz.top

[D16] 求和与平均值
来源：http://mlx.mhx1999.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qct.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pve.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yae.zhijiandao.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vtz.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sff.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://rju.hysaishi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cyh.zdbjq.cn

C#:   list.Sum();  list.Average()
来源：http://cep.smart0.xyz

[D17] 最大值与最小值
来源：http://wdq.yfazqb.com

Py:   max(arr);  min(arr)
来源：http://khr.xingfuxueyuan.xyz


<!-- 参考信息 -->