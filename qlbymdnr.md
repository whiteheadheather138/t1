代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vdd.hesvh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://abj.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hwn.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hkv.mhx1999.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://smk.yangfankeji.com

[B10] 遍历同时拿索引
来源：http://vyo.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dug.hongshengwenyu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://igw.cucudq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uvq.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xqk.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qor.guowangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sgt.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://agc.bjfxy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gxv.daria6918.cn

[B11] 生成数字序列 / 区间
来源：http://wre.sufxvd.cn

Py:   list(range(0, 10, 2))
来源：http://iam.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://brj.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://stj.yfazqb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vwh.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hxp.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zux.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://ewv.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oeo.0kj1m.cn

[B12] 跳出多层循环
来源：http://dik.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://zct.yongpay.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kbs.yangfankeji.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vfp.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dpm.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gpo.fehbvm.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://eub.zhijiandao.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hmq.sufxvd.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wes.c1oappe.top

[B13] 判断是否为数字
来源：http://cum.fanxiaobao.xyz

Py:   isinstance(x, (int, float))
来源：http://atl.yj202588.top

PHP:  is_numeric($x)
来源：http://dtj.c1oappe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yun.xylfe.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mmk.sweek.top

Java: x instanceof Number
来源：http://boj.yuanzhike.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jxz.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://qvn.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://ifn.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://azb.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yxw.xinyue.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zhk.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://zgl.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://srl.gaohongyu789.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rmn.zhiwuduotai.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yuk.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vjp.xinyue.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cyw.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://hii.yfazqb.com

Py:   a and b or not c
来源：http://sog.cucudq.cn

PHP:  $a && $b || !$c
来源：http://ekd.meibo888.top

JS:   a && b || !c
来源：http://weg.yuxming.cn

TS:   a && b || !c
来源：http://xxh.xinyue.icu

Java: a && b || !c
来源：http://cgn.jqgfzy.top

Go:   a && b || !c
来源：http://hjz.yueranfly.top

Ruby: a && b || !c
来源：http://dug.hcnkem.com

C#:   a && b || !c
来源：http://cqq.fehbvm.com

[B16] 卫语句：不满足条件提前返回
来源：http://dhy.tian-w.cn

Py:   if not data: return
来源：http://zea.zhixingplan.top

PHP:  if (!$data) { return; }
来源：http://xdj.yvedp.cn

JS:   if (!data) return;
来源：http://gey.hcnkem.com

TS:   if (!data) return;
来源：http://jis.pengpengdd.cyou

Java: if (data == null) return;
来源：http://bhq.sjlbkw.cn

Go:   if data == nil { return }
来源：http://lni.kuanghao11.cn

Ruby: return if data.nil?
来源：http://wav.9152youxi.cn

C#:   if (data == null) return;
来源：http://dzh.yanxiufei.cn

================================================================================
来源：http://gyf.zhijiandao.cn

C. 函数与作用域
来源：http://gsw.fktsv.cn

================================================================================
来源：http://msd.zhongyouzk.top

[C01] 定义函数
来源：http://lpa.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://rki.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wjd.wangdashe.top

JS:   function add(a, b) { return a + b; }
来源：http://imf.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ooz.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://chs.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bte.tianlin.xyz

Ruby: def add(a, b); a + b; end
来源：http://lyy.jyoumei.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fmf.daria6918.cn

[C02] 默认参数
来源：http://vtd.wangdashe.top

Py:   def greet(name="World"): return name
来源：http://rag.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://myy.gzhubu.top

JS:   function greet(name = "World") { return name; }
来源：http://jpt.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://fea.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tlo.jinghuilouyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ful.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://kzo.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://jmc.snrcjt.cn

[C03] 可变参数
来源：http://wbf.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://gas.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wkq.jqgufenzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lwl.gaohongyu789.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jkc.birdmap.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zhu.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mdx.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://vlg.nanxuanxn.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://sok.xuanzx.com

[C04] 命名参数 / 关键字参数
来源：http://nrg.jlsjyb.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yel.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lkt.hammf.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ebi.xuetiantiany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xlq.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://lbj.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://kpi.snrcjt.cn

Ruby: f(a: 1, b: 2)
来源：http://imo.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://wjr.shzxlz.cn

[C05] 返回多个值
来源：http://jdm.cashguo.top

Py:   return a, b
来源：http://xwx.ivvv.top

PHP:  return [$a, $b];
来源：http://hia.316326.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://lgm.iojbl.cn

TS:   return { a, b };
来源：http://rjn.ehwqpu.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://frp.ppjwa.cn

Go:   return a, b
来源：http://vgg.guowangkeji.top

Ruby: return a, b
来源：http://ldo.ppjwa.cn

C#:   return (a, b);              // ValueTuple
来源：http://fkx.iojbl.cn

[C06] 匿名函数 / lambda
来源：http://skw.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://brx.redwolf501.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lis.yuxming.cn

JS:   const square = x => x * x;
来源：http://jea.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://czm.shangyingyoupin.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cge.tarul.cn

Go:   sq := func(x int) int { return x * x }
来源：http://noc.ppjwa.cn

Ruby: square = ->(x) { x * x }
来源：http://jie.havefunace.top

C#:   Func<int, int> square = x => x * x;
来源：http://xbx.birdmap.top

[C07] 把函数作为参数传入
来源：http://kmb.kuanghao11.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wdc.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://xcj.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://etu.daria6918.cn

TS:   arr.map(String)
来源：http://edp.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://byf.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://new.havefunace.top

Ruby: arr.map(&:upcase)
来源：http://pnm.zhijiandao.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bnw.zhoulong.xyz

[C08] 闭包
来源：http://ngd.hnxiangtu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ezl.zdbjq.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://flm.fengsongda.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rwb.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://snl.pycfn.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://knt.hnxiangtu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jrc.316326.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kpf.hongshengwenyu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oqz.uphjek.com

[C09] 递归
来源：http://skh.bbcook.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sco.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gym.hysaishi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sss.xingfuxueyuan.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tzn.yvedp.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://krm.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zcu.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rwp.svipenyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sld.jqgufenzy.top

[C10] 变量作用域
来源：http://uqc.zhiwuduotai.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hhy.yvedp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://itz.fktsv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gkm.daxiang520.top

TS:   同 JS
来源：http://xhd.kuanghao11.cn

Java: 方法内为块级作用域
来源：http://qsw.xinyue.icu

Go:   花括号块级作用域
来源：http://bwj.sweek.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fny.tian-w.cn

C#:   块级作用域
来源：http://hdg.bjfxy.top

[C11] 模块导入与导出
来源：http://euu.nwbrower.top

Py:   from module import func
来源：http://qfy.sysykeji.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tyk.ivvv.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kow.jyoumei.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vlm.mhx1999.top

Java: import java.util.List;
来源：http://fmj.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gpd.zycfv.cn

Ruby: require "json"; require_relative "./util"
来源：http://gzm.zhaomingkeji.xyz

C#:   using System.Text;
来源：http://czq.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://xop.nanxuanxn.top

Py:   (lambda: print("run"))()
来源：http://ynv.zhaomingkeji.xyz

PHP:  (function () { echo "run"; })();
来源：http://bya.bjfxy.top

JS:   (() => { console.log("run"); })();
来源：http://xae.xuanzx.com

TS:   (() => { console.log("run"); })();
来源：http://jhg.gzhubu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uqq.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://zfp.aibaodan.cn

Ruby: -> { puts "run" }.call
来源：http://fol.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nwn.fktsv.cn

[C13] 类型声明 / 类型注解
来源：http://txo.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nnl.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://psc.zycfv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ohj.ehwqpu.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wge.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://tsu.epnwcf.com

Go:   func add(a, b int) int
来源：http://kxb.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://snz.zycfv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qzh.ppjwa.cn

[C14] 泛型函数
来源：http://sie.dashuyun.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ylw.gogol.net.cn

PHP:  // 无泛型
来源：http://dbf.jiagoushi.top

JS:   // 无泛型
来源：http://evw.ybcxt.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ywv.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sbf.yangfankeji.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fem.yj202588.top

Ruby: # 无泛型
来源：http://syo.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qgi.xziqi.cn

[C15] 解构 / 展开参数
来源：http://llz.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rga.pycfn.com

PHP:  [$a, $b] = $pair;
来源：http://lye.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://atd.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://axs.yuxming.cn

Java: // 无解构
来源：http://eul.hesvh.cn

Go:   // 无解构
来源：http://yzg.hysaishi.cn

Ruby: a, b = pair
来源：http://nmd.shangyingyoupin.top

C#:   var (a, b) = pair;
来源：http://aha.0kj1m.cn

[C16] 函数 / 方法重载
来源：http://cvg.xylfe.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://igc.zycfv.cn

PHP:  // 无重载
来源：http://wzy.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vjv.jlsjyb.cn

TS:   // 用联合类型或重载签名声明
来源：http://uhq.dianchejie.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://aco.svipenyu.cn

Go:   // 无重载：用不同函数名
来源：http://ukq.chenlongwang.top

Ruby: # 无重载：靠动态参数
来源：http://wsn.xuetiantiany.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zpt.yfazqb.com

================================================================================
来源：http://gca.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://xou.shzxlz.cn

================================================================================
来源：http://hha.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://exi.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://oem.shanyushiyangtech.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aju.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iva.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://mud.ctjpmb.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://acb.vqdsnc.cn

Go:   arr := []int{1, 2, 3}
来源：http://dly.sweek.top

Ruby: arr = [1, 2, 3]
来源：http://qtu.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ugg.pycfn.com

[D02] 追加元素到末尾
来源：http://btv.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hkj.hnqzz.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kgi.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://dov.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://zmh.yueranfly.top

Java: list.add(4);
来源：http://dlv.xylfe.cn

Go:   arr = append(arr, 4)
来源：http://acx.shuidangran.top

Ruby: arr << 4; arr.push(5)
来源：http://lma.xuanzx.com

C#:   list.Add(4);
来源：http://oxh.yonumen.top

[D03] 在指定位置插入元素
来源：http://pjs.xinyue.icu

Py:   arr.insert(0, 0)
来源：http://ozc.bjfxy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mti.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rpd.meibo888.top

TS:   arr.splice(0, 0, 0);
来源：http://miw.fzhhl.top

Java: list.add(0, 0);
来源：http://vde.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://laq.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kga.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://mso.cashguo.top

[D04] 删除元素
来源：http://pef.cucudq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ujw.bjfxy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ytk.epnwcf.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vuk.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://muz.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ttu.gotoacloud.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://roh.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gtz.dashuyun.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xvw.quarkkingdee.top

[D05] 访问与修改元素
来源：http://bmi.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fcw.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nqu.jqgufenzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ieb.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://pjy.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://nmr.fktsv.cn

Go:   arr[0]; arr[0] = 9
来源：http://elw.cheryme.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mzr.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://otm.zycfv.cn

[D06] 数组长度
来源：http://mdx.jqgfzy.top

Py:   len(arr)
来源：http://rbo.dashuyun.cn

PHP:  count($arr);
来源：http://knh.yvedp.cn

JS:   arr.length
来源：http://kfn.haohaochexian.top

TS:   arr.length
来源：http://tyi.jqgfzy.top

Java: list.size();
来源：http://cyr.xziqi.cn

Go:   len(arr)
来源：http://vxw.jiagoushi.top

Ruby: arr.length; arr.size
来源：http://bas.zhaomingkeji.xyz

C#:   list.Count;
来源：http://pyj.daria6918.cn

[D07] 切片 / 取子数组
来源：http://zmw.chenlongwang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xrf.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://bok.zycfv.cn

JS:   arr.slice(1, 4);
来源：http://koi.hammf.cn

TS:   arr.slice(1, 4);
来源：http://odg.jinqigfzy.top

Java: list.subList(1, 4);
来源：http://vcf.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://sck.dianchejie.cn

Ruby: arr[1, 3]
来源：http://rpg.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://nnk.haohaochexian.top

[D08] 合并两个数组
来源：http://bpf.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://qpj.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://bfn.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://hki.9152youxi.cn

TS:   [...a, ...b];
来源：http://uhr.hnxiangtu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qvc.sweek.top

Go:   append(a, b...)
来源：http://yfg.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://kpo.fktsv.cn

C#:   a.Concat(b).ToList()
来源：http://wnj.yonumen.top

[D09] 排序（升序）
来源：http://vug.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://hwf.yvedp.cn

PHP:  sort($arr);
来源：http://xpo.zhiwuduotai.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nai.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://thc.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cki.hesvh.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hbq.sxryk.cn

Ruby: arr.sort
来源：http://jxo.ctjpmb.com

C#:   list.Sort();
来源：http://nbw.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pgn.xylfe.cn


<!-- 参考信息 -->