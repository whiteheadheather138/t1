代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://fax.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wai.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://ydk.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://mdy.yvedp.cn

[B09] break 与 continue
来源：http://hot.redwolf501.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kuz.xziqi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yxf.shuidangran.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxf.hongshengwenyu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://afr.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nwh.xylfe.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kmp.jqgufenzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://knh.dianchejie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dax.mhx1999.top

[B10] 遍历同时拿索引
来源：http://cke.jinqigufen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oiy.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://byu.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ybu.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://abg.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://exi.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://odu.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pxs.yj20258888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tty.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://rdq.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://lux.52xcode.cn

PHP:  range(0, 10, 2);
来源：http://kvn.guowangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lvu.shuidangran.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ypf.jianghu66.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mtu.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://djw.chenlongwang.top

Ruby: (0...10).step(2).to_a
来源：http://xlm.ehwqpu.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xrk.sweek.top

[B12] 跳出多层循环
来源：http://icc.smart0.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://sdk.fzhhl.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cju.xinyue.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jgt.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ucj.bjfxy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hho.sjlbkw.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hbo.hnxiangtu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ior.sweek.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fbq.52xcode.cn

[B13] 判断是否为数字
来源：http://fdx.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://xwo.hywenlv.cn

PHP:  is_numeric($x)
来源：http://zys.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cnd.yuanzhike.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bvd.fzhhl.top

Java: x instanceof Number
来源：http://xvs.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://acy.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://fay.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://txk.cheryme.top

[B14] 判断值是否在集合内
来源：http://wdu.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yks.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ngb.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://hpl.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://sjg.yueranfly.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kgq.9152youxi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dsv.guannengcc.top

Ruby: [1, 2, 3].include?(x)
来源：http://cqx.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://odb.cqqwz.cn

[B15] 布尔运算与取反
来源：http://lne.yueranfly.top

Py:   a and b or not c
来源：http://pls.ivvv.top

PHP:  $a && $b || !$c
来源：http://byr.xinyue.icu

JS:   a && b || !c
来源：http://fej.ehwqpu.com

TS:   a && b || !c
来源：http://awg.sweek.top

Java: a && b || !c
来源：http://tex.chenlongwang.top

Go:   a && b || !c
来源：http://hqi.daria6918.cn

Ruby: a && b || !c
来源：http://zpa.ybcxt.top

C#:   a && b || !c
来源：http://dyp.aibaodan.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mtm.chenjidiqi.icu

Py:   if not data: return
来源：http://lpk.0kj1m.cn

PHP:  if (!$data) { return; }
来源：http://dgd.dashuyun.cn

JS:   if (!data) return;
来源：http://ziz.chenlongwang.top

TS:   if (!data) return;
来源：http://uxk.sxryk.cn

Java: if (data == null) return;
来源：http://psh.ywan-chungtsiang.top

Go:   if data == nil { return }
来源：http://zyu.redwolf501.top

Ruby: return if data.nil?
来源：http://mum.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://kup.jqgfzy.top

================================================================================
来源：http://eyr.fehbvm.com

C. 函数与作用域
来源：http://hgh.xziqi.cn

================================================================================
来源：http://xso.chenjidiqi.icu

[C01] 定义函数
来源：http://btc.tarul.cn

Py:   def add(a, b): return a + b
来源：http://kmb.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fvx.birdmap.top

JS:   function add(a, b) { return a + b; }
来源：http://jtt.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xyx.daria6918.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://vwx.jlsjyb.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fka.aibaodan.cn

Ruby: def add(a, b); a + b; end
来源：http://phw.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pkc.yonumen.top

[C02] 默认参数
来源：http://usz.daxiang520.top

Py:   def greet(name="World"): return name
来源：http://ryv.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ynt.cdnleiting.top

JS:   function greet(name = "World") { return name; }
来源：http://kmc.jianghu66.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bjy.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hrg.guannengcc.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cpb.quarkkingdee.top

Ruby: def greet(name = "World") = name
来源：http://ppx.jinyuanbaomall.cn

C#:   string Greet(string name = "World") => name;
来源：http://iip.tian-w.cn

[C03] 可变参数
来源：http://mcr.chenzaomai.com

Py:   def total(*args): return sum(args)
来源：http://jua.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vfu.xuetiantiany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mlz.vehdjk.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dvq.0kj1m.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://unz.quarkkingdee.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ped.nwbrower.top

Ruby: def total(*nums); nums.sum; end
来源：http://jmv.nanxuanxn.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kam.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://pzo.snrcjt.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oqj.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vup.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://shl.yj20258.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://okl.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://ooe.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://xau.gogol.net.cn

Ruby: f(a: 1, b: 2)
来源：http://bpe.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://phg.andypj.xyz

[C05] 返回多个值
来源：http://jyj.uphjek.com

Py:   return a, b
来源：http://vmf.jiagoushi.top

PHP:  return [$a, $b];
来源：http://kxt.gotoacloud.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vof.zhaomingkeji.xyz

TS:   return { a, b };
来源：http://shx.xziqi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kag.jlsjyb.cn

Go:   return a, b
来源：http://knp.zycfv.cn

Ruby: return a, b
来源：http://ned.zhoulong.xyz

C#:   return (a, b);              // ValueTuple
来源：http://voo.chenlongwang.top

[C06] 匿名函数 / lambda
来源：http://squ.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://now.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://szv.xziqi.cn

JS:   const square = x => x * x;
来源：http://hzc.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://vti.chenlongwang.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pmq.gzhubu.top

Go:   sq := func(x int) int { return x * x }
来源：http://eww.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://btk.uphjek.com

C#:   Func<int, int> square = x => x * x;
来源：http://lcf.yongpay.top

[C07] 把函数作为参数传入
来源：http://kdm.shangyingyoupin.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ucl.xylfe.cn

PHP:  array_map("strtoupper", $arr);
来源：http://atc.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cpm.sufxvd.cn

TS:   arr.map(String)
来源：http://sow.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wou.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nmu.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://yiw.shuidangran.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fpm.jinqigfzy.top

[C08] 闭包
来源：http://wlx.nanxinkj.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cng.mhx1999.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gcb.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ajz.jqgfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jcw.guowangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xmr.sjlbkw.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rdm.chenlongwang.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wwv.xylfe.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qnh.c1oappe.top

[C09] 递归
来源：http://zwo.jqgfzy.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://muk.shuidangran.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sny.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hiu.yj20258888.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kpt.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://scs.vqdsnc.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xgf.xziqi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://knh.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dlb.vehdjk.com

[C10] 变量作用域
来源：http://voi.hfpthk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wyu.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://prp.pycfn.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vgv.epnwcf.com

TS:   同 JS
来源：http://rll.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://nld.ywan-chungtsiang.top

Go:   花括号块级作用域
来源：http://qcq.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://onk.smart0.xyz

C#:   块级作用域
来源：http://ack.jyoumei.cn

[C11] 模块导入与导出
来源：http://cil.9152youxi.cn

Py:   from module import func
来源：http://eup.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://oyl.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tuu.hysaishi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qhv.cqqwz.cn

Java: import java.util.List;
来源：http://qhi.wangshuangyany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://goh.hammf.cn

Ruby: require "json"; require_relative "./util"
来源：http://yaq.meibo888.top

C#:   using System.Text;
来源：http://haa.ybcxt.top

[C12] 立即执行函数 IIFE
来源：http://kjo.zdqjudy.top

Py:   (lambda: print("run"))()
来源：http://vzk.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://lbh.ivvv.top

JS:   (() => { console.log("run"); })();
来源：http://uyx.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://utp.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://noe.0kj1m.cn

Go:   func() { fmt.Println("run") }()
来源：http://jxi.bjfxy.top

Ruby: -> { puts "run" }.call
来源：http://gta.xuetiantiany.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xwz.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://cik.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pzc.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pqz.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gbn.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nqi.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://pwd.hongshengwenyu.top

Go:   func add(a, b int) int
来源：http://mhl.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kdl.fanxiaobao.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://whi.52xcode.cn

[C14] 泛型函数
来源：http://hlr.jyoumei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://deu.xinyue.icu

PHP:  // 无泛型
来源：http://qwg.bjfxy.top

JS:   // 无泛型
来源：http://sej.ppjwa.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rbh.ppjwa.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zoa.gotoacloud.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bce.daxiang520.top

Ruby: # 无泛型
来源：http://mma.316326.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lpj.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://moh.jinyuanbaomall.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pnn.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://vso.xingfuxueyuan.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pck.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xro.cucudq.cn

Java: // 无解构
来源：http://knv.chenjidiqi.icu

Go:   // 无解构
来源：http://uer.ydzc1.top

Ruby: a, b = pair
来源：http://xbk.epnwcf.com

C#:   var (a, b) = pair;
来源：http://jkk.yueranfly.top

[C16] 函数 / 方法重载
来源：http://xtg.jinghuilouyu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ukn.9152youxi.cn

PHP:  // 无重载
来源：http://imo.zhijiandao.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://cnw.shanyushiyangkeji.top

TS:   // 用联合类型或重载签名声明
来源：http://akx.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://day.bjfxy.top

Go:   // 无重载：用不同函数名
来源：http://sph.xylfe.cn

Ruby: # 无重载：靠动态参数
来源：http://lzi.shanyushiyangtech.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lrh.zhoulong.xyz

================================================================================
来源：http://wea.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://rou.jqgfzy.top

================================================================================
来源：http://vyf.jiagoushi.top

[D01] 创建数组 / 列表
来源：http://gik.birdmap.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zon.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yfg.jyoumei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fuh.fktsv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hug.sjlbkw.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ctf.zycfv.cn

Go:   arr := []int{1, 2, 3}
来源：http://rtf.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://skw.fengsongda.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fid.bjfxy.top

[D02] 追加元素到末尾
来源：http://qgx.smart0.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hxz.redwolf501.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aza.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://slp.fehbvm.com

TS:   arr.push(4);
来源：http://alu.zdbjq.cn

Java: list.add(4);
来源：http://iql.hywenlv.cn

Go:   arr = append(arr, 4)
来源：http://zzu.nanxinkj.top

Ruby: arr << 4; arr.push(5)
来源：http://tur.zhijiandao.cn

C#:   list.Add(4);
来源：http://dmu.ybcxt.top

[D03] 在指定位置插入元素
来源：http://ufq.ppjwa.cn

Py:   arr.insert(0, 0)
来源：http://ieu.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pju.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://amx.jiagoushi.top

TS:   arr.splice(0, 0, 0);
来源：http://jly.chenzaomai.com

Java: list.add(0, 0);
来源：http://brs.xuetiantiany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sfv.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ocs.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://khp.shuidangran.top

[D04] 删除元素
来源：http://mhj.nanxinkj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nng.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fwn.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uqq.yangfankeji.com

TS:   arr.splice(0, 1);
来源：http://toy.yangfankeji.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kvc.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ziz.dianchejie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://toc.yueranfly.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fcf.tanke756.top

[D05] 访问与修改元素
来源：http://qsb.hammf.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hvj.gogol.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cva.aizwys.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nwz.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://lpq.xylfe.cn

Java: list.get(0); list.set(0, 9);
来源：http://cma.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://spn.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xam.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nhv.nanxuanxn.top

[D06] 数组长度
来源：http://buf.hesvh.cn

Py:   len(arr)
来源：http://kdt.daria6918.cn

PHP:  count($arr);
来源：http://hws.yuxming.cn

JS:   arr.length
来源：http://cdc.yueranfly.top

TS:   arr.length
来源：http://lui.tianlin.xyz

Java: list.size();
来源：http://cng.cdnleiting.top

Go:   len(arr)
来源：http://ecs.tanke756.top

Ruby: arr.length; arr.size
来源：http://nho.zycfv.cn

C#:   list.Count;
来源：http://asj.cqqwz.cn

[D07] 切片 / 取子数组
来源：http://xov.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ssl.jqgufenzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://lji.xingfuxueyuan.xyz

JS:   arr.slice(1, 4);
来源：http://qaw.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://kjy.yj202588.top

Java: list.subList(1, 4);
来源：http://ttu.ppjwa.cn

Go:   arr[1:4]
来源：http://rlt.yanxiufei.cn

Ruby: arr[1, 3]
来源：http://hjm.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://suw.cheryme.top

[D08] 合并两个数组
来源：http://qga.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://qdy.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://znj.jyoumei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ujw.aibaodan.cn

TS:   [...a, ...b];
来源：http://aqv.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aoj.epnwcf.com

Go:   append(a, b...)
来源：http://qzv.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://xko.sweek.top

C#:   a.Concat(b).ToList()
来源：http://kme.cucudq.cn

[D09] 排序（升序）
来源：http://hjz.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://dsd.yuanzhike.top


<!-- 参考信息 -->