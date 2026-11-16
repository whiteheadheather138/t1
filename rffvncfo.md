代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qhx.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://vuk.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lce.ydjk.org.cn

[B12] 跳出多层循环
来源：http://duh.zhijiandao.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://afk.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vsj.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ahp.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ksh.fengsongda.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tyz.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tfa.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hbi.redwolf501.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kbn.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://jys.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://jkq.316326.xyz

PHP:  is_numeric($x)
来源：http://wrx.guowangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zqv.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sla.gaohongyu789.top

Java: x instanceof Number
来源：http://idc.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xxx.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://npb.zdqjudy.top

C#:   x is int or double or decimal
来源：http://nzb.yj20258.top

[B14] 判断值是否在集合内
来源：http://cez.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ssf.zhengqikj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://utb.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://zzp.yuanzhike.top

TS:   [1, 2, 3].includes(x)
来源：http://lzt.chenzaomai.com

Java: List.of(1, 2, 3).contains(x)
来源：http://sjc.sxryk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qmj.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gte.c1oappe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://upj.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://xom.nanxuanxn.top

Py:   a and b or not c
来源：http://zdk.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://kpy.ydzc1.top

JS:   a && b || !c
来源：http://lyz.yongpay.top

TS:   a && b || !c
来源：http://dst.zycfv.cn

Java: a && b || !c
来源：http://klh.pengpengdd.cyou

Go:   a && b || !c
来源：http://ynj.gaohongyu789.top

Ruby: a && b || !c
来源：http://fdi.c1oappe.top

C#:   a && b || !c
来源：http://wxf.xziqi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ijx.tanke756.top

Py:   if not data: return
来源：http://zpa.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://ien.hongshengwenyu.top

JS:   if (!data) return;
来源：http://thc.tarul.cn

TS:   if (!data) return;
来源：http://yck.daria6918.cn

Java: if (data == null) return;
来源：http://isn.jqgufenzy.top

Go:   if data == nil { return }
来源：http://nki.zhixingplan.top

Ruby: return if data.nil?
来源：http://orw.yuanzhike.top

C#:   if (data == null) return;
来源：http://vuz.yj202588.top

================================================================================
来源：http://gny.zhongyouzk.top

C. 函数与作用域
来源：http://ffv.shanyushiyangtech.top

================================================================================
来源：http://hld.fengsongda.top

[C01] 定义函数
来源：http://dco.zhixingplan.top

Py:   def add(a, b): return a + b
来源：http://egy.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xai.hysaishi.cn

JS:   function add(a, b) { return a + b; }
来源：http://xnv.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mfh.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://uwj.svipenyu.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rxz.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://jgh.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ynq.sweek.top

[C02] 默认参数
来源：http://fsf.jianghu66.top

Py:   def greet(name="World"): return name
来源：http://oil.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://nuy.fehbvm.com

JS:   function greet(name = "World") { return name; }
来源：http://cvs.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kwh.hnqzz.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ewc.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xto.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://zwx.gotoacloud.top

C#:   string Greet(string name = "World") => name;
来源：http://qsj.hesvh.cn

[C03] 可变参数
来源：http://ygv.hnxiangtu.top

Py:   def total(*args): return sum(args)
来源：http://hiq.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eqe.jianghu66.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cwc.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zgo.xuanzx.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ayg.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bwo.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://mhu.jyoumei.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nwz.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://dyy.epnwcf.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kzy.sjlbkw.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dgj.feifeiyinyue.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fhi.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qkz.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://gvh.chenjidiqi.icu

Go:   // 无：用配置结构体参数
来源：http://itn.hesvh.cn

Ruby: f(a: 1, b: 2)
来源：http://akc.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://rat.yangfankeji.com

[C05] 返回多个值
来源：http://lrb.hnqzz.top

Py:   return a, b
来源：http://qof.fanxiaobao.xyz

PHP:  return [$a, $b];
来源：http://lvy.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://yhg.hysaishi.cn

TS:   return { a, b };
来源：http://lof.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xxr.sysykeji.top

Go:   return a, b
来源：http://zhs.jlsjyb.cn

Ruby: return a, b
来源：http://jki.dianchejie.cn

C#:   return (a, b);              // ValueTuple
来源：http://fxf.chenzaomai.com

[C06] 匿名函数 / lambda
来源：http://xwc.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://qjo.iojbl.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wyz.haohaochexian.top

JS:   const square = x => x * x;
来源：http://aew.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://nag.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uoy.bbcook.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fjb.cashguo.top

Ruby: square = ->(x) { x * x }
来源：http://vwj.yvedp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mlj.bjfxy.top

[C07] 把函数作为参数传入
来源：http://iqq.fktsv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bkg.andypj.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://qms.yvedp.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://grr.hnqzz.top

TS:   arr.map(String)
来源：http://gfq.fengsongda.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sfg.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xqp.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://qxz.ydzc1.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wph.zhoulong.xyz

[C08] 闭包
来源：http://gfq.chenzaomai.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ghc.ydjk.org.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hwh.zhijiandao.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bqc.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ctp.yj20258.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gma.nanxinkj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://idr.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nry.hnqzz.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jub.ybcxt.top

[C09] 递归
来源：http://nmh.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://esz.ydjk.org.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qey.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oce.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hzn.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://krc.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hit.uphjek.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kwi.shuidangran.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pdp.zhengqikj.top

[C10] 变量作用域
来源：http://bbb.zhoulong.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hvd.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vxh.vqdsnc.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tki.chenlongwang.top

TS:   同 JS
来源：http://lql.nanxuanxn.top

Java: 方法内为块级作用域
来源：http://jzu.xylfe.cn

Go:   花括号块级作用域
来源：http://pgr.zhijiandao.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xkc.jqgufenzy.top

C#:   块级作用域
来源：http://wuf.yueranfly.top

[C11] 模块导入与导出
来源：http://iud.yonumen.top

Py:   from module import func
来源：http://hui.snrcjt.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cbv.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://jhw.chenjidiqi.icu

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ocd.birdmap.top

Java: import java.util.List;
来源：http://uvk.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eeh.yj20258888.top

Ruby: require "json"; require_relative "./util"
来源：http://qdh.yongpay.top

C#:   using System.Text;
来源：http://eot.shzxlz.cn

[C12] 立即执行函数 IIFE
来源：http://cgb.ivvv.top

Py:   (lambda: print("run"))()
来源：http://ite.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://oix.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://ury.yanxiufei.cn

TS:   (() => { console.log("run"); })();
来源：http://kod.jinqigufen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eob.hammf.cn

Go:   func() { fmt.Println("run") }()
来源：http://fzk.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://sfh.ivvv.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jsm.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://msr.yuanzhike.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lhe.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://okc.zhijiandao.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gst.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://asv.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://gux.aizwys.cn

Go:   func add(a, b int) int
来源：http://wwy.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pat.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://pvd.fengsongda.top

[C14] 泛型函数
来源：http://fxg.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://die.ivvv.top

PHP:  // 无泛型
来源：http://nom.daria6918.cn

JS:   // 无泛型
来源：http://jjq.uphjek.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pcm.shanyushiyangkeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zvh.chenlongwang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fko.tian-w.cn

Ruby: # 无泛型
来源：http://tdp.gotoacloud.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://owm.aibaodan.cn

[C15] 解构 / 展开参数
来源：http://lcn.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ukr.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://eaa.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jbx.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ghk.hesvh.cn

Java: // 无解构
来源：http://xnl.yueranfly.top

Go:   // 无解构
来源：http://qkl.yueranfly.top

Ruby: a, b = pair
来源：http://czf.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://poy.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://eig.birdmap.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lte.ctjpmb.com

PHP:  // 无重载
来源：http://ezc.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vyc.daxiang520.top

TS:   // 用联合类型或重载签名声明
来源：http://kqg.uphjek.com

Java: void f(int a) {}  void f(String a) {}
来源：http://gvp.yj20258888.top

Go:   // 无重载：用不同函数名
来源：http://ftj.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://zqf.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yds.zhijiandao.cn

================================================================================
来源：http://eoa.gotoacloud.top

D. 数组 / 列表 / 集合
来源：http://ige.cheryme.top

================================================================================
来源：http://skj.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://pdf.xingfuxueyuan.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://gkn.hcnkem.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://teb.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vkx.chenzaomai.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://iva.andypj.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://twm.zhaomingkeji.xyz

Go:   arr := []int{1, 2, 3}
来源：http://rwn.yj20258.top

Ruby: arr = [1, 2, 3]
来源：http://sua.cucudq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://goj.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://vtr.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://axa.shanyushiyangtech.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xkh.pengpengdd.cyou

JS:   arr.push(4);
来源：http://czs.jlsjyb.cn

TS:   arr.push(4);
来源：http://erh.guowangkeji.top

Java: list.add(4);
来源：http://gzq.shanyushiyangtech.top

Go:   arr = append(arr, 4)
来源：http://lvx.svipenyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://ycs.yanxiufei.cn

C#:   list.Add(4);
来源：http://egh.ydzc1.top

[D03] 在指定位置插入元素
来源：http://tzt.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://erd.pengpengdd.cyou

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fmi.zdbjq.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wru.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://wsj.meibo888.top

Java: list.add(0, 0);
来源：http://vwz.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ica.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wmq.zhongyouzk.top

C#:   list.Insert(0, 0);
来源：http://zgp.yj20258888.top

[D04] 删除元素
来源：http://tsf.zhiwuduotai.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xbv.ywan-chungtsiang.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wnj.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qdc.meibo888.top

TS:   arr.splice(0, 1);
来源：http://dpk.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cdd.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ozu.yj20258888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pod.hammf.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xqy.ydjk.org.cn

[D05] 访问与修改元素
来源：http://rma.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nfj.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tzf.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pyy.cheryme.top

TS:   arr[0]; arr.at(-1);
来源：http://qjc.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://dzt.ehwqpu.com

Go:   arr[0]; arr[0] = 9
来源：http://ega.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wok.kuanghao11.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jsm.c1oappe.top

[D06] 数组长度
来源：http://yez.yueranfly.top

Py:   len(arr)
来源：http://mbn.jqgfzy.top

PHP:  count($arr);
来源：http://ska.shanyushiyangkeji.top

JS:   arr.length
来源：http://odj.wangdashe.top

TS:   arr.length
来源：http://bil.hcnkem.com

Java: list.size();
来源：http://xud.nwbrower.top

Go:   len(arr)
来源：http://spt.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://plx.fanxiaobao.xyz

C#:   list.Count;
来源：http://ybj.yj202588.top

[D07] 切片 / 取子数组
来源：http://otu.xingfuxueyuan.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hkm.wangshuangyany.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zmd.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://fsc.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://txm.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://uai.jinyuanbaomall.cn

Go:   arr[1:4]
来源：http://lxy.sxryk.cn

Ruby: arr[1, 3]
来源：http://zru.tianlin.xyz

C#:   list.GetRange(1, 3);
来源：http://ooz.jinqigfzy.top

[D08] 合并两个数组
来源：http://yzu.bbcook.cn

Py:   a + b;  a.extend(b)
来源：http://qhb.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://zzw.0kj1m.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fkz.aibaodan.cn

TS:   [...a, ...b];
来源：http://vpa.ydjk.org.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iwo.sweek.top

Go:   append(a, b...)
来源：http://rik.52xcode.cn

Ruby: a + b;  a.concat(b)
来源：http://ysr.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://vnk.chenlongwang.top

[D09] 排序（升序）
来源：http://nza.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://koq.aizwys.cn

PHP:  sort($arr);
来源：http://dar.cdnleiting.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://omp.yueranfly.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tiq.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mws.pycfn.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pgw.snrcjt.cn

Ruby: arr.sort
来源：http://bbb.wangshuangyany.cn

C#:   list.Sort();
来源：http://iyz.shangyingyoupin.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bhn.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lij.mhx1999.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mmd.yj202588.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dbc.vqdsnc.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wpi.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xlo.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fef.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hqv.shanyushiyangtech.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dpk.fengsongda.top

[D11] 反转数组
来源：http://rdj.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://uvn.tian-w.cn

PHP:  array_reverse($arr);
来源：http://dwv.haohaochexian.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nzj.cheryme.top

TS:   [...arr].reverse();
来源：http://vgl.mhx1999.top

Java: Collections.reverse(list);
来源：http://dyf.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://mdn.jyoumei.cn

Ruby: arr.reverse
来源：http://ida.hnxiangtu.top

C#:   list.Reverse();
来源：http://xui.aizwys.cn

[D12] 查找元素下标
来源：http://wdm.zhongyouzk.top

Py:   arr.index(x);  x in arr
来源：http://qcp.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://csr.jinghuilouyu.cn


<!-- 参考信息 -->