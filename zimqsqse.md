代发 wailian999

PHP:  $a && $b || !$c
来源：http://ass.iojbl.cn

JS:   a && b || !c
来源：http://uhl.hongshengwenyu.top

TS:   a && b || !c
来源：http://jqm.cashguo.top

Java: a && b || !c
来源：http://uqf.wangdashe.top

Go:   a && b || !c
来源：http://tyw.zhiwuduotai.top

Ruby: a && b || !c
来源：http://pxc.feifeiyinyue.top

C#:   a && b || !c
来源：http://oft.birdmap.top

[B16] 卫语句：不满足条件提前返回
来源：http://ecz.smart0.xyz

Py:   if not data: return
来源：http://unk.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://gww.sxryk.cn

JS:   if (!data) return;
来源：http://zpl.ydzc1.top

TS:   if (!data) return;
来源：http://bpp.chenlongwang.top

Java: if (data == null) return;
来源：http://gev.zhoulong.xyz

Go:   if data == nil { return }
来源：http://pbr.hywenlv.cn

Ruby: return if data.nil?
来源：http://zah.zhengqikj.top

C#:   if (data == null) return;
来源：http://wsa.wangshuangyany.cn

================================================================================
来源：http://sbk.snrcjt.cn

C. 函数与作用域
来源：http://mhd.hcnkem.com

================================================================================
来源：http://gou.jinqigufen.top

[C01] 定义函数
来源：http://pyf.shanyushiyangkeji.top

Py:   def add(a, b): return a + b
来源：http://mmm.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rnt.nanxinkj.top

JS:   function add(a, b) { return a + b; }
来源：http://xqr.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ukm.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ngi.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tuy.shangyingyoupin.top

Ruby: def add(a, b); a + b; end
来源：http://zlq.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oum.wangshuangyany.cn

[C02] 默认参数
来源：http://qxh.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://syh.zhixingplan.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hsq.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://qxg.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xyq.cdnleiting.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kfh.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://shj.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://npk.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://gdb.zhengqikj.top

[C03] 可变参数
来源：http://eum.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://cvf.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fjr.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qwg.yuanzhike.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ypv.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cmg.uphjek.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://obf.yj202588.top

Ruby: def total(*nums); nums.sum; end
来源：http://nmk.yj202588.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zdt.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://wgn.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fdz.ehwqpu.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vtq.shuidangran.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lpt.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xzl.kuanghao11.cn

Java: // 无：用 Builder 模式或 record
来源：http://ygs.cheryme.top

Go:   // 无：用配置结构体参数
来源：http://htg.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://zgz.pengpengdd.cyou

C#:   f(a: 1, b: 2)
来源：http://jnb.ydjk.org.cn

[C05] 返回多个值
来源：http://hxu.jinghuilouyu.cn

Py:   return a, b
来源：http://pby.jiagoushi.top

PHP:  return [$a, $b];
来源：http://uxj.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pfw.quarkkingdee.top

TS:   return { a, b };
来源：http://eif.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kts.gzhubu.top

Go:   return a, b
来源：http://qty.zhengqikj.top

Ruby: return a, b
来源：http://vah.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://zgi.gzhubu.top

[C06] 匿名函数 / lambda
来源：http://lcg.ybcxt.top

Py:   square = lambda x: x * x
来源：http://jih.jqgufenzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wze.316326.xyz

JS:   const square = x => x * x;
来源：http://yid.ehwqpu.com

TS:   const square = (x: number): number => x * x;
来源：http://grf.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vhl.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://stg.zdqjudy.top

Ruby: square = ->(x) { x * x }
来源：http://gha.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://qfv.smart0.xyz

[C07] 把函数作为参数传入
来源：http://vwx.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://emz.ivvv.top

PHP:  array_map("strtoupper", $arr);
来源：http://cru.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://loa.ppjwa.cn

TS:   arr.map(String)
来源：http://oba.jinghuilouyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lce.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kgl.fzhhl.top

Ruby: arr.map(&:upcase)
来源：http://uza.aibaodan.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://apv.gotoacloud.top

[C08] 闭包
来源：http://zky.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tps.xziqi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://owr.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://olo.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tsd.sufxvd.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bag.52xcode.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wgb.hesvh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ckv.ctjpmb.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://spn.meibo888.top

[C09] 递归
来源：http://itz.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zcy.hnqzz.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cnt.yongpay.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://afs.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oqt.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gza.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uul.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hbe.chenjidiqi.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qgo.c1oappe.top

[C10] 变量作用域
来源：http://itg.xziqi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rzs.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ego.chenlongwang.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hhr.ywan-chungtsiang.top

TS:   同 JS
来源：http://wlt.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://dvp.jianghu66.top

Go:   花括号块级作用域
来源：http://jgo.gaohongyu789.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hzp.ppjwa.cn

C#:   块级作用域
来源：http://gfx.quarkkingdee.top

[C11] 模块导入与导出
来源：http://ghl.havefunace.top

Py:   from module import func
来源：http://tfn.zhaomingkeji.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://ens.feifeiyinyue.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://lvp.cheryme.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nzh.haohaochexian.top

Java: import java.util.List;
来源：http://gty.shzxlz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ugk.ppjwa.cn

Ruby: require "json"; require_relative "./util"
来源：http://lyo.ctjpmb.com

C#:   using System.Text;
来源：http://uqq.yueranfly.top

[C12] 立即执行函数 IIFE
来源：http://wgc.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://vcs.andypj.xyz

PHP:  (function () { echo "run"; })();
来源：http://bqd.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://zgy.dashuyun.cn

TS:   (() => { console.log("run"); })();
来源：http://tnu.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fea.xziqi.cn

Go:   func() { fmt.Println("run") }()
来源：http://cbn.zycfv.cn

Ruby: -> { puts "run" }.call
来源：http://wgx.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gfi.gogol.net.cn

[C13] 类型声明 / 类型注解
来源：http://bbp.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cpn.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://spn.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://aho.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ipi.jinqigufen.top

Java: int add(int a, int b) { return a + b; }
来源：http://ejw.yj20258888.top

Go:   func add(a, b int) int
来源：http://iji.aizwys.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mdd.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://wfq.zhaomingkeji.xyz

[C14] 泛型函数
来源：http://hid.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://orh.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://qcv.yj20258888.top

JS:   // 无泛型
来源：http://bna.shzxlz.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aas.chenzaomai.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iff.hywenlv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qdl.ivvv.top

Ruby: # 无泛型
来源：http://xjo.havefunace.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tmm.yvedp.cn

[C15] 解构 / 展开参数
来源：http://ghq.hfpthk.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jlc.wangdashe.top

PHP:  [$a, $b] = $pair;
来源：http://hyp.xinyue.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://peo.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iya.guannengcc.top

Java: // 无解构
来源：http://nos.zdbjq.cn

Go:   // 无解构
来源：http://zha.fzhhl.top

Ruby: a, b = pair
来源：http://cbu.birdmap.top

C#:   var (a, b) = pair;
来源：http://uof.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://rzt.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nmm.shuidangran.top

PHP:  // 无重载
来源：http://ylw.yj202588.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xvh.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://zxi.iojbl.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ilm.yonumen.top

Go:   // 无重载：用不同函数名
来源：http://uto.jiagoushi.top

Ruby: # 无重载：靠动态参数
来源：http://mpl.yj20258.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xnb.shanyushiyangtech.top

================================================================================
来源：http://ilx.yj202588.top

D. 数组 / 列表 / 集合
来源：http://azy.yfazqb.com

================================================================================
来源：http://iix.zhongyouzk.top

[D01] 创建数组 / 列表
来源：http://vwm.xylfe.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nuz.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oan.jqgufenzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tjh.cashguo.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wvp.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cbd.shangyingyoupin.top

Go:   arr := []int{1, 2, 3}
来源：http://ciy.sweek.top

Ruby: arr = [1, 2, 3]
来源：http://hch.tianlin.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mvx.gzhubu.top

[D02] 追加元素到末尾
来源：http://pcm.yj202588.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yik.ivvv.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tpe.yueranfly.top

JS:   arr.push(4);
来源：http://wot.yuanzhike.top

TS:   arr.push(4);
来源：http://ofk.wangdashe.top

Java: list.add(4);
来源：http://vzy.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://fit.gogol.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://kjx.ctjpmb.com

C#:   list.Add(4);
来源：http://sqm.xuanzx.com

[D03] 在指定位置插入元素
来源：http://bcc.xingfuxueyuan.xyz

Py:   arr.insert(0, 0)
来源：http://zvc.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gmx.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dbk.shanyushiyangtech.top

TS:   arr.splice(0, 0, 0);
来源：http://ngo.cashguo.top

Java: list.add(0, 0);
来源：http://wfc.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nep.birdmap.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eps.jyoumei.cn

C#:   list.Insert(0, 0);
来源：http://iad.0kj1m.cn

[D04] 删除元素
来源：http://dmx.fengsongda.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://reb.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xxs.316326.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xqe.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://jwi.birdmap.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zld.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://djs.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ioy.chenlongwang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sia.fzhhl.top

[D05] 访问与修改元素
来源：http://mez.smart0.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gvj.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yyb.jinqigfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tvd.sysykeji.top

TS:   arr[0]; arr.at(-1);
来源：http://jyu.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://eub.sufxvd.cn

Go:   arr[0]; arr[0] = 9
来源：http://gom.gotoacloud.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ndc.andypj.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://paw.zhoulong.xyz

[D06] 数组长度
来源：http://foi.gzhubu.top

Py:   len(arr)
来源：http://wdl.fehbvm.com

PHP:  count($arr);
来源：http://gyg.daria6918.cn

JS:   arr.length
来源：http://xli.fehbvm.com

TS:   arr.length
来源：http://zek.nanxinkj.top

Java: list.size();
来源：http://ksx.wangshuangyany.cn

Go:   len(arr)
来源：http://dvm.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://nhg.ctjpmb.com

C#:   list.Count;
来源：http://guf.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://okh.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rwp.shuidangran.top

PHP:  array_slice($arr, 1, 3);
来源：http://wum.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://ypr.zhongyouzk.top

TS:   arr.slice(1, 4);
来源：http://vcr.zhixingplan.top

Java: list.subList(1, 4);
来源：http://fid.jiagoushi.top

Go:   arr[1:4]
来源：http://cps.uphjek.com

Ruby: arr[1, 3]
来源：http://dxl.redwolf501.top

C#:   list.GetRange(1, 3);
来源：http://mrm.shangyingyoupin.top

[D08] 合并两个数组
来源：http://jod.haohaochexian.top

Py:   a + b;  a.extend(b)
来源：http://oxx.yfazqb.com

PHP:  array_merge($a, $b);
来源：http://nxy.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nat.c1oappe.top

TS:   [...a, ...b];
来源：http://yro.tanke756.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jik.316326.xyz

Go:   append(a, b...)
来源：http://ufr.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://ilf.wangshuangyany.cn

C#:   a.Concat(b).ToList()
来源：http://ygc.yanxiufei.cn

[D09] 排序（升序）
来源：http://rqw.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ixz.zhoulong.xyz

PHP:  sort($arr);
来源：http://cqv.yj202588.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://njx.chenzaomai.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ffw.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://jgu.chenlongwang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://juf.wangdashe.top

Ruby: arr.sort
来源：http://wiu.jyoumei.cn

C#:   list.Sort();
来源：http://bdi.zhixingplan.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cwj.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vkm.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fxx.yueranfly.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://amb.sufxvd.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qmi.zhengqikj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kyn.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vos.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://aqz.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tag.sxryk.cn

[D11] 反转数组
来源：http://oeu.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://puk.cheryme.top

PHP:  array_reverse($arr);
来源：http://pir.andypj.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kzp.ctjpmb.com

TS:   [...arr].reverse();
来源：http://xyy.zdbjq.cn

Java: Collections.reverse(list);
来源：http://exm.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://cae.quarkkingdee.top

Ruby: arr.reverse
来源：http://cqn.bbcook.cn

C#:   list.Reverse();
来源：http://irx.ybcxt.top

[D12] 查找元素下标
来源：http://irw.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://vsc.tian-w.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eyv.ctjpmb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ixj.svipenyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zbc.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://orz.fehbvm.com

Go:   slices.Index(arr, x)
来源：http://qil.aizwys.cn

Ruby: arr.index(x)
来源：http://svf.jianghu66.top

C#:   list.IndexOf(x);
来源：http://noa.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://vug.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ich.c1oappe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gdq.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://eyd.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://ycf.vehdjk.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tji.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://czn.andypj.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ses.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nfa.jlsjyb.cn

[D14] 映射转换（每个元素变形）
来源：http://nsh.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oee.shanyushiyangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gev.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://fbq.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://kad.c1oappe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gsv.hnxiangtu.top

Go:   // 手写循环
来源：http://nys.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://zru.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zxu.fzhhl.top

[D15] 去重
来源：http://rba.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zqy.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://lpx.zdqjudy.top

JS:   [...new Set(arr)]
来源：http://ckr.vehdjk.com

TS:   [...new Set(arr)]
来源：http://jap.wangdashe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pjr.0kj1m.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kew.yvedp.cn

Ruby: arr.uniq
来源：http://ikt.gogol.net.cn


<!-- 参考信息 -->