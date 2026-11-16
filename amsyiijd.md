代发 wailian999

PHP:  range(0, 10, 2);
来源：http://soh.nanxinkj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dic.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lyp.nanxinkj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dhy.shangyingyoupin.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://awf.quarkkingdee.top

Ruby: (0...10).step(2).to_a
来源：http://odq.nanxinkj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dwx.smart0.xyz

[B12] 跳出多层循环
来源：http://pzm.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ayq.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://ctv.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tso.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dfu.fengsongda.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://doa.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://usf.yfazqb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yss.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kmt.yuanzhike.top

[B13] 判断是否为数字
来源：http://lph.zhengqikj.top

Py:   isinstance(x, (int, float))
来源：http://rww.yuanzhike.top

PHP:  is_numeric($x)
来源：http://suf.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fyy.havefunace.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nmk.gaohongyu789.top

Java: x instanceof Number
来源：http://dhl.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jho.vqdsnc.cn

Ruby: x.is_a?(Numeric)
来源：http://gun.xuanzx.com

C#:   x is int or double or decimal
来源：http://rar.zhiwuduotai.top

[B14] 判断值是否在集合内
来源：http://goy.andypj.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zop.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kbx.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://qwq.shanyushiyangkeji.top

TS:   [1, 2, 3].includes(x)
来源：http://zze.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tfs.yuxming.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rms.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://cil.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fhv.ybcxt.top

[B15] 布尔运算与取反
来源：http://ysf.cdnleiting.top

Py:   a and b or not c
来源：http://ljn.haohaochexian.top

PHP:  $a && $b || !$c
来源：http://ndx.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://dgc.uphjek.com

TS:   a && b || !c
来源：http://ucp.birdmap.top

Java: a && b || !c
来源：http://yfp.pengpengdd.cyou

Go:   a && b || !c
来源：http://ebi.guowangkeji.top

Ruby: a && b || !c
来源：http://dtj.tian-w.cn

C#:   a && b || !c
来源：http://uti.dashuyun.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lfp.cqqwz.cn

Py:   if not data: return
来源：http://maw.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://dua.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://eci.hongshengwenyu.top

TS:   if (!data) return;
来源：http://sfi.nwbrower.top

Java: if (data == null) return;
来源：http://fzx.birdmap.top

Go:   if data == nil { return }
来源：http://wjb.wangdashe.top

Ruby: return if data.nil?
来源：http://qgv.yanxiufei.cn

C#:   if (data == null) return;
来源：http://ufd.ctjpmb.com

================================================================================
来源：http://qws.ctjpmb.com

C. 函数与作用域
来源：http://xwy.uphjek.com

================================================================================
来源：http://bpl.jqgufenzy.top

[C01] 定义函数
来源：http://zzb.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://ema.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tnx.daria6918.cn

JS:   function add(a, b) { return a + b; }
来源：http://cau.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dct.zhixingplan.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sfx.smart0.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://psl.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://til.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lhb.ybcxt.top

[C02] 默认参数
来源：http://grk.tian-w.cn

Py:   def greet(name="World"): return name
来源：http://nzt.fktsv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lpn.ywan-chungtsiang.top

JS:   function greet(name = "World") { return name; }
来源：http://tqo.xylfe.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yrc.kuanghao11.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wuf.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ufs.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://voj.quarkkingdee.top

C#:   string Greet(string name = "World") => name;
来源：http://eub.yfazqb.com

[C03] 可变参数
来源：http://ylt.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://hfx.shzxlz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ctj.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rmu.jqgfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ore.jinqigfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iin.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zop.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://vlf.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://opb.zhoulong.xyz

[C04] 命名参数 / 关键字参数
来源：http://xsj.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bwm.guannengcc.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rom.redwolf501.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hnd.dashuyun.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eok.0kj1m.cn

Java: // 无：用 Builder 模式或 record
来源：http://pxq.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://eaw.nanxinkj.top

Ruby: f(a: 1, b: 2)
来源：http://dkb.nanxinkj.top

C#:   f(a: 1, b: 2)
来源：http://ncy.jlsjyb.cn

[C05] 返回多个值
来源：http://mox.quarkkingdee.top

Py:   return a, b
来源：http://lvb.zhongyouzk.top

PHP:  return [$a, $b];
来源：http://vhv.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jca.sufxvd.cn

TS:   return { a, b };
来源：http://pli.yvedp.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fhk.ywan-chungtsiang.top

Go:   return a, b
来源：http://nar.jinyuanbaomall.cn

Ruby: return a, b
来源：http://ctz.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://cko.fzhhl.top

[C06] 匿名函数 / lambda
来源：http://eju.aibaodan.cn

Py:   square = lambda x: x * x
来源：http://vgt.jqgfzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cbn.c1oappe.top

JS:   const square = x => x * x;
来源：http://ptt.yongpay.top

TS:   const square = (x: number): number => x * x;
来源：http://vpd.hnqzz.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sgi.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://ild.xinyue.icu

Ruby: square = ->(x) { x * x }
来源：http://sbo.jianghu66.top

C#:   Func<int, int> square = x => x * x;
来源：http://sit.gzhubu.top

[C07] 把函数作为参数传入
来源：http://toq.yj20258.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://thb.pengpengdd.cyou

PHP:  array_map("strtoupper", $arr);
来源：http://rzm.hfpthk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oqe.smart0.xyz

TS:   arr.map(String)
来源：http://mfn.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nfs.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://onr.jyoumei.cn

Ruby: arr.map(&:upcase)
来源：http://fps.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://asj.daria6918.cn

[C08] 闭包
来源：http://ydx.xingfuxueyuan.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://npo.zhoulong.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ypw.chenjidiqi.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bwl.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://szy.xuanzx.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hso.pengpengdd.cyou

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pwf.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kki.cdnleiting.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ejj.ydzc1.top

[C09] 递归
来源：http://toq.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gyt.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://akg.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oih.ybcxt.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jic.dashuyun.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yzf.jianghu66.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xdp.ctjpmb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qxq.sysykeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ehj.haohaochexian.top

[C10] 变量作用域
来源：http://yug.zdqjudy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wmq.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hwp.jinyuanbaomall.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ucz.hongshengwenyu.top

TS:   同 JS
来源：http://hvf.quarkkingdee.top

Java: 方法内为块级作用域
来源：http://rht.zdbjq.cn

Go:   花括号块级作用域
来源：http://lid.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aiz.fehbvm.com

C#:   块级作用域
来源：http://bul.ybcxt.top

[C11] 模块导入与导出
来源：http://gvx.gzhubu.top

Py:   from module import func
来源：http://hkp.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vhg.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mjr.fzhhl.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fsb.nwbrower.top

Java: import java.util.List;
来源：http://dyw.yj20258888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pii.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://vco.ydjk.org.cn

C#:   using System.Text;
来源：http://deo.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://cix.52xcode.cn

Py:   (lambda: print("run"))()
来源：http://qec.birdmap.top

PHP:  (function () { echo "run"; })();
来源：http://wyx.vqdsnc.cn

JS:   (() => { console.log("run"); })();
来源：http://rmg.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://mrf.vehdjk.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xyd.yj202588.top

Go:   func() { fmt.Println("run") }()
来源：http://lrb.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://xqn.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://opz.ybcxt.top

[C13] 类型声明 / 类型注解
来源：http://zpx.yongpay.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://asv.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nha.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yfx.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ypd.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qcm.feifeiyinyue.top

Go:   func add(a, b int) int
来源：http://izm.jqgfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wts.ehwqpu.com

C#:   int Add(int a, int b) => a + b;
来源：http://jia.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://prj.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pct.yuxming.cn

PHP:  // 无泛型
来源：http://lcd.feifeiyinyue.top

JS:   // 无泛型
来源：http://oqi.jinqigufen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jeb.jinghuilouyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qby.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://poc.jqgfzy.top

Ruby: # 无泛型
来源：http://gni.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kmb.cucudq.cn

[C15] 解构 / 展开参数
来源：http://bdl.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://phv.fengsongda.top

PHP:  [$a, $b] = $pair;
来源：http://wak.yuanzhike.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iep.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uzp.tianlin.xyz

Java: // 无解构
来源：http://kwk.zhongyouzk.top

Go:   // 无解构
来源：http://fuy.havefunace.top

Ruby: a, b = pair
来源：http://mcp.yj202588.top

C#:   var (a, b) = pair;
来源：http://cqm.tanke756.top

[C16] 函数 / 方法重载
来源：http://hpe.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mfi.sysykeji.top

PHP:  // 无重载
来源：http://jsy.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://oqo.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://nba.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://iml.chenjidiqi.icu

Go:   // 无重载：用不同函数名
来源：http://kdh.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://pdj.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zib.redwolf501.top

================================================================================
来源：http://umf.hongshengwenyu.top

D. 数组 / 列表 / 集合
来源：http://jdd.zhongyouzk.top

================================================================================
来源：http://qlm.tanke756.top

[D01] 创建数组 / 列表
来源：http://nai.pycfn.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://euk.dianchejie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://evb.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dmp.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xjx.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xiy.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://tgv.ppjwa.cn

Ruby: arr = [1, 2, 3]
来源：http://krv.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eby.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://ofg.chenjidiqi.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oyw.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kpy.xinyue.icu

JS:   arr.push(4);
来源：http://vnq.jiagoushi.top

TS:   arr.push(4);
来源：http://qrd.zhongyouzk.top

Java: list.add(4);
来源：http://nzc.sufxvd.cn

Go:   arr = append(arr, 4)
来源：http://hvt.fengsongda.top

Ruby: arr << 4; arr.push(5)
来源：http://jqe.ehwqpu.com

C#:   list.Add(4);
来源：http://vpi.snrcjt.cn

[D03] 在指定位置插入元素
来源：http://tij.xuetiantiany.cn

Py:   arr.insert(0, 0)
来源：http://tza.ydzc1.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wre.jiagoushi.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://emk.tianlin.xyz

TS:   arr.splice(0, 0, 0);
来源：http://qbu.c1oappe.top

Java: list.add(0, 0);
来源：http://ojz.zhijiandao.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ahz.tianlin.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ivw.bbcook.cn

C#:   list.Insert(0, 0);
来源：http://icc.cucudq.cn

[D04] 删除元素
来源：http://omx.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wbo.yanxiufei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tkq.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sqw.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://aun.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kbo.pycfn.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qdm.smart0.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fhq.chenlongwang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sld.9152youxi.cn

[D05] 访问与修改元素
来源：http://qpv.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wyl.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ypa.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dlj.jqgfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://yky.ybcxt.top

Java: list.get(0); list.set(0, 9);
来源：http://jpl.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://bjv.cheryme.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://csd.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blq.shanyushiyangtech.top

[D06] 数组长度
来源：http://iaz.yj202588.top

Py:   len(arr)
来源：http://fvl.xinyue.icu

PHP:  count($arr);
来源：http://dyq.wangshuangyany.cn

JS:   arr.length
来源：http://fzo.daxiang520.top

TS:   arr.length
来源：http://rvt.zhengqikj.top

Java: list.size();
来源：http://fjs.epnwcf.com

Go:   len(arr)
来源：http://lkd.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://mfs.yanxiufei.cn

C#:   list.Count;
来源：http://maw.xuanzx.com

[D07] 切片 / 取子数组
来源：http://jzb.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wqb.ywan-chungtsiang.top

PHP:  array_slice($arr, 1, 3);
来源：http://ikh.wangshuangyany.cn

JS:   arr.slice(1, 4);
来源：http://nhg.zhongyouzk.top

TS:   arr.slice(1, 4);
来源：http://din.nwbrower.top

Java: list.subList(1, 4);
来源：http://hkh.meibo888.top

Go:   arr[1:4]
来源：http://axr.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://xzz.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://yzf.epnwcf.com

[D08] 合并两个数组
来源：http://wti.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://lqe.ydjk.org.cn

PHP:  array_merge($a, $b);
来源：http://hdc.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mpr.cheryme.top

TS:   [...a, ...b];
来源：http://cfi.yueranfly.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bqu.chenzaomai.com

Go:   append(a, b...)
来源：http://jld.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://bof.nanxinkj.top

C#:   a.Concat(b).ToList()
来源：http://sgx.yvedp.cn

[D09] 排序（升序）
来源：http://xqt.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://vsm.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://ggm.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://plb.yongpay.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://axh.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vhj.feifeiyinyue.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ibn.feifeiyinyue.top

Ruby: arr.sort
来源：http://vok.aizwys.cn

C#:   list.Sort();
来源：http://itc.xuanzx.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://keo.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uoa.cashguo.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dqa.vehdjk.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iqb.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tdi.dianchejie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hjb.sufxvd.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cde.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://soy.zhaomingkeji.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yyk.nwbrower.top

[D11] 反转数组
来源：http://sfx.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://tji.kuanghao11.cn

PHP:  array_reverse($arr);
来源：http://maa.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lyl.shuidangran.top

TS:   [...arr].reverse();
来源：http://lys.cheryme.top

Java: Collections.reverse(list);
来源：http://vpp.havefunace.top

Go:   slices.Reverse(arr)
来源：http://pjk.cheryme.top

Ruby: arr.reverse
来源：http://nuu.ppjwa.cn


<!-- 参考信息 -->