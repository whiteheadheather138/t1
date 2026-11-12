代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rim.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tdr.birdmap.top

[B03] switch / match / case
来源：http://yei.yangfankeji.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://njn.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://opy.gzhubu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uwj.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://whx.haohaochexian.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://otq.nanxuanxn.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dir.nanxuanxn.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lnc.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cxv.jianghu66.top

[B04] for 计数循环
来源：http://dqh.jinyuanbaomall.cn

Py:   for i in range(10): print(i)
来源：http://vxe.redwolf501.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://avd.jianghu66.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://znt.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bhs.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vhs.fanxiaobao.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tch.yvedp.cn

Ruby: 10.times { |i| puts i }
来源：http://scm.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mfu.ctjpmb.com

[B05] 遍历数组 / 列表
来源：http://xli.shzxlz.cn

Py:   for item in arr: print(item)
来源：http://ozk.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://foe.chenlongwang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lrw.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hlp.xinyue.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://fql.aibaodan.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gwg.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://emb.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eil.iojbl.cn

[B06] 遍历字典 / 对象
来源：http://nrs.ybcxt.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dvy.smart0.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://exi.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://scu.yfazqb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vdi.52xcode.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yml.daxiang520.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oqn.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lis.jianghu66.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wgo.hcnkem.com

[B07] while 循环
来源：http://vts.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://flk.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://alu.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://wjn.hnxiangtu.top

TS:   while (i < 10) { i++; }
来源：http://tqi.guowangkeji.top

Java: while (i < 10) { i++; }
来源：http://fsb.mhx1999.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://eus.jiagoushi.top

Ruby: while i < 10; i += 1; end
来源：http://hcf.hfpthk.cn

C#:   while (i < 10) { i++; }
来源：http://qqx.hammf.cn

[B08] do-while（至少执行一次）
来源：http://jth.pengpengdd.cyou

Py:   # 无 do-while：用 while True + break
来源：http://hiv.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jxz.epnwcf.com

JS:   do { i++; } while (i < 10);
来源：http://fbh.jinyuanbaomall.cn

TS:   do { i++; } while (i < 10);
来源：http://xwt.epnwcf.com

Java: do { i++; } while (i < 10);
来源：http://zwe.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://jby.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://sud.aibaodan.cn

C#:   do { i++; } while (i < 10);
来源：http://yyz.quarkkingdee.top

[B09] break 与 continue
来源：http://bpi.yfazqb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zqj.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fov.hnxiangtu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://icy.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zux.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pnm.ybcxt.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mmi.wangshuangyany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fhj.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oun.ydzc1.top

[B10] 遍历同时拿索引
来源：http://bhq.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gsv.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://npy.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jiq.aizwys.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fse.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sxw.cqqwz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bqh.svipenyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://orn.yj20258888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uob.jinghuilouyu.cn

[B11] 生成数字序列 / 区间
来源：http://fhn.yuxming.cn

Py:   list(range(0, 10, 2))
来源：http://axy.zhoulong.xyz

PHP:  range(0, 10, 2);
来源：http://iiv.bjfxy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qyn.ehwqpu.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sih.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xys.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nuu.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://ojo.0kj1m.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kcs.dashuyun.cn

[B12] 跳出多层循环
来源：http://umu.jinyuanbaomall.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gaf.yj202588.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pui.hywenlv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jvk.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uws.fehbvm.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://imd.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qek.nwbrower.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xrs.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bew.yonumen.top

[B13] 判断是否为数字
来源：http://dpi.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://qfq.sweek.top

PHP:  is_numeric($x)
来源：http://rkb.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sfu.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wkq.yj20258.top

Java: x instanceof Number
来源：http://ruj.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xlv.hammf.cn

Ruby: x.is_a?(Numeric)
来源：http://pno.chenlongwang.top

C#:   x is int or double or decimal
来源：http://ilt.kuanghao11.cn

[B14] 判断值是否在集合内
来源：http://utf.ctjpmb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://juo.cdnleiting.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tch.yvedp.cn

JS:   [1, 2, 3].includes(x)
来源：http://ujl.daxiang520.top

TS:   [1, 2, 3].includes(x)
来源：http://kxn.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vls.xylfe.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mrc.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://hjz.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vez.svipenyu.cn

[B15] 布尔运算与取反
来源：http://mjg.pengpengdd.cyou

Py:   a and b or not c
来源：http://ueh.hesvh.cn

PHP:  $a && $b || !$c
来源：http://yth.nwbrower.top

JS:   a && b || !c
来源：http://ibd.jyoumei.cn

TS:   a && b || !c
来源：http://agx.zhengqikj.top

Java: a && b || !c
来源：http://qhn.hysaishi.cn

Go:   a && b || !c
来源：http://ppk.tanke756.top

Ruby: a && b || !c
来源：http://sfq.havefunace.top

C#:   a && b || !c
来源：http://gvf.yj20258.top

[B16] 卫语句：不满足条件提前返回
来源：http://eau.aibaodan.cn

Py:   if not data: return
来源：http://meq.sweek.top

PHP:  if (!$data) { return; }
来源：http://fdg.nanxinkj.top

JS:   if (!data) return;
来源：http://rzx.zdqjudy.top

TS:   if (!data) return;
来源：http://glc.snrcjt.cn

Java: if (data == null) return;
来源：http://rze.zdbjq.cn

Go:   if data == nil { return }
来源：http://pxr.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://utr.andypj.xyz

C#:   if (data == null) return;
来源：http://hrk.fzhhl.top

================================================================================
来源：http://aft.feifeiyinyue.top

C. 函数与作用域
来源：http://ucq.cashguo.top

================================================================================
来源：http://xte.sweek.top

[C01] 定义函数
来源：http://slf.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://wqu.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bav.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ytp.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zsq.pycfn.com

Java: static int add(int a, int b) { return a + b; }
来源：http://blm.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ctu.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://ypx.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rcq.zhixingplan.top

[C02] 默认参数
来源：http://boa.haohaochexian.top

Py:   def greet(name="World"): return name
来源：http://uhx.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mmr.xuetiantiany.cn

JS:   function greet(name = "World") { return name; }
来源：http://vxf.52xcode.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lyk.fehbvm.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ldn.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hhj.andypj.xyz

Ruby: def greet(name = "World") = name
来源：http://dzk.epnwcf.com

C#:   string Greet(string name = "World") => name;
来源：http://oyb.daxiang520.top

[C03] 可变参数
来源：http://shs.guowangkeji.top

Py:   def total(*args): return sum(args)
来源：http://dvr.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hiq.chenzaomai.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gpg.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hff.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rmf.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pew.chenlongwang.top

Ruby: def total(*nums); nums.sum; end
来源：http://luh.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rrt.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://ykb.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://knx.zhixingplan.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fya.cdnleiting.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eie.yuanzhike.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wxb.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://opk.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://lwo.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://etu.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://gwt.aibaodan.cn

[C05] 返回多个值
来源：http://uup.pycfn.com

Py:   return a, b
来源：http://jbv.ywan-chungtsiang.top

PHP:  return [$a, $b];
来源：http://ycj.feifeiyinyue.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fno.gotoacloud.top

TS:   return { a, b };
来源：http://tiu.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wsh.zycfv.cn

Go:   return a, b
来源：http://cml.shangyingyoupin.top

Ruby: return a, b
来源：http://vhs.yj20258.top

C#:   return (a, b);              // ValueTuple
来源：http://qii.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://yid.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://fzr.zdqjudy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qvj.redwolf501.top

JS:   const square = x => x * x;
来源：http://nlj.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://veo.tianlin.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wmr.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://knv.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://wvd.ydzc1.top

C#:   Func<int, int> square = x => x * x;
来源：http://nys.birdmap.top

[C07] 把函数作为参数传入
来源：http://hev.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nxc.cucudq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://qpo.zhongyouzk.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kvm.9152youxi.cn

TS:   arr.map(String)
来源：http://hfz.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zhz.sxryk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://paw.sjlbkw.cn

Ruby: arr.map(&:upcase)
来源：http://wql.hnqzz.top

C#:   arr.Select(s => s.ToUpper())
来源：http://oaq.guannengcc.top

[C08] 闭包
来源：http://uaz.shanyushiyangtech.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qfl.cheryme.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://sfe.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zgf.cashguo.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ksj.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mmh.ppjwa.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jzr.fengsongda.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jcy.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://urk.zhijiandao.cn

[C09] 递归
来源：http://wis.zhaomingkeji.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tky.ydjk.org.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jlp.ehwqpu.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://obl.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ske.52xcode.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://elz.fzhhl.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xha.ivvv.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cje.cheryme.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pmx.zhijiandao.cn

[C10] 变量作用域
来源：http://kco.yanxiufei.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tbx.nwbrower.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://swo.jqgfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mrg.ydzc1.top

TS:   同 JS
来源：http://vqk.zhiwuduotai.top

Java: 方法内为块级作用域
来源：http://xmb.yueranfly.top

Go:   花括号块级作用域
来源：http://byr.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://aae.birdmap.top

C#:   块级作用域
来源：http://fsa.xuetiantiany.cn

[C11] 模块导入与导出
来源：http://yvf.guannengcc.top

Py:   from module import func
来源：http://fbg.chenlongwang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://brr.jianghu66.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kmq.yueranfly.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xjb.cqqwz.cn

Java: import java.util.List;
来源：http://ptw.havefunace.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hdk.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://hyq.gotoacloud.top

C#:   using System.Text;
来源：http://ljo.uphjek.com

[C12] 立即执行函数 IIFE
来源：http://nnr.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://nfy.jinghuilouyu.cn

PHP:  (function () { echo "run"; })();
来源：http://otc.yanxiufei.cn

JS:   (() => { console.log("run"); })();
来源：http://nbc.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://hpj.hysaishi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tch.epnwcf.com

Go:   func() { fmt.Println("run") }()
来源：http://swl.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://osz.ctjpmb.com

C#:   // 无 IIFE：用静态构造函数
来源：http://mbd.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://olk.yj20258888.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jyu.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gql.sjlbkw.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wng.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://btg.zycfv.cn

Java: int add(int a, int b) { return a + b; }
来源：http://puw.yj202588.top

Go:   func add(a, b int) int
来源：http://jlc.daxiang520.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tfn.fktsv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://bqy.ctjpmb.com

[C14] 泛型函数
来源：http://kcp.yj202588.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uxg.yangfankeji.com

PHP:  // 无泛型
来源：http://oai.zhiwuduotai.top

JS:   // 无泛型
来源：http://heh.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pjf.pengpengdd.cyou

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://iiz.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wnh.epnwcf.com

Ruby: # 无泛型
来源：http://wby.sufxvd.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rng.ydjk.org.cn

[C15] 解构 / 展开参数
来源：http://hpu.jqgufenzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bjf.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://otx.cucudq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lxd.daxiang520.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ypn.yj202588.top

Java: // 无解构
来源：http://zes.dianchejie.cn

Go:   // 无解构
来源：http://qvd.hammf.cn

Ruby: a, b = pair
来源：http://hnd.shzxlz.cn

C#:   var (a, b) = pair;
来源：http://fda.bbcook.cn

[C16] 函数 / 方法重载
来源：http://cwr.ywan-chungtsiang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mhv.shzxlz.cn

PHP:  // 无重载
来源：http://xuz.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ymd.yangfankeji.com

TS:   // 用联合类型或重载签名声明
来源：http://zei.hcnkem.com

Java: void f(int a) {}  void f(String a) {}
来源：http://nmb.shangyingyoupin.top

Go:   // 无重载：用不同函数名
来源：http://qms.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://gjx.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hkd.zhoulong.xyz

================================================================================
来源：http://hya.uphjek.com

D. 数组 / 列表 / 集合
来源：http://fnb.dashuyun.cn

================================================================================
来源：http://ihz.jinqigfzy.top

[D01] 创建数组 / 列表
来源：http://hiz.gogol.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://msb.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aln.tianlin.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://szk.cdnleiting.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gkl.shanyushiyangtech.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zsv.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://mxe.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://jhd.zdqjudy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nmf.cashguo.top

[D02] 追加元素到末尾
来源：http://zqv.shzxlz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zqz.yuxming.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ivr.kuanghao11.cn

JS:   arr.push(4);
来源：http://cjs.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://pud.dianchejie.cn

Java: list.add(4);
来源：http://ili.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://jmh.ppjwa.cn

Ruby: arr << 4; arr.push(5)
来源：http://tao.0kj1m.cn

C#:   list.Add(4);
来源：http://zfp.iojbl.cn

[D03] 在指定位置插入元素
来源：http://lbg.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://geg.hcnkem.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tse.yonumen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pnx.zhixingplan.top


<!-- 参考信息 -->