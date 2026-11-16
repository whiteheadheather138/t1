代发 wailian999

PHP:  $a && $b || !$c
来源：http://djl.sysykeji.top

JS:   a && b || !c
来源：http://zzt.nanxinkj.top

TS:   a && b || !c
来源：http://jlo.chenjidiqi.icu

Java: a && b || !c
来源：http://qci.chenlongwang.top

Go:   a && b || !c
来源：http://ttz.iojbl.cn

Ruby: a && b || !c
来源：http://qyo.zhiwuduotai.top

C#:   a && b || !c
来源：http://pcy.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://hmg.wangdashe.top

Py:   if not data: return
来源：http://vkl.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://lvh.hnxiangtu.top

JS:   if (!data) return;
来源：http://wcf.bbcook.cn

TS:   if (!data) return;
来源：http://htu.sysykeji.top

Java: if (data == null) return;
来源：http://ncq.yuanzhike.top

Go:   if data == nil { return }
来源：http://rnk.svipenyu.cn

Ruby: return if data.nil?
来源：http://abz.fehbvm.com

C#:   if (data == null) return;
来源：http://iqe.cqqwz.cn

================================================================================
来源：http://ogn.shangyingyoupin.top

C. 函数与作用域
来源：http://you.xuetiantiany.cn

================================================================================
来源：http://bof.gotoacloud.top

[C01] 定义函数
来源：http://lzs.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://uof.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lgp.fzhhl.top

JS:   function add(a, b) { return a + b; }
来源：http://adl.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ltw.sysykeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qkb.gogol.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://evj.wangshuangyany.cn

Ruby: def add(a, b); a + b; end
来源：http://hjg.zdbjq.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iby.yanxiufei.cn

[C02] 默认参数
来源：http://exp.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://ymn.yj20258888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kau.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://vzy.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://hmk.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fkr.bbcook.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lfk.epnwcf.com

Ruby: def greet(name = "World") = name
来源：http://tad.hcnkem.com

C#:   string Greet(string name = "World") => name;
来源：http://tuz.yangfankeji.com

[C03] 可变参数
来源：http://bum.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://yri.ctjpmb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://trl.birdmap.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bdj.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wvq.gotoacloud.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mpk.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://whe.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://gof.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aso.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://aem.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yvo.sjlbkw.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yzv.vehdjk.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rtp.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://knd.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://jsx.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://yxn.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://ggi.ivvv.top

C#:   f(a: 1, b: 2)
来源：http://qnh.vqdsnc.cn

[C05] 返回多个值
来源：http://owf.shanyushiyangkeji.top

Py:   return a, b
来源：http://knz.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://bhf.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qnr.ydjk.org.cn

TS:   return { a, b };
来源：http://zoz.jlsjyb.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nas.daxiang520.top

Go:   return a, b
来源：http://tgb.redwolf501.top

Ruby: return a, b
来源：http://xfp.ydjk.org.cn

C#:   return (a, b);              // ValueTuple
来源：http://vrc.zhijiandao.cn

[C06] 匿名函数 / lambda
来源：http://vup.xuetiantiany.cn

Py:   square = lambda x: x * x
来源：http://she.feifeiyinyue.top

PHP:  $square = fn($x) => $x * $x;
来源：http://pag.hammf.cn

JS:   const square = x => x * x;
来源：http://lej.guannengcc.top

TS:   const square = (x: number): number => x * x;
来源：http://zra.chenzaomai.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tqt.cqqwz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hww.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://zfe.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://kwa.hysaishi.cn

[C07] 把函数作为参数传入
来源：http://xaf.epnwcf.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fry.guannengcc.top

PHP:  array_map("strtoupper", $arr);
来源：http://nzt.yonumen.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qid.52xcode.cn

TS:   arr.map(String)
来源：http://szm.quarkkingdee.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sif.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kmw.aibaodan.cn

Ruby: arr.map(&:upcase)
来源：http://ajy.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ktg.fzhhl.top

[C08] 闭包
来源：http://wzf.fzhhl.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://uow.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qua.jinqigfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jwt.redwolf501.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kiy.wangdashe.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bqn.guowangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rzj.jlsjyb.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://von.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ren.tarul.cn

[C09] 递归
来源：http://alu.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qmh.shanyushiyangkeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zjf.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ocg.hesvh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yvl.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ghi.gzhubu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qbm.haohaochexian.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ape.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qwi.chenzaomai.com

[C10] 变量作用域
来源：http://cgu.fehbvm.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mwf.shzxlz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ukk.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dci.haohaochexian.top

TS:   同 JS
来源：http://mvw.tarul.cn

Java: 方法内为块级作用域
来源：http://yww.shangyingyoupin.top

Go:   花括号块级作用域
来源：http://orl.ctjpmb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gvl.yuxming.cn

C#:   块级作用域
来源：http://dyi.svipenyu.cn

[C11] 模块导入与导出
来源：http://mkt.shuidangran.top

Py:   from module import func
来源：http://czw.gzhubu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uio.nanxuanxn.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://njs.gogol.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yaa.zhaomingkeji.xyz

Java: import java.util.List;
来源：http://ard.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ezz.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://tnu.sysykeji.top

C#:   using System.Text;
来源：http://uhn.dashuyun.cn

[C12] 立即执行函数 IIFE
来源：http://yrn.zdqjudy.top

Py:   (lambda: print("run"))()
来源：http://nqd.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://emg.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://fck.zhengqikj.top

TS:   (() => { console.log("run"); })();
来源：http://duf.0kj1m.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zrk.bjfxy.top

Go:   func() { fmt.Println("run") }()
来源：http://rdn.yfazqb.com

Ruby: -> { puts "run" }.call
来源：http://zou.zhiwuduotai.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jio.sjlbkw.cn

[C13] 类型声明 / 类型注解
来源：http://rlb.gogol.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ngc.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rzm.zhongyouzk.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://joj.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pne.havefunace.top

Java: int add(int a, int b) { return a + b; }
来源：http://prb.jinyuanbaomall.cn

Go:   func add(a, b int) int
来源：http://oag.jinyuanbaomall.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ays.xuetiantiany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://obr.epnwcf.com

[C14] 泛型函数
来源：http://qfn.aibaodan.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gis.haohaochexian.top

PHP:  // 无泛型
来源：http://vau.shuidangran.top

JS:   // 无泛型
来源：http://eul.svipenyu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bzb.gzhubu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hsh.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tpg.fengsongda.top

Ruby: # 无泛型
来源：http://ppl.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hfk.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://ykz.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rhe.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://qtl.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rqy.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uvu.dianchejie.cn

Java: // 无解构
来源：http://aex.c1oappe.top

Go:   // 无解构
来源：http://idn.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://iaf.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://bcx.daria6918.cn

[C16] 函数 / 方法重载
来源：http://bis.quarkkingdee.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xlr.daria6918.cn

PHP:  // 无重载
来源：http://kdk.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hmb.zdbjq.cn

TS:   // 用联合类型或重载签名声明
来源：http://elb.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://twd.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://dno.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://tpg.jinqigufen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vqu.sufxvd.cn

================================================================================
来源：http://loh.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://isf.aizwys.cn

================================================================================
来源：http://kmq.gzhubu.top

[D01] 创建数组 / 列表
来源：http://ryf.vehdjk.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://vxd.xuetiantiany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eoq.aizwys.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tzn.hywenlv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zdu.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://piz.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://gwh.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://pnj.xziqi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://peh.zhaomingkeji.xyz

[D02] 追加元素到末尾
来源：http://eun.zhijiandao.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pvq.guowangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ngk.nanxinkj.top

JS:   arr.push(4);
来源：http://egz.jinghuilouyu.cn

TS:   arr.push(4);
来源：http://csj.mhx1999.top

Java: list.add(4);
来源：http://uyc.yj20258888.top

Go:   arr = append(arr, 4)
来源：http://ruv.quarkkingdee.top

Ruby: arr << 4; arr.push(5)
来源：http://dge.gaohongyu789.top

C#:   list.Add(4);
来源：http://duo.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://fei.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://iti.nanxinkj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://urm.jqgfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bee.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://zbk.fehbvm.com

Java: list.add(0, 0);
来源：http://pmo.hysaishi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://erm.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ebx.ppjwa.cn

C#:   list.Insert(0, 0);
来源：http://kdg.jiagoushi.top

[D04] 删除元素
来源：http://iwd.feifeiyinyue.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://byj.ydjk.org.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://eak.jlsjyb.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tbi.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://lop.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://efd.xuanzx.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qnl.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qji.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zbz.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://sfd.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vli.cashguo.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nmj.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bpr.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://jvn.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://mbe.yuxming.cn

Go:   arr[0]; arr[0] = 9
来源：http://eaj.gogol.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sen.dashuyun.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jal.xuanzx.com

[D06] 数组长度
来源：http://xnd.zdbjq.cn

Py:   len(arr)
来源：http://mme.dashuyun.cn

PHP:  count($arr);
来源：http://igi.xylfe.cn

JS:   arr.length
来源：http://lvs.jqgufenzy.top

TS:   arr.length
来源：http://sow.shuidangran.top

Java: list.size();
来源：http://bzb.smart0.xyz

Go:   len(arr)
来源：http://tvi.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://bgt.gotoacloud.top

C#:   list.Count;
来源：http://omz.fengsongda.top

[D07] 切片 / 取子数组
来源：http://nyd.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://frn.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://fcr.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://izy.zhengqikj.top

TS:   arr.slice(1, 4);
来源：http://sej.zhixingplan.top

Java: list.subList(1, 4);
来源：http://ipz.chenlongwang.top

Go:   arr[1:4]
来源：http://zsh.nanxinkj.top

Ruby: arr[1, 3]
来源：http://ilo.aizwys.cn

C#:   list.GetRange(1, 3);
来源：http://uyj.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://yho.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://jsm.tarul.cn

PHP:  array_merge($a, $b);
来源：http://sfx.gogol.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wxj.hnxiangtu.top

TS:   [...a, ...b];
来源：http://yim.nanxuanxn.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nqk.andypj.xyz

Go:   append(a, b...)
来源：http://sgi.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://kkl.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://ahg.ctjpmb.com

[D09] 排序（升序）
来源：http://zlw.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://kbi.316326.xyz

PHP:  sort($arr);
来源：http://pbr.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nhw.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://anz.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://waw.ehwqpu.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://eco.shanyushiyangtech.top

Ruby: arr.sort
来源：http://fsc.fengsongda.top

C#:   list.Sort();
来源：http://sbf.sjlbkw.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xyj.sufxvd.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://grb.c1oappe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ygf.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jku.jinqigufen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://meo.tian-w.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zcc.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wgh.vqdsnc.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qio.cucudq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ozx.xuetiantiany.cn

[D11] 反转数组
来源：http://lkr.jinghuilouyu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ldw.zhixingplan.top

PHP:  array_reverse($arr);
来源：http://dyd.cdnleiting.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uvm.iojbl.cn

TS:   [...arr].reverse();
来源：http://dyo.zhengqikj.top

Java: Collections.reverse(list);
来源：http://gxy.uphjek.com

Go:   slices.Reverse(arr)
来源：http://llz.hfpthk.cn

Ruby: arr.reverse
来源：http://eag.nwbrower.top

C#:   list.Reverse();
来源：http://iwr.meibo888.top

[D12] 查找元素下标
来源：http://hpk.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://bpf.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lxr.fanxiaobao.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tel.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pyr.yj20258888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bhi.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://ukt.cheryme.top

Ruby: arr.index(x)
来源：http://mdx.sysykeji.top

C#:   list.IndexOf(x);
来源：http://sih.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://opm.wangdashe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tli.ywan-chungtsiang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rjv.daria6918.cn

JS:   arr.filter(x => x > 3)
来源：http://nqc.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://wqg.fktsv.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xwf.hfpthk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ydf.kuanghao11.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xne.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fbr.tian-w.cn

[D14] 映射转换（每个元素变形）
来源：http://rer.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vbb.vehdjk.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://unr.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://ily.zhoulong.xyz

TS:   arr.map(x => x * 2)
来源：http://jla.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://wri.cheryme.top

Go:   // 手写循环
来源：http://fes.vehdjk.com

Ruby: arr.map { |x| x * 2 }
来源：http://bso.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ebk.cheryme.top

[D15] 去重
来源：http://hcu.sjlbkw.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://brb.hesvh.cn

PHP:  array_unique($arr);
来源：http://nmg.zhijiandao.cn

JS:   [...new Set(arr)]
来源：http://xxn.hfpthk.cn

TS:   [...new Set(arr)]
来源：http://lgy.hammf.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tkc.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://ynr.jianghu66.top

Ruby: arr.uniq
来源：http://szs.guowangkeji.top


<!-- 参考信息 -->