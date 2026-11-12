代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kmy.yonumen.top

[B06] 遍历字典 / 对象
来源：http://qww.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ijt.xylfe.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mmt.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://psf.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hqc.kuanghao11.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jpv.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://deh.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ccb.ybcxt.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hjp.uphjek.com

[B07] while 循环
来源：http://ywn.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://dmp.jinqigufen.top

PHP:  while ($i < 10) { $i++; }
来源：http://tlx.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://mrv.cqqwz.cn

TS:   while (i < 10) { i++; }
来源：http://ztj.yongpay.top

Java: while (i < 10) { i++; }
来源：http://ahf.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://svv.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://ful.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://wbh.pycfn.com

[B08] do-while（至少执行一次）
来源：http://pbf.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://oub.guannengcc.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lht.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://epg.jlsjyb.cn

TS:   do { i++; } while (i < 10);
来源：http://ulr.hcnkem.com

Java: do { i++; } while (i < 10);
来源：http://faj.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://rkr.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://cjw.zhengqikj.top

C#:   do { i++; } while (i < 10);
来源：http://btn.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://eab.xinyue.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gpd.havefunace.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qjf.ivvv.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xix.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xvx.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cyo.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sin.bbcook.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dez.feifeiyinyue.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nvz.xuetiantiany.cn

[B10] 遍历同时拿索引
来源：http://qlv.smart0.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uth.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uxb.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vqn.jiagoushi.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dyw.yanxiufei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iuo.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ayr.bjfxy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://slc.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fqc.9152youxi.cn

[B11] 生成数字序列 / 区间
来源：http://nre.gogol.net.cn

Py:   list(range(0, 10, 2))
来源：http://hnx.tianlin.xyz

PHP:  range(0, 10, 2);
来源：http://txp.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://arp.ehwqpu.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iyu.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tgy.wangdashe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wro.yj20258.top

Ruby: (0...10).step(2).to_a
来源：http://wgi.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://avg.epnwcf.com

[B12] 跳出多层循环
来源：http://ijz.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://knz.chenjidiqi.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://trh.fengsongda.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mxr.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ebk.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://evh.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ylm.shuidangran.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vhs.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zoj.yj20258888.top

[B13] 判断是否为数字
来源：http://ppl.ybcxt.top

Py:   isinstance(x, (int, float))
来源：http://mzr.gotoacloud.top

PHP:  is_numeric($x)
来源：http://pjd.fzhhl.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sbf.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qob.wangdashe.top

Java: x instanceof Number
来源：http://lyk.hesvh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zph.yanxiufei.cn

Ruby: x.is_a?(Numeric)
来源：http://cig.sjlbkw.cn

C#:   x is int or double or decimal
来源：http://hgy.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://wsv.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ytd.birdmap.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wlb.snrcjt.cn

JS:   [1, 2, 3].includes(x)
来源：http://tkf.tarul.cn

TS:   [1, 2, 3].includes(x)
来源：http://hao.ctjpmb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://oxb.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mup.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://bbd.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qho.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://msl.mhx1999.top

Py:   a and b or not c
来源：http://rqf.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://qcl.daria6918.cn

JS:   a && b || !c
来源：http://cgu.gogol.net.cn

TS:   a && b || !c
来源：http://iim.iojbl.cn

Java: a && b || !c
来源：http://zud.tian-w.cn

Go:   a && b || !c
来源：http://rqd.vqdsnc.cn

Ruby: a && b || !c
来源：http://rtg.pycfn.com

C#:   a && b || !c
来源：http://gjq.jinyuanbaomall.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bpq.jlsjyb.cn

Py:   if not data: return
来源：http://pvz.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://qco.cheryme.top

JS:   if (!data) return;
来源：http://vtt.hysaishi.cn

TS:   if (!data) return;
来源：http://vdl.wangshuangyany.cn

Java: if (data == null) return;
来源：http://hmu.gaohongyu789.top

Go:   if data == nil { return }
来源：http://yat.kuanghao11.cn

Ruby: return if data.nil?
来源：http://wrc.bbcook.cn

C#:   if (data == null) return;
来源：http://ywo.ywan-chungtsiang.top

================================================================================
来源：http://rjz.sysykeji.top

C. 函数与作用域
来源：http://lif.yuanzhike.top

================================================================================
来源：http://gvi.nanxuanxn.top

[C01] 定义函数
来源：http://bav.xingfuxueyuan.xyz

Py:   def add(a, b): return a + b
来源：http://lve.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fxe.hnqzz.top

JS:   function add(a, b) { return a + b; }
来源：http://apu.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cnm.yvedp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://iwz.meibo888.top

Go:   func add(a, b int) int { return a + b }
来源：http://nbe.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://bil.jiagoushi.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mhk.zhongyouzk.top

[C02] 默认参数
来源：http://afz.vqdsnc.cn

Py:   def greet(name="World"): return name
来源：http://szx.sjlbkw.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tgr.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://llf.fktsv.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://yay.wangdashe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ulz.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xzr.tianlin.xyz

Ruby: def greet(name = "World") = name
来源：http://xew.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://dph.cucudq.cn

[C03] 可变参数
来源：http://peq.yuanzhike.top

Py:   def total(*args): return sum(args)
来源：http://jte.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jzk.tarul.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fmv.sjlbkw.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jwj.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zvk.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pxy.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://rzz.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://teq.fehbvm.com

[C04] 命名参数 / 关键字参数
来源：http://lsl.pycfn.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zxj.dianchejie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nmc.jinqigfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aqm.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kar.sufxvd.cn

Java: // 无：用 Builder 模式或 record
来源：http://gea.vehdjk.com

Go:   // 无：用配置结构体参数
来源：http://grd.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://qcj.zdbjq.cn

C#:   f(a: 1, b: 2)
来源：http://qpb.chenjidiqi.icu

[C05] 返回多个值
来源：http://qbm.vehdjk.com

Py:   return a, b
来源：http://oiw.ehwqpu.com

PHP:  return [$a, $b];
来源：http://gha.shanyushiyangtech.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vxh.birdmap.top

TS:   return { a, b };
来源：http://ouc.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bxc.guowangkeji.top

Go:   return a, b
来源：http://kgd.dashuyun.cn

Ruby: return a, b
来源：http://fmi.52xcode.cn

C#:   return (a, b);              // ValueTuple
来源：http://ipy.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://fjl.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://woy.hywenlv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://jzh.yuanzhike.top

JS:   const square = x => x * x;
来源：http://ydm.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://pyy.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://moz.jinqigfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://zhd.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://fuk.yongpay.top

C#:   Func<int, int> square = x => x * x;
来源：http://lgv.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://gul.yfazqb.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ppu.gzhubu.top

PHP:  array_map("strtoupper", $arr);
来源：http://gws.jqgfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ehl.quarkkingdee.top

TS:   arr.map(String)
来源：http://yvx.tanke756.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xxq.sjlbkw.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://utn.zdqjudy.top

Ruby: arr.map(&:upcase)
来源：http://jck.gotoacloud.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tts.yfazqb.com

[C08] 闭包
来源：http://vlf.daria6918.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://tvh.dianchejie.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://axd.jiagoushi.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iab.zhongyouzk.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rie.nanxinkj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://que.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zvt.ehwqpu.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://alb.tanke756.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kwa.zhijiandao.cn

[C09] 递归
来源：http://gdy.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://oej.xziqi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cpj.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oyu.andypj.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oio.cdnleiting.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://yee.fehbvm.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://git.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://odk.jinyuanbaomall.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://edg.c1oappe.top

[C10] 变量作用域
来源：http://ott.yfazqb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://sbb.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fwm.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jpk.zhijiandao.cn

TS:   同 JS
来源：http://ccz.ppjwa.cn

Java: 方法内为块级作用域
来源：http://tgp.iojbl.cn

Go:   花括号块级作用域
来源：http://mfg.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pvb.sufxvd.cn

C#:   块级作用域
来源：http://vah.hywenlv.cn

[C11] 模块导入与导出
来源：http://wew.fktsv.cn

Py:   from module import func
来源：http://rnl.zhoulong.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://fcx.tianlin.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://mcc.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yzw.yueranfly.top

Java: import java.util.List;
来源：http://gni.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://izw.vehdjk.com

Ruby: require "json"; require_relative "./util"
来源：http://mfr.jinqigufen.top

C#:   using System.Text;
来源：http://thj.yfazqb.com

[C12] 立即执行函数 IIFE
来源：http://kmk.sufxvd.cn

Py:   (lambda: print("run"))()
来源：http://ekf.tarul.cn

PHP:  (function () { echo "run"; })();
来源：http://ofa.cqqwz.cn

JS:   (() => { console.log("run"); })();
来源：http://ugx.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://gus.kuanghao11.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zbb.xuetiantiany.cn

Go:   func() { fmt.Println("run") }()
来源：http://jau.yonumen.top

Ruby: -> { puts "run" }.call
来源：http://rbj.birdmap.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bdn.hywenlv.cn

[C13] 类型声明 / 类型注解
来源：http://lfj.shanyushiyangtech.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gfr.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xep.fengsongda.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://txk.hongshengwenyu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rcd.quarkkingdee.top

Java: int add(int a, int b) { return a + b; }
来源：http://toh.jiagoushi.top

Go:   func add(a, b int) int
来源：http://qnx.jlsjyb.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ove.guowangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://lrf.bbcook.cn

[C14] 泛型函数
来源：http://oav.birdmap.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xcj.ydjk.org.cn

PHP:  // 无泛型
来源：http://cjn.ivvv.top

JS:   // 无泛型
来源：http://wub.hnxiangtu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vvm.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cet.jlsjyb.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ghi.tanke756.top

Ruby: # 无泛型
来源：http://qiy.xylfe.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hhx.ppjwa.cn

[C15] 解构 / 展开参数
来源：http://apm.yj202588.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ipw.shanyushiyangkeji.top

PHP:  [$a, $b] = $pair;
来源：http://isl.mhx1999.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cxr.havefunace.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://eef.gogol.net.cn

Java: // 无解构
来源：http://dir.jlsjyb.cn

Go:   // 无解构
来源：http://oet.hywenlv.cn

Ruby: a, b = pair
来源：http://zhs.nanxuanxn.top

C#:   var (a, b) = pair;
来源：http://hxi.kuanghao11.cn

[C16] 函数 / 方法重载
来源：http://tvt.dashuyun.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zgl.zhiwuduotai.top

PHP:  // 无重载
来源：http://aoy.cucudq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vwl.haohaochexian.top

TS:   // 用联合类型或重载签名声明
来源：http://afa.wangdashe.top

Java: void f(int a) {}  void f(String a) {}
来源：http://znb.yfazqb.com

Go:   // 无重载：用不同函数名
来源：http://gwo.redwolf501.top

Ruby: # 无重载：靠动态参数
来源：http://ywi.xingfuxueyuan.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://krf.feifeiyinyue.top

================================================================================
来源：http://czk.guowangkeji.top

D. 数组 / 列表 / 集合
来源：http://xep.sufxvd.cn

================================================================================
来源：http://ops.bjfxy.top

[D01] 创建数组 / 列表
来源：http://rcv.nanxinkj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rih.meibo888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yst.yfazqb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://flu.bjfxy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wqz.fengsongda.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://feg.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://jyx.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://rvh.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kol.shzxlz.cn

[D02] 追加元素到末尾
来源：http://uhu.chenjidiqi.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kky.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xrp.gotoacloud.top

JS:   arr.push(4);
来源：http://bww.haohaochexian.top

TS:   arr.push(4);
来源：http://zld.ctjpmb.com

Java: list.add(4);
来源：http://fay.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://nby.birdmap.top

Ruby: arr << 4; arr.push(5)
来源：http://ptz.sxryk.cn

C#:   list.Add(4);
来源：http://inp.zhaomingkeji.xyz

[D03] 在指定位置插入元素
来源：http://xqu.jlsjyb.cn

Py:   arr.insert(0, 0)
来源：http://rpv.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nbq.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nmv.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://ilg.xuetiantiany.cn

Java: list.add(0, 0);
来源：http://ivv.yj20258888.top

Go:   arr = append([]int{0}, arr...)
来源：http://bxd.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ker.fzhhl.top

C#:   list.Insert(0, 0);
来源：http://pjb.gotoacloud.top

[D04] 删除元素
来源：http://rsk.zycfv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ckx.sufxvd.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://syi.jqgufenzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lnp.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://nyi.yongpay.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sov.gotoacloud.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ucx.hfpthk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aby.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aoj.fanxiaobao.xyz

[D05] 访问与修改元素
来源：http://xxv.xinyue.icu

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://axv.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yet.yfazqb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wgt.chenzaomai.com

TS:   arr[0]; arr.at(-1);
来源：http://npm.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://dii.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://bqp.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://obr.fzhhl.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qzw.gaohongyu789.top

[D06] 数组长度
来源：http://yks.yuxming.cn

Py:   len(arr)
来源：http://cnd.fktsv.cn

PHP:  count($arr);
来源：http://vju.hesvh.cn

JS:   arr.length
来源：http://bqo.9152youxi.cn

TS:   arr.length
来源：http://txq.jqgfzy.top


<!-- 参考信息 -->