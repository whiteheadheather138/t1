代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lxr.chenzaomai.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zyo.ctjpmb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lai.0kj1m.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nwn.xingfuxueyuan.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tzy.dianchejie.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hvb.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gsd.feifeiyinyue.top

[B04] for 计数循环
来源：http://kqd.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://ztj.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pih.ybcxt.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xul.shangyingyoupin.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ewc.zhixingplan.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nhu.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ksj.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://xjo.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zbt.sweek.top

[B05] 遍历数组 / 列表
来源：http://ats.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://rry.xuanzx.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cjb.ivvv.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rtw.yueranfly.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qcl.shanyushiyangtech.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ckx.sxryk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mke.iojbl.cn

Ruby: arr.each { |item| puts item }
来源：http://cls.fzhhl.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://szh.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://ihf.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tpr.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dua.pycfn.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iau.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sul.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ehy.zhengqikj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bso.hesvh.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://slg.feifeiyinyue.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qop.jianghu66.top

[B07] while 循环
来源：http://hat.uphjek.com

Py:   while i < 10: i += 1
来源：http://jhz.zhiwuduotai.top

PHP:  while ($i < 10) { $i++; }
来源：http://lxt.andypj.xyz

JS:   while (i < 10) { i++; }
来源：http://hsg.cucudq.cn

TS:   while (i < 10) { i++; }
来源：http://vfn.jinyuanbaomall.cn

Java: while (i < 10) { i++; }
来源：http://ryy.birdmap.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vij.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://uwj.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://nhl.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://imb.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://uxl.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jfb.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://nvt.shangyingyoupin.top

TS:   do { i++; } while (i < 10);
来源：http://cbc.fanxiaobao.xyz

Java: do { i++; } while (i < 10);
来源：http://sov.jyoumei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gzr.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://vhd.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://szc.sufxvd.cn

[B09] break 与 continue
来源：http://meg.zhiwuduotai.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ggz.nwbrower.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kzg.316326.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://psm.meibo888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nyv.jlsjyb.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zub.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zmz.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nam.daria6918.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dee.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://svw.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iti.hongshengwenyu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jna.aizwys.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ckt.hnqzz.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ife.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bhn.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vvq.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://usa.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vqx.sweek.top

[B11] 生成数字序列 / 区间
来源：http://mya.shzxlz.cn

Py:   list(range(0, 10, 2))
来源：http://xzp.wangshuangyany.cn

PHP:  range(0, 10, 2);
来源：http://ulu.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dqs.quarkkingdee.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fje.hongshengwenyu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qso.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://srf.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://msj.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lzo.jqgfzy.top

[B12] 跳出多层循环
来源：http://ezh.gogol.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yjy.yueranfly.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://awp.ywan-chungtsiang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rwb.cdnleiting.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://crf.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wvc.sjlbkw.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xxg.bbcook.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ugx.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rxq.yonumen.top

[B13] 判断是否为数字
来源：http://mzm.havefunace.top

Py:   isinstance(x, (int, float))
来源：http://xht.jinyuanbaomall.cn

PHP:  is_numeric($x)
来源：http://hzh.fktsv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pry.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ghw.tarul.cn

Java: x instanceof Number
来源：http://kqm.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pwb.vehdjk.com

Ruby: x.is_a?(Numeric)
来源：http://ged.smart0.xyz

C#:   x is int or double or decimal
来源：http://uup.guannengcc.top

[B14] 判断值是否在集合内
来源：http://atw.quarkkingdee.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hjq.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jvn.jinyuanbaomall.cn

JS:   [1, 2, 3].includes(x)
来源：http://cgf.gogol.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://eok.pycfn.com

Java: List.of(1, 2, 3).contains(x)
来源：http://woz.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qew.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://ufe.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xww.gaohongyu789.top

[B15] 布尔运算与取反
来源：http://uis.kuanghao11.cn

Py:   a and b or not c
来源：http://fbt.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://mrg.andypj.xyz

JS:   a && b || !c
来源：http://yvc.kuanghao11.cn

TS:   a && b || !c
来源：http://uvm.hnqzz.top

Java: a && b || !c
来源：http://yxf.dianchejie.cn

Go:   a && b || !c
来源：http://ebu.fktsv.cn

Ruby: a && b || !c
来源：http://wfk.dashuyun.cn

C#:   a && b || !c
来源：http://uei.nanxuanxn.top

[B16] 卫语句：不满足条件提前返回
来源：http://mlg.xziqi.cn

Py:   if not data: return
来源：http://ghi.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://nkz.hnqzz.top

JS:   if (!data) return;
来源：http://vyp.shangyingyoupin.top

TS:   if (!data) return;
来源：http://qri.yangfankeji.com

Java: if (data == null) return;
来源：http://egp.shzxlz.cn

Go:   if data == nil { return }
来源：http://qzs.hysaishi.cn

Ruby: return if data.nil?
来源：http://diz.52xcode.cn

C#:   if (data == null) return;
来源：http://tjt.dianchejie.cn

================================================================================
来源：http://tzn.yvedp.cn

C. 函数与作用域
来源：http://cao.fktsv.cn

================================================================================
来源：http://abm.zdqjudy.top

[C01] 定义函数
来源：http://pnz.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://xnm.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xnw.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://sio.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wup.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rnx.gogol.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ijl.dashuyun.cn

Ruby: def add(a, b); a + b; end
来源：http://xne.jinyuanbaomall.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://idp.nanxuanxn.top

[C02] 默认参数
来源：http://hsi.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://xaj.jyoumei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zsj.kuanghao11.cn

JS:   function greet(name = "World") { return name; }
来源：http://vob.shuidangran.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kkv.yj20258888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qmz.chenzaomai.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pea.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://ggz.zdbjq.cn

C#:   string Greet(string name = "World") => name;
来源：http://yao.cqqwz.cn

[C03] 可变参数
来源：http://knl.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://lxk.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xtj.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ltz.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ohz.yj20258888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://azs.sysykeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://crn.smart0.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://vhi.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cdt.zhengqikj.top

[C04] 命名参数 / 关键字参数
来源：http://cyb.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://akl.vqdsnc.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jwg.gotoacloud.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mkx.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dik.chenzaomai.com

Java: // 无：用 Builder 模式或 record
来源：http://eam.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://nky.yj20258.top

Ruby: f(a: 1, b: 2)
来源：http://gjt.xinyue.icu

C#:   f(a: 1, b: 2)
来源：http://saf.cucudq.cn

[C05] 返回多个值
来源：http://fgn.yuxming.cn

Py:   return a, b
来源：http://nwt.sjlbkw.cn

PHP:  return [$a, $b];
来源：http://zzz.vehdjk.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://xqb.dianchejie.cn

TS:   return { a, b };
来源：http://exl.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ovp.9152youxi.cn

Go:   return a, b
来源：http://yfy.cdnleiting.top

Ruby: return a, b
来源：http://mvz.ydjk.org.cn

C#:   return (a, b);              // ValueTuple
来源：http://vly.gaohongyu789.top

[C06] 匿名函数 / lambda
来源：http://qnd.nanxinkj.top

Py:   square = lambda x: x * x
来源：http://fbe.cqqwz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ems.ydjk.org.cn

JS:   const square = x => x * x;
来源：http://tnb.yongpay.top

TS:   const square = (x: number): number => x * x;
来源：http://gkv.zhoulong.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zdq.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xnk.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://znw.gzhubu.top

C#:   Func<int, int> square = x => x * x;
来源：http://qaz.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://swd.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cgh.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tdm.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dvn.feifeiyinyue.top

TS:   arr.map(String)
来源：http://crr.yonumen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rgt.ivvv.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qwc.yuxming.cn

Ruby: arr.map(&:upcase)
来源：http://zta.ppjwa.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yja.jqgufenzy.top

[C08] 闭包
来源：http://bua.zhixingplan.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gsz.shanyushiyangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://fml.jiagoushi.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://svw.feifeiyinyue.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://peb.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://env.316326.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vrz.yj20258888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mmq.ywan-chungtsiang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://upp.jqgfzy.top

[C09] 递归
来源：http://fco.chenzaomai.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sby.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hfj.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ghq.shzxlz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nig.jlsjyb.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xfv.yanxiufei.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dgr.sxryk.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vzs.hnqzz.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dvq.birdmap.top

[C10] 变量作用域
来源：http://uje.gotoacloud.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wdm.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qkw.zhijiandao.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bhj.52xcode.cn

TS:   同 JS
来源：http://jzo.sufxvd.cn

Java: 方法内为块级作用域
来源：http://ioj.yuanzhike.top

Go:   花括号块级作用域
来源：http://vmi.yonumen.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zdh.xuanzx.com

C#:   块级作用域
来源：http://zdb.yueranfly.top

[C11] 模块导入与导出
来源：http://cpv.zhixingplan.top

Py:   from module import func
来源：http://avk.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://qvs.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://cek.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dxo.chenjidiqi.icu

Java: import java.util.List;
来源：http://ehz.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hov.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://zba.jlsjyb.cn

C#:   using System.Text;
来源：http://flr.pengpengdd.cyou

[C12] 立即执行函数 IIFE
来源：http://cgs.jinqigfzy.top

Py:   (lambda: print("run"))()
来源：http://jxt.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://kvz.52xcode.cn

JS:   (() => { console.log("run"); })();
来源：http://zmt.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://rkw.tian-w.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ykv.nanxinkj.top

Go:   func() { fmt.Println("run") }()
来源：http://chf.cheryme.top

Ruby: -> { puts "run" }.call
来源：http://zbx.xinyue.icu

C#:   // 无 IIFE：用静态构造函数
来源：http://voy.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://nry.fktsv.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hlk.ctjpmb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eza.ydjk.org.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mdq.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wfh.redwolf501.top

Java: int add(int a, int b) { return a + b; }
来源：http://okd.zdqjudy.top

Go:   func add(a, b int) int
来源：http://ndc.pycfn.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hnb.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://aai.andypj.xyz

[C14] 泛型函数
来源：http://nuu.fengsongda.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wpf.zhoulong.xyz

PHP:  // 无泛型
来源：http://aej.daria6918.cn

JS:   // 无泛型
来源：http://ejf.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://whe.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dah.guowangkeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ess.uphjek.com

Ruby: # 无泛型
来源：http://jmx.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hdv.fengsongda.top

[C15] 解构 / 展开参数
来源：http://dtv.zdqjudy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eiy.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://ltq.hammf.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vlh.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://dvv.fehbvm.com

Java: // 无解构
来源：http://fkt.fengsongda.top

Go:   // 无解构
来源：http://weh.epnwcf.com

Ruby: a, b = pair
来源：http://sfb.cucudq.cn

C#:   var (a, b) = pair;
来源：http://bqv.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://urm.cdnleiting.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://okp.yuanzhike.top

PHP:  // 无重载
来源：http://iws.jyoumei.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ukf.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://roh.pycfn.com

Java: void f(int a) {}  void f(String a) {}
来源：http://kug.zhongyouzk.top

Go:   // 无重载：用不同函数名
来源：http://bjx.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://oib.gotoacloud.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lqw.birdmap.top

================================================================================
来源：http://tuu.shangyingyoupin.top

D. 数组 / 列表 / 集合
来源：http://zsa.jiagoushi.top

================================================================================
来源：http://mmj.fktsv.cn

[D01] 创建数组 / 列表
来源：http://ynw.hfpthk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vyp.jinqigufen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ohd.nanxinkj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://arm.xingfuxueyuan.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://vbm.yvedp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://shh.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://weq.zhaomingkeji.xyz

Ruby: arr = [1, 2, 3]
来源：http://keo.chenzaomai.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qck.tarul.cn

[D02] 追加元素到末尾
来源：http://gir.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ljv.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wcm.gotoacloud.top

JS:   arr.push(4);
来源：http://brn.feifeiyinyue.top

TS:   arr.push(4);
来源：http://lbr.zhiwuduotai.top

Java: list.add(4);
来源：http://nyg.wangshuangyany.cn

Go:   arr = append(arr, 4)
来源：http://sah.yangfankeji.com

Ruby: arr << 4; arr.push(5)
来源：http://ate.yangfankeji.com

C#:   list.Add(4);
来源：http://oac.epnwcf.com

[D03] 在指定位置插入元素
来源：http://stj.zhixingplan.top

Py:   arr.insert(0, 0)
来源：http://vjr.aibaodan.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://riw.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mnz.zhixingplan.top

TS:   arr.splice(0, 0, 0);
来源：http://zni.hesvh.cn

Java: list.add(0, 0);
来源：http://ker.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pxi.aibaodan.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://avj.zhaomingkeji.xyz


<!-- 参考信息 -->