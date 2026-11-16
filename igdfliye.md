代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mei.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uyv.cheryme.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rmm.yuxming.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ieh.hnqzz.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uxe.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://zwb.wangshuangyany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pyl.jinyuanbaomall.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sjo.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gpr.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ypg.9152youxi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tor.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eur.bbcook.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nsz.shzxlz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ivo.havefunace.top

[B11] 生成数字序列 / 区间
来源：http://qam.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://ffg.guowangkeji.top

PHP:  range(0, 10, 2);
来源：http://ozm.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uwn.c1oappe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gry.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vpd.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zgo.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://egk.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qif.jiagoushi.top

[B12] 跳出多层循环
来源：http://zzh.daria6918.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kdh.gzhubu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mjy.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hqz.ywan-chungtsiang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zip.sufxvd.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://emh.shangyingyoupin.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wki.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mup.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uax.jinqigfzy.top

[B13] 判断是否为数字
来源：http://sza.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://rtq.jinqigufen.top

PHP:  is_numeric($x)
来源：http://bui.ehwqpu.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yge.ctjpmb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lds.cucudq.cn

Java: x instanceof Number
来源：http://sll.jiagoushi.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vej.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://vsx.shzxlz.cn

C#:   x is int or double or decimal
来源：http://xsy.xingfuxueyuan.xyz

[B14] 判断值是否在集合内
来源：http://keu.sweek.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yzk.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wtq.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://ahd.svipenyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://izq.yj20258.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ryi.vehdjk.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yiv.nanxuanxn.top

Ruby: [1, 2, 3].include?(x)
来源：http://ork.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jfb.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://qsx.hywenlv.cn

Py:   a and b or not c
来源：http://wie.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://jtq.ppjwa.cn

JS:   a && b || !c
来源：http://vjc.jianghu66.top

TS:   a && b || !c
来源：http://aqc.zhaomingkeji.xyz

Java: a && b || !c
来源：http://nqw.zycfv.cn

Go:   a && b || !c
来源：http://trc.yangfankeji.com

Ruby: a && b || !c
来源：http://khy.ywan-chungtsiang.top

C#:   a && b || !c
来源：http://jly.jyoumei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://pbf.yj202588.top

Py:   if not data: return
来源：http://hrx.ppjwa.cn

PHP:  if (!$data) { return; }
来源：http://grf.tarul.cn

JS:   if (!data) return;
来源：http://duj.cqqwz.cn

TS:   if (!data) return;
来源：http://lrg.chenlongwang.top

Java: if (data == null) return;
来源：http://uei.xziqi.cn

Go:   if data == nil { return }
来源：http://sfw.tarul.cn

Ruby: return if data.nil?
来源：http://lbe.shuidangran.top

C#:   if (data == null) return;
来源：http://ytt.xziqi.cn

================================================================================
来源：http://nkt.52xcode.cn

C. 函数与作用域
来源：http://qil.smart0.xyz

================================================================================
来源：http://ddp.sufxvd.cn

[C01] 定义函数
来源：http://sti.jinghuilouyu.cn

Py:   def add(a, b): return a + b
来源：http://sxr.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uev.shangyingyoupin.top

JS:   function add(a, b) { return a + b; }
来源：http://chy.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rbk.yvedp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aet.chenjidiqi.icu

Go:   func add(a, b int) int { return a + b }
来源：http://grf.tian-w.cn

Ruby: def add(a, b); a + b; end
来源：http://umv.nanxuanxn.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nfz.shanyushiyangtech.top

[C02] 默认参数
来源：http://xdk.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://vqz.shanyushiyangtech.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fdn.chenlongwang.top

JS:   function greet(name = "World") { return name; }
来源：http://irl.vqdsnc.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ges.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dua.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ilb.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://lba.ybcxt.top

C#:   string Greet(string name = "World") => name;
来源：http://vts.zdbjq.cn

[C03] 可变参数
来源：http://vdk.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://wzq.xuanzx.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tke.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gzk.jinqigfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aoo.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dor.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ocw.quarkkingdee.top

Ruby: def total(*nums); nums.sum; end
来源：http://nkc.sjlbkw.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xoe.fehbvm.com

[C04] 命名参数 / 关键字参数
来源：http://kng.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ozt.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://djb.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://puo.ehwqpu.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fwg.9152youxi.cn

Java: // 无：用 Builder 模式或 record
来源：http://vxp.jinyuanbaomall.cn

Go:   // 无：用配置结构体参数
来源：http://aje.vqdsnc.cn

Ruby: f(a: 1, b: 2)
来源：http://jih.nwbrower.top

C#:   f(a: 1, b: 2)
来源：http://baf.kuanghao11.cn

[C05] 返回多个值
来源：http://mec.jinghuilouyu.cn

Py:   return a, b
来源：http://tms.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://biv.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mch.ehwqpu.com

TS:   return { a, b };
来源：http://gwj.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://upy.fzhhl.top

Go:   return a, b
来源：http://cws.chenjidiqi.icu

Ruby: return a, b
来源：http://reg.pengpengdd.cyou

C#:   return (a, b);              // ValueTuple
来源：http://lou.wangshuangyany.cn

[C06] 匿名函数 / lambda
来源：http://ckt.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://pzg.jyoumei.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://yeg.sxryk.cn

JS:   const square = x => x * x;
来源：http://jkp.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://jxp.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zbg.tanke756.top

Go:   sq := func(x int) int { return x * x }
来源：http://jov.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://btf.fanxiaobao.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://tuv.epnwcf.com

[C07] 把函数作为参数传入
来源：http://agm.zdqjudy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cci.tian-w.cn

PHP:  array_map("strtoupper", $arr);
来源：http://asi.tian-w.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dvv.nanxuanxn.top

TS:   arr.map(String)
来源：http://vhg.hcnkem.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wyw.chenzaomai.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qul.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://bnp.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://xij.ydjk.org.cn

[C08] 闭包
来源：http://dzi.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jzv.yonumen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://acz.zycfv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://deh.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wfx.yangfankeji.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ixd.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tjr.daria6918.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sug.yueranfly.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://goe.fzhhl.top

[C09] 递归
来源：http://mvy.daxiang520.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fyq.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rpn.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lmt.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mcg.zhengqikj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hjm.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ckr.pengpengdd.cyou

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jxo.andypj.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fzw.pengpengdd.cyou

[C10] 变量作用域
来源：http://rha.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jhy.zhiwuduotai.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://iye.9152youxi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dvo.ppjwa.cn

TS:   同 JS
来源：http://tnw.redwolf501.top

Java: 方法内为块级作用域
来源：http://zlz.cdnleiting.top

Go:   花括号块级作用域
来源：http://kiv.vqdsnc.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://azr.hnqzz.top

C#:   块级作用域
来源：http://kla.fengsongda.top

[C11] 模块导入与导出
来源：http://etu.fanxiaobao.xyz

Py:   from module import func
来源：http://nhz.ivvv.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pmv.zhaomingkeji.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://qjw.hcnkem.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bbp.daxiang520.top

Java: import java.util.List;
来源：http://mpm.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gjp.zhaomingkeji.xyz

Ruby: require "json"; require_relative "./util"
来源：http://odt.zycfv.cn

C#:   using System.Text;
来源：http://ixf.ydzc1.top

[C12] 立即执行函数 IIFE
来源：http://qbt.havefunace.top

Py:   (lambda: print("run"))()
来源：http://uxq.daria6918.cn

PHP:  (function () { echo "run"; })();
来源：http://zgf.gotoacloud.top

JS:   (() => { console.log("run"); })();
来源：http://cpj.birdmap.top

TS:   (() => { console.log("run"); })();
来源：http://aum.xinyue.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://srn.ehwqpu.com

Go:   func() { fmt.Println("run") }()
来源：http://zph.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://wyw.sxryk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://onu.chenzaomai.com

[C13] 类型声明 / 类型注解
来源：http://jgt.aizwys.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://osh.yangfankeji.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jtc.xziqi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rqt.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nkv.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://aeq.sysykeji.top

Go:   func add(a, b int) int
来源：http://sdw.yueranfly.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zkx.yangfankeji.com

C#:   int Add(int a, int b) => a + b;
来源：http://fna.fanxiaobao.xyz

[C14] 泛型函数
来源：http://jbp.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://flm.snrcjt.cn

PHP:  // 无泛型
来源：http://isn.kuanghao11.cn

JS:   // 无泛型
来源：http://sxl.zhoulong.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://two.zhijiandao.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vpq.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mvu.hysaishi.cn

Ruby: # 无泛型
来源：http://toe.haohaochexian.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aqz.birdmap.top

[C15] 解构 / 展开参数
来源：http://weu.yonumen.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xws.sxryk.cn

PHP:  [$a, $b] = $pair;
来源：http://tnl.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hxe.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ups.zdbjq.cn

Java: // 无解构
来源：http://irc.0kj1m.cn

Go:   // 无解构
来源：http://jtl.hysaishi.cn

Ruby: a, b = pair
来源：http://zol.guannengcc.top

C#:   var (a, b) = pair;
来源：http://cbk.dashuyun.cn

[C16] 函数 / 方法重载
来源：http://shr.sysykeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uab.vehdjk.com

PHP:  // 无重载
来源：http://udm.jinghuilouyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zgu.jinghuilouyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://xdy.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jso.daria6918.cn

Go:   // 无重载：用不同函数名
来源：http://lmf.cucudq.cn

Ruby: # 无重载：靠动态参数
来源：http://let.yanxiufei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fpt.jinqigufen.top

================================================================================
来源：http://yhp.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://nut.gaohongyu789.top

================================================================================
来源：http://hah.yuanzhike.top

[D01] 创建数组 / 列表
来源：http://lsu.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zbt.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kdd.jinghuilouyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zyx.daria6918.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uaq.jqgfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xlb.hnxiangtu.top

Go:   arr := []int{1, 2, 3}
来源：http://src.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://dzn.fzhhl.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wsg.nanxinkj.top

[D02] 追加元素到末尾
来源：http://itl.svipenyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ffd.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://omn.xinyue.icu

JS:   arr.push(4);
来源：http://zmh.52xcode.cn

TS:   arr.push(4);
来源：http://kvq.hcnkem.com

Java: list.add(4);
来源：http://sww.havefunace.top

Go:   arr = append(arr, 4)
来源：http://ksy.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://yaw.meibo888.top

C#:   list.Add(4);
来源：http://lwl.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://onm.fengsongda.top

Py:   arr.insert(0, 0)
来源：http://apr.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yrd.vehdjk.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kqt.gotoacloud.top

TS:   arr.splice(0, 0, 0);
来源：http://muw.jinqigufen.top

Java: list.add(0, 0);
来源：http://qgf.jyoumei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qxo.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vbe.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://rlk.yj20258.top

[D04] 删除元素
来源：http://gsd.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jid.ehwqpu.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zaz.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://izj.yj202588.top

TS:   arr.splice(0, 1);
来源：http://zml.fengsongda.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://arj.aizwys.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dbc.uphjek.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tfi.cucudq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uen.yuanzhike.top

[D05] 访问与修改元素
来源：http://kmi.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cnr.jinqigufen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kig.zdbjq.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://czc.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://dmh.yj20258.top

Java: list.get(0); list.set(0, 9);
来源：http://dgm.havefunace.top

Go:   arr[0]; arr[0] = 9
来源：http://vdv.ydzc1.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ijx.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gdi.hammf.cn

[D06] 数组长度
来源：http://dpo.gaohongyu789.top

Py:   len(arr)
来源：http://wyl.ppjwa.cn

PHP:  count($arr);
来源：http://xjw.wangdashe.top

JS:   arr.length
来源：http://nke.xuanzx.com

TS:   arr.length
来源：http://vlh.yfazqb.com

Java: list.size();
来源：http://pdo.xziqi.cn

Go:   len(arr)
来源：http://exo.52xcode.cn

Ruby: arr.length; arr.size
来源：http://wkq.quarkkingdee.top

C#:   list.Count;
来源：http://sjy.hesvh.cn

[D07] 切片 / 取子数组
来源：http://hcm.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://udx.xuanzx.com

PHP:  array_slice($arr, 1, 3);
来源：http://zeo.wangdashe.top

JS:   arr.slice(1, 4);
来源：http://nkw.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://lea.quarkkingdee.top

Java: list.subList(1, 4);
来源：http://ysm.meibo888.top

Go:   arr[1:4]
来源：http://ape.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://bwy.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://xgo.daria6918.cn

[D08] 合并两个数组
来源：http://rgs.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://bqo.yueranfly.top

PHP:  array_merge($a, $b);
来源：http://kvo.guannengcc.top

JS:   [...a, ...b];  a.concat(b);
来源：http://eed.nanxinkj.top

TS:   [...a, ...b];
来源：http://oeg.tarul.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://huo.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://guy.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://csg.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://shj.wangshuangyany.cn

[D09] 排序（升序）
来源：http://mqn.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://ilq.sysykeji.top

PHP:  sort($arr);
来源：http://oiq.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://azm.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jys.ybcxt.top

Java: Collections.sort(list);  list.sort(null);
来源：http://frh.jiagoushi.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zgw.cheryme.top

Ruby: arr.sort
来源：http://iyi.ivvv.top

C#:   list.Sort();
来源：http://mdj.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tir.tarul.cn


<!-- 参考信息 -->