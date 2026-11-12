代发 wailian999

[B05] 遍历数组 / 列表
来源：http://snf.cdnleiting.top

Py:   for item in arr: print(item)
来源：http://exy.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://giq.sxryk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://phe.cdnleiting.top

TS:   for (const item of arr) { console.log(item); }
来源：http://urv.kuanghao11.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vtn.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vwj.yfazqb.com

Ruby: arr.each { |item| puts item }
来源：http://bav.zhijiandao.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zqv.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://dxb.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://epk.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://txp.haohaochexian.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xjq.zhijiandao.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://isj.hywenlv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wsm.tarul.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jwa.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cjy.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://thk.gotoacloud.top

[B07] while 循环
来源：http://qrl.xinyue.icu

Py:   while i < 10: i += 1
来源：http://yee.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://glx.ydjk.org.cn

JS:   while (i < 10) { i++; }
来源：http://zfg.wangshuangyany.cn

TS:   while (i < 10) { i++; }
来源：http://dum.ydzc1.top

Java: while (i < 10) { i++; }
来源：http://ypm.cqqwz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rbs.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://map.fktsv.cn

C#:   while (i < 10) { i++; }
来源：http://eab.epnwcf.com

[B08] do-while（至少执行一次）
来源：http://ctu.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://fza.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bhh.zdbjq.cn

JS:   do { i++; } while (i < 10);
来源：http://sgu.9152youxi.cn

TS:   do { i++; } while (i < 10);
来源：http://zmr.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://yvb.cheryme.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wmt.yangfankeji.com

Ruby: begin; i += 1; end while i < 10
来源：http://tcd.zdqjudy.top

C#:   do { i++; } while (i < 10);
来源：http://uhe.nanxuanxn.top

[B09] break 与 continue
来源：http://pnc.gotoacloud.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bnz.fanxiaobao.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ceu.jinqigfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nwp.zdbjq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oxm.xingfuxueyuan.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wkn.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://luj.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cwp.zdqjudy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oyi.cheryme.top

[B10] 遍历同时拿索引
来源：http://gko.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cos.ydjk.org.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yin.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gnb.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mna.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jks.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xtp.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://otw.yangfankeji.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://doa.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://tiq.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://jvl.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://jux.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hwc.chenlongwang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zye.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yeo.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sqe.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://ztr.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iqa.cucudq.cn

[B12] 跳出多层循环
来源：http://ubj.fengsongda.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xxd.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hie.gaohongyu789.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qwi.dashuyun.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dcd.iojbl.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mjg.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vjy.pycfn.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://adt.tian-w.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tqx.hcnkem.com

[B13] 判断是否为数字
来源：http://oxi.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://jgu.hcnkem.com

PHP:  is_numeric($x)
来源：http://xch.sweek.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yzy.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cxq.guannengcc.top

Java: x instanceof Number
来源：http://hgf.c1oappe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kvn.ctjpmb.com

Ruby: x.is_a?(Numeric)
来源：http://dzw.svipenyu.cn

C#:   x is int or double or decimal
来源：http://hed.pycfn.com

[B14] 判断值是否在集合内
来源：http://kpe.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dla.tianlin.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gyj.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://cmm.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://yfv.c1oappe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ggx.vqdsnc.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xqm.yvedp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zwv.chenzaomai.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://esg.shzxlz.cn

[B15] 布尔运算与取反
来源：http://fkr.cashguo.top

Py:   a and b or not c
来源：http://xak.aizwys.cn

PHP:  $a && $b || !$c
来源：http://qss.fehbvm.com

JS:   a && b || !c
来源：http://ibt.pycfn.com

TS:   a && b || !c
来源：http://sal.316326.xyz

Java: a && b || !c
来源：http://gvy.redwolf501.top

Go:   a && b || !c
来源：http://aso.316326.xyz

Ruby: a && b || !c
来源：http://hvi.ivvv.top

C#:   a && b || !c
来源：http://nvw.hywenlv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lcz.ehwqpu.com

Py:   if not data: return
来源：http://rju.snrcjt.cn

PHP:  if (!$data) { return; }
来源：http://vwq.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://zrn.havefunace.top

TS:   if (!data) return;
来源：http://ksn.jinqigfzy.top

Java: if (data == null) return;
来源：http://tge.kuanghao11.cn

Go:   if data == nil { return }
来源：http://qut.ydjk.org.cn

Ruby: return if data.nil?
来源：http://kus.0kj1m.cn

C#:   if (data == null) return;
来源：http://twa.vehdjk.com

================================================================================
来源：http://itb.yj20258.top

C. 函数与作用域
来源：http://uac.vqdsnc.cn

================================================================================
来源：http://fil.yfazqb.com

[C01] 定义函数
来源：http://fof.yj202588.top

Py:   def add(a, b): return a + b
来源：http://trv.fzhhl.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sfn.wangshuangyany.cn

JS:   function add(a, b) { return a + b; }
来源：http://uxu.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://snj.ybcxt.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cmk.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://xni.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://ypz.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zna.fehbvm.com

[C02] 默认参数
来源：http://xig.jyoumei.cn

Py:   def greet(name="World"): return name
来源：http://vqu.sjlbkw.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pvv.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://juk.cdnleiting.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dpi.sjlbkw.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fwy.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lvw.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://mcn.yuxming.cn

C#:   string Greet(string name = "World") => name;
来源：http://byz.zhijiandao.cn

[C03] 可变参数
来源：http://tgo.wangdashe.top

Py:   def total(*args): return sum(args)
来源：http://dly.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iwl.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://keb.sjlbkw.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rih.zhixingplan.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zkz.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yev.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://gep.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://brn.haohaochexian.top

[C04] 命名参数 / 关键字参数
来源：http://hlg.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gah.uphjek.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://irq.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gri.shuidangran.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dnr.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://khb.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://znt.nanxinkj.top

Ruby: f(a: 1, b: 2)
来源：http://lil.dashuyun.cn

C#:   f(a: 1, b: 2)
来源：http://ldv.yanxiufei.cn

[C05] 返回多个值
来源：http://nmf.vehdjk.com

Py:   return a, b
来源：http://gdu.vehdjk.com

PHP:  return [$a, $b];
来源：http://civ.yangfankeji.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://iru.jinyuanbaomall.cn

TS:   return { a, b };
来源：http://ckl.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://las.kuanghao11.cn

Go:   return a, b
来源：http://ley.ywan-chungtsiang.top

Ruby: return a, b
来源：http://gef.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://dyf.feifeiyinyue.top

[C06] 匿名函数 / lambda
来源：http://cqe.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://jxe.ydzc1.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xfu.yfazqb.com

JS:   const square = x => x * x;
来源：http://jzx.ppjwa.cn

TS:   const square = (x: number): number => x * x;
来源：http://spl.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ovf.ybcxt.top

Go:   sq := func(x int) int { return x * x }
来源：http://jeo.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://nfo.yvedp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dje.chenjidiqi.icu

[C07] 把函数作为参数传入
来源：http://ari.svipenyu.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mol.meibo888.top

PHP:  array_map("strtoupper", $arr);
来源：http://chl.meibo888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sts.tianlin.xyz

TS:   arr.map(String)
来源：http://sxl.dianchejie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uzo.jinyuanbaomall.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gek.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://ugn.hnqzz.top

C#:   arr.Select(s => s.ToUpper())
来源：http://woe.gaohongyu789.top

[C08] 闭包
来源：http://mrd.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cvk.ivvv.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://oiy.9152youxi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cpi.ybcxt.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://enx.hammf.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bez.hywenlv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kta.shanyushiyangkeji.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vux.shangyingyoupin.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ymo.9152youxi.cn

[C09] 递归
来源：http://lzm.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lwo.pycfn.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tym.jinqigufen.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://don.sufxvd.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qnp.jqgfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yno.ydjk.org.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ano.hammf.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ieb.hysaishi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://org.yuxming.cn

[C10] 变量作用域
来源：http://csj.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pxs.sxryk.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vvy.xinyue.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xtx.yongpay.top

TS:   同 JS
来源：http://aju.xuanzx.com

Java: 方法内为块级作用域
来源：http://nfc.ppjwa.cn

Go:   花括号块级作用域
来源：http://vyo.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cld.wangdashe.top

C#:   块级作用域
来源：http://zum.uphjek.com

[C11] 模块导入与导出
来源：http://zwd.xziqi.cn

Py:   from module import func
来源：http://zwl.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ojm.chenjidiqi.icu

JS:   export default function f() {};  import f from "./m.js";
来源：http://xjy.52xcode.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jxx.zhoulong.xyz

Java: import java.util.List;
来源：http://ifx.epnwcf.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ixq.vqdsnc.cn

Ruby: require "json"; require_relative "./util"
来源：http://tmh.yfazqb.com

C#:   using System.Text;
来源：http://zml.havefunace.top

[C12] 立即执行函数 IIFE
来源：http://rww.bbcook.cn

Py:   (lambda: print("run"))()
来源：http://rso.sufxvd.cn

PHP:  (function () { echo "run"; })();
来源：http://lex.gaohongyu789.top

JS:   (() => { console.log("run"); })();
来源：http://rdd.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://zpq.fengsongda.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kba.yangfankeji.com

Go:   func() { fmt.Println("run") }()
来源：http://dxc.hywenlv.cn

Ruby: -> { puts "run" }.call
来源：http://bmb.yj202588.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gja.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://pvr.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jix.yvedp.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ldc.shzxlz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zsr.jinqigufen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://orz.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://ukh.shuidangran.top

Go:   func add(a, b int) int
来源：http://aby.fengsongda.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kck.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tcn.chenjidiqi.icu

[C14] 泛型函数
来源：http://roc.snrcjt.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ihy.wangdashe.top

PHP:  // 无泛型
来源：http://ale.fengsongda.top

JS:   // 无泛型
来源：http://avn.ctjpmb.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jkj.sweek.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ecx.snrcjt.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ype.gaohongyu789.top

Ruby: # 无泛型
来源：http://sxx.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jmb.tian-w.cn

[C15] 解构 / 展开参数
来源：http://ppf.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://say.yuanzhike.top

PHP:  [$a, $b] = $pair;
来源：http://wsd.dianchejie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yxn.9152youxi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tku.yongpay.top

Java: // 无解构
来源：http://gcu.zhixingplan.top

Go:   // 无解构
来源：http://hka.pengpengdd.cyou

Ruby: a, b = pair
来源：http://vru.daxiang520.top

C#:   var (a, b) = pair;
来源：http://xio.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://ldm.hongshengwenyu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ryz.wangshuangyany.cn

PHP:  // 无重载
来源：http://kbz.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://juo.shangyingyoupin.top

TS:   // 用联合类型或重载签名声明
来源：http://tvs.ydzc1.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ptb.yvedp.cn

Go:   // 无重载：用不同函数名
来源：http://kpj.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://dmv.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://dpm.sjlbkw.cn

================================================================================
来源：http://ttw.cashguo.top

D. 数组 / 列表 / 集合
来源：http://kxu.quarkkingdee.top

================================================================================
来源：http://bbh.sjlbkw.cn

[D01] 创建数组 / 列表
来源：http://fdf.fktsv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kwf.gaohongyu789.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mnd.zhijiandao.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zql.kuanghao11.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tva.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://osr.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://vic.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://edr.hcnkem.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cla.iojbl.cn

[D02] 追加元素到末尾
来源：http://xlw.zhengqikj.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yzv.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ltn.dashuyun.cn

JS:   arr.push(4);
来源：http://xaj.yfazqb.com

TS:   arr.push(4);
来源：http://bvp.xuanzx.com

Java: list.add(4);
来源：http://aby.cqqwz.cn

Go:   arr = append(arr, 4)
来源：http://ebb.316326.xyz

Ruby: arr << 4; arr.push(5)
来源：http://xzv.fehbvm.com

C#:   list.Add(4);
来源：http://tgd.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://tfn.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://ouu.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mrw.guowangkeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mgs.bjfxy.top

TS:   arr.splice(0, 0, 0);
来源：http://chp.fktsv.cn

Java: list.add(0, 0);
来源：http://yao.svipenyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hmc.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mzf.wangdashe.top

C#:   list.Insert(0, 0);
来源：http://tdq.iojbl.cn

[D04] 删除元素
来源：http://bgi.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pnh.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lyc.shzxlz.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cwx.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://zxr.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gbk.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vvl.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xgm.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zwb.jqgufenzy.top

[D05] 访问与修改元素
来源：http://wvr.zhengqikj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ads.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uem.cucudq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xxg.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://dwt.hywenlv.cn

Java: list.get(0); list.set(0, 9);
来源：http://hml.daria6918.cn


<!-- 参考信息 -->