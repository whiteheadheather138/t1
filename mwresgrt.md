代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zqk.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mew.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://byf.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xqq.fehbvm.com

[B13] 判断是否为数字
来源：http://vdc.gotoacloud.top

Py:   isinstance(x, (int, float))
来源：http://wah.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://nzi.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mwb.zycfv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dwx.shanyushiyangtech.top

Java: x instanceof Number
来源：http://tqe.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ctl.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://czp.yuanzhike.top

C#:   x is int or double or decimal
来源：http://gmn.zhiwuduotai.top

[B14] 判断值是否在集合内
来源：http://nux.shanyushiyangkeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ctp.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zpo.yj202588.top

JS:   [1, 2, 3].includes(x)
来源：http://vlr.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://pmo.ywan-chungtsiang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://roz.yuxming.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ppk.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tax.aizwys.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://grj.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://had.ydzc1.top

Py:   a and b or not c
来源：http://ppz.ppjwa.cn

PHP:  $a && $b || !$c
来源：http://iqr.fengsongda.top

JS:   a && b || !c
来源：http://tfy.tanke756.top

TS:   a && b || !c
来源：http://uyk.fehbvm.com

Java: a && b || !c
来源：http://fid.jlsjyb.cn

Go:   a && b || !c
来源：http://efh.ivvv.top

Ruby: a && b || !c
来源：http://uai.daria6918.cn

C#:   a && b || !c
来源：http://klb.yj20258.top

[B16] 卫语句：不满足条件提前返回
来源：http://oyr.tian-w.cn

Py:   if not data: return
来源：http://vni.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://zfn.hywenlv.cn

JS:   if (!data) return;
来源：http://bjd.316326.xyz

TS:   if (!data) return;
来源：http://kmj.birdmap.top

Java: if (data == null) return;
来源：http://sfq.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://jah.chenlongwang.top

Ruby: return if data.nil?
来源：http://pfd.zycfv.cn

C#:   if (data == null) return;
来源：http://bcp.jyoumei.cn

================================================================================
来源：http://elz.aizwys.cn

C. 函数与作用域
来源：http://ago.birdmap.top

================================================================================
来源：http://wdq.jianghu66.top

[C01] 定义函数
来源：http://ubg.nwbrower.top

Py:   def add(a, b): return a + b
来源：http://hdn.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rja.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://pqo.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xdq.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ogm.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://mtr.havefunace.top

Ruby: def add(a, b); a + b; end
来源：http://pku.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://osk.xylfe.cn

[C02] 默认参数
来源：http://fbt.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://ynw.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jcr.svipenyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://khb.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lbs.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pjt.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ocn.ywan-chungtsiang.top

Ruby: def greet(name = "World") = name
来源：http://tfd.shuidangran.top

C#:   string Greet(string name = "World") => name;
来源：http://ygy.quarkkingdee.top

[C03] 可变参数
来源：http://wtc.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://ioo.wangshuangyany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kjq.shzxlz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://uwy.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ptk.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eyq.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kbz.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://yaa.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hvo.iojbl.cn

[C04] 命名参数 / 关键字参数
来源：http://agx.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oul.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gvq.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eex.hfpthk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mym.ppjwa.cn

Java: // 无：用 Builder 模式或 record
来源：http://vmk.cqqwz.cn

Go:   // 无：用配置结构体参数
来源：http://jeb.hysaishi.cn

Ruby: f(a: 1, b: 2)
来源：http://uds.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://dal.uphjek.com

[C05] 返回多个值
来源：http://mgq.0kj1m.cn

Py:   return a, b
来源：http://jwl.tarul.cn

PHP:  return [$a, $b];
来源：http://epq.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mie.nanxuanxn.top

TS:   return { a, b };
来源：http://akg.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hnq.wangshuangyany.cn

Go:   return a, b
来源：http://pll.ybcxt.top

Ruby: return a, b
来源：http://asg.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://pcx.yanxiufei.cn

[C06] 匿名函数 / lambda
来源：http://edz.cqqwz.cn

Py:   square = lambda x: x * x
来源：http://lgz.shangyingyoupin.top

PHP:  $square = fn($x) => $x * $x;
来源：http://htv.yj20258888.top

JS:   const square = x => x * x;
来源：http://guw.ppjwa.cn

TS:   const square = (x: number): number => x * x;
来源：http://mei.pycfn.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sly.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rvd.pengpengdd.cyou

Ruby: square = ->(x) { x * x }
来源：http://eje.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://rsp.cdnleiting.top

[C07] 把函数作为参数传入
来源：http://nap.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://npb.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://bxn.jiagoushi.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gjp.zhoulong.xyz

TS:   arr.map(String)
来源：http://krq.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sxm.jinqigfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://izs.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://bjg.c1oappe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yie.kuanghao11.cn

[C08] 闭包
来源：http://yog.nanxuanxn.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://avv.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fcw.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zkw.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://swv.nwbrower.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ngr.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lbl.yuxming.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hkq.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://awg.zhiwuduotai.top

[C09] 递归
来源：http://urd.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dsa.ppjwa.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xtq.shanyushiyangkeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gdd.shzxlz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qji.xylfe.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hki.cucudq.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ezc.jqgfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yji.c1oappe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ypv.wangshuangyany.cn

[C10] 变量作用域
来源：http://kpw.yj20258.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qba.shanyushiyangtech.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oas.zhoulong.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hnz.zhoulong.xyz

TS:   同 JS
来源：http://mrr.fehbvm.com

Java: 方法内为块级作用域
来源：http://urp.zycfv.cn

Go:   花括号块级作用域
来源：http://owm.cashguo.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yze.vqdsnc.cn

C#:   块级作用域
来源：http://lyk.sjlbkw.cn

[C11] 模块导入与导出
来源：http://row.tanke756.top

Py:   from module import func
来源：http://lxn.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://jes.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wqt.fengsongda.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://udf.kuanghao11.cn

Java: import java.util.List;
来源：http://hmx.shuidangran.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qwt.meibo888.top

Ruby: require "json"; require_relative "./util"
来源：http://ymy.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://lvk.sjlbkw.cn

[C12] 立即执行函数 IIFE
来源：http://pjq.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://czd.aizwys.cn

PHP:  (function () { echo "run"; })();
来源：http://awj.fktsv.cn

JS:   (() => { console.log("run"); })();
来源：http://vek.gaohongyu789.top

TS:   (() => { console.log("run"); })();
来源：http://ynk.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ikx.xuanzx.com

Go:   func() { fmt.Println("run") }()
来源：http://owe.zhixingplan.top

Ruby: -> { puts "run" }.call
来源：http://bvx.yj20258.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lhy.cashguo.top

[C13] 类型声明 / 类型注解
来源：http://wsq.gzhubu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://crv.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qvk.pengpengdd.cyou

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bqh.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lcf.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wlm.hnqzz.top

Go:   func add(a, b int) int
来源：http://hjz.yuxming.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cvj.nanxuanxn.top

C#:   int Add(int a, int b) => a + b;
来源：http://ysb.yj202588.top

[C14] 泛型函数
来源：http://cbj.hnqzz.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qkv.fktsv.cn

PHP:  // 无泛型
来源：http://mwm.haohaochexian.top

JS:   // 无泛型
来源：http://eqm.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dgj.xuetiantiany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nrh.zhixingplan.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kyb.sweek.top

Ruby: # 无泛型
来源：http://cku.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://soz.hammf.cn

[C15] 解构 / 展开参数
来源：http://rli.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://elu.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://tkc.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gqk.yuxming.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hrx.yuanzhike.top

Java: // 无解构
来源：http://qja.ctjpmb.com

Go:   // 无解构
来源：http://nuf.ivvv.top

Ruby: a, b = pair
来源：http://zql.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://uvr.yueranfly.top

[C16] 函数 / 方法重载
来源：http://ftv.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yvo.yj202588.top

PHP:  // 无重载
来源：http://emh.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://tcb.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://aji.meibo888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://zet.gotoacloud.top

Go:   // 无重载：用不同函数名
来源：http://gca.hfpthk.cn

Ruby: # 无重载：靠动态参数
来源：http://vpk.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://kdg.ppjwa.cn

================================================================================
来源：http://qvk.yanxiufei.cn

D. 数组 / 列表 / 集合
来源：http://plo.jinyuanbaomall.cn

================================================================================
来源：http://zus.tian-w.cn

[D01] 创建数组 / 列表
来源：http://tax.meibo888.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pec.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://htg.gotoacloud.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lfr.sweek.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lzv.wangshuangyany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kpn.jinqigufen.top

Go:   arr := []int{1, 2, 3}
来源：http://etk.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://nyf.shzxlz.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ynl.svipenyu.cn

[D02] 追加元素到末尾
来源：http://uqq.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jan.jinghuilouyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://frj.tanke756.top

JS:   arr.push(4);
来源：http://who.tanke756.top

TS:   arr.push(4);
来源：http://xib.zdbjq.cn

Java: list.add(4);
来源：http://mqh.chenlongwang.top

Go:   arr = append(arr, 4)
来源：http://urr.daria6918.cn

Ruby: arr << 4; arr.push(5)
来源：http://pyh.xuetiantiany.cn

C#:   list.Add(4);
来源：http://yta.meibo888.top

[D03] 在指定位置插入元素
来源：http://rlo.yuanzhike.top

Py:   arr.insert(0, 0)
来源：http://xme.andypj.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hjt.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hqg.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://nsf.fzhhl.top

Java: list.add(0, 0);
来源：http://drb.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://wxu.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zvs.sufxvd.cn

C#:   list.Insert(0, 0);
来源：http://urc.sufxvd.cn

[D04] 删除元素
来源：http://tbu.iojbl.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qyd.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zvo.0kj1m.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://scu.ctjpmb.com

TS:   arr.splice(0, 1);
来源：http://sir.hongshengwenyu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xzy.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ffo.gzhubu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mpc.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oex.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://shc.birdmap.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://euu.pycfn.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fkc.ywan-chungtsiang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ufm.xuetiantiany.cn

TS:   arr[0]; arr.at(-1);
来源：http://lzw.cqqwz.cn

Java: list.get(0); list.set(0, 9);
来源：http://iza.zhiwuduotai.top

Go:   arr[0]; arr[0] = 9
来源：http://acb.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mjr.zhongyouzk.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bvu.jinqigufen.top

[D06] 数组长度
来源：http://hqj.jiagoushi.top

Py:   len(arr)
来源：http://xjs.cqqwz.cn

PHP:  count($arr);
来源：http://bxq.fehbvm.com

JS:   arr.length
来源：http://igt.sufxvd.cn

TS:   arr.length
来源：http://wqx.feifeiyinyue.top

Java: list.size();
来源：http://whf.quarkkingdee.top

Go:   len(arr)
来源：http://cnh.yvedp.cn

Ruby: arr.length; arr.size
来源：http://dmj.shangyingyoupin.top

C#:   list.Count;
来源：http://sot.chenzaomai.com

[D07] 切片 / 取子数组
来源：http://kei.zdqjudy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pry.svipenyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vhu.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://yxu.uphjek.com

TS:   arr.slice(1, 4);
来源：http://fvw.hcnkem.com

Java: list.subList(1, 4);
来源：http://lqe.nwbrower.top

Go:   arr[1:4]
来源：http://ywd.uphjek.com

Ruby: arr[1, 3]
来源：http://fgg.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://ahm.hnxiangtu.top

[D08] 合并两个数组
来源：http://ecf.sufxvd.cn

Py:   a + b;  a.extend(b)
来源：http://hvo.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://gjk.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wss.yj20258888.top

TS:   [...a, ...b];
来源：http://vqb.zhongyouzk.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nfk.fengsongda.top

Go:   append(a, b...)
来源：http://aki.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://qky.shanyushiyangtech.top

C#:   a.Concat(b).ToList()
来源：http://bbb.zhiwuduotai.top

[D09] 排序（升序）
来源：http://chx.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://fyd.epnwcf.com

PHP:  sort($arr);
来源：http://wcz.xziqi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://taq.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jxv.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dtz.yj20258888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kgw.havefunace.top

Ruby: arr.sort
来源：http://nir.shangyingyoupin.top

C#:   list.Sort();
来源：http://iut.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ohm.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://odp.jiagoushi.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rut.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xap.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dnd.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xar.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aee.yanxiufei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://odq.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jxv.shanyushiyangkeji.top

[D11] 反转数组
来源：http://hty.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://fxo.yj20258.top

PHP:  array_reverse($arr);
来源：http://gbc.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wku.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://sdd.zhixingplan.top

Java: Collections.reverse(list);
来源：http://xcw.cdnleiting.top

Go:   slices.Reverse(arr)
来源：http://htb.haohaochexian.top

Ruby: arr.reverse
来源：http://abv.hnxiangtu.top

C#:   list.Reverse();
来源：http://hnr.uphjek.com

[D12] 查找元素下标
来源：http://qmn.shuidangran.top

Py:   arr.index(x);  x in arr
来源：http://pxo.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vvo.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lco.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qrh.aizwys.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mvp.yonumen.top

Go:   slices.Index(arr, x)
来源：http://ean.yongpay.top

Ruby: arr.index(x)
来源：http://jih.jianghu66.top

C#:   list.IndexOf(x);
来源：http://zxj.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://tyo.shanyushiyangtech.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rfg.jqgufenzy.top


<!-- 参考信息 -->