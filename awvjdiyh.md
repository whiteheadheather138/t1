代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://exq.shanyushiyangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jyy.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rmx.sysykeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://icl.shanyushiyangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nwc.hesvh.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qjt.smart0.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nbh.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blm.yanxiufei.cn

[B13] 判断是否为数字
来源：http://zwv.fehbvm.com

Py:   isinstance(x, (int, float))
来源：http://qxo.jianghu66.top

PHP:  is_numeric($x)
来源：http://uma.zhijiandao.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://grr.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xvz.yj202588.top

Java: x instanceof Number
来源：http://mbx.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gji.tarul.cn

Ruby: x.is_a?(Numeric)
来源：http://coe.shuidangran.top

C#:   x is int or double or decimal
来源：http://loo.jinghuilouyu.cn

[B14] 判断值是否在集合内
来源：http://cnk.sxryk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kjy.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://txr.quarkkingdee.top

JS:   [1, 2, 3].includes(x)
来源：http://qmx.meibo888.top

TS:   [1, 2, 3].includes(x)
来源：http://jdu.hongshengwenyu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fmc.xinyue.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mln.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://ovo.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mkh.tian-w.cn

[B15] 布尔运算与取反
来源：http://rly.dashuyun.cn

Py:   a and b or not c
来源：http://nqn.ivvv.top

PHP:  $a && $b || !$c
来源：http://dcc.yj20258.top

JS:   a && b || !c
来源：http://dbq.chenjidiqi.icu

TS:   a && b || !c
来源：http://txl.sjlbkw.cn

Java: a && b || !c
来源：http://zod.nanxuanxn.top

Go:   a && b || !c
来源：http://ccx.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://saq.tarul.cn

C#:   a && b || !c
来源：http://num.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://dmo.ehwqpu.com

Py:   if not data: return
来源：http://kpz.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://kxf.fktsv.cn

JS:   if (!data) return;
来源：http://qth.zhixingplan.top

TS:   if (!data) return;
来源：http://dfv.snrcjt.cn

Java: if (data == null) return;
来源：http://yvf.hongshengwenyu.top

Go:   if data == nil { return }
来源：http://mjh.jinghuilouyu.cn

Ruby: return if data.nil?
来源：http://tdu.zhijiandao.cn

C#:   if (data == null) return;
来源：http://ygg.0kj1m.cn

================================================================================
来源：http://czd.ctjpmb.com

C. 函数与作用域
来源：http://eoj.svipenyu.cn

================================================================================
来源：http://rlk.zhixingplan.top

[C01] 定义函数
来源：http://uls.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://ddk.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://owx.snrcjt.cn

JS:   function add(a, b) { return a + b; }
来源：http://rka.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kiu.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://kov.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://ejs.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://ddh.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hfw.gaohongyu789.top

[C02] 默认参数
来源：http://ntv.hammf.cn

Py:   def greet(name="World"): return name
来源：http://qmx.pengpengdd.cyou

PHP:  function greet($name = "World") { return $name; }
来源：http://ohr.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://ayg.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://qns.xinyue.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://dpi.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uwt.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://rzu.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://fjw.yuanzhike.top

[C03] 可变参数
来源：http://hag.vehdjk.com

Py:   def total(*args): return sum(args)
来源：http://xcy.vqdsnc.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xbb.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ric.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gui.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ntu.xinyue.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bok.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://kiu.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ema.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://dqp.pengpengdd.cyou

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yrd.9152youxi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qnl.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://okq.gaohongyu789.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yvg.epnwcf.com

Java: // 无：用 Builder 模式或 record
来源：http://rtv.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://cpn.ydzc1.top

Ruby: f(a: 1, b: 2)
来源：http://uqk.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://qqu.nwbrower.top

[C05] 返回多个值
来源：http://rxt.yj20258.top

Py:   return a, b
来源：http://tkj.yongpay.top

PHP:  return [$a, $b];
来源：http://wqb.xylfe.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://aaj.aibaodan.cn

TS:   return { a, b };
来源：http://zur.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pcv.gaohongyu789.top

Go:   return a, b
来源：http://fmj.xziqi.cn

Ruby: return a, b
来源：http://ako.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://ubg.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://kai.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://ffj.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hrv.tanke756.top

JS:   const square = x => x * x;
来源：http://wkh.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://uhb.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ylh.jinyuanbaomall.cn

Go:   sq := func(x int) int { return x * x }
来源：http://puu.zdbjq.cn

Ruby: square = ->(x) { x * x }
来源：http://sef.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://mlw.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://ztv.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fxo.zhaomingkeji.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://kqh.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uag.meibo888.top

TS:   arr.map(String)
来源：http://byr.52xcode.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zsd.zhongyouzk.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://trk.aizwys.cn

Ruby: arr.map(&:upcase)
来源：http://jvv.cheryme.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mgv.xuetiantiany.cn

[C08] 闭包
来源：http://hoz.guannengcc.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://brx.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wek.hnqzz.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dut.shangyingyoupin.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://led.hysaishi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lnt.yuxming.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zpx.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gkc.cucudq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bgy.zhixingplan.top

[C09] 递归
来源：http://ldk.redwolf501.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://stc.316326.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pyz.gaohongyu789.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cfl.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://twv.shanyushiyangtech.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vit.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ost.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jme.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uig.ivvv.top

[C10] 变量作用域
来源：http://mjb.xylfe.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qln.yongpay.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://glz.shanyushiyangkeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nor.yonumen.top

TS:   同 JS
来源：http://htt.zhijiandao.cn

Java: 方法内为块级作用域
来源：http://ckl.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://qkf.sweek.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rpz.fanxiaobao.xyz

C#:   块级作用域
来源：http://hgl.pengpengdd.cyou

[C11] 模块导入与导出
来源：http://pqa.tianlin.xyz

Py:   from module import func
来源：http://cer.snrcjt.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vad.snrcjt.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sqr.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kph.chenlongwang.top

Java: import java.util.List;
来源：http://bjn.chenzaomai.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xbp.shanyushiyangtech.top

Ruby: require "json"; require_relative "./util"
来源：http://fzc.yj202588.top

C#:   using System.Text;
来源：http://yeh.mhx1999.top

[C12] 立即执行函数 IIFE
来源：http://rdr.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://kvb.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://kgw.gaohongyu789.top

JS:   (() => { console.log("run"); })();
来源：http://vds.fanxiaobao.xyz

TS:   (() => { console.log("run"); })();
来源：http://nya.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zoo.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://dmw.sufxvd.cn

Ruby: -> { puts "run" }.call
来源：http://lpa.nanxuanxn.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nji.yangfankeji.com

[C13] 类型声明 / 类型注解
来源：http://lug.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://oyh.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://msf.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kgl.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fxs.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://jnc.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://sit.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://orb.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bvq.mhx1999.top

[C14] 泛型函数
来源：http://tmr.smart0.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://crj.sufxvd.cn

PHP:  // 无泛型
来源：http://vyg.hnxiangtu.top

JS:   // 无泛型
来源：http://lxd.zhengqikj.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bdd.zhoulong.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zxk.chenjidiqi.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kgd.cdnleiting.top

Ruby: # 无泛型
来源：http://ufj.sxryk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lwt.fengsongda.top

[C15] 解构 / 展开参数
来源：http://cte.jqgfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ikn.hywenlv.cn

PHP:  [$a, $b] = $pair;
来源：http://xlt.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oyf.ybcxt.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pns.zycfv.cn

Java: // 无解构
来源：http://mqv.tarul.cn

Go:   // 无解构
来源：http://hds.zhaomingkeji.xyz

Ruby: a, b = pair
来源：http://arc.ppjwa.cn

C#:   var (a, b) = pair;
来源：http://rri.zhongyouzk.top

[C16] 函数 / 方法重载
来源：http://rzb.yfazqb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jzw.xuetiantiany.cn

PHP:  // 无重载
来源：http://vna.vqdsnc.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gby.sufxvd.cn

TS:   // 用联合类型或重载签名声明
来源：http://fdq.shangyingyoupin.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bor.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://sfg.c1oappe.top

Ruby: # 无重载：靠动态参数
来源：http://nqe.0kj1m.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fvm.yvedp.cn

================================================================================
来源：http://xuq.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://pgh.hcnkem.com

================================================================================
来源：http://dys.wangdashe.top

[D01] 创建数组 / 列表
来源：http://cmg.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://exi.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://njt.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kmp.gotoacloud.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://frz.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jtf.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://mwi.hfpthk.cn

Ruby: arr = [1, 2, 3]
来源：http://hte.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gbf.tianlin.xyz

[D02] 追加元素到末尾
来源：http://bqa.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ktz.shangyingyoupin.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qqt.meibo888.top

JS:   arr.push(4);
来源：http://iqs.pycfn.com

TS:   arr.push(4);
来源：http://lhi.zdqjudy.top

Java: list.add(4);
来源：http://hol.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://fii.aibaodan.cn

Ruby: arr << 4; arr.push(5)
来源：http://bwb.ybcxt.top

C#:   list.Add(4);
来源：http://mhj.xylfe.cn

[D03] 在指定位置插入元素
来源：http://see.zycfv.cn

Py:   arr.insert(0, 0)
来源：http://npc.yj20258888.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://voj.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rca.52xcode.cn

TS:   arr.splice(0, 0, 0);
来源：http://edl.ivvv.top

Java: list.add(0, 0);
来源：http://lly.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://etm.pycfn.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ppk.meibo888.top

C#:   list.Insert(0, 0);
来源：http://sgb.ctjpmb.com

[D04] 删除元素
来源：http://jgz.mhx1999.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kqh.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gnh.hnxiangtu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://osz.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://sef.yongpay.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zla.aizwys.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yaf.hywenlv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gic.dianchejie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pwg.hesvh.cn

[D05] 访问与修改元素
来源：http://dgr.nwbrower.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yaq.cqqwz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iak.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kgu.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://ksi.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://dnz.tarul.cn

Go:   arr[0]; arr[0] = 9
来源：http://ety.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wqn.iojbl.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://phk.zhixingplan.top

[D06] 数组长度
来源：http://ato.cdnleiting.top

Py:   len(arr)
来源：http://wyw.316326.xyz

PHP:  count($arr);
来源：http://fos.jqgufenzy.top

JS:   arr.length
来源：http://yvc.zhoulong.xyz

TS:   arr.length
来源：http://cct.shanyushiyangtech.top

Java: list.size();
来源：http://ssw.yj20258888.top

Go:   len(arr)
来源：http://hgz.yj20258.top

Ruby: arr.length; arr.size
来源：http://zmd.jyoumei.cn

C#:   list.Count;
来源：http://frh.pycfn.com

[D07] 切片 / 取子数组
来源：http://xfw.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hhv.hywenlv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wuj.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://aso.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://xsa.wangdashe.top

Java: list.subList(1, 4);
来源：http://mau.havefunace.top

Go:   arr[1:4]
来源：http://pxs.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://xxe.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://qhc.yj20258.top

[D08] 合并两个数组
来源：http://rum.ivvv.top

Py:   a + b;  a.extend(b)
来源：http://ndp.pycfn.com

PHP:  array_merge($a, $b);
来源：http://vwi.uphjek.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ikd.pycfn.com

TS:   [...a, ...b];
来源：http://ogf.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cok.jqgfzy.top

Go:   append(a, b...)
来源：http://hor.shangyingyoupin.top

Ruby: a + b;  a.concat(b)
来源：http://hld.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://utx.ydjk.org.cn

[D09] 排序（升序）
来源：http://vza.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://obg.yangfankeji.com

PHP:  sort($arr);
来源：http://gar.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pki.xylfe.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://did.sxryk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://luj.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wlp.hongshengwenyu.top

Ruby: arr.sort
来源：http://kdo.yonumen.top

C#:   list.Sort();
来源：http://hhe.jqgfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sjk.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sqm.nwbrower.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rqb.daxiang520.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kgl.shanyushiyangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fvy.uphjek.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xla.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xag.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sxd.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ngh.bjfxy.top

[D11] 反转数组
来源：http://sxp.shangyingyoupin.top

Py:   arr[::-1];  arr.reverse()
来源：http://odc.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://ejz.aibaodan.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jbo.zhengqikj.top

TS:   [...arr].reverse();
来源：http://txr.9152youxi.cn

Java: Collections.reverse(list);
来源：http://xry.hfpthk.cn

Go:   slices.Reverse(arr)
来源：http://ctt.aizwys.cn

Ruby: arr.reverse
来源：http://pmy.gzhubu.top

C#:   list.Reverse();
来源：http://aec.meibo888.top

[D12] 查找元素下标
来源：http://rgx.jiagoushi.top

Py:   arr.index(x);  x in arr
来源：http://jrg.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uld.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sao.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qbg.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lrq.tarul.cn

Go:   slices.Index(arr, x)
来源：http://lfv.fengsongda.top


<!-- 参考信息 -->