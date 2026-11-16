代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aeb.dashuyun.cn

[B10] 遍历同时拿索引
来源：http://zpc.uphjek.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iqw.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dst.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ygt.shuidangran.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qlk.tianlin.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oin.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rnv.daria6918.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vif.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lqx.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://tfl.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://mwq.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://lzx.fktsv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://txd.nwbrower.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jsh.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vio.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nqj.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://wej.quarkkingdee.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hfe.epnwcf.com

[B12] 跳出多层循环
来源：http://xqs.yj20258888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vtg.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://usu.uphjek.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://afj.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://glz.yuxming.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ybb.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rpv.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pcw.redwolf501.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pgr.jlsjyb.cn

[B13] 判断是否为数字
来源：http://aon.yfazqb.com

Py:   isinstance(x, (int, float))
来源：http://vbd.zhongyouzk.top

PHP:  is_numeric($x)
来源：http://exa.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kwr.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tjs.gotoacloud.top

Java: x instanceof Number
来源：http://jor.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://crv.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://vao.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://usr.uphjek.com

[B14] 判断值是否在集合内
来源：http://qhq.andypj.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wwo.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gnz.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://acb.fengsongda.top

TS:   [1, 2, 3].includes(x)
来源：http://ggh.ivvv.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dsj.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zyw.sufxvd.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yfp.ppjwa.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xmm.yangfankeji.com

[B15] 布尔运算与取反
来源：http://vnx.vehdjk.com

Py:   a and b or not c
来源：http://ksf.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://voi.yfazqb.com

JS:   a && b || !c
来源：http://ecz.sysykeji.top

TS:   a && b || !c
来源：http://uqr.snrcjt.cn

Java: a && b || !c
来源：http://swl.chenjidiqi.icu

Go:   a && b || !c
来源：http://rzs.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://piw.jlsjyb.cn

C#:   a && b || !c
来源：http://uqr.zhiwuduotai.top

[B16] 卫语句：不满足条件提前返回
来源：http://zma.dianchejie.cn

Py:   if not data: return
来源：http://knk.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://qxy.yangfankeji.com

JS:   if (!data) return;
来源：http://coo.fzhhl.top

TS:   if (!data) return;
来源：http://nwb.ehwqpu.com

Java: if (data == null) return;
来源：http://gxq.pycfn.com

Go:   if data == nil { return }
来源：http://tae.pycfn.com

Ruby: return if data.nil?
来源：http://ypc.xuanzx.com

C#:   if (data == null) return;
来源：http://skd.ybcxt.top

================================================================================
来源：http://ieu.xylfe.cn

C. 函数与作用域
来源：http://qzh.daria6918.cn

================================================================================
来源：http://pzx.zhiwuduotai.top

[C01] 定义函数
来源：http://jis.chenjidiqi.icu

Py:   def add(a, b): return a + b
来源：http://bgy.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gem.pycfn.com

JS:   function add(a, b) { return a + b; }
来源：http://sup.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tbx.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://lcj.shuidangran.top

Go:   func add(a, b int) int { return a + b }
来源：http://twh.bbcook.cn

Ruby: def add(a, b); a + b; end
来源：http://bon.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wxk.gzhubu.top

[C02] 默认参数
来源：http://bfi.ydzc1.top

Py:   def greet(name="World"): return name
来源：http://pdc.xziqi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hqh.daxiang520.top

JS:   function greet(name = "World") { return name; }
来源：http://yzp.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://ngu.cqqwz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ole.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://scy.xinyue.icu

Ruby: def greet(name = "World") = name
来源：http://ajd.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://pkh.aizwys.cn

[C03] 可变参数
来源：http://ysw.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://rgs.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iij.epnwcf.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wdk.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fsm.dashuyun.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aoo.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://itv.gaohongyu789.top

Ruby: def total(*nums); nums.sum; end
来源：http://skf.nanxuanxn.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lhz.fktsv.cn

[C04] 命名参数 / 关键字参数
来源：http://hmu.pycfn.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vdw.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pxs.haohaochexian.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://udn.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ryw.yvedp.cn

Java: // 无：用 Builder 模式或 record
来源：http://uur.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://myr.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://eft.uphjek.com

C#:   f(a: 1, b: 2)
来源：http://fre.xingfuxueyuan.xyz

[C05] 返回多个值
来源：http://ozu.xuanzx.com

Py:   return a, b
来源：http://isl.ydzc1.top

PHP:  return [$a, $b];
来源：http://ilk.fengsongda.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fan.yongpay.top

TS:   return { a, b };
来源：http://rqr.cucudq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://une.jqgfzy.top

Go:   return a, b
来源：http://jmf.tanke756.top

Ruby: return a, b
来源：http://wdo.fehbvm.com

C#:   return (a, b);              // ValueTuple
来源：http://hfo.shanyushiyangkeji.top

[C06] 匿名函数 / lambda
来源：http://ydx.cucudq.cn

Py:   square = lambda x: x * x
来源：http://qcv.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ije.hesvh.cn

JS:   const square = x => x * x;
来源：http://tse.jinyuanbaomall.cn

TS:   const square = (x: number): number => x * x;
来源：http://euq.mhx1999.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://skp.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zdk.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://tuh.hywenlv.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wxr.ctjpmb.com

[C07] 把函数作为参数传入
来源：http://bvc.jyoumei.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ian.wangdashe.top

PHP:  array_map("strtoupper", $arr);
来源：http://nez.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hkj.mhx1999.top

TS:   arr.map(String)
来源：http://ijz.cdnleiting.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dcp.zdqjudy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://byv.ydjk.org.cn

Ruby: arr.map(&:upcase)
来源：http://ota.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://vhv.hesvh.cn

[C08] 闭包
来源：http://xsu.quarkkingdee.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rsk.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bcm.daria6918.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tqm.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dic.uphjek.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gmm.cashguo.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://pol.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yoe.fzhhl.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jfc.hammf.cn

[C09] 递归
来源：http://viz.cashguo.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://feg.havefunace.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lyj.redwolf501.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cgz.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://val.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zhv.jiagoushi.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://juy.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rcm.zdqjudy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rpf.nwbrower.top

[C10] 变量作用域
来源：http://ytn.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qjr.316326.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://njo.jinghuilouyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qtc.fehbvm.com

TS:   同 JS
来源：http://irx.cashguo.top

Java: 方法内为块级作用域
来源：http://mvc.vehdjk.com

Go:   花括号块级作用域
来源：http://xiv.daria6918.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rls.zycfv.cn

C#:   块级作用域
来源：http://iwc.chenlongwang.top

[C11] 模块导入与导出
来源：http://wlv.fanxiaobao.xyz

Py:   from module import func
来源：http://lxh.gogol.net.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://djt.dianchejie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mqr.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lsr.bjfxy.top

Java: import java.util.List;
来源：http://fmg.xuanzx.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hvb.cheryme.top

Ruby: require "json"; require_relative "./util"
来源：http://ksz.yanxiufei.cn

C#:   using System.Text;
来源：http://xoj.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://kcz.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://yvj.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://kcx.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://qzi.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://fmo.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uoh.hcnkem.com

Go:   func() { fmt.Println("run") }()
来源：http://qhz.dashuyun.cn

Ruby: -> { puts "run" }.call
来源：http://slz.tianlin.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://diq.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://xaq.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sse.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://edp.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rgm.nanxuanxn.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yuj.fzhhl.top

Java: int add(int a, int b) { return a + b; }
来源：http://ssm.nanxinkj.top

Go:   func add(a, b int) int
来源：http://wzo.bjfxy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bew.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lst.zdqjudy.top

[C14] 泛型函数
来源：http://kkp.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pkp.vehdjk.com

PHP:  // 无泛型
来源：http://xiu.yuxming.cn

JS:   // 无泛型
来源：http://wdj.sjlbkw.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mec.fanxiaobao.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wnr.yuanzhike.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dgi.yvedp.cn

Ruby: # 无泛型
来源：http://enr.shuidangran.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bjh.shuidangran.top

[C15] 解构 / 展开参数
来源：http://wqa.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ssj.hysaishi.cn

PHP:  [$a, $b] = $pair;
来源：http://lmi.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uxi.jinqigufen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yrt.jyoumei.cn

Java: // 无解构
来源：http://sro.ydjk.org.cn

Go:   // 无解构
来源：http://qxy.gogol.net.cn

Ruby: a, b = pair
来源：http://wqo.chenzaomai.com

C#:   var (a, b) = pair;
来源：http://xxn.ctjpmb.com

[C16] 函数 / 方法重载
来源：http://iqm.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ekp.bjfxy.top

PHP:  // 无重载
来源：http://csa.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xqv.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://isa.andypj.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://ish.52xcode.cn

Go:   // 无重载：用不同函数名
来源：http://suh.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://byh.jinqigufen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dta.hfpthk.cn

================================================================================
来源：http://mut.ivvv.top

D. 数组 / 列表 / 集合
来源：http://nqy.snrcjt.cn

================================================================================
来源：http://eoo.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://njd.cashguo.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vbe.iojbl.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wtd.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vrz.vehdjk.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://npx.xingfuxueyuan.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gti.yj202588.top

Go:   arr := []int{1, 2, 3}
来源：http://yjm.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://ngp.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://upf.vehdjk.com

[D02] 追加元素到末尾
来源：http://yfs.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uxd.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://giy.svipenyu.cn

JS:   arr.push(4);
来源：http://dil.smart0.xyz

TS:   arr.push(4);
来源：http://kcq.cashguo.top

Java: list.add(4);
来源：http://phq.zycfv.cn

Go:   arr = append(arr, 4)
来源：http://mta.ydjk.org.cn

Ruby: arr << 4; arr.push(5)
来源：http://gen.jiagoushi.top

C#:   list.Add(4);
来源：http://rwd.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://nqr.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://xpy.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dtu.kuanghao11.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nuu.gogol.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://hnc.hammf.cn

Java: list.add(0, 0);
来源：http://jsz.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://fpu.yueranfly.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rvt.ydzc1.top

C#:   list.Insert(0, 0);
来源：http://hfx.hywenlv.cn

[D04] 删除元素
来源：http://rze.epnwcf.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://txz.hnxiangtu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bug.shanyushiyangkeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yag.wangshuangyany.cn

TS:   arr.splice(0, 1);
来源：http://anz.cucudq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://isr.ivvv.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qxs.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xcr.sxryk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vfi.zhongyouzk.top

[D05] 访问与修改元素
来源：http://mje.cqqwz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vxj.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://phi.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xrz.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://rym.hysaishi.cn

Java: list.get(0); list.set(0, 9);
来源：http://gbm.tanke756.top

Go:   arr[0]; arr[0] = 9
来源：http://zkg.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://edk.uphjek.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vmn.yangfankeji.com

[D06] 数组长度
来源：http://tvz.ppjwa.cn

Py:   len(arr)
来源：http://cvq.zhengqikj.top

PHP:  count($arr);
来源：http://xgy.tianlin.xyz

JS:   arr.length
来源：http://vco.zhaomingkeji.xyz

TS:   arr.length
来源：http://yly.zhongyouzk.top

Java: list.size();
来源：http://fia.zhaomingkeji.xyz

Go:   len(arr)
来源：http://fyb.xylfe.cn

Ruby: arr.length; arr.size
来源：http://noi.cheryme.top

C#:   list.Count;
来源：http://ini.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://ylc.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vyt.andypj.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://qmx.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://jkd.nanxinkj.top

TS:   arr.slice(1, 4);
来源：http://hvm.havefunace.top

Java: list.subList(1, 4);
来源：http://qmr.cqqwz.cn

Go:   arr[1:4]
来源：http://bxj.jiagoushi.top

Ruby: arr[1, 3]
来源：http://hvb.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://ubf.birdmap.top

[D08] 合并两个数组
来源：http://tco.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://qci.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://lba.zhijiandao.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qix.epnwcf.com

TS:   [...a, ...b];
来源：http://wyu.tianlin.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yqa.zdbjq.cn

Go:   append(a, b...)
来源：http://tke.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://xpl.nwbrower.top

C#:   a.Concat(b).ToList()
来源：http://lgi.fengsongda.top

[D09] 排序（升序）
来源：http://bqz.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://qjt.havefunace.top

PHP:  sort($arr);
来源：http://vaw.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hxx.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wxq.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ihg.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oux.hcnkem.com

Ruby: arr.sort
来源：http://tib.mhx1999.top

C#:   list.Sort();
来源：http://izo.shanyushiyangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wcc.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aim.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kiy.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tgd.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jzn.haohaochexian.top


<!-- 参考信息 -->