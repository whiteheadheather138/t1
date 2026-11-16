代发 wailian999

Py:   for i in range(10): print(i)
来源：http://hbc.zhoulong.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mur.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aze.xylfe.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://loh.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hmv.9152youxi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://izg.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://xhf.jlsjyb.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hfe.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://vua.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://tta.jlsjyb.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vpk.nanxinkj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ttg.aibaodan.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uhi.zhixingplan.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wju.ywan-chungtsiang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wss.xingfuxueyuan.xyz

Ruby: arr.each { |item| puts item }
来源：http://hkm.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://agw.cdnleiting.top

[B06] 遍历字典 / 对象
来源：http://roy.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ixf.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vxx.vqdsnc.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xjw.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ehq.gzhubu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mbs.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rso.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rtw.yueranfly.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qti.gaohongyu789.top

[B07] while 循环
来源：http://ohh.dashuyun.cn

Py:   while i < 10: i += 1
来源：http://nac.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://wix.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://rui.jiagoushi.top

TS:   while (i < 10) { i++; }
来源：http://ahy.birdmap.top

Java: while (i < 10) { i++; }
来源：http://xfv.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zzh.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://zba.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://atg.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://gtc.vqdsnc.cn

Py:   # 无 do-while：用 while True + break
来源：http://pdy.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rtj.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://srz.ppjwa.cn

TS:   do { i++; } while (i < 10);
来源：http://zbb.fktsv.cn

Java: do { i++; } while (i < 10);
来源：http://thg.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xsp.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://scd.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://gpq.chenzaomai.com

[B09] break 与 continue
来源：http://tbp.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nkn.shzxlz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://okg.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wiq.jinqigufen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qlt.dashuyun.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmm.shanyushiyangtech.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eze.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://myj.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://off.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://koh.zhoulong.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ems.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blv.daxiang520.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jqz.yueranfly.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uvb.zhengqikj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ljg.hysaishi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lsj.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fpo.jinghuilouyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://swx.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://rsa.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://ziw.yongpay.top

PHP:  range(0, 10, 2);
来源：http://gov.yuxming.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nuz.sufxvd.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ebj.zhiwuduotai.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zwx.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://drk.uphjek.com

Ruby: (0...10).step(2).to_a
来源：http://uvo.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dxn.zhiwuduotai.top

[B12] 跳出多层循环
来源：http://vrl.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://spr.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cbt.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lgi.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hua.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pwu.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aun.snrcjt.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ege.redwolf501.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vqw.zhixingplan.top

[B13] 判断是否为数字
来源：http://and.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://rdu.zhoulong.xyz

PHP:  is_numeric($x)
来源：http://pbu.fktsv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nen.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hzi.hywenlv.cn

Java: x instanceof Number
来源：http://ivj.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ira.zhongyouzk.top

Ruby: x.is_a?(Numeric)
来源：http://ouw.ivvv.top

C#:   x is int or double or decimal
来源：http://kym.xinyue.icu

[B14] 判断值是否在集合内
来源：http://ypk.shuidangran.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zsp.sxryk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zyj.zhoulong.xyz

JS:   [1, 2, 3].includes(x)
来源：http://hsa.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://hnf.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nyi.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cdy.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mum.chenlongwang.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://caj.epnwcf.com

[B15] 布尔运算与取反
来源：http://odf.ydzc1.top

Py:   a and b or not c
来源：http://wod.c1oappe.top

PHP:  $a && $b || !$c
来源：http://ezi.yuxming.cn

JS:   a && b || !c
来源：http://lhn.daria6918.cn

TS:   a && b || !c
来源：http://vkq.0kj1m.cn

Java: a && b || !c
来源：http://ody.fanxiaobao.xyz

Go:   a && b || !c
来源：http://oxc.cqqwz.cn

Ruby: a && b || !c
来源：http://bpf.nanxuanxn.top

C#:   a && b || !c
来源：http://cto.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://slh.zhiwuduotai.top

Py:   if not data: return
来源：http://wvs.hywenlv.cn

PHP:  if (!$data) { return; }
来源：http://vfi.hesvh.cn

JS:   if (!data) return;
来源：http://tvd.birdmap.top

TS:   if (!data) return;
来源：http://ujw.hcnkem.com

Java: if (data == null) return;
来源：http://rms.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://uwe.cashguo.top

Ruby: return if data.nil?
来源：http://wju.hcnkem.com

C#:   if (data == null) return;
来源：http://jzt.uphjek.com

================================================================================
来源：http://thp.xinyue.icu

C. 函数与作用域
来源：http://sjl.fengsongda.top

================================================================================
来源：http://ecl.xingfuxueyuan.xyz

[C01] 定义函数
来源：http://ocj.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://guk.shanyushiyangtech.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qdq.tanke756.top

JS:   function add(a, b) { return a + b; }
来源：http://ewt.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://okj.jinghuilouyu.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://wgx.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://ktt.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://cdu.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qmc.chenzaomai.com

[C02] 默认参数
来源：http://web.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://iel.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rqg.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://hig.zhaomingkeji.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://itf.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://miq.cdnleiting.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zyg.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://iqz.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://wue.zycfv.cn

[C03] 可变参数
来源：http://xtu.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://jfq.zhixingplan.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nvm.chenlongwang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qjy.0kj1m.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xnz.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mnw.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://djk.zhaomingkeji.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://agh.redwolf501.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ruh.ivvv.top

[C04] 命名参数 / 关键字参数
来源：http://htx.zhongyouzk.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tps.fzhhl.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zjb.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nej.hnxiangtu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wtv.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://yja.tanke756.top

Go:   // 无：用配置结构体参数
来源：http://lwl.daxiang520.top

Ruby: f(a: 1, b: 2)
来源：http://ynp.tarul.cn

C#:   f(a: 1, b: 2)
来源：http://pob.gogol.net.cn

[C05] 返回多个值
来源：http://cgu.ppjwa.cn

Py:   return a, b
来源：http://hva.jqgufenzy.top

PHP:  return [$a, $b];
来源：http://ggs.0kj1m.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jml.pycfn.com

TS:   return { a, b };
来源：http://deh.ehwqpu.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fdj.xingfuxueyuan.xyz

Go:   return a, b
来源：http://bmq.hfpthk.cn

Ruby: return a, b
来源：http://dqk.zdqjudy.top

C#:   return (a, b);              // ValueTuple
来源：http://ozz.yongpay.top

[C06] 匿名函数 / lambda
来源：http://muc.ivvv.top

Py:   square = lambda x: x * x
来源：http://jrr.dashuyun.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gkn.zdqjudy.top

JS:   const square = x => x * x;
来源：http://nky.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://fnm.yonumen.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hhp.bbcook.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qxr.hywenlv.cn

Ruby: square = ->(x) { x * x }
来源：http://ouz.haohaochexian.top

C#:   Func<int, int> square = x => x * x;
来源：http://new.ehwqpu.com

[C07] 把函数作为参数传入
来源：http://vap.gzhubu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://evs.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ull.ivvv.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://asv.yj202588.top

TS:   arr.map(String)
来源：http://btz.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rjd.shangyingyoupin.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vas.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://mdq.nanxinkj.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pok.zdqjudy.top

[C08] 闭包
来源：http://jcz.andypj.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://iqv.vqdsnc.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qan.jqgufenzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vpx.xziqi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pte.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lgh.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gkf.cashguo.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cfg.uphjek.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xfr.hcnkem.com

[C09] 递归
来源：http://hjl.ywan-chungtsiang.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fhl.sxryk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://enz.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://akh.yvedp.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dco.pycfn.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://prv.yanxiufei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nfz.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nsz.shanyushiyangkeji.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bdn.zhijiandao.cn

[C10] 变量作用域
来源：http://ghr.fehbvm.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://itn.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kav.xylfe.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gmv.pycfn.com

TS:   同 JS
来源：http://tln.yvedp.cn

Java: 方法内为块级作用域
来源：http://rce.hammf.cn

Go:   花括号块级作用域
来源：http://ofn.kuanghao11.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fkf.kuanghao11.cn

C#:   块级作用域
来源：http://xdn.jianghu66.top

[C11] 模块导入与导出
来源：http://ooj.yvedp.cn

Py:   from module import func
来源：http://ber.feifeiyinyue.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wov.yj20258888.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fdl.shangyingyoupin.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cnw.wangshuangyany.cn

Java: import java.util.List;
来源：http://bqi.sweek.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gtm.bbcook.cn

Ruby: require "json"; require_relative "./util"
来源：http://tfi.jinghuilouyu.cn

C#:   using System.Text;
来源：http://pcv.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://oqk.quarkkingdee.top

Py:   (lambda: print("run"))()
来源：http://rpv.yongpay.top

PHP:  (function () { echo "run"; })();
来源：http://tqv.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://cuf.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://dhu.hongshengwenyu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lrv.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://wcw.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://jap.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vvy.cucudq.cn

[C13] 类型声明 / 类型注解
来源：http://rua.yj202588.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qpa.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kjn.fzhhl.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ayx.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eez.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://osy.gogol.net.cn

Go:   func add(a, b int) int
来源：http://wic.ybcxt.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nbs.vehdjk.com

C#:   int Add(int a, int b) => a + b;
来源：http://snx.jinqigufen.top

[C14] 泛型函数
来源：http://vhu.yonumen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ahv.dashuyun.cn

PHP:  // 无泛型
来源：http://jhb.zhongyouzk.top

JS:   // 无泛型
来源：http://vdg.yongpay.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jdw.ctjpmb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jiq.zycfv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tkp.kuanghao11.cn

Ruby: # 无泛型
来源：http://ket.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xaj.tian-w.cn

[C15] 解构 / 展开参数
来源：http://ftv.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://acy.jqgufenzy.top

PHP:  [$a, $b] = $pair;
来源：http://kto.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nxb.yuxming.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://amx.ydzc1.top

Java: // 无解构
来源：http://czp.zhoulong.xyz

Go:   // 无解构
来源：http://fsq.sjlbkw.cn

Ruby: a, b = pair
来源：http://nvl.chenjidiqi.icu

C#:   var (a, b) = pair;
来源：http://qss.wangdashe.top

[C16] 函数 / 方法重载
来源：http://iqk.smart0.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zjk.yuxming.cn

PHP:  // 无重载
来源：http://qsa.bjfxy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://aqh.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://rlr.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lbj.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://huy.guannengcc.top

Ruby: # 无重载：靠动态参数
来源：http://oen.shanyushiyangkeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ofq.xziqi.cn

================================================================================
来源：http://ckv.gaohongyu789.top

D. 数组 / 列表 / 集合
来源：http://gsd.jinqigfzy.top

================================================================================
来源：http://frf.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://uql.ydjk.org.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yce.sxryk.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://czv.jyoumei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://frv.jianghu66.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://tdp.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://idy.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://tey.pengpengdd.cyou

Ruby: arr = [1, 2, 3]
来源：http://hqe.cqqwz.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://eic.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://vqj.yongpay.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://buw.yj20258.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rxk.jianghu66.top

JS:   arr.push(4);
来源：http://pzr.gotoacloud.top

TS:   arr.push(4);
来源：http://hrm.hnqzz.top

Java: list.add(4);
来源：http://wyo.smart0.xyz

Go:   arr = append(arr, 4)
来源：http://xpz.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://yvd.vqdsnc.cn

C#:   list.Add(4);
来源：http://tll.ydzc1.top

[D03] 在指定位置插入元素
来源：http://fig.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://qka.pycfn.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qso.pycfn.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jkl.hammf.cn

TS:   arr.splice(0, 0, 0);
来源：http://qvz.epnwcf.com

Java: list.add(0, 0);
来源：http://zeq.tianlin.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://evb.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iyx.jyoumei.cn

C#:   list.Insert(0, 0);
来源：http://jet.316326.xyz

[D04] 删除元素
来源：http://fgh.ydjk.org.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cem.hcnkem.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yht.zhiwuduotai.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nnz.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://lye.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mqb.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eyj.zhixingplan.top


<!-- 参考信息 -->