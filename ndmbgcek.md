代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://ubj.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://bkt.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zfq.bbcook.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mec.yvedp.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vpu.aibaodan.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://thc.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zty.yvedp.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zea.yongpay.top

[B13] 判断是否为数字
来源：http://crl.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://bjo.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://bzt.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uoa.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://len.fengsongda.top

Java: x instanceof Number
来源：http://ppd.ydzc1.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pck.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://rkl.ehwqpu.com

C#:   x is int or double or decimal
来源：http://tbv.yongpay.top

[B14] 判断值是否在集合内
来源：http://csz.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ecr.meibo888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://upc.yongpay.top

JS:   [1, 2, 3].includes(x)
来源：http://jgs.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://epv.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fmq.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wvu.yj20258.top

Ruby: [1, 2, 3].include?(x)
来源：http://oxg.yuanzhike.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mdv.shanyushiyangkeji.top

[B15] 布尔运算与取反
来源：http://esg.sxryk.cn

Py:   a and b or not c
来源：http://bfv.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://vul.hywenlv.cn

JS:   a && b || !c
来源：http://afq.yj20258888.top

TS:   a && b || !c
来源：http://olh.fanxiaobao.xyz

Java: a && b || !c
来源：http://xzk.zdqjudy.top

Go:   a && b || !c
来源：http://wzh.redwolf501.top

Ruby: a && b || !c
来源：http://rji.quarkkingdee.top

C#:   a && b || !c
来源：http://kvd.ppjwa.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ynz.fanxiaobao.xyz

Py:   if not data: return
来源：http://vjc.yanxiufei.cn

PHP:  if (!$data) { return; }
来源：http://nzc.zhixingplan.top

JS:   if (!data) return;
来源：http://zih.cashguo.top

TS:   if (!data) return;
来源：http://fzk.guowangkeji.top

Java: if (data == null) return;
来源：http://van.xziqi.cn

Go:   if data == nil { return }
来源：http://xvg.jqgfzy.top

Ruby: return if data.nil?
来源：http://zgq.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://ovy.yongpay.top

================================================================================
来源：http://fli.mhx1999.top

C. 函数与作用域
来源：http://ikp.pycfn.com

================================================================================
来源：http://tsl.gotoacloud.top

[C01] 定义函数
来源：http://fdv.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://her.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xmk.iojbl.cn

JS:   function add(a, b) { return a + b; }
来源：http://kse.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ole.gzhubu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tbt.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://wvo.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://nrp.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dlm.xziqi.cn

[C02] 默认参数
来源：http://elu.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://kcr.zhaomingkeji.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://kum.tarul.cn

JS:   function greet(name = "World") { return name; }
来源：http://xwy.hongshengwenyu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kne.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://oug.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qzo.shangyingyoupin.top

Ruby: def greet(name = "World") = name
来源：http://wxb.dianchejie.cn

C#:   string Greet(string name = "World") => name;
来源：http://mlm.snrcjt.cn

[C03] 可变参数
来源：http://udn.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://ijy.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gtp.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nmu.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rra.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zcs.xziqi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tdb.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://ayl.haohaochexian.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://foe.jyoumei.cn

[C04] 命名参数 / 关键字参数
来源：http://cqq.hywenlv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oxb.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vnn.fengsongda.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fec.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rnw.andypj.xyz

Java: // 无：用 Builder 模式或 record
来源：http://jig.cashguo.top

Go:   // 无：用配置结构体参数
来源：http://fzh.zhaomingkeji.xyz

Ruby: f(a: 1, b: 2)
来源：http://qfh.fanxiaobao.xyz

C#:   f(a: 1, b: 2)
来源：http://kre.bjfxy.top

[C05] 返回多个值
来源：http://toj.yuxming.cn

Py:   return a, b
来源：http://xsg.gaohongyu789.top

PHP:  return [$a, $b];
来源：http://stn.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://aog.tarul.cn

TS:   return { a, b };
来源：http://sbi.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xtn.pycfn.com

Go:   return a, b
来源：http://naw.nanxinkj.top

Ruby: return a, b
来源：http://gmw.9152youxi.cn

C#:   return (a, b);              // ValueTuple
来源：http://fjd.yvedp.cn

[C06] 匿名函数 / lambda
来源：http://fxg.yangfankeji.com

Py:   square = lambda x: x * x
来源：http://dnp.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wnt.dashuyun.cn

JS:   const square = x => x * x;
来源：http://mlc.zhiwuduotai.top

TS:   const square = (x: number): number => x * x;
来源：http://fsp.ywan-chungtsiang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yyd.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://hde.svipenyu.cn

Ruby: square = ->(x) { x * x }
来源：http://frh.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://wbu.cashguo.top

[C07] 把函数作为参数传入
来源：http://lun.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nvh.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pus.wangshuangyany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hwy.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://egv.hesvh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://etm.sxryk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ysz.yfazqb.com

Ruby: arr.map(&:upcase)
来源：http://gdh.hongshengwenyu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gve.uphjek.com

[C08] 闭包
来源：http://onj.c1oappe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://oqd.redwolf501.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uvg.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hog.quarkkingdee.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mmo.uphjek.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://njo.jinghuilouyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cdb.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://auy.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vdw.zhengqikj.top

[C09] 递归
来源：http://rng.jqgufenzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xof.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ssf.xylfe.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sns.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gnk.yj20258888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ixk.xuanzx.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ekj.shuidangran.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vot.shzxlz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rch.yuxming.cn

[C10] 变量作用域
来源：http://sev.sysykeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kwq.shuidangran.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vet.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fua.cheryme.top

TS:   同 JS
来源：http://byg.ctjpmb.com

Java: 方法内为块级作用域
来源：http://zyy.chenzaomai.com

Go:   花括号块级作用域
来源：http://udm.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kyt.vehdjk.com

C#:   块级作用域
来源：http://qzx.chenjidiqi.icu

[C11] 模块导入与导出
来源：http://ivf.uphjek.com

Py:   from module import func
来源：http://ude.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://eol.yj20258888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wxk.redwolf501.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qjx.redwolf501.top

Java: import java.util.List;
来源：http://txv.uphjek.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mtz.hongshengwenyu.top

Ruby: require "json"; require_relative "./util"
来源：http://yzg.feifeiyinyue.top

C#:   using System.Text;
来源：http://xqg.jinyuanbaomall.cn

[C12] 立即执行函数 IIFE
来源：http://ypf.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://ule.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://qyi.dianchejie.cn

JS:   (() => { console.log("run"); })();
来源：http://esh.ivvv.top

TS:   (() => { console.log("run"); })();
来源：http://xjg.sxryk.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jah.shanyushiyangkeji.top

Go:   func() { fmt.Println("run") }()
来源：http://byt.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://hri.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jmt.sysykeji.top

[C13] 类型声明 / 类型注解
来源：http://ieh.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xmb.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hou.wangdashe.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://srr.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qsd.mhx1999.top

Java: int add(int a, int b) { return a + b; }
来源：http://mfz.shanyushiyangtech.top

Go:   func add(a, b int) int
来源：http://iux.yvedp.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kxe.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://jyo.tarul.cn

[C14] 泛型函数
来源：http://gvw.chenlongwang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://syp.uphjek.com

PHP:  // 无泛型
来源：http://ckq.bbcook.cn

JS:   // 无泛型
来源：http://uem.yj20258888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xxx.316326.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lnk.tian-w.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bpw.316326.xyz

Ruby: # 无泛型
来源：http://lku.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pxe.zhengqikj.top

[C15] 解构 / 展开参数
来源：http://rmo.iojbl.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vpv.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://udt.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qpq.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cea.pycfn.com

Java: // 无解构
来源：http://gab.ehwqpu.com

Go:   // 无解构
来源：http://wgt.nwbrower.top

Ruby: a, b = pair
来源：http://mob.jinqigufen.top

C#:   var (a, b) = pair;
来源：http://ymy.yuxming.cn

[C16] 函数 / 方法重载
来源：http://uiv.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wdn.yongpay.top

PHP:  // 无重载
来源：http://sku.zhaomingkeji.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://fzt.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://omi.daxiang520.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ubh.xingfuxueyuan.xyz

Go:   // 无重载：用不同函数名
来源：http://azh.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://tlb.jqgfzy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jtj.shangyingyoupin.top

================================================================================
来源：http://mcp.aizwys.cn

D. 数组 / 列表 / 集合
来源：http://gad.zhiwuduotai.top

================================================================================
来源：http://eod.gaohongyu789.top

[D01] 创建数组 / 列表
来源：http://wma.hnxiangtu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ctr.cucudq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hhq.snrcjt.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lhk.jqgfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lhz.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oww.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://asc.smart0.xyz

Ruby: arr = [1, 2, 3]
来源：http://kvj.jianghu66.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jll.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://uwz.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://orn.nanxuanxn.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uew.fehbvm.com

JS:   arr.push(4);
来源：http://lao.zdbjq.cn

TS:   arr.push(4);
来源：http://mql.ywan-chungtsiang.top

Java: list.add(4);
来源：http://yvb.shangyingyoupin.top

Go:   arr = append(arr, 4)
来源：http://qlw.aizwys.cn

Ruby: arr << 4; arr.push(5)
来源：http://fzn.yangfankeji.com

C#:   list.Add(4);
来源：http://itq.jianghu66.top

[D03] 在指定位置插入元素
来源：http://drg.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://btm.yongpay.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wol.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mee.fengsongda.top

TS:   arr.splice(0, 0, 0);
来源：http://zpi.ctjpmb.com

Java: list.add(0, 0);
来源：http://snf.xinyue.icu

Go:   arr = append([]int{0}, arr...)
来源：http://dku.zdqjudy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cfb.zhiwuduotai.top

C#:   list.Insert(0, 0);
来源：http://jff.sweek.top

[D04] 删除元素
来源：http://fhg.shzxlz.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pob.yvedp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jrb.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rnc.kuanghao11.cn

TS:   arr.splice(0, 1);
来源：http://jhl.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gxx.hcnkem.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ahm.andypj.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rbe.yanxiufei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xiy.hnqzz.top

[D05] 访问与修改元素
来源：http://psc.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kxh.jinghuilouyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ofa.tarul.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ffg.tian-w.cn

TS:   arr[0]; arr.at(-1);
来源：http://osb.haohaochexian.top

Java: list.get(0); list.set(0, 9);
来源：http://ois.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://ycs.zhaomingkeji.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ghq.zhixingplan.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ygk.shangyingyoupin.top

[D06] 数组长度
来源：http://jlh.redwolf501.top

Py:   len(arr)
来源：http://zax.yongpay.top

PHP:  count($arr);
来源：http://hvt.sweek.top

JS:   arr.length
来源：http://gdq.yuxming.cn

TS:   arr.length
来源：http://zvr.iojbl.cn

Java: list.size();
来源：http://wak.aibaodan.cn

Go:   len(arr)
来源：http://bjz.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://whf.yj202588.top

C#:   list.Count;
来源：http://uwj.zhoulong.xyz

[D07] 切片 / 取子数组
来源：http://upe.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rix.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://acf.haohaochexian.top

JS:   arr.slice(1, 4);
来源：http://fin.havefunace.top

TS:   arr.slice(1, 4);
来源：http://aaw.pycfn.com

Java: list.subList(1, 4);
来源：http://hch.jqgfzy.top

Go:   arr[1:4]
来源：http://eeu.fktsv.cn

Ruby: arr[1, 3]
来源：http://sof.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://udk.andypj.xyz

[D08] 合并两个数组
来源：http://etq.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://vxo.nanxinkj.top

PHP:  array_merge($a, $b);
来源：http://jlq.redwolf501.top

JS:   [...a, ...b];  a.concat(b);
来源：http://yxb.chenzaomai.com

TS:   [...a, ...b];
来源：http://yvp.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hwv.52xcode.cn

Go:   append(a, b...)
来源：http://wqr.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://mdj.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://hel.zdqjudy.top

[D09] 排序（升序）
来源：http://rcy.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://lnk.kuanghao11.cn

PHP:  sort($arr);
来源：http://bit.ctjpmb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kyz.jinghuilouyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://coo.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oex.c1oappe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gni.0kj1m.cn

Ruby: arr.sort
来源：http://fuw.kuanghao11.cn

C#:   list.Sort();
来源：http://dpw.snrcjt.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fnz.0kj1m.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ccn.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://axr.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://srh.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aad.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fnm.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uum.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jws.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mal.daxiang520.top

[D11] 反转数组
来源：http://rgk.cdnleiting.top

Py:   arr[::-1];  arr.reverse()
来源：http://tux.sjlbkw.cn

PHP:  array_reverse($arr);
来源：http://jlb.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vtt.smart0.xyz

TS:   [...arr].reverse();
来源：http://jqi.yuxming.cn

Java: Collections.reverse(list);
来源：http://aqi.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://yvh.cashguo.top

Ruby: arr.reverse
来源：http://ial.zhixingplan.top

C#:   list.Reverse();
来源：http://usn.havefunace.top

[D12] 查找元素下标
来源：http://ekm.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://uiq.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://frn.sweek.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uqn.vehdjk.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tme.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vas.xziqi.cn

Go:   slices.Index(arr, x)
来源：http://ddk.tarul.cn


<!-- 参考信息 -->