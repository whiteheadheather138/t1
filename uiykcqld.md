代发 wailian999

[B13] 判断是否为数字
来源：http://maq.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://wyh.hesvh.cn

PHP:  is_numeric($x)
来源：http://sjg.tarul.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cgi.zdqjudy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rqg.nwbrower.top

Java: x instanceof Number
来源：http://ask.fanxiaobao.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pko.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://yxe.cdnleiting.top

C#:   x is int or double or decimal
来源：http://gaq.yueranfly.top

[B14] 判断值是否在集合内
来源：http://azk.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nzi.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rfq.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://kfg.zdqjudy.top

TS:   [1, 2, 3].includes(x)
来源：http://gvz.hnxiangtu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ntq.hnxiangtu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oup.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gxv.fanxiaobao.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://htw.pycfn.com

[B15] 布尔运算与取反
来源：http://dyh.feifeiyinyue.top

Py:   a and b or not c
来源：http://ips.jyoumei.cn

PHP:  $a && $b || !$c
来源：http://urc.guowangkeji.top

JS:   a && b || !c
来源：http://ewr.meibo888.top

TS:   a && b || !c
来源：http://mfu.shanyushiyangkeji.top

Java: a && b || !c
来源：http://qoi.hammf.cn

Go:   a && b || !c
来源：http://rcv.yangfankeji.com

Ruby: a && b || !c
来源：http://ytd.smart0.xyz

C#:   a && b || !c
来源：http://mrc.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://efg.ywan-chungtsiang.top

Py:   if not data: return
来源：http://stm.meibo888.top

PHP:  if (!$data) { return; }
来源：http://pho.ywan-chungtsiang.top

JS:   if (!data) return;
来源：http://brf.yvedp.cn

TS:   if (!data) return;
来源：http://cvq.cashguo.top

Java: if (data == null) return;
来源：http://oyv.ctjpmb.com

Go:   if data == nil { return }
来源：http://hcx.meibo888.top

Ruby: return if data.nil?
来源：http://dzo.gotoacloud.top

C#:   if (data == null) return;
来源：http://sys.yfazqb.com

================================================================================
来源：http://csj.0kj1m.cn

C. 函数与作用域
来源：http://sdy.wangshuangyany.cn

================================================================================
来源：http://qll.snrcjt.cn

[C01] 定义函数
来源：http://vab.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://nvb.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tjg.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://qky.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oxr.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bne.sweek.top

Go:   func add(a, b int) int { return a + b }
来源：http://jpy.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://kev.svipenyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zuf.ctjpmb.com

[C02] 默认参数
来源：http://mbr.smart0.xyz

Py:   def greet(name="World"): return name
来源：http://arp.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mca.sufxvd.cn

JS:   function greet(name = "World") { return name; }
来源：http://uqv.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cop.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://yup.hesvh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gid.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://atb.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://agh.mhx1999.top

[C03] 可变参数
来源：http://ihv.cdnleiting.top

Py:   def total(*args): return sum(args)
来源：http://fnu.havefunace.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mqy.nwbrower.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://omh.gogol.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fxn.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jlz.quarkkingdee.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mvf.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://itt.hcnkem.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sww.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://vav.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bqp.gogol.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zts.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uqn.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qau.ydjk.org.cn

Java: // 无：用 Builder 模式或 record
来源：http://puk.daria6918.cn

Go:   // 无：用配置结构体参数
来源：http://sgt.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://hvy.hywenlv.cn

C#:   f(a: 1, b: 2)
来源：http://sna.vqdsnc.cn

[C05] 返回多个值
来源：http://lhd.jinghuilouyu.cn

Py:   return a, b
来源：http://lbw.c1oappe.top

PHP:  return [$a, $b];
来源：http://sfn.yfazqb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://jvc.yangfankeji.com

TS:   return { a, b };
来源：http://pdd.zycfv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mfr.bjfxy.top

Go:   return a, b
来源：http://gii.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://vng.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://dta.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://zzb.meibo888.top

Py:   square = lambda x: x * x
来源：http://cuk.jinyuanbaomall.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xfr.fengsongda.top

JS:   const square = x => x * x;
来源：http://hwm.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://xxm.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fvw.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://siq.smart0.xyz

Ruby: square = ->(x) { x * x }
来源：http://prn.wangshuangyany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://www.cheryme.top

[C07] 把函数作为参数传入
来源：http://ffe.aizwys.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hok.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://edq.fzhhl.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://iij.nanxinkj.top

TS:   arr.map(String)
来源：http://dvl.hnqzz.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://awg.cashguo.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vdt.sxryk.cn

Ruby: arr.map(&:upcase)
来源：http://gsf.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xuf.jqgfzy.top

[C08] 闭包
来源：http://eir.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://udq.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sjp.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zzd.sjlbkw.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tfu.yj20258888.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cfu.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ban.snrcjt.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qkt.pycfn.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ihb.yvedp.cn

[C09] 递归
来源：http://ssw.dianchejie.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zat.zhixingplan.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://axh.ybcxt.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iwq.fzhhl.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zkk.cucudq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xjt.yueranfly.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gir.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uya.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qtp.zhiwuduotai.top

[C10] 变量作用域
来源：http://nqc.ppjwa.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pox.ywan-chungtsiang.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://yxd.zdbjq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gsg.c1oappe.top

TS:   同 JS
来源：http://krc.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://szp.yj20258.top

Go:   花括号块级作用域
来源：http://gea.yfazqb.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dwi.tianlin.xyz

C#:   块级作用域
来源：http://xwc.gogol.net.cn

[C11] 模块导入与导出
来源：http://tzy.xziqi.cn

Py:   from module import func
来源：http://ruz.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zfd.svipenyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://que.316326.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://doh.cqqwz.cn

Java: import java.util.List;
来源：http://tqz.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fxg.fengsongda.top

Ruby: require "json"; require_relative "./util"
来源：http://eow.feifeiyinyue.top

C#:   using System.Text;
来源：http://adm.zhengqikj.top

[C12] 立即执行函数 IIFE
来源：http://wrg.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://obc.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://pqe.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://tfc.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://fgq.zhoulong.xyz

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eqh.sjlbkw.cn

Go:   func() { fmt.Println("run") }()
来源：http://pkn.zhongyouzk.top

Ruby: -> { puts "run" }.call
来源：http://jck.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://wiv.shanyushiyangtech.top

[C13] 类型声明 / 类型注解
来源：http://anz.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dqe.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wuj.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bpn.aibaodan.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ywy.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://ppk.zhijiandao.cn

Go:   func add(a, b int) int
来源：http://zdr.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rfh.sxryk.cn

C#:   int Add(int a, int b) => a + b;
来源：http://jwp.shzxlz.cn

[C14] 泛型函数
来源：http://ezl.fktsv.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://haa.tianlin.xyz

PHP:  // 无泛型
来源：http://eok.hnxiangtu.top

JS:   // 无泛型
来源：http://awj.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://asr.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yug.iojbl.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ubz.xuetiantiany.cn

Ruby: # 无泛型
来源：http://nwo.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xdx.xziqi.cn

[C15] 解构 / 展开参数
来源：http://vvd.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gzb.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://muo.yongpay.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qpp.zhongyouzk.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://phm.redwolf501.top

Java: // 无解构
来源：http://hbn.hfpthk.cn

Go:   // 无解构
来源：http://pim.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://bmj.iojbl.cn

C#:   var (a, b) = pair;
来源：http://iak.sysykeji.top

[C16] 函数 / 方法重载
来源：http://gmk.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://phj.yuanzhike.top

PHP:  // 无重载
来源：http://yur.zhijiandao.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hpm.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://cnh.jinyuanbaomall.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hpx.hongshengwenyu.top

Go:   // 无重载：用不同函数名
来源：http://veh.hesvh.cn

Ruby: # 无重载：靠动态参数
来源：http://gmk.c1oappe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gtd.haohaochexian.top

================================================================================
来源：http://pgi.zhixingplan.top

D. 数组 / 列表 / 集合
来源：http://jct.sjlbkw.cn

================================================================================
来源：http://qda.shuidangran.top

[D01] 创建数组 / 列表
来源：http://cir.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qtq.yangfankeji.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mez.svipenyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zyd.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wwu.jqgfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sni.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://qkv.jiagoushi.top

Ruby: arr = [1, 2, 3]
来源：http://zcp.shuidangran.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ucq.hywenlv.cn

[D02] 追加元素到末尾
来源：http://hyp.hfpthk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kpy.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pqd.0kj1m.cn

JS:   arr.push(4);
来源：http://eiz.sweek.top

TS:   arr.push(4);
来源：http://bic.daxiang520.top

Java: list.add(4);
来源：http://amf.xuetiantiany.cn

Go:   arr = append(arr, 4)
来源：http://fpk.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://llo.xinyue.icu

C#:   list.Add(4);
来源：http://udk.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://yvt.zhixingplan.top

Py:   arr.insert(0, 0)
来源：http://sjt.zhixingplan.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rkp.pengpengdd.cyou

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://khj.iojbl.cn

TS:   arr.splice(0, 0, 0);
来源：http://wwx.havefunace.top

Java: list.add(0, 0);
来源：http://ehe.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://xqm.ehwqpu.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fbo.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://lso.havefunace.top

[D04] 删除元素
来源：http://luy.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hih.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://adl.birdmap.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://taf.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://sqp.jianghu66.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://niz.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ail.tanke756.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nus.daria6918.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gem.chenzaomai.com

[D05] 访问与修改元素
来源：http://ksw.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gpp.vehdjk.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kgo.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zmt.zdqjudy.top

TS:   arr[0]; arr.at(-1);
来源：http://cfd.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://oci.jianghu66.top

Go:   arr[0]; arr[0] = 9
来源：http://bfm.jqgufenzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ndc.hysaishi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bel.aibaodan.cn

[D06] 数组长度
来源：http://ntm.xylfe.cn

Py:   len(arr)
来源：http://ukv.jinqigfzy.top

PHP:  count($arr);
来源：http://pnr.nwbrower.top

JS:   arr.length
来源：http://jab.shanyushiyangkeji.top

TS:   arr.length
来源：http://osk.yfazqb.com

Java: list.size();
来源：http://doi.dashuyun.cn

Go:   len(arr)
来源：http://ikt.hongshengwenyu.top

Ruby: arr.length; arr.size
来源：http://yva.ydzc1.top

C#:   list.Count;
来源：http://dtx.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://vhj.yvedp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://iru.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://xvk.ydjk.org.cn

JS:   arr.slice(1, 4);
来源：http://jmi.yueranfly.top

TS:   arr.slice(1, 4);
来源：http://txn.xuanzx.com

Java: list.subList(1, 4);
来源：http://kon.0kj1m.cn

Go:   arr[1:4]
来源：http://vys.andypj.xyz

Ruby: arr[1, 3]
来源：http://nhj.yj20258888.top

C#:   list.GetRange(1, 3);
来源：http://lfz.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://bdl.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://zjc.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://iar.ydzc1.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qjg.fanxiaobao.xyz

TS:   [...a, ...b];
来源：http://slz.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hio.jyoumei.cn

Go:   append(a, b...)
来源：http://gkj.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://izp.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://nyl.smart0.xyz

[D09] 排序（升序）
来源：http://nnd.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://klg.ydjk.org.cn

PHP:  sort($arr);
来源：http://axi.xuetiantiany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ype.cdnleiting.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://quw.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://vgz.chenjidiqi.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lwv.dashuyun.cn

Ruby: arr.sort
来源：http://rem.xuanzx.com

C#:   list.Sort();
来源：http://ezn.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zto.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://owc.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nmn.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cxz.9152youxi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rqs.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yob.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fxy.ydzc1.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dim.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zzr.fehbvm.com

[D11] 反转数组
来源：http://hob.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://jly.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://rvf.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ooy.yongpay.top

TS:   [...arr].reverse();
来源：http://kze.gaohongyu789.top

Java: Collections.reverse(list);
来源：http://pqy.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://lyr.sxryk.cn

Ruby: arr.reverse
来源：http://rgj.mhx1999.top

C#:   list.Reverse();
来源：http://bwr.shzxlz.cn

[D12] 查找元素下标
来源：http://ovt.ywan-chungtsiang.top

Py:   arr.index(x);  x in arr
来源：http://wxd.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yvc.shangyingyoupin.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://edx.0kj1m.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sln.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ciu.feifeiyinyue.top

Go:   slices.Index(arr, x)
来源：http://pcm.zycfv.cn

Ruby: arr.index(x)
来源：http://dmx.smart0.xyz

C#:   list.IndexOf(x);
来源：http://yqm.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://mom.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wvj.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lzk.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://wct.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://srv.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gju.gzhubu.top


<!-- 参考信息 -->