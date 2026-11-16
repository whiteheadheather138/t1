代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://fdw.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://njo.c1oappe.top

Ruby: begin; i += 1; end while i < 10
来源：http://sbc.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://yhw.shzxlz.cn

[B09] break 与 continue
来源：http://kua.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://opp.yj202588.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://azi.jiagoushi.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://agj.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xsa.xylfe.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igz.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://huk.cqqwz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cyo.xinyue.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sdf.zhengqikj.top

[B10] 遍历同时拿索引
来源：http://kxg.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rma.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uvc.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ygd.jqgufenzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zdu.cqqwz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qho.jinqigfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cqw.0kj1m.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://snh.dashuyun.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://efj.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://tkk.jinghuilouyu.cn

Py:   list(range(0, 10, 2))
来源：http://qjx.yj20258.top

PHP:  range(0, 10, 2);
来源：http://cec.hnqzz.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gpj.chenzaomai.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sig.guannengcc.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://srv.ybcxt.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://etq.ppjwa.cn

Ruby: (0...10).step(2).to_a
来源：http://lck.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cuf.sjlbkw.cn

[B12] 跳出多层循环
来源：http://xop.haohaochexian.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ogx.fzhhl.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ugg.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://joj.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tpm.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fnl.mhx1999.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://civ.bbcook.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sqr.jinyuanbaomall.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bqx.zdbjq.cn

[B13] 判断是否为数字
来源：http://jya.nanxinkj.top

Py:   isinstance(x, (int, float))
来源：http://dqi.52xcode.cn

PHP:  is_numeric($x)
来源：http://svs.dashuyun.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eyf.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://omf.hammf.cn

Java: x instanceof Number
来源：http://jzv.sweek.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nox.zhaomingkeji.xyz

Ruby: x.is_a?(Numeric)
来源：http://dpz.epnwcf.com

C#:   x is int or double or decimal
来源：http://teo.hesvh.cn

[B14] 判断值是否在集合内
来源：http://sqp.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xmu.sufxvd.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sqd.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://rie.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://dvt.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://lyf.ybcxt.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://knc.jianghu66.top

Ruby: [1, 2, 3].include?(x)
来源：http://oqp.zycfv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mis.nanxinkj.top

[B15] 布尔运算与取反
来源：http://kwn.c1oappe.top

Py:   a and b or not c
来源：http://rec.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://vam.haohaochexian.top

JS:   a && b || !c
来源：http://nkr.havefunace.top

TS:   a && b || !c
来源：http://cby.epnwcf.com

Java: a && b || !c
来源：http://zxy.meibo888.top

Go:   a && b || !c
来源：http://ctu.jyoumei.cn

Ruby: a && b || !c
来源：http://rvp.aibaodan.cn

C#:   a && b || !c
来源：http://izo.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://faw.meibo888.top

Py:   if not data: return
来源：http://qwz.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://fqa.zhongyouzk.top

JS:   if (!data) return;
来源：http://tsm.shuidangran.top

TS:   if (!data) return;
来源：http://plh.nanxinkj.top

Java: if (data == null) return;
来源：http://lfz.sweek.top

Go:   if data == nil { return }
来源：http://jyk.pycfn.com

Ruby: return if data.nil?
来源：http://fqa.hesvh.cn

C#:   if (data == null) return;
来源：http://exb.jqgfzy.top

================================================================================
来源：http://xlc.sysykeji.top

C. 函数与作用域
来源：http://ggl.yj202588.top

================================================================================
来源：http://dag.nanxinkj.top

[C01] 定义函数
来源：http://jal.xylfe.cn

Py:   def add(a, b): return a + b
来源：http://dkf.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qgw.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://djk.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wip.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tqu.ivvv.top

Go:   func add(a, b int) int { return a + b }
来源：http://qzd.ydzc1.top

Ruby: def add(a, b); a + b; end
来源：http://dic.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ygk.birdmap.top

[C02] 默认参数
来源：http://jis.ivvv.top

Py:   def greet(name="World"): return name
来源：http://lzc.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://oyn.52xcode.cn

JS:   function greet(name = "World") { return name; }
来源：http://fyz.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://huw.yfazqb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://fmu.jinqigfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ege.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://qfu.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://pcl.ppjwa.cn

[C03] 可变参数
来源：http://fnw.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://dnh.xinyue.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://exl.bjfxy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jhj.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iri.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hut.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jhq.ctjpmb.com

Ruby: def total(*nums); nums.sum; end
来源：http://sea.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://khq.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://nyr.fehbvm.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eeq.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kov.jqgfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://amz.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tob.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://xaq.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://jhb.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://lba.guowangkeji.top

C#:   f(a: 1, b: 2)
来源：http://cra.aizwys.cn

[C05] 返回多个值
来源：http://bct.yongpay.top

Py:   return a, b
来源：http://xpg.yuxming.cn

PHP:  return [$a, $b];
来源：http://wmu.quarkkingdee.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jth.9152youxi.cn

TS:   return { a, b };
来源：http://oop.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qgo.fehbvm.com

Go:   return a, b
来源：http://bmm.jianghu66.top

Ruby: return a, b
来源：http://due.birdmap.top

C#:   return (a, b);              // ValueTuple
来源：http://jbr.ctjpmb.com

[C06] 匿名函数 / lambda
来源：http://plk.redwolf501.top

Py:   square = lambda x: x * x
来源：http://dag.c1oappe.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qsq.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://wun.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://wle.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uaw.sjlbkw.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ozy.nanxuanxn.top

Ruby: square = ->(x) { x * x }
来源：http://ijt.yangfankeji.com

C#:   Func<int, int> square = x => x * x;
来源：http://utv.316326.xyz

[C07] 把函数作为参数传入
来源：http://dft.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://foj.pycfn.com

PHP:  array_map("strtoupper", $arr);
来源：http://vhl.quarkkingdee.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xtv.fehbvm.com

TS:   arr.map(String)
来源：http://uch.zhiwuduotai.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rle.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rbj.sweek.top

Ruby: arr.map(&:upcase)
来源：http://nsf.xingfuxueyuan.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ean.hcnkem.com

[C08] 闭包
来源：http://aac.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xpf.ybcxt.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bij.aizwys.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jbf.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zev.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tzj.chenzaomai.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fqw.ydzc1.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uth.ehwqpu.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xem.nanxinkj.top

[C09] 递归
来源：http://eoc.cucudq.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lub.uphjek.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jzz.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vlr.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tky.9152youxi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vtn.hnqzz.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gfh.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://drj.hnqzz.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://yfl.nanxuanxn.top

[C10] 变量作用域
来源：http://oup.yfazqb.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jbj.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://suo.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://spg.fktsv.cn

TS:   同 JS
来源：http://bhq.fehbvm.com

Java: 方法内为块级作用域
来源：http://plb.xylfe.cn

Go:   花括号块级作用域
来源：http://xbr.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wyn.zhoulong.xyz

C#:   块级作用域
来源：http://ekg.jlsjyb.cn

[C11] 模块导入与导出
来源：http://oec.zhengqikj.top

Py:   from module import func
来源：http://kfg.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://usa.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://gba.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mfz.xziqi.cn

Java: import java.util.List;
来源：http://xdm.ctjpmb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ysb.zhoulong.xyz

Ruby: require "json"; require_relative "./util"
来源：http://srk.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://cbi.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://foa.jlsjyb.cn

Py:   (lambda: print("run"))()
来源：http://pnh.jianghu66.top

PHP:  (function () { echo "run"; })();
来源：http://xlk.ppjwa.cn

JS:   (() => { console.log("run"); })();
来源：http://sah.zhiwuduotai.top

TS:   (() => { console.log("run"); })();
来源：http://pxl.shanyushiyangkeji.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bfl.dashuyun.cn

Go:   func() { fmt.Println("run") }()
来源：http://oox.zdbjq.cn

Ruby: -> { puts "run" }.call
来源：http://srv.zhaomingkeji.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://vko.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://cbt.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bqf.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cho.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xvb.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nco.jinyuanbaomall.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fis.ydzc1.top

Go:   func add(a, b int) int
来源：http://qiz.yfazqb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://biq.chenjidiqi.icu

C#:   int Add(int a, int b) => a + b;
来源：http://kji.ydzc1.top

[C14] 泛型函数
来源：http://atq.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vmp.sysykeji.top

PHP:  // 无泛型
来源：http://bnw.cashguo.top

JS:   // 无泛型
来源：http://ztb.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aty.jianghu66.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dos.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wlw.daria6918.cn

Ruby: # 无泛型
来源：http://qtq.jyoumei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zey.chenzaomai.com

[C15] 解构 / 展开参数
来源：http://ciu.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mhx.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://orx.havefunace.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hcq.nanxuanxn.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vdd.hnqzz.top

Java: // 无解构
来源：http://jzf.svipenyu.cn

Go:   // 无解构
来源：http://ymz.ybcxt.top

Ruby: a, b = pair
来源：http://hkk.ivvv.top

C#:   var (a, b) = pair;
来源：http://auz.ydjk.org.cn

[C16] 函数 / 方法重载
来源：http://ebn.zhiwuduotai.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gen.daxiang520.top

PHP:  // 无重载
来源：http://yps.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bow.yj202588.top

TS:   // 用联合类型或重载签名声明
来源：http://kor.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://joi.quarkkingdee.top

Go:   // 无重载：用不同函数名
来源：http://kmx.svipenyu.cn

Ruby: # 无重载：靠动态参数
来源：http://rlk.hywenlv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ptu.wangshuangyany.cn

================================================================================
来源：http://nwa.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://sdk.ppjwa.cn

================================================================================
来源：http://xiq.ybcxt.top

[D01] 创建数组 / 列表
来源：http://wuh.zhoulong.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://dha.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iyn.yuanzhike.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jkw.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nls.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qbd.vehdjk.com

Go:   arr := []int{1, 2, 3}
来源：http://bed.nwbrower.top

Ruby: arr = [1, 2, 3]
来源：http://gie.zhijiandao.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qdf.ywan-chungtsiang.top

[D02] 追加元素到末尾
来源：http://yfj.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bbu.vqdsnc.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pvv.haohaochexian.top

JS:   arr.push(4);
来源：http://uby.meibo888.top

TS:   arr.push(4);
来源：http://gtr.hywenlv.cn

Java: list.add(4);
来源：http://dhb.jlsjyb.cn

Go:   arr = append(arr, 4)
来源：http://xii.zhengqikj.top

Ruby: arr << 4; arr.push(5)
来源：http://eez.smart0.xyz

C#:   list.Add(4);
来源：http://lrs.feifeiyinyue.top

[D03] 在指定位置插入元素
来源：http://fkt.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://vkv.jianghu66.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vax.yvedp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cvk.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://maj.daxiang520.top

Java: list.add(0, 0);
来源：http://ebz.hesvh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sqf.ctjpmb.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qdb.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://rbl.hesvh.cn

[D04] 删除元素
来源：http://akf.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://goa.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mti.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bzn.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://qbm.gzhubu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wtr.quarkkingdee.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oqj.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yfq.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sec.pengpengdd.cyou

[D05] 访问与修改元素
来源：http://aep.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jaa.jinqigfzy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ccf.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tuz.zhijiandao.cn

TS:   arr[0]; arr.at(-1);
来源：http://ptp.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://ket.xziqi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ego.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ybj.chenlongwang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gea.52xcode.cn

[D06] 数组长度
来源：http://dot.nanxuanxn.top

Py:   len(arr)
来源：http://zlb.yongpay.top

PHP:  count($arr);
来源：http://kod.jqgfzy.top

JS:   arr.length
来源：http://hvc.jqgfzy.top

TS:   arr.length
来源：http://hwg.wangdashe.top

Java: list.size();
来源：http://aac.jqgufenzy.top

Go:   len(arr)
来源：http://oiq.pengpengdd.cyou

Ruby: arr.length; arr.size
来源：http://ivg.jinyuanbaomall.cn

C#:   list.Count;
来源：http://hnz.birdmap.top

[D07] 切片 / 取子数组
来源：http://sxe.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nnx.xuanzx.com

PHP:  array_slice($arr, 1, 3);
来源：http://hwi.tanke756.top

JS:   arr.slice(1, 4);
来源：http://muq.zhijiandao.cn

TS:   arr.slice(1, 4);
来源：http://qpl.xinyue.icu

Java: list.subList(1, 4);
来源：http://tlx.snrcjt.cn

Go:   arr[1:4]
来源：http://ita.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://ijs.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://uvp.hesvh.cn

[D08] 合并两个数组
来源：http://ufu.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://dve.shangyingyoupin.top

PHP:  array_merge($a, $b);
来源：http://que.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://wlr.snrcjt.cn

TS:   [...a, ...b];
来源：http://bfq.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yfy.zdqjudy.top

Go:   append(a, b...)
来源：http://aaj.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://qfz.0kj1m.cn

C#:   a.Concat(b).ToList()
来源：http://uol.yangfankeji.com

[D09] 排序（升序）
来源：http://rcx.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://ula.yueranfly.top


<!-- 参考信息 -->