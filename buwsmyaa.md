代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hph.sweek.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mdt.chenjidiqi.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ucc.vehdjk.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kfa.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://maq.kuanghao11.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mzp.gaohongyu789.top

[B07] while 循环
来源：http://uak.tanke756.top

Py:   while i < 10: i += 1
来源：http://ady.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://kng.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://pub.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://csl.gotoacloud.top

Java: while (i < 10) { i++; }
来源：http://tav.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zif.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://itm.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://wbj.zhongyouzk.top

[B08] do-while（至少执行一次）
来源：http://hwz.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://yzh.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://esh.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://asd.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://evy.fehbvm.com

Java: do { i++; } while (i < 10);
来源：http://giw.hnqzz.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cye.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://cbc.shangyingyoupin.top

C#:   do { i++; } while (i < 10);
来源：http://jvj.chenzaomai.com

[B09] break 与 continue
来源：http://lsr.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pfb.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cmu.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yor.mhx1999.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iio.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vrw.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tfn.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wld.iojbl.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yjc.sxryk.cn

[B10] 遍历同时拿索引
来源：http://cgt.hywenlv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kmt.jinyuanbaomall.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yne.52xcode.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cwa.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qrb.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ros.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lah.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gsm.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ogt.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://llo.hysaishi.cn

Py:   list(range(0, 10, 2))
来源：http://kfg.yueranfly.top

PHP:  range(0, 10, 2);
来源：http://zub.hcnkem.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://myt.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yjo.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eux.snrcjt.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wya.zhiwuduotai.top

Ruby: (0...10).step(2).to_a
来源：http://mfl.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zpo.zdbjq.cn

[B12] 跳出多层循环
来源：http://hai.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zhz.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://arl.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gop.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wss.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lcz.9152youxi.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yqb.shzxlz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://liy.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gri.yueranfly.top

[B13] 判断是否为数字
来源：http://aon.shuidangran.top

Py:   isinstance(x, (int, float))
来源：http://vpm.hnqzz.top

PHP:  is_numeric($x)
来源：http://xvn.c1oappe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dzp.zhixingplan.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dxf.cheryme.top

Java: x instanceof Number
来源：http://wuu.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ebb.zhiwuduotai.top

Ruby: x.is_a?(Numeric)
来源：http://tjh.pengpengdd.cyou

C#:   x is int or double or decimal
来源：http://umy.pycfn.com

[B14] 判断值是否在集合内
来源：http://dwq.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zvr.jlsjyb.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kjy.fzhhl.top

JS:   [1, 2, 3].includes(x)
来源：http://umv.dashuyun.cn

TS:   [1, 2, 3].includes(x)
来源：http://kwt.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://aeg.cucudq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hdr.gogol.net.cn

Ruby: [1, 2, 3].include?(x)
来源：http://etu.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ppg.guannengcc.top

[B15] 布尔运算与取反
来源：http://xnu.snrcjt.cn

Py:   a and b or not c
来源：http://bdh.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://hbz.smart0.xyz

JS:   a && b || !c
来源：http://ldn.mhx1999.top

TS:   a && b || !c
来源：http://asz.nanxuanxn.top

Java: a && b || !c
来源：http://dxa.nanxinkj.top

Go:   a && b || !c
来源：http://dta.fengsongda.top

Ruby: a && b || !c
来源：http://zgo.hysaishi.cn

C#:   a && b || !c
来源：http://bau.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ljx.zhaomingkeji.xyz

Py:   if not data: return
来源：http://aji.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://oer.uphjek.com

JS:   if (!data) return;
来源：http://exk.zhengqikj.top

TS:   if (!data) return;
来源：http://nlg.yonumen.top

Java: if (data == null) return;
来源：http://xme.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://dqk.jiagoushi.top

Ruby: return if data.nil?
来源：http://bfx.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://rsc.hongshengwenyu.top

================================================================================
来源：http://jjl.hesvh.cn

C. 函数与作用域
来源：http://vcx.jqgfzy.top

================================================================================
来源：http://qzo.shanyushiyangtech.top

[C01] 定义函数
来源：http://exi.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://tse.jinqigufen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hzz.jinghuilouyu.cn

JS:   function add(a, b) { return a + b; }
来源：http://xbp.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tnu.andypj.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://hqm.hongshengwenyu.top

Go:   func add(a, b int) int { return a + b }
来源：http://fut.jinghuilouyu.cn

Ruby: def add(a, b); a + b; end
来源：http://tyv.vehdjk.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mmb.9152youxi.cn

[C02] 默认参数
来源：http://bdv.c1oappe.top

Py:   def greet(name="World"): return name
来源：http://amv.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://hjb.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://wuz.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yzc.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://hks.tanke756.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oou.chenzaomai.com

Ruby: def greet(name = "World") = name
来源：http://vph.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://jyt.shanyushiyangtech.top

[C03] 可变参数
来源：http://ena.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://vqq.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zhf.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qxf.shzxlz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xrp.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qdu.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uqc.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://xyf.jlsjyb.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rxt.epnwcf.com

[C04] 命名参数 / 关键字参数
来源：http://gkw.hongshengwenyu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://npp.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zrn.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fxo.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tet.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://fss.andypj.xyz

Go:   // 无：用配置结构体参数
来源：http://ksb.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://bdn.ydjk.org.cn

C#:   f(a: 1, b: 2)
来源：http://cbi.shuidangran.top

[C05] 返回多个值
来源：http://iwt.cheryme.top

Py:   return a, b
来源：http://axs.yj20258.top

PHP:  return [$a, $b];
来源：http://ptc.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xbx.jqgufenzy.top

TS:   return { a, b };
来源：http://zst.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://twz.gotoacloud.top

Go:   return a, b
来源：http://kkv.bjfxy.top

Ruby: return a, b
来源：http://upv.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://vkd.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://zhh.bbcook.cn

Py:   square = lambda x: x * x
来源：http://krt.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ctz.yj20258888.top

JS:   const square = x => x * x;
来源：http://usl.jqgfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://yjk.ctjpmb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vzr.jinqigufen.top

Go:   sq := func(x int) int { return x * x }
来源：http://ffb.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://dvu.wangshuangyany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gyg.bbcook.cn

[C07] 把函数作为参数传入
来源：http://ofq.hfpthk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ofn.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://kqk.andypj.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pci.ctjpmb.com

TS:   arr.map(String)
来源：http://gqb.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xuy.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ifu.aibaodan.cn

Ruby: arr.map(&:upcase)
来源：http://bkg.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lxl.jlsjyb.cn

[C08] 闭包
来源：http://dri.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://czs.xuanzx.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tmm.vehdjk.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://csy.svipenyu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://omo.ydzc1.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vxf.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fgm.pengpengdd.cyou

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mtq.sysykeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tfa.xziqi.cn

[C09] 递归
来源：http://smi.yj20258888.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://niw.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vgd.fktsv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://els.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cuw.kuanghao11.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nyt.cdnleiting.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nbe.ybcxt.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vqg.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://deg.cqqwz.cn

[C10] 变量作用域
来源：http://hdx.pengpengdd.cyou

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zim.c1oappe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ifn.ppjwa.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://htl.svipenyu.cn

TS:   同 JS
来源：http://qsr.yj20258.top

Java: 方法内为块级作用域
来源：http://xeo.shanyushiyangtech.top

Go:   花括号块级作用域
来源：http://irw.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ywg.sxryk.cn

C#:   块级作用域
来源：http://ayx.redwolf501.top

[C11] 模块导入与导出
来源：http://vpj.nanxinkj.top

Py:   from module import func
来源：http://ubr.cheryme.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wok.nanxinkj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://wvp.ybcxt.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ury.nwbrower.top

Java: import java.util.List;
来源：http://bak.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cud.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://dxd.ctjpmb.com

C#:   using System.Text;
来源：http://kmp.pycfn.com

[C12] 立即执行函数 IIFE
来源：http://zzc.jinghuilouyu.cn

Py:   (lambda: print("run"))()
来源：http://srw.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://hzu.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://lai.guowangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://nmc.ydjk.org.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://frc.shzxlz.cn

Go:   func() { fmt.Println("run") }()
来源：http://ssf.wangshuangyany.cn

Ruby: -> { puts "run" }.call
来源：http://kmi.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://sgx.jinyuanbaomall.cn

[C13] 类型声明 / 类型注解
来源：http://max.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kcb.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jaq.nanxinkj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mgt.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wvl.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://yie.svipenyu.cn

Go:   func add(a, b int) int
来源：http://ivz.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fmh.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://wnp.ydjk.org.cn

[C14] 泛型函数
来源：http://psd.316326.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pny.jinyuanbaomall.cn

PHP:  // 无泛型
来源：http://fma.fehbvm.com

JS:   // 无泛型
来源：http://uzu.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hem.gotoacloud.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://idv.52xcode.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yde.fanxiaobao.xyz

Ruby: # 无泛型
来源：http://xnn.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rkm.yvedp.cn

[C15] 解构 / 展开参数
来源：http://rzg.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vxw.yanxiufei.cn

PHP:  [$a, $b] = $pair;
来源：http://mja.yj20258888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hbe.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ecl.jqgufenzy.top

Java: // 无解构
来源：http://wow.jinqigufen.top

Go:   // 无解构
来源：http://zye.nanxuanxn.top

Ruby: a, b = pair
来源：http://vlr.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://teg.shangyingyoupin.top

[C16] 函数 / 方法重载
来源：http://zgf.kuanghao11.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ldi.cashguo.top

PHP:  // 无重载
来源：http://fdg.shuidangran.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xvj.shzxlz.cn

TS:   // 用联合类型或重载签名声明
来源：http://eci.ehwqpu.com

Java: void f(int a) {}  void f(String a) {}
来源：http://jpk.sweek.top

Go:   // 无重载：用不同函数名
来源：http://aav.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://kdy.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://tlu.tanke756.top

================================================================================
来源：http://gub.zhixingplan.top

D. 数组 / 列表 / 集合
来源：http://gpc.ctjpmb.com

================================================================================
来源：http://hcj.fehbvm.com

[D01] 创建数组 / 列表
来源：http://cpc.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://auf.cucudq.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jst.tarul.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gjs.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://dep.tanke756.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xom.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://cat.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://fuj.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://plr.c1oappe.top

[D02] 追加元素到末尾
来源：http://qmt.quarkkingdee.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dsv.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://abi.quarkkingdee.top

JS:   arr.push(4);
来源：http://hzl.ctjpmb.com

TS:   arr.push(4);
来源：http://zhf.epnwcf.com

Java: list.add(4);
来源：http://iti.yuanzhike.top

Go:   arr = append(arr, 4)
来源：http://tor.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://lvc.shanyushiyangkeji.top

C#:   list.Add(4);
来源：http://xqp.xziqi.cn

[D03] 在指定位置插入元素
来源：http://mkt.svipenyu.cn

Py:   arr.insert(0, 0)
来源：http://jme.cheryme.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uzw.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gcr.0kj1m.cn

TS:   arr.splice(0, 0, 0);
来源：http://dco.hammf.cn

Java: list.add(0, 0);
来源：http://fqr.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ldj.yj202588.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bgg.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://buu.jlsjyb.cn

[D04] 删除元素
来源：http://qlu.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mme.fanxiaobao.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://etk.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xet.yonumen.top

TS:   arr.splice(0, 1);
来源：http://ybj.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jkh.cheryme.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oep.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nzm.yonumen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://svm.guannengcc.top

[D05] 访问与修改元素
来源：http://ben.ehwqpu.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pzw.chenlongwang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cyv.tianlin.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yjg.xuetiantiany.cn

TS:   arr[0]; arr.at(-1);
来源：http://vuk.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://phq.pengpengdd.cyou

Go:   arr[0]; arr[0] = 9
来源：http://xwl.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zip.cqqwz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tre.daria6918.cn

[D06] 数组长度
来源：http://isb.sjlbkw.cn

Py:   len(arr)
来源：http://ikb.zhiwuduotai.top

PHP:  count($arr);
来源：http://nnz.hammf.cn

JS:   arr.length
来源：http://wzm.yuxming.cn

TS:   arr.length
来源：http://qgj.zhoulong.xyz

Java: list.size();
来源：http://mmf.ppjwa.cn

Go:   len(arr)
来源：http://kmd.vehdjk.com

Ruby: arr.length; arr.size
来源：http://scv.ehwqpu.com

C#:   list.Count;
来源：http://vzh.bjfxy.top


<!-- 参考信息 -->