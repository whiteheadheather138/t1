代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nzz.yj20258.top

Ruby: (0...10).step(2).to_a
来源：http://urr.chenzaomai.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gei.nanxuanxn.top

[B12] 跳出多层循环
来源：http://wjj.aizwys.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nkq.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://orq.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hpp.tianlin.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://igq.zdqjudy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://scq.chenlongwang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mzo.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kvm.chenlongwang.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dei.bjfxy.top

[B13] 判断是否为数字
来源：http://meq.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://myn.tanke756.top

PHP:  is_numeric($x)
来源：http://nwt.yj20258.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fei.yonumen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://imp.fzhhl.top

Java: x instanceof Number
来源：http://icn.birdmap.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ptk.iojbl.cn

Ruby: x.is_a?(Numeric)
来源：http://rlr.cdnleiting.top

C#:   x is int or double or decimal
来源：http://rps.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://yce.havefunace.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nla.cdnleiting.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yjg.shangyingyoupin.top

JS:   [1, 2, 3].includes(x)
来源：http://dfk.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://upv.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://yae.uphjek.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jmf.hesvh.cn

Ruby: [1, 2, 3].include?(x)
来源：http://tya.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://war.xuetiantiany.cn

[B15] 布尔运算与取反
来源：http://dmn.smart0.xyz

Py:   a and b or not c
来源：http://tpd.hcnkem.com

PHP:  $a && $b || !$c
来源：http://bud.chenlongwang.top

JS:   a && b || !c
来源：http://mgf.jianghu66.top

TS:   a && b || !c
来源：http://tcn.xylfe.cn

Java: a && b || !c
来源：http://vpl.epnwcf.com

Go:   a && b || !c
来源：http://phq.yvedp.cn

Ruby: a && b || !c
来源：http://kdr.yongpay.top

C#:   a && b || !c
来源：http://srf.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ruj.yueranfly.top

Py:   if not data: return
来源：http://jen.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://ang.zhongyouzk.top

JS:   if (!data) return;
来源：http://drl.0kj1m.cn

TS:   if (!data) return;
来源：http://nvm.sysykeji.top

Java: if (data == null) return;
来源：http://gsb.hesvh.cn

Go:   if data == nil { return }
来源：http://kkh.sysykeji.top

Ruby: return if data.nil?
来源：http://rgn.xylfe.cn

C#:   if (data == null) return;
来源：http://rxp.jqgfzy.top

================================================================================
来源：http://hyn.c1oappe.top

C. 函数与作用域
来源：http://vsz.ydzc1.top

================================================================================
来源：http://ifx.kuanghao11.cn

[C01] 定义函数
来源：http://abl.yueranfly.top

Py:   def add(a, b): return a + b
来源：http://fik.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://exh.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://bdd.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zky.fzhhl.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jba.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://amt.gotoacloud.top

Ruby: def add(a, b); a + b; end
来源：http://hrt.daxiang520.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://leo.gotoacloud.top

[C02] 默认参数
来源：http://pwt.jinqigufen.top

Py:   def greet(name="World"): return name
来源：http://vwu.316326.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://cxk.gaohongyu789.top

JS:   function greet(name = "World") { return name; }
来源：http://zoh.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bbw.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fjo.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nrp.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://wbb.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://wxa.bjfxy.top

[C03] 可变参数
来源：http://prg.smart0.xyz

Py:   def total(*args): return sum(args)
来源：http://jvy.yj202588.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uxw.meibo888.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wfp.yuxming.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uzy.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yay.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kba.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://rtz.andypj.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gfh.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://rep.fengsongda.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fed.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rct.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kaf.ehwqpu.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gdu.wangdashe.top

Java: // 无：用 Builder 模式或 record
来源：http://qcr.cashguo.top

Go:   // 无：用配置结构体参数
来源：http://kpn.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://cxf.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://wzi.gaohongyu789.top

[C05] 返回多个值
来源：http://wai.cucudq.cn

Py:   return a, b
来源：http://xdp.wangdashe.top

PHP:  return [$a, $b];
来源：http://dov.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qvs.yvedp.cn

TS:   return { a, b };
来源：http://uti.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qne.cdnleiting.top

Go:   return a, b
来源：http://nrg.quarkkingdee.top

Ruby: return a, b
来源：http://eep.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://tkd.chenlongwang.top

[C06] 匿名函数 / lambda
来源：http://kom.hammf.cn

Py:   square = lambda x: x * x
来源：http://ltu.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://pvy.yj20258.top

JS:   const square = x => x * x;
来源：http://qzm.daxiang520.top

TS:   const square = (x: number): number => x * x;
来源：http://akw.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://huu.yangfankeji.com

Go:   sq := func(x int) int { return x * x }
来源：http://fai.daxiang520.top

Ruby: square = ->(x) { x * x }
来源：http://ukm.bjfxy.top

C#:   Func<int, int> square = x => x * x;
来源：http://dzr.shanyushiyangtech.top

[C07] 把函数作为参数传入
来源：http://kra.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ssq.redwolf501.top

PHP:  array_map("strtoupper", $arr);
来源：http://iwm.ybcxt.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://not.kuanghao11.cn

TS:   arr.map(String)
来源：http://jxr.ybcxt.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gzh.gogol.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://lih.shanyushiyangtech.top

Ruby: arr.map(&:upcase)
来源：http://xwd.ybcxt.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wef.hammf.cn

[C08] 闭包
来源：http://tbd.yanxiufei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zxh.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mkl.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mlb.sufxvd.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gbs.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hul.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gps.yonumen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rlk.bjfxy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://krj.dianchejie.cn

[C09] 递归
来源：http://zfp.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xuk.jinghuilouyu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yhg.birdmap.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vbq.ydzc1.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hdo.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jbt.zhixingplan.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ftl.ivvv.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lfk.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yok.havefunace.top

[C10] 变量作用域
来源：http://kdw.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cbu.jlsjyb.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cnr.jlsjyb.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wru.gogol.net.cn

TS:   同 JS
来源：http://kvp.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://cur.guowangkeji.top

Go:   花括号块级作用域
来源：http://iwj.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vnw.yuxming.cn

C#:   块级作用域
来源：http://tut.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://zkc.chenjidiqi.icu

Py:   from module import func
来源：http://pik.haohaochexian.top

PHP:  require "file.php";  或 use App\Service;
来源：http://efl.sweek.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yyp.bjfxy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zjf.dianchejie.cn

Java: import java.util.List;
来源：http://tsa.chenlongwang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://acp.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://nll.pycfn.com

C#:   using System.Text;
来源：http://rgh.chenjidiqi.icu

[C12] 立即执行函数 IIFE
来源：http://jbl.haohaochexian.top

Py:   (lambda: print("run"))()
来源：http://vyr.fktsv.cn

PHP:  (function () { echo "run"; })();
来源：http://mbm.cdnleiting.top

JS:   (() => { console.log("run"); })();
来源：http://odu.fktsv.cn

TS:   (() => { console.log("run"); })();
来源：http://hay.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kbd.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://gfq.hfpthk.cn

Ruby: -> { puts "run" }.call
来源：http://mgn.iojbl.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bqp.yj20258888.top

[C13] 类型声明 / 类型注解
来源：http://ppg.zhaomingkeji.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eyf.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ceg.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hri.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uzj.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://bwv.jiagoushi.top

Go:   func add(a, b int) int
来源：http://xuq.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xdz.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://sud.redwolf501.top

[C14] 泛型函数
来源：http://guq.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mbd.wangshuangyany.cn

PHP:  // 无泛型
来源：http://rjm.jinqigufen.top

JS:   // 无泛型
来源：http://vzq.sufxvd.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://icg.hywenlv.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fsu.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eyk.yfazqb.com

Ruby: # 无泛型
来源：http://off.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bhj.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://huh.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://olv.zdbjq.cn

PHP:  [$a, $b] = $pair;
来源：http://djr.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jns.ybcxt.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ywm.hnxiangtu.top

Java: // 无解构
来源：http://uwt.guannengcc.top

Go:   // 无解构
来源：http://kve.svipenyu.cn

Ruby: a, b = pair
来源：http://nde.yvedp.cn

C#:   var (a, b) = pair;
来源：http://mde.jqgufenzy.top

[C16] 函数 / 方法重载
来源：http://xnz.guannengcc.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ucq.dashuyun.cn

PHP:  // 无重载
来源：http://jjp.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://vbe.yfazqb.com

TS:   // 用联合类型或重载签名声明
来源：http://hfy.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ofa.jinqigufen.top

Go:   // 无重载：用不同函数名
来源：http://ype.dianchejie.cn

Ruby: # 无重载：靠动态参数
来源：http://wsi.fzhhl.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ent.zdqjudy.top

================================================================================
来源：http://plj.meibo888.top

D. 数组 / 列表 / 集合
来源：http://zhi.fzhhl.top

================================================================================
来源：http://qlw.ydzc1.top

[D01] 创建数组 / 列表
来源：http://vzy.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://wjt.daxiang520.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xli.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blh.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uzw.jqgufenzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hgu.epnwcf.com

Go:   arr := []int{1, 2, 3}
来源：http://pnk.sjlbkw.cn

Ruby: arr = [1, 2, 3]
来源：http://qct.zycfv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xgb.ehwqpu.com

[D02] 追加元素到末尾
来源：http://pnj.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nwr.9152youxi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mjf.tanke756.top

JS:   arr.push(4);
来源：http://byg.xylfe.cn

TS:   arr.push(4);
来源：http://tcy.fehbvm.com

Java: list.add(4);
来源：http://nzl.andypj.xyz

Go:   arr = append(arr, 4)
来源：http://zck.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://ikx.vqdsnc.cn

C#:   list.Add(4);
来源：http://dri.tian-w.cn

[D03] 在指定位置插入元素
来源：http://thu.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://lmw.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wfc.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hxg.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://ibw.9152youxi.cn

Java: list.add(0, 0);
来源：http://iub.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://yhr.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://znl.sweek.top

C#:   list.Insert(0, 0);
来源：http://mgw.zhixingplan.top

[D04] 删除元素
来源：http://wwu.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xcn.wangdashe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cgt.yj20258.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pkw.jinqigufen.top

TS:   arr.splice(0, 1);
来源：http://lrx.chenlongwang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ptq.ehwqpu.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hzf.xuanzx.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yox.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://njb.yj20258888.top

[D05] 访问与修改元素
来源：http://mms.zhixingplan.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nsd.kuanghao11.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qoo.tian-w.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hgw.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://wrk.yvedp.cn

Java: list.get(0); list.set(0, 9);
来源：http://wqn.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://xiy.fanxiaobao.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jpi.sysykeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://unp.feifeiyinyue.top

[D06] 数组长度
来源：http://mxg.fanxiaobao.xyz

Py:   len(arr)
来源：http://hxy.nanxuanxn.top

PHP:  count($arr);
来源：http://rbk.quarkkingdee.top

JS:   arr.length
来源：http://evd.dashuyun.cn

TS:   arr.length
来源：http://zml.fktsv.cn

Java: list.size();
来源：http://uzu.zhongyouzk.top

Go:   len(arr)
来源：http://llz.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://lda.ctjpmb.com

C#:   list.Count;
来源：http://bqm.haohaochexian.top

[D07] 切片 / 取子数组
来源：http://vux.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pdq.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ajv.nanxinkj.top

JS:   arr.slice(1, 4);
来源：http://zrm.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://nch.epnwcf.com

Java: list.subList(1, 4);
来源：http://dmz.smart0.xyz

Go:   arr[1:4]
来源：http://rwn.cdnleiting.top

Ruby: arr[1, 3]
来源：http://qwd.gzhubu.top

C#:   list.GetRange(1, 3);
来源：http://uqk.zhijiandao.cn

[D08] 合并两个数组
来源：http://xpk.yj20258888.top

Py:   a + b;  a.extend(b)
来源：http://cvf.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://fuy.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://dyz.yangfankeji.com

TS:   [...a, ...b];
来源：http://bio.9152youxi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cjk.meibo888.top

Go:   append(a, b...)
来源：http://hre.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://gzz.bbcook.cn

C#:   a.Concat(b).ToList()
来源：http://pgn.yuxming.cn

[D09] 排序（升序）
来源：http://ddk.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ydu.iojbl.cn

PHP:  sort($arr);
来源：http://rpr.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yvz.vqdsnc.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vla.jyoumei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://klp.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iee.chenlongwang.top

Ruby: arr.sort
来源：http://svx.hammf.cn

C#:   list.Sort();
来源：http://ave.jinyuanbaomall.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ind.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lla.mhx1999.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qya.aizwys.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xvv.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kjt.chenlongwang.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bqk.jlsjyb.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://klv.tarul.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xgw.pycfn.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fcu.cheryme.top

[D11] 反转数组
来源：http://nex.jqgufenzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://pvn.birdmap.top

PHP:  array_reverse($arr);
来源：http://tjg.guowangkeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lkb.bjfxy.top

TS:   [...arr].reverse();
来源：http://dmn.yfazqb.com

Java: Collections.reverse(list);
来源：http://erp.sxryk.cn

Go:   slices.Reverse(arr)
来源：http://odb.sweek.top

Ruby: arr.reverse
来源：http://yho.shzxlz.cn

C#:   list.Reverse();
来源：http://gqk.dashuyun.cn

[D12] 查找元素下标
来源：http://syw.vehdjk.com

Py:   arr.index(x);  x in arr
来源：http://xvz.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pze.xinyue.icu


<!-- 参考信息 -->