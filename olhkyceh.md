代发 wailian999

PHP:  $a && $b || !$c
来源：http://ttv.shuidangran.top

JS:   a && b || !c
来源：http://svd.dashuyun.cn

TS:   a && b || !c
来源：http://quu.sysykeji.top

Java: a && b || !c
来源：http://rhn.pycfn.com

Go:   a && b || !c
来源：http://tez.aibaodan.cn

Ruby: a && b || !c
来源：http://vit.daria6918.cn

C#:   a && b || !c
来源：http://qce.sysykeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://gch.fengsongda.top

Py:   if not data: return
来源：http://qyz.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://yuo.gogol.net.cn

JS:   if (!data) return;
来源：http://vbz.jqgufenzy.top

TS:   if (!data) return;
来源：http://hdi.zycfv.cn

Java: if (data == null) return;
来源：http://adc.ivvv.top

Go:   if data == nil { return }
来源：http://sov.cashguo.top

Ruby: return if data.nil?
来源：http://xza.kuanghao11.cn

C#:   if (data == null) return;
来源：http://yxr.shanyushiyangkeji.top

================================================================================
来源：http://ech.hnxiangtu.top

C. 函数与作用域
来源：http://ptq.cheryme.top

================================================================================
来源：http://kgv.uphjek.com

[C01] 定义函数
来源：http://xzb.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://sus.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yqx.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://zqm.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bdw.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://xcj.yj202588.top

Go:   func add(a, b int) int { return a + b }
来源：http://aif.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://puv.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://std.smart0.xyz

[C02] 默认参数
来源：http://kbc.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://yxg.sufxvd.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://euz.dianchejie.cn

JS:   function greet(name = "World") { return name; }
来源：http://ubc.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://cgg.cdnleiting.top

Java: // 无默认参数：方法重载或 Optional
来源：http://avw.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qyr.yvedp.cn

Ruby: def greet(name = "World") = name
来源：http://qbc.yj202588.top

C#:   string Greet(string name = "World") => name;
来源：http://whx.daria6918.cn

[C03] 可变参数
来源：http://knq.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://daj.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lyu.hfpthk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ibj.zhoulong.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nye.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vas.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wpe.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tfa.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ouh.c1oappe.top

[C04] 命名参数 / 关键字参数
来源：http://uia.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rel.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xoa.xziqi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xri.gotoacloud.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dyn.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://mxw.daria6918.cn

Go:   // 无：用配置结构体参数
来源：http://kpk.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://ske.jinqigufen.top

C#:   f(a: 1, b: 2)
来源：http://dis.pengpengdd.cyou

[C05] 返回多个值
来源：http://nim.zhijiandao.cn

Py:   return a, b
来源：http://msw.chenzaomai.com

PHP:  return [$a, $b];
来源：http://etc.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://jki.jlsjyb.cn

TS:   return { a, b };
来源：http://uwu.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ltm.ivvv.top

Go:   return a, b
来源：http://dpn.zhoulong.xyz

Ruby: return a, b
来源：http://jom.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://zpg.ivvv.top

[C06] 匿名函数 / lambda
来源：http://jth.yj20258888.top

Py:   square = lambda x: x * x
来源：http://dth.feifeiyinyue.top

PHP:  $square = fn($x) => $x * $x;
来源：http://irg.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://obs.ywan-chungtsiang.top

TS:   const square = (x: number): number => x * x;
来源：http://ywl.cheryme.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pvr.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://uvf.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://ijc.smart0.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://hhl.ivvv.top

[C07] 把函数作为参数传入
来源：http://nsb.cheryme.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yjz.ydjk.org.cn

PHP:  array_map("strtoupper", $arr);
来源：http://twg.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://key.zycfv.cn

TS:   arr.map(String)
来源：http://ukr.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://bpm.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ynq.meibo888.top

Ruby: arr.map(&:upcase)
来源：http://cyl.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jyd.wangshuangyany.cn

[C08] 闭包
来源：http://qbb.yueranfly.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dof.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ekz.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oun.hnxiangtu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xao.cucudq.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fpb.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xjt.jinyuanbaomall.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vwj.birdmap.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rtz.hnxiangtu.top

[C09] 递归
来源：http://gpg.xylfe.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fkk.52xcode.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hzf.316326.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rnq.52xcode.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fjc.tanke756.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://foq.tianlin.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sba.fengsongda.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hsz.guowangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hls.fzhhl.top

[C10] 变量作用域
来源：http://lif.zhijiandao.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ant.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://tes.gogol.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://txp.fzhhl.top

TS:   同 JS
来源：http://qda.zhaomingkeji.xyz

Java: 方法内为块级作用域
来源：http://riz.fktsv.cn

Go:   花括号块级作用域
来源：http://ljp.fzhhl.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xoh.dianchejie.cn

C#:   块级作用域
来源：http://vtf.snrcjt.cn

[C11] 模块导入与导出
来源：http://jfv.zdbjq.cn

Py:   from module import func
来源：http://qya.yj20258.top

PHP:  require "file.php";  或 use App\Service;
来源：http://rlg.haohaochexian.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pgn.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ekz.tarul.cn

Java: import java.util.List;
来源：http://zjh.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gsk.gaohongyu789.top

Ruby: require "json"; require_relative "./util"
来源：http://hqp.wangshuangyany.cn

C#:   using System.Text;
来源：http://fcu.jiagoushi.top

[C12] 立即执行函数 IIFE
来源：http://llu.gzhubu.top

Py:   (lambda: print("run"))()
来源：http://hmf.jlsjyb.cn

PHP:  (function () { echo "run"; })();
来源：http://ndy.fanxiaobao.xyz

JS:   (() => { console.log("run"); })();
来源：http://kjl.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://cfn.yangfankeji.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://job.fengsongda.top

Go:   func() { fmt.Println("run") }()
来源：http://prp.hnxiangtu.top

Ruby: -> { puts "run" }.call
来源：http://juj.tarul.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xpz.zhongyouzk.top

[C13] 类型声明 / 类型注解
来源：http://noh.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://usr.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kcd.xuanzx.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://scz.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aqe.quarkkingdee.top

Java: int add(int a, int b) { return a + b; }
来源：http://laz.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://thu.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://gss.shzxlz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ont.tarul.cn

[C14] 泛型函数
来源：http://bvn.ywan-chungtsiang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tsj.nanxinkj.top

PHP:  // 无泛型
来源：http://azf.smart0.xyz

JS:   // 无泛型
来源：http://lej.kuanghao11.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fmi.svipenyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qwg.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://irp.gogol.net.cn

Ruby: # 无泛型
来源：http://wis.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pnh.bjfxy.top

[C15] 解构 / 展开参数
来源：http://tht.daria6918.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vhb.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://axn.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xyz.chenjidiqi.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://udg.nanxinkj.top

Java: // 无解构
来源：http://tsw.meibo888.top

Go:   // 无解构
来源：http://ios.yongpay.top

Ruby: a, b = pair
来源：http://her.ydzc1.top

C#:   var (a, b) = pair;
来源：http://zuj.fanxiaobao.xyz

[C16] 函数 / 方法重载
来源：http://rqf.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tbz.xziqi.cn

PHP:  // 无重载
来源：http://oyh.hesvh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fzt.haohaochexian.top

TS:   // 用联合类型或重载签名声明
来源：http://jjt.yj20258888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://kqf.ybcxt.top

Go:   // 无重载：用不同函数名
来源：http://flq.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://dkv.nwbrower.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fcf.pycfn.com

================================================================================
来源：http://npv.smart0.xyz

D. 数组 / 列表 / 集合
来源：http://kmj.hfpthk.cn

================================================================================
来源：http://msq.aizwys.cn

[D01] 创建数组 / 列表
来源：http://ttw.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://wqf.xuanzx.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hzv.zhengqikj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zgk.xinyue.icu

TS:   const arr: number[] = [1, 2, 3];
来源：http://cse.zhaomingkeji.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mxz.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://fcs.cqqwz.cn

Ruby: arr = [1, 2, 3]
来源：http://osa.bjfxy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bqg.zdbjq.cn

[D02] 追加元素到末尾
来源：http://qyv.xuetiantiany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://puv.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://drt.ybcxt.top

JS:   arr.push(4);
来源：http://lkb.zhaomingkeji.xyz

TS:   arr.push(4);
来源：http://fop.epnwcf.com

Java: list.add(4);
来源：http://snl.haohaochexian.top

Go:   arr = append(arr, 4)
来源：http://iut.aizwys.cn

Ruby: arr << 4; arr.push(5)
来源：http://mer.fzhhl.top

C#:   list.Add(4);
来源：http://obo.dashuyun.cn

[D03] 在指定位置插入元素
来源：http://lnv.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://kon.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bcf.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zid.hammf.cn

TS:   arr.splice(0, 0, 0);
来源：http://kev.zhengqikj.top

Java: list.add(0, 0);
来源：http://gwl.havefunace.top

Go:   arr = append([]int{0}, arr...)
来源：http://zxf.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ylh.yfazqb.com

C#:   list.Insert(0, 0);
来源：http://wse.wangdashe.top

[D04] 删除元素
来源：http://tlf.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jvz.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wty.yvedp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zqz.sysykeji.top

TS:   arr.splice(0, 1);
来源：http://dqq.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rsj.shuidangran.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jsu.c1oappe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tfz.sxryk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oaf.xuanzx.com

[D05] 访问与修改元素
来源：http://ggz.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://msn.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kcl.guowangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vta.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://hln.bbcook.cn

Java: list.get(0); list.set(0, 9);
来源：http://cip.gaohongyu789.top

Go:   arr[0]; arr[0] = 9
来源：http://tix.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oeo.quarkkingdee.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://htx.tian-w.cn

[D06] 数组长度
来源：http://xny.ctjpmb.com

Py:   len(arr)
来源：http://xxv.xuetiantiany.cn

PHP:  count($arr);
来源：http://ucd.jinqigufen.top

JS:   arr.length
来源：http://tib.andypj.xyz

TS:   arr.length
来源：http://pmc.zhoulong.xyz

Java: list.size();
来源：http://ras.shuidangran.top

Go:   len(arr)
来源：http://uyy.shanyushiyangtech.top

Ruby: arr.length; arr.size
来源：http://umn.bjfxy.top

C#:   list.Count;
来源：http://jei.ctjpmb.com

[D07] 切片 / 取子数组
来源：http://ofg.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ypm.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://rjs.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://kky.hammf.cn

TS:   arr.slice(1, 4);
来源：http://lge.xylfe.cn

Java: list.subList(1, 4);
来源：http://ojx.hcnkem.com

Go:   arr[1:4]
来源：http://ojs.daxiang520.top

Ruby: arr[1, 3]
来源：http://hwq.yueranfly.top

C#:   list.GetRange(1, 3);
来源：http://pvh.ivvv.top

[D08] 合并两个数组
来源：http://mvx.tianlin.xyz

Py:   a + b;  a.extend(b)
来源：http://nyf.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://glp.birdmap.top

JS:   [...a, ...b];  a.concat(b);
来源：http://obq.cdnleiting.top

TS:   [...a, ...b];
来源：http://qgi.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ffh.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://afa.fehbvm.com

Ruby: a + b;  a.concat(b)
来源：http://guo.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://ruw.yueranfly.top

[D09] 排序（升序）
来源：http://clv.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://etn.svipenyu.cn

PHP:  sort($arr);
来源：http://mjh.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sjq.epnwcf.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://mvd.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://htr.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://unu.yj20258888.top

Ruby: arr.sort
来源：http://apo.wangdashe.top

C#:   list.Sort();
来源：http://zuv.meibo888.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mld.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rby.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xhz.yj20258.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hmo.jinqigufen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qxx.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xka.chenjidiqi.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ytj.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mdm.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qsw.c1oappe.top

[D11] 反转数组
来源：http://gbn.havefunace.top

Py:   arr[::-1];  arr.reverse()
来源：http://afb.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://vlz.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uso.uphjek.com

TS:   [...arr].reverse();
来源：http://nnm.fktsv.cn

Java: Collections.reverse(list);
来源：http://qwq.aibaodan.cn

Go:   slices.Reverse(arr)
来源：http://hlo.sysykeji.top

Ruby: arr.reverse
来源：http://xpl.sufxvd.cn

C#:   list.Reverse();
来源：http://mih.jqgfzy.top

[D12] 查找元素下标
来源：http://gzh.hammf.cn

Py:   arr.index(x);  x in arr
来源：http://ehq.haohaochexian.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tko.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hnq.daxiang520.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sqb.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ngl.nwbrower.top

Go:   slices.Index(arr, x)
来源：http://cph.andypj.xyz

Ruby: arr.index(x)
来源：http://xly.aizwys.cn

C#:   list.IndexOf(x);
来源：http://kky.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://qys.daria6918.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nsr.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rqc.chenlongwang.top

JS:   arr.filter(x => x > 3)
来源：http://pha.quarkkingdee.top

TS:   arr.filter(x => x > 3)
来源：http://ywl.bbcook.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iet.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bdl.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://zmq.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cex.cqqwz.cn

[D14] 映射转换（每个元素变形）
来源：http://qbp.uphjek.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dfd.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jqt.gotoacloud.top

JS:   arr.map(x => x * 2)
来源：http://vvd.aizwys.cn

TS:   arr.map(x => x * 2)
来源：http://nbb.yvedp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://evs.cashguo.top

Go:   // 手写循环
来源：http://ofx.svipenyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wmg.haohaochexian.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hzh.hfpthk.cn

[D15] 去重
来源：http://mws.yvedp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tjx.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://gjs.fengsongda.top

JS:   [...new Set(arr)]
来源：http://hij.sufxvd.cn

TS:   [...new Set(arr)]
来源：http://vqs.ehwqpu.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ony.tanke756.top

Go:   // 用 map[T]struct{} 手写
来源：http://yzk.tianlin.xyz

Ruby: arr.uniq
来源：http://gob.gzhubu.top


<!-- 参考信息 -->