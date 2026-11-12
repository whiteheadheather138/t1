代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aft.svipenyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vdc.sweek.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://off.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tdh.zhixingplan.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://okd.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tfp.zycfv.cn

[B03] switch / match / case
来源：http://cfb.zhaomingkeji.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cjp.jlsjyb.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wim.ydjk.org.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aqv.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://thp.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jqw.yanxiufei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://prn.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uzc.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gat.tianlin.xyz

[B04] for 计数循环
来源：http://gfv.guowangkeji.top

Py:   for i in range(10): print(i)
来源：http://kkc.pengpengdd.cyou

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vfq.shanyushiyangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sui.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wdi.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tum.uphjek.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lsm.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://vsa.zhoulong.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qjq.snrcjt.cn

[B05] 遍历数组 / 列表
来源：http://mzt.ydzc1.top

Py:   for item in arr: print(item)
来源：http://rmu.cashguo.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kei.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dsa.hesvh.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://nzp.yuxming.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tkp.smart0.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wdo.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://jmf.fzhhl.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zza.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://qyy.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mun.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pwf.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dam.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qux.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zlh.yvedp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vzg.nanxinkj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ytr.ywan-chungtsiang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mbu.jlsjyb.cn

[B07] while 循环
来源：http://cdv.bbcook.cn

Py:   while i < 10: i += 1
来源：http://fnm.meibo888.top

PHP:  while ($i < 10) { $i++; }
来源：http://ybu.hnxiangtu.top

JS:   while (i < 10) { i++; }
来源：http://ijr.xingfuxueyuan.xyz

TS:   while (i < 10) { i++; }
来源：http://kwu.tarul.cn

Java: while (i < 10) { i++; }
来源：http://nrp.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fsg.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://vgy.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://bsx.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://ncj.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://ukv.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wom.feifeiyinyue.top

JS:   do { i++; } while (i < 10);
来源：http://dap.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://uku.haohaochexian.top

Java: do { i++; } while (i < 10);
来源：http://cch.zhiwuduotai.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vnh.fehbvm.com

Ruby: begin; i += 1; end while i < 10
来源：http://xtg.smart0.xyz

C#:   do { i++; } while (i < 10);
来源：http://gwx.9152youxi.cn

[B09] break 与 continue
来源：http://aor.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vpo.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gvm.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cyt.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://but.ppjwa.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zke.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ame.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xhk.jiagoushi.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mtf.meibo888.top

[B10] 遍历同时拿索引
来源：http://soy.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://opg.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sxf.yj20258.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eyb.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pnl.guowangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zav.hfpthk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hga.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uys.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qhb.hnxiangtu.top

[B11] 生成数字序列 / 区间
来源：http://iyp.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://avc.jinyuanbaomall.cn

PHP:  range(0, 10, 2);
来源：http://efu.snrcjt.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qjz.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jcd.haohaochexian.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dhm.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ywc.gogol.net.cn

Ruby: (0...10).step(2).to_a
来源：http://chi.hcnkem.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zmf.dianchejie.cn

[B12] 跳出多层循环
来源：http://hen.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://lgx.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xbz.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jeu.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hza.dashuyun.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tio.hongshengwenyu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://duq.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lmp.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://koi.sxryk.cn

[B13] 判断是否为数字
来源：http://ppd.0kj1m.cn

Py:   isinstance(x, (int, float))
来源：http://rwk.havefunace.top

PHP:  is_numeric($x)
来源：http://rmf.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gzt.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lro.ppjwa.cn

Java: x instanceof Number
来源：http://dnz.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cse.yvedp.cn

Ruby: x.is_a?(Numeric)
来源：http://igr.yuxming.cn

C#:   x is int or double or decimal
来源：http://xab.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://wqz.ybcxt.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pdl.hongshengwenyu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vvy.hcnkem.com

JS:   [1, 2, 3].includes(x)
来源：http://tte.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://cls.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://viu.fengsongda.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qhv.zhongyouzk.top

Ruby: [1, 2, 3].include?(x)
来源：http://lne.ybcxt.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ebd.fktsv.cn

[B15] 布尔运算与取反
来源：http://yju.ybcxt.top

Py:   a and b or not c
来源：http://qat.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://wat.snrcjt.cn

JS:   a && b || !c
来源：http://yaq.zhijiandao.cn

TS:   a && b || !c
来源：http://rzg.yj20258.top

Java: a && b || !c
来源：http://sxr.andypj.xyz

Go:   a && b || !c
来源：http://riz.yangfankeji.com

Ruby: a && b || !c
来源：http://cbt.zhaomingkeji.xyz

C#:   a && b || !c
来源：http://nbz.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://xhi.quarkkingdee.top

Py:   if not data: return
来源：http://kgx.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://tan.havefunace.top

JS:   if (!data) return;
来源：http://nau.fanxiaobao.xyz

TS:   if (!data) return;
来源：http://equ.xylfe.cn

Java: if (data == null) return;
来源：http://kor.chenjidiqi.icu

Go:   if data == nil { return }
来源：http://azm.yonumen.top

Ruby: return if data.nil?
来源：http://bzz.meibo888.top

C#:   if (data == null) return;
来源：http://ayh.hammf.cn

================================================================================
来源：http://pbg.zhijiandao.cn

C. 函数与作用域
来源：http://mcr.vqdsnc.cn

================================================================================
来源：http://ahc.vqdsnc.cn

[C01] 定义函数
来源：http://rot.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://dvu.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ztk.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://ory.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zaq.shanyushiyangtech.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mwf.ehwqpu.com

Go:   func add(a, b int) int { return a + b }
来源：http://jnc.hesvh.cn

Ruby: def add(a, b); a + b; end
来源：http://wqr.fktsv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yrv.c1oappe.top

[C02] 默认参数
来源：http://pac.chenjidiqi.icu

Py:   def greet(name="World"): return name
来源：http://jcj.ybcxt.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kgv.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://eoa.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uvl.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vfa.redwolf501.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://toq.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://mjc.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://qgb.sjlbkw.cn

[C03] 可变参数
来源：http://mlu.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://eom.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jqv.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sej.ehwqpu.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fqo.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qyl.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jmn.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://bvx.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vjq.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://vak.meibo888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xsy.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zep.ybcxt.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eji.fktsv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aux.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://hxz.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://dlu.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://kgk.jianghu66.top

C#:   f(a: 1, b: 2)
来源：http://ggu.sweek.top

[C05] 返回多个值
来源：http://zfw.guowangkeji.top

Py:   return a, b
来源：http://bxx.jyoumei.cn

PHP:  return [$a, $b];
来源：http://hcx.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iux.tianlin.xyz

TS:   return { a, b };
来源：http://qzl.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://puc.zhiwuduotai.top

Go:   return a, b
来源：http://tap.zhongyouzk.top

Ruby: return a, b
来源：http://kwq.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://onq.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://cdp.yj20258.top

Py:   square = lambda x: x * x
来源：http://kvt.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://riv.xziqi.cn

JS:   const square = x => x * x;
来源：http://fme.jinghuilouyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://vxx.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fes.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zpu.dianchejie.cn

Ruby: square = ->(x) { x * x }
来源：http://uzo.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://sqb.zhaomingkeji.xyz

[C07] 把函数作为参数传入
来源：http://fxq.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ats.xuanzx.com

PHP:  array_map("strtoupper", $arr);
来源：http://ukf.nwbrower.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jsv.9152youxi.cn

TS:   arr.map(String)
来源：http://tey.cucudq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ycp.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mup.yvedp.cn

Ruby: arr.map(&:upcase)
来源：http://mno.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zov.snrcjt.cn

[C08] 闭包
来源：http://ore.quarkkingdee.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qko.yj20258888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jku.wangdashe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://opb.daria6918.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wkt.birdmap.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://lxt.yonumen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jqs.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dwe.sufxvd.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://akv.xinyue.icu

[C09] 递归
来源：http://qus.zycfv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xst.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dsl.aizwys.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tej.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://umu.ehwqpu.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zfa.tanke756.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rsj.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cvv.sjlbkw.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ezn.sjlbkw.cn

[C10] 变量作用域
来源：http://rxl.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wiy.yfazqb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ien.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ggc.xuanzx.com

TS:   同 JS
来源：http://kgb.shanyushiyangtech.top

Java: 方法内为块级作用域
来源：http://gzt.smart0.xyz

Go:   花括号块级作用域
来源：http://uyu.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gjy.yj20258888.top

C#:   块级作用域
来源：http://hpn.hammf.cn

[C11] 模块导入与导出
来源：http://svd.jinqigfzy.top

Py:   from module import func
来源：http://dvi.guowangkeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://mgf.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://zhw.chenzaomai.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fby.jinqigfzy.top

Java: import java.util.List;
来源：http://nxb.zhijiandao.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hfu.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://xvi.nanxinkj.top

C#:   using System.Text;
来源：http://clr.xuanzx.com

[C12] 立即执行函数 IIFE
来源：http://zbo.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://ypv.cucudq.cn

PHP:  (function () { echo "run"; })();
来源：http://kir.zhixingplan.top

JS:   (() => { console.log("run"); })();
来源：http://etj.hnxiangtu.top

TS:   (() => { console.log("run"); })();
来源：http://imj.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sry.xuanzx.com

Go:   func() { fmt.Println("run") }()
来源：http://qgo.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://fhg.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rub.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://ebf.yj20258.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xmh.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bwg.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tlu.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ydk.birdmap.top

Java: int add(int a, int b) { return a + b; }
来源：http://ypf.hcnkem.com

Go:   func add(a, b int) int
来源：http://csz.meibo888.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bnu.jiagoushi.top

C#:   int Add(int a, int b) => a + b;
来源：http://oka.tianlin.xyz

[C14] 泛型函数
来源：http://crx.tanke756.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://urt.zdbjq.cn

PHP:  // 无泛型
来源：http://mej.tanke756.top

JS:   // 无泛型
来源：http://nnj.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lux.0kj1m.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pka.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mro.fzhhl.top

Ruby: # 无泛型
来源：http://mpt.vehdjk.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hep.hnxiangtu.top

[C15] 解构 / 展开参数
来源：http://clx.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qwf.hywenlv.cn

PHP:  [$a, $b] = $pair;
来源：http://dni.ydjk.org.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qug.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hgi.ybcxt.top

Java: // 无解构
来源：http://ymb.c1oappe.top

Go:   // 无解构
来源：http://bae.bjfxy.top

Ruby: a, b = pair
来源：http://kww.52xcode.cn

C#:   var (a, b) = pair;
来源：http://ozj.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://hvo.nanxinkj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fxn.zhaomingkeji.xyz

PHP:  // 无重载
来源：http://upp.zhengqikj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bkc.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://ywo.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jck.ivvv.top

Go:   // 无重载：用不同函数名
来源：http://pic.sysykeji.top

Ruby: # 无重载：靠动态参数
来源：http://vqj.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mxl.zdbjq.cn

================================================================================
来源：http://qxh.yuanzhike.top

D. 数组 / 列表 / 集合
来源：http://lwq.epnwcf.com

================================================================================
来源：http://sof.daxiang520.top

[D01] 创建数组 / 列表
来源：http://eft.jinqigufen.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bqc.mhx1999.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lyg.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vla.epnwcf.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://nej.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lta.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://pjq.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://eij.pengpengdd.cyou

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://upo.cucudq.cn

[D02] 追加元素到末尾
来源：http://fwb.316326.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jwo.dianchejie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ugi.nanxuanxn.top

JS:   arr.push(4);
来源：http://eyw.hammf.cn

TS:   arr.push(4);
来源：http://zuv.jqgfzy.top

Java: list.add(4);
来源：http://ucc.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://mvq.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://dzv.jiagoushi.top

C#:   list.Add(4);
来源：http://mxv.aibaodan.cn


<!-- 参考信息 -->