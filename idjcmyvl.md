代发 wailian999

[B09] break 与 continue
来源：http://hhp.yj20258888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yqq.wangshuangyany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zpp.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fig.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zok.ydzc1.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tfi.fehbvm.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yja.aizwys.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hsk.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jwf.jinqigufen.top

[B10] 遍历同时拿索引
来源：http://svr.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kia.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rsi.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wxu.zdqjudy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zza.gaohongyu789.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ugx.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://azj.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vgl.xuetiantiany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://skq.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://xru.9152youxi.cn

Py:   list(range(0, 10, 2))
来源：http://sae.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://djl.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mfn.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rke.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zvz.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://imr.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://sns.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rhm.cqqwz.cn

[B12] 跳出多层循环
来源：http://chv.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gsz.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mhs.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uur.zdqjudy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pqr.pycfn.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wfj.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cad.guannengcc.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ixn.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://knj.andypj.xyz

[B13] 判断是否为数字
来源：http://nei.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://imm.yangfankeji.com

PHP:  is_numeric($x)
来源：http://gpe.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xxl.jyoumei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://agd.yuanzhike.top

Java: x instanceof Number
来源：http://ooj.haohaochexian.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xll.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://eya.aizwys.cn

C#:   x is int or double or decimal
来源：http://dgn.feifeiyinyue.top

[B14] 判断值是否在集合内
来源：http://udj.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dxk.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rsm.tianlin.xyz

JS:   [1, 2, 3].includes(x)
来源：http://mzw.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://udb.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://obz.svipenyu.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wka.gogol.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://upd.aizwys.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fff.chenzaomai.com

[B15] 布尔运算与取反
来源：http://ssb.hongshengwenyu.top

Py:   a and b or not c
来源：http://rzl.daxiang520.top

PHP:  $a && $b || !$c
来源：http://ogt.tarul.cn

JS:   a && b || !c
来源：http://xua.hysaishi.cn

TS:   a && b || !c
来源：http://yds.sweek.top

Java: a && b || !c
来源：http://oak.wangshuangyany.cn

Go:   a && b || !c
来源：http://zfe.zhixingplan.top

Ruby: a && b || !c
来源：http://jiv.guannengcc.top

C#:   a && b || !c
来源：http://xhn.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://faq.kuanghao11.cn

Py:   if not data: return
来源：http://yga.chenlongwang.top

PHP:  if (!$data) { return; }
来源：http://hog.ydzc1.top

JS:   if (!data) return;
来源：http://haz.jyoumei.cn

TS:   if (!data) return;
来源：http://vaw.yangfankeji.com

Java: if (data == null) return;
来源：http://ffp.gaohongyu789.top

Go:   if data == nil { return }
来源：http://lic.chenzaomai.com

Ruby: return if data.nil?
来源：http://tre.yj20258.top

C#:   if (data == null) return;
来源：http://xez.fktsv.cn

================================================================================
来源：http://ogw.chenlongwang.top

C. 函数与作用域
来源：http://oru.guannengcc.top

================================================================================
来源：http://ync.zhongyouzk.top

[C01] 定义函数
来源：http://cnd.zhengqikj.top

Py:   def add(a, b): return a + b
来源：http://rem.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zed.ivvv.top

JS:   function add(a, b) { return a + b; }
来源：http://mut.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oro.0kj1m.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://piu.dianchejie.cn

Go:   func add(a, b int) int { return a + b }
来源：http://equ.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://yzx.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lob.ctjpmb.com

[C02] 默认参数
来源：http://xaw.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://eps.haohaochexian.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ddw.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://dxx.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vmj.sweek.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hze.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rut.jyoumei.cn

Ruby: def greet(name = "World") = name
来源：http://poj.yuanzhike.top

C#:   string Greet(string name = "World") => name;
来源：http://kgw.52xcode.cn

[C03] 可变参数
来源：http://fjy.dashuyun.cn

Py:   def total(*args): return sum(args)
来源：http://wwz.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qwf.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vty.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pne.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ljk.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hem.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://pjb.shangyingyoupin.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nzl.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://llb.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mva.bjfxy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://isa.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dzl.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vbg.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://dis.xinyue.icu

Go:   // 无：用配置结构体参数
来源：http://jyn.cdnleiting.top

Ruby: f(a: 1, b: 2)
来源：http://yjy.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://sho.shuidangran.top

[C05] 返回多个值
来源：http://smy.daxiang520.top

Py:   return a, b
来源：http://msv.redwolf501.top

PHP:  return [$a, $b];
来源：http://ynq.xuanzx.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://kfk.kuanghao11.cn

TS:   return { a, b };
来源：http://krn.haohaochexian.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lzv.cqqwz.cn

Go:   return a, b
来源：http://apv.zhijiandao.cn

Ruby: return a, b
来源：http://idy.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://eoe.zdqjudy.top

[C06] 匿名函数 / lambda
来源：http://amm.xylfe.cn

Py:   square = lambda x: x * x
来源：http://qgl.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://yft.yuxming.cn

JS:   const square = x => x * x;
来源：http://pzs.jinqigfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://ayj.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pjk.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://iax.hfpthk.cn

Ruby: square = ->(x) { x * x }
来源：http://ygq.hnxiangtu.top

C#:   Func<int, int> square = x => x * x;
来源：http://ftu.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://rof.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yss.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://ahb.hnqzz.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qun.shzxlz.cn

TS:   arr.map(String)
来源：http://fxs.quarkkingdee.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ceb.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cno.zdqjudy.top

Ruby: arr.map(&:upcase)
来源：http://vfd.jinqigufen.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gjc.ppjwa.cn

[C08] 闭包
来源：http://dmo.fktsv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xfl.ctjpmb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://xot.jyoumei.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vpm.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://eun.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ctz.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jxl.yueranfly.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wls.yanxiufei.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bva.tanke756.top

[C09] 递归
来源：http://sfp.yuanzhike.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qaw.chenlongwang.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cqk.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ubj.hnxiangtu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kie.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://azy.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yur.jlsjyb.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jzz.xuanzx.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sab.yj20258.top

[C10] 变量作用域
来源：http://ipl.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ktv.haohaochexian.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iaf.shuidangran.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bsu.zhixingplan.top

TS:   同 JS
来源：http://ncx.yj202588.top

Java: 方法内为块级作用域
来源：http://blz.guowangkeji.top

Go:   花括号块级作用域
来源：http://yja.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://khz.316326.xyz

C#:   块级作用域
来源：http://hdz.jinyuanbaomall.cn

[C11] 模块导入与导出
来源：http://bgd.jqgufenzy.top

Py:   from module import func
来源：http://hgu.svipenyu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://upo.vehdjk.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://ayd.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qmi.cheryme.top

Java: import java.util.List;
来源：http://unn.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uyf.fehbvm.com

Ruby: require "json"; require_relative "./util"
来源：http://avz.zdqjudy.top

C#:   using System.Text;
来源：http://lsz.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://eac.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://pwe.svipenyu.cn

PHP:  (function () { echo "run"; })();
来源：http://ybu.wangdashe.top

JS:   (() => { console.log("run"); })();
来源：http://qao.andypj.xyz

TS:   (() => { console.log("run"); })();
来源：http://lpu.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zmx.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://czj.sxryk.cn

Ruby: -> { puts "run" }.call
来源：http://bxd.zdqjudy.top

C#:   // 无 IIFE：用静态构造函数
来源：http://skl.aizwys.cn

[C13] 类型声明 / 类型注解
来源：http://uwd.cashguo.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ipn.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://giw.xingfuxueyuan.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lgi.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hce.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://mtt.yongpay.top

Go:   func add(a, b int) int
来源：http://tuy.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://afd.yanxiufei.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nwm.sufxvd.cn

[C14] 泛型函数
来源：http://cyw.gotoacloud.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hsj.birdmap.top

PHP:  // 无泛型
来源：http://xlh.9152youxi.cn

JS:   // 无泛型
来源：http://nfu.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://omq.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xqe.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dqk.zhongyouzk.top

Ruby: # 无泛型
来源：http://hmg.cqqwz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bgn.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://xrc.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cof.zhijiandao.cn

PHP:  [$a, $b] = $pair;
来源：http://tmm.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pxo.sjlbkw.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gaf.sxryk.cn

Java: // 无解构
来源：http://nkk.tanke756.top

Go:   // 无解构
来源：http://quh.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://afc.snrcjt.cn

C#:   var (a, b) = pair;
来源：http://zni.chenlongwang.top

[C16] 函数 / 方法重载
来源：http://ere.snrcjt.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iws.tian-w.cn

PHP:  // 无重载
来源：http://wms.yanxiufei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xid.xuetiantiany.cn

TS:   // 用联合类型或重载签名声明
来源：http://vjw.jinyuanbaomall.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://frn.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://zet.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://zou.hongshengwenyu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zpy.yangfankeji.com

================================================================================
来源：http://nrs.jianghu66.top

D. 数组 / 列表 / 集合
来源：http://cfg.bbcook.cn

================================================================================
来源：http://jmf.yj20258888.top

[D01] 创建数组 / 列表
来源：http://hzu.chenjidiqi.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://odd.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xgz.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yvy.ppjwa.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vqf.ivvv.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gtm.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://zlb.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://esg.vqdsnc.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://srd.daria6918.cn

[D02] 追加元素到末尾
来源：http://box.vehdjk.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tkw.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yqm.chenzaomai.com

JS:   arr.push(4);
来源：http://ylx.sxryk.cn

TS:   arr.push(4);
来源：http://tiq.hnxiangtu.top

Java: list.add(4);
来源：http://iui.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://jih.zhongyouzk.top

Ruby: arr << 4; arr.push(5)
来源：http://vgi.cdnleiting.top

C#:   list.Add(4);
来源：http://qvb.0kj1m.cn

[D03] 在指定位置插入元素
来源：http://zfz.shanyushiyangkeji.top

Py:   arr.insert(0, 0)
来源：http://dze.andypj.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://paq.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wkh.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://aqh.quarkkingdee.top

Java: list.add(0, 0);
来源：http://qsa.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://ttv.9152youxi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://arr.zhiwuduotai.top

C#:   list.Insert(0, 0);
来源：http://ltp.yvedp.cn

[D04] 删除元素
来源：http://ndu.chenjidiqi.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ujx.daria6918.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tzy.feifeiyinyue.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pyw.xylfe.cn

TS:   arr.splice(0, 1);
来源：http://luu.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://muh.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jjw.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://puh.xinyue.icu

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ocl.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://bkw.redwolf501.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kmk.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tcb.nanxuanxn.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gua.ywan-chungtsiang.top

TS:   arr[0]; arr.at(-1);
来源：http://uns.zhongyouzk.top

Java: list.get(0); list.set(0, 9);
来源：http://uqf.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://omq.fzhhl.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zwy.ivvv.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hap.havefunace.top

[D06] 数组长度
来源：http://wsj.andypj.xyz

Py:   len(arr)
来源：http://jtn.uphjek.com

PHP:  count($arr);
来源：http://xmf.yueranfly.top

JS:   arr.length
来源：http://rpu.fengsongda.top

TS:   arr.length
来源：http://cey.hywenlv.cn

Java: list.size();
来源：http://sut.zhongyouzk.top

Go:   len(arr)
来源：http://nap.yonumen.top

Ruby: arr.length; arr.size
来源：http://sqo.zhaomingkeji.xyz

C#:   list.Count;
来源：http://moj.jianghu66.top

[D07] 切片 / 取子数组
来源：http://awv.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lmc.yangfankeji.com

PHP:  array_slice($arr, 1, 3);
来源：http://vad.hongshengwenyu.top

JS:   arr.slice(1, 4);
来源：http://evs.yuanzhike.top

TS:   arr.slice(1, 4);
来源：http://jhg.zhongyouzk.top

Java: list.subList(1, 4);
来源：http://qkl.jianghu66.top

Go:   arr[1:4]
来源：http://jxv.tianlin.xyz

Ruby: arr[1, 3]
来源：http://afl.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://muo.pengpengdd.cyou

[D08] 合并两个数组
来源：http://gaw.shzxlz.cn

Py:   a + b;  a.extend(b)
来源：http://fhq.sufxvd.cn

PHP:  array_merge($a, $b);
来源：http://wzy.gogol.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lyl.snrcjt.cn

TS:   [...a, ...b];
来源：http://cuo.ybcxt.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aan.sweek.top

Go:   append(a, b...)
来源：http://enq.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://abn.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://ndf.ydjk.org.cn

[D09] 排序（升序）
来源：http://nsw.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://bju.xuanzx.com

PHP:  sort($arr);
来源：http://ivp.kuanghao11.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vjr.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://tjw.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bkl.epnwcf.com


<!-- 参考信息 -->