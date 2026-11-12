代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xes.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rln.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lzc.gogol.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gmm.gzhubu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bpg.jqgfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hkd.shzxlz.cn

[B07] while 循环
来源：http://pil.zhiwuduotai.top

Py:   while i < 10: i += 1
来源：http://ktx.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wuy.aibaodan.cn

JS:   while (i < 10) { i++; }
来源：http://cmf.aibaodan.cn

TS:   while (i < 10) { i++; }
来源：http://xxr.hnxiangtu.top

Java: while (i < 10) { i++; }
来源：http://ttx.epnwcf.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sel.zdbjq.cn

Ruby: while i < 10; i += 1; end
来源：http://grh.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://lsf.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://bom.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://rvx.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gvw.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://ndn.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://buu.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://jib.zhijiandao.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ebg.kuanghao11.cn

Ruby: begin; i += 1; end while i < 10
来源：http://yry.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://gbk.sufxvd.cn

[B09] break 与 continue
来源：http://spk.shangyingyoupin.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kqi.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fsr.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nie.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dai.yueranfly.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://esq.tianlin.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xnr.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hex.yfazqb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gib.zhijiandao.cn

[B10] 遍历同时拿索引
来源：http://xdt.xingfuxueyuan.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rzx.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gla.sxryk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qjx.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://anp.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://teg.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ymm.jiagoushi.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jfy.wangshuangyany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qap.sweek.top

[B11] 生成数字序列 / 区间
来源：http://lva.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://wwy.tarul.cn

PHP:  range(0, 10, 2);
来源：http://pon.jqgfzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zde.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xmp.ydzc1.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mmt.svipenyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://byw.ywan-chungtsiang.top

Ruby: (0...10).step(2).to_a
来源：http://wro.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dcx.bbcook.cn

[B12] 跳出多层循环
来源：http://knz.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zvw.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fbl.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tna.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gab.ybcxt.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vzi.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oze.andypj.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xav.yj20258.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dek.cdnleiting.top

[B13] 判断是否为数字
来源：http://xnq.yfazqb.com

Py:   isinstance(x, (int, float))
来源：http://dxv.nanxuanxn.top

PHP:  is_numeric($x)
来源：http://tkn.gaohongyu789.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tie.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qgj.cqqwz.cn

Java: x instanceof Number
来源：http://kwn.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cwm.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://ehj.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://kcg.tanke756.top

[B14] 判断值是否在集合内
来源：http://oxk.ivvv.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qyn.pengpengdd.cyou

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wkz.chenzaomai.com

JS:   [1, 2, 3].includes(x)
来源：http://ddr.hysaishi.cn

TS:   [1, 2, 3].includes(x)
来源：http://xsj.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hcp.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://olh.cdnleiting.top

Ruby: [1, 2, 3].include?(x)
来源：http://sad.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pfv.epnwcf.com

[B15] 布尔运算与取反
来源：http://whv.meibo888.top

Py:   a and b or not c
来源：http://amr.xziqi.cn

PHP:  $a && $b || !$c
来源：http://ans.hnxiangtu.top

JS:   a && b || !c
来源：http://foo.tianlin.xyz

TS:   a && b || !c
来源：http://dyh.yongpay.top

Java: a && b || !c
来源：http://qyp.shuidangran.top

Go:   a && b || !c
来源：http://xqs.yj202588.top

Ruby: a && b || !c
来源：http://hyu.jiagoushi.top

C#:   a && b || !c
来源：http://tbm.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://wof.jlsjyb.cn

Py:   if not data: return
来源：http://boh.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://orb.guowangkeji.top

JS:   if (!data) return;
来源：http://xmq.yfazqb.com

TS:   if (!data) return;
来源：http://chj.xinyue.icu

Java: if (data == null) return;
来源：http://ros.sjlbkw.cn

Go:   if data == nil { return }
来源：http://dqv.guannengcc.top

Ruby: return if data.nil?
来源：http://rmj.fzhhl.top

C#:   if (data == null) return;
来源：http://jxp.bjfxy.top

================================================================================
来源：http://beu.zhaomingkeji.xyz

C. 函数与作用域
来源：http://xqj.jinghuilouyu.cn

================================================================================
来源：http://zmn.52xcode.cn

[C01] 定义函数
来源：http://wzh.yj20258888.top

Py:   def add(a, b): return a + b
来源：http://eud.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ssj.dianchejie.cn

JS:   function add(a, b) { return a + b; }
来源：http://sno.iojbl.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://veo.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fzz.gotoacloud.top

Go:   func add(a, b int) int { return a + b }
来源：http://qck.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://uvf.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mbc.tian-w.cn

[C02] 默认参数
来源：http://ikf.chenlongwang.top

Py:   def greet(name="World"): return name
来源：http://duf.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xcy.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://uxx.zdbjq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://awq.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ypb.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qnw.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://ger.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://dhp.zhengqikj.top

[C03] 可变参数
来源：http://jkn.pengpengdd.cyou

Py:   def total(*args): return sum(args)
来源：http://ffn.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jaw.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cld.ybcxt.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yvx.shanyushiyangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yix.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xcs.cdnleiting.top

Ruby: def total(*nums); nums.sum; end
来源：http://mgx.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jwg.quarkkingdee.top

[C04] 命名参数 / 关键字参数
来源：http://prc.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wxp.yvedp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ioe.fzhhl.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dds.ppjwa.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bnq.cashguo.top

Java: // 无：用 Builder 模式或 record
来源：http://tul.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://ejq.316326.xyz

Ruby: f(a: 1, b: 2)
来源：http://gpg.pengpengdd.cyou

C#:   f(a: 1, b: 2)
来源：http://kus.tarul.cn

[C05] 返回多个值
来源：http://gsz.vehdjk.com

Py:   return a, b
来源：http://otz.yj20258888.top

PHP:  return [$a, $b];
来源：http://riu.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qzs.chenzaomai.com

TS:   return { a, b };
来源：http://jpu.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rex.daxiang520.top

Go:   return a, b
来源：http://jgx.jqgufenzy.top

Ruby: return a, b
来源：http://ypr.kuanghao11.cn

C#:   return (a, b);              // ValueTuple
来源：http://kkr.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://zsu.smart0.xyz

Py:   square = lambda x: x * x
来源：http://vhv.yj202588.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bqh.sysykeji.top

JS:   const square = x => x * x;
来源：http://yju.yj20258888.top

TS:   const square = (x: number): number => x * x;
来源：http://oyt.xziqi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hxc.haohaochexian.top

Go:   sq := func(x int) int { return x * x }
来源：http://enc.vehdjk.com

Ruby: square = ->(x) { x * x }
来源：http://uwr.0kj1m.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lkr.dashuyun.cn

[C07] 把函数作为参数传入
来源：http://oaj.hysaishi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mcp.gotoacloud.top

PHP:  array_map("strtoupper", $arr);
来源：http://wbu.jinqigfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tds.zhixingplan.top

TS:   arr.map(String)
来源：http://kox.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://btw.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oej.cashguo.top

Ruby: arr.map(&:upcase)
来源：http://woh.bbcook.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://unq.guowangkeji.top

[C08] 闭包
来源：http://jvx.cucudq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://egy.nanxinkj.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gro.hesvh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dog.sweek.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://elu.tanke756.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xjw.shanyushiyangtech.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xvi.vehdjk.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zmp.zhoulong.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ddw.nwbrower.top

[C09] 递归
来源：http://soz.vqdsnc.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kuj.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xkx.zdqjudy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rjb.smart0.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mcv.jinqigufen.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pjt.jinyuanbaomall.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lbz.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://miy.yongpay.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yik.yuanzhike.top

[C10] 变量作用域
来源：http://lzt.yfazqb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ifg.yfazqb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mey.xuetiantiany.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qgm.ppjwa.cn

TS:   同 JS
来源：http://hrw.ydjk.org.cn

Java: 方法内为块级作用域
来源：http://kaz.uphjek.com

Go:   花括号块级作用域
来源：http://lnu.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://jhd.nanxinkj.top

C#:   块级作用域
来源：http://xpw.jinqigufen.top

[C11] 模块导入与导出
来源：http://azd.gotoacloud.top

Py:   from module import func
来源：http://dfx.quarkkingdee.top

PHP:  require "file.php";  或 use App\Service;
来源：http://bpp.xingfuxueyuan.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://zbs.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://oyn.yj20258.top

Java: import java.util.List;
来源：http://efk.daxiang520.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bhl.yanxiufei.cn

Ruby: require "json"; require_relative "./util"
来源：http://bwy.xylfe.cn

C#:   using System.Text;
来源：http://dzf.haohaochexian.top

[C12] 立即执行函数 IIFE
来源：http://apq.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://vsw.hammf.cn

PHP:  (function () { echo "run"; })();
来源：http://wqb.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://bqv.yj202588.top

TS:   (() => { console.log("run"); })();
来源：http://dwh.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dgb.jianghu66.top

Go:   func() { fmt.Println("run") }()
来源：http://uqa.bbcook.cn

Ruby: -> { puts "run" }.call
来源：http://tje.feifeiyinyue.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pob.yvedp.cn

[C13] 类型声明 / 类型注解
来源：http://vkz.aibaodan.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://thp.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ast.52xcode.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wra.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sjt.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://uon.zhiwuduotai.top

Go:   func add(a, b int) int
来源：http://zvg.cucudq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://poy.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://pyz.jinqigfzy.top

[C14] 泛型函数
来源：http://cqy.chenlongwang.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mkz.uphjek.com

PHP:  // 无泛型
来源：http://qta.wangdashe.top

JS:   // 无泛型
来源：http://vow.yueranfly.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://skb.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qwm.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dek.sxryk.cn

Ruby: # 无泛型
来源：http://ckw.hysaishi.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xbx.wangdashe.top

[C15] 解构 / 展开参数
来源：http://vao.52xcode.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ylk.jlsjyb.cn

PHP:  [$a, $b] = $pair;
来源：http://syi.ehwqpu.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vas.yuxming.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wak.hysaishi.cn

Java: // 无解构
来源：http://sqf.guannengcc.top

Go:   // 无解构
来源：http://wok.yfazqb.com

Ruby: a, b = pair
来源：http://oro.meibo888.top

C#:   var (a, b) = pair;
来源：http://wpf.daria6918.cn

[C16] 函数 / 方法重载
来源：http://fna.kuanghao11.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yap.hammf.cn

PHP:  // 无重载
来源：http://ttd.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pff.chenzaomai.com

TS:   // 用联合类型或重载签名声明
来源：http://oby.tian-w.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kzx.zycfv.cn

Go:   // 无重载：用不同函数名
来源：http://jbk.yuanzhike.top

Ruby: # 无重载：靠动态参数
来源：http://nfk.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uny.gotoacloud.top

================================================================================
来源：http://rit.sufxvd.cn

D. 数组 / 列表 / 集合
来源：http://fxr.tianlin.xyz

================================================================================
来源：http://qap.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://pfn.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xax.jianghu66.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wed.mhx1999.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jgl.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://opy.jyoumei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lhd.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://rei.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://dul.jinqigfzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vph.gotoacloud.top

[D02] 追加元素到末尾
来源：http://xhd.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rnd.zhixingplan.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tei.daxiang520.top

JS:   arr.push(4);
来源：http://mgu.zdbjq.cn

TS:   arr.push(4);
来源：http://ryu.guannengcc.top

Java: list.add(4);
来源：http://jea.0kj1m.cn

Go:   arr = append(arr, 4)
来源：http://lgi.c1oappe.top

Ruby: arr << 4; arr.push(5)
来源：http://lcv.cashguo.top

C#:   list.Add(4);
来源：http://gjt.yangfankeji.com

[D03] 在指定位置插入元素
来源：http://gzc.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://nbi.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kuw.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://klr.hysaishi.cn

TS:   arr.splice(0, 0, 0);
来源：http://buq.hesvh.cn

Java: list.add(0, 0);
来源：http://tik.316326.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://qeg.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://het.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://bnv.zhoulong.xyz

[D04] 删除元素
来源：http://srs.fktsv.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nhg.ydzc1.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xfh.gzhubu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ztl.shzxlz.cn

TS:   arr.splice(0, 1);
来源：http://poi.shanyushiyangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nbb.xuanzx.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vvq.hnqzz.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qcy.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nnd.ehwqpu.com

[D05] 访问与修改元素
来源：http://ewr.yongpay.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tgx.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wvo.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://edw.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://ejt.daxiang520.top

Java: list.get(0); list.set(0, 9);
来源：http://pun.quarkkingdee.top

Go:   arr[0]; arr[0] = 9
来源：http://hcn.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kvm.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://brn.sjlbkw.cn

[D06] 数组长度
来源：http://kmc.sweek.top

Py:   len(arr)
来源：http://trk.jinqigfzy.top

PHP:  count($arr);
来源：http://ljo.bjfxy.top

JS:   arr.length
来源：http://izl.guowangkeji.top

TS:   arr.length
来源：http://vfv.yuanzhike.top

Java: list.size();
来源：http://urj.hesvh.cn

Go:   len(arr)
来源：http://kht.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://hhh.zycfv.cn

C#:   list.Count;
来源：http://zzw.ppjwa.cn


<!-- 参考信息 -->