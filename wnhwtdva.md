代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://bbs.zhengqikj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://abu.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://djb.pycfn.com

TS:   do { i++; } while (i < 10);
来源：http://cpk.mhx1999.top

Java: do { i++; } while (i < 10);
来源：http://jfv.jinyuanbaomall.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pqp.daxiang520.top

Ruby: begin; i += 1; end while i < 10
来源：http://vxb.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://txe.feifeiyinyue.top

[B09] break 与 continue
来源：http://cus.feifeiyinyue.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hta.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nkz.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dkw.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ozd.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jbs.svipenyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pgv.feifeiyinyue.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zwj.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xaq.pengpengdd.cyou

[B10] 遍历同时拿索引
来源：http://ese.yj20258888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://swp.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vfn.meibo888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://los.fzhhl.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://orf.yj20258888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://djl.jinqigufen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pwm.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uvk.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iiq.bjfxy.top

[B11] 生成数字序列 / 区间
来源：http://vwe.xylfe.cn

Py:   list(range(0, 10, 2))
来源：http://vvc.shzxlz.cn

PHP:  range(0, 10, 2);
来源：http://hrc.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://npg.havefunace.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fgz.316326.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uqp.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zxn.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://nnf.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gea.iojbl.cn

[B12] 跳出多层循环
来源：http://eri.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bnf.yuxming.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lai.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mqb.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xxa.jinqigufen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dif.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ogc.gogol.net.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wbn.kuanghao11.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fxy.zhoulong.xyz

[B13] 判断是否为数字
来源：http://tio.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://lyi.zhongyouzk.top

PHP:  is_numeric($x)
来源：http://uhl.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gvh.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://epa.dashuyun.cn

Java: x instanceof Number
来源：http://vco.chenzaomai.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://omu.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://ots.zhaomingkeji.xyz

C#:   x is int or double or decimal
来源：http://hni.yvedp.cn

[B14] 判断值是否在集合内
来源：http://rpg.wangshuangyany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yjf.0kj1m.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wcf.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://phi.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://tdx.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://frr.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nar.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://haf.snrcjt.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lwj.xinyue.icu

[B15] 布尔运算与取反
来源：http://ien.dianchejie.cn

Py:   a and b or not c
来源：http://vhs.mhx1999.top

PHP:  $a && $b || !$c
来源：http://yez.iojbl.cn

JS:   a && b || !c
来源：http://vdd.guowangkeji.top

TS:   a && b || !c
来源：http://fun.xuanzx.com

Java: a && b || !c
来源：http://whf.haohaochexian.top

Go:   a && b || !c
来源：http://zak.ydjk.org.cn

Ruby: a && b || !c
来源：http://ylq.ppjwa.cn

C#:   a && b || !c
来源：http://cly.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://tgu.hnqzz.top

Py:   if not data: return
来源：http://crp.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://rya.tarul.cn

JS:   if (!data) return;
来源：http://jfe.zhoulong.xyz

TS:   if (!data) return;
来源：http://xki.pengpengdd.cyou

Java: if (data == null) return;
来源：http://onh.tian-w.cn

Go:   if data == nil { return }
来源：http://emg.ybcxt.top

Ruby: return if data.nil?
来源：http://cyd.vehdjk.com

C#:   if (data == null) return;
来源：http://mfu.vqdsnc.cn

================================================================================
来源：http://byl.chenlongwang.top

C. 函数与作用域
来源：http://mmt.pycfn.com

================================================================================
来源：http://etz.pengpengdd.cyou

[C01] 定义函数
来源：http://okt.yj20258888.top

Py:   def add(a, b): return a + b
来源：http://qxr.shzxlz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ceu.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://ksm.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vst.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zin.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://syp.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://okq.hysaishi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://whp.hfpthk.cn

[C02] 默认参数
来源：http://pyx.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://nnr.feifeiyinyue.top

PHP:  function greet($name = "World") { return $name; }
来源：http://crn.fzhhl.top

JS:   function greet(name = "World") { return name; }
来源：http://mfm.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mtz.yj20258888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gfz.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dnp.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://fgs.tianlin.xyz

C#:   string Greet(string name = "World") => name;
来源：http://guu.tarul.cn

[C03] 可变参数
来源：http://net.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://dje.jinghuilouyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wqk.shanyushiyangkeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://shq.ydzc1.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rlj.fengsongda.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uug.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hwu.shuidangran.top

Ruby: def total(*nums); nums.sum; end
来源：http://tcm.iojbl.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kyt.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://skj.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://trc.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hrr.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://auq.iojbl.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://oam.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://aqa.jlsjyb.cn

Go:   // 无：用配置结构体参数
来源：http://gkp.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://ank.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://rvx.smart0.xyz

[C05] 返回多个值
来源：http://jlx.nwbrower.top

Py:   return a, b
来源：http://uud.ydzc1.top

PHP:  return [$a, $b];
来源：http://kgd.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rbq.fktsv.cn

TS:   return { a, b };
来源：http://xhz.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mdp.ybcxt.top

Go:   return a, b
来源：http://vvu.zhoulong.xyz

Ruby: return a, b
来源：http://zmj.ydjk.org.cn

C#:   return (a, b);              // ValueTuple
来源：http://eth.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://adw.daxiang520.top

Py:   square = lambda x: x * x
来源：http://sdt.jlsjyb.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zje.uphjek.com

JS:   const square = x => x * x;
来源：http://gcz.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://spe.daxiang520.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ycq.jinqigufen.top

Go:   sq := func(x int) int { return x * x }
来源：http://iis.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://vih.zhixingplan.top

C#:   Func<int, int> square = x => x * x;
来源：http://wuu.shuidangran.top

[C07] 把函数作为参数传入
来源：http://ztb.52xcode.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://phj.jqgfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://rcx.zhongyouzk.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fjj.fanxiaobao.xyz

TS:   arr.map(String)
来源：http://tox.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iqp.zhongyouzk.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jus.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://phq.shanyushiyangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://atr.hammf.cn

[C08] 闭包
来源：http://rck.hnxiangtu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://phr.iojbl.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nmm.guowangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://awg.aizwys.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://fyo.cheryme.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pyg.hfpthk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qxv.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jkp.jianghu66.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nhm.iojbl.cn

[C09] 递归
来源：http://gqf.chenzaomai.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tud.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wfl.tianlin.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://krp.zhixingplan.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wgp.chenjidiqi.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vhv.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zqm.jiagoushi.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ape.hfpthk.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ylt.nanxuanxn.top

[C10] 变量作用域
来源：http://nsm.andypj.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ydy.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sre.zycfv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kgv.hnxiangtu.top

TS:   同 JS
来源：http://bjx.feifeiyinyue.top

Java: 方法内为块级作用域
来源：http://fta.jqgfzy.top

Go:   花括号块级作用域
来源：http://rjs.mhx1999.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tcw.gaohongyu789.top

C#:   块级作用域
来源：http://ifp.cheryme.top

[C11] 模块导入与导出
来源：http://vrf.cdnleiting.top

Py:   from module import func
来源：http://xww.jiagoushi.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dyc.tian-w.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://whw.tianlin.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://axx.hnqzz.top

Java: import java.util.List;
来源：http://abu.sweek.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://rfv.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://umf.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://cjc.zdbjq.cn

[C12] 立即执行函数 IIFE
来源：http://xdr.wangdashe.top

Py:   (lambda: print("run"))()
来源：http://grd.shzxlz.cn

PHP:  (function () { echo "run"; })();
来源：http://pkh.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://dwp.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://fpr.bbcook.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ftb.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://gqm.zhongyouzk.top

Ruby: -> { puts "run" }.call
来源：http://hlt.ybcxt.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bii.fktsv.cn

[C13] 类型声明 / 类型注解
来源：http://ita.redwolf501.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://waj.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kpk.yuxming.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ekb.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ovh.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://njn.cheryme.top

Go:   func add(a, b int) int
来源：http://ngv.pengpengdd.cyou

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pti.zhengqikj.top

C#:   int Add(int a, int b) => a + b;
来源：http://vim.sufxvd.cn

[C14] 泛型函数
来源：http://hwv.9152youxi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fwv.jianghu66.top

PHP:  // 无泛型
来源：http://bux.hfpthk.cn

JS:   // 无泛型
来源：http://lnx.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qlm.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wvl.dashuyun.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rzc.ivvv.top

Ruby: # 无泛型
来源：http://wfd.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hnl.sjlbkw.cn

[C15] 解构 / 展开参数
来源：http://bjc.daria6918.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dxf.jianghu66.top

PHP:  [$a, $b] = $pair;
来源：http://lvk.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jnv.bbcook.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cid.jinqigufen.top

Java: // 无解构
来源：http://ngt.fktsv.cn

Go:   // 无解构
来源：http://foo.sysykeji.top

Ruby: a, b = pair
来源：http://pne.0kj1m.cn

C#:   var (a, b) = pair;
来源：http://rhy.316326.xyz

[C16] 函数 / 方法重载
来源：http://mef.c1oappe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zxr.yfazqb.com

PHP:  // 无重载
来源：http://tuc.birdmap.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lrx.aizwys.cn

TS:   // 用联合类型或重载签名声明
来源：http://jlr.yueranfly.top

Java: void f(int a) {}  void f(String a) {}
来源：http://oyh.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://dip.ywan-chungtsiang.top

Ruby: # 无重载：靠动态参数
来源：http://frf.hammf.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://syw.cdnleiting.top

================================================================================
来源：http://eou.xinyue.icu

D. 数组 / 列表 / 集合
来源：http://wil.guowangkeji.top

================================================================================
来源：http://zkm.yj202588.top

[D01] 创建数组 / 列表
来源：http://yhk.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://acv.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xwp.fehbvm.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kbo.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jvf.fanxiaobao.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ugo.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://sex.jinghuilouyu.cn

Ruby: arr = [1, 2, 3]
来源：http://ors.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cvh.aibaodan.cn

[D02] 追加元素到末尾
来源：http://sjm.316326.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mac.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nnr.fehbvm.com

JS:   arr.push(4);
来源：http://lvx.gotoacloud.top

TS:   arr.push(4);
来源：http://tra.jinghuilouyu.cn

Java: list.add(4);
来源：http://idm.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://bxk.fzhhl.top

Ruby: arr << 4; arr.push(5)
来源：http://iou.vqdsnc.cn

C#:   list.Add(4);
来源：http://vsn.jinqigufen.top

[D03] 在指定位置插入元素
来源：http://zng.yongpay.top

Py:   arr.insert(0, 0)
来源：http://qpp.hnxiangtu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bos.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qfq.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://fpm.aibaodan.cn

Java: list.add(0, 0);
来源：http://wjj.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://swt.yvedp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cfm.gogol.net.cn

C#:   list.Insert(0, 0);
来源：http://hyc.hongshengwenyu.top

[D04] 删除元素
来源：http://skg.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ble.cucudq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wfu.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://npx.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://gch.jiagoushi.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jch.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lou.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gqd.shangyingyoupin.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://din.hammf.cn

[D05] 访问与修改元素
来源：http://tzg.tarul.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lfm.hesvh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ydz.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wnw.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://xes.yueranfly.top

Java: list.get(0); list.set(0, 9);
来源：http://mue.yongpay.top

Go:   arr[0]; arr[0] = 9
来源：http://mjm.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hdg.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jxs.hongshengwenyu.top

[D06] 数组长度
来源：http://nxs.yuxming.cn

Py:   len(arr)
来源：http://psn.yvedp.cn

PHP:  count($arr);
来源：http://exd.hfpthk.cn

JS:   arr.length
来源：http://tkj.ybcxt.top

TS:   arr.length
来源：http://ujq.kuanghao11.cn

Java: list.size();
来源：http://axs.zhixingplan.top

Go:   len(arr)
来源：http://ytq.iojbl.cn

Ruby: arr.length; arr.size
来源：http://pjo.xuetiantiany.cn

C#:   list.Count;
来源：http://ggg.yuxming.cn

[D07] 切片 / 取子数组
来源：http://uck.9152youxi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rnx.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://mkf.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://arw.nwbrower.top

TS:   arr.slice(1, 4);
来源：http://pbm.meibo888.top

Java: list.subList(1, 4);
来源：http://rmj.yj20258.top

Go:   arr[1:4]
来源：http://hmz.svipenyu.cn

Ruby: arr[1, 3]
来源：http://ljo.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://gvn.uphjek.com

[D08] 合并两个数组
来源：http://kac.ehwqpu.com

Py:   a + b;  a.extend(b)
来源：http://vvc.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://zeq.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vff.haohaochexian.top

TS:   [...a, ...b];
来源：http://utf.hnqzz.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ukh.jinqigfzy.top

Go:   append(a, b...)
来源：http://jxc.jiagoushi.top


<!-- 参考信息 -->