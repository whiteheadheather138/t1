代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://szm.ydzc1.top

[B10] 遍历同时拿索引
来源：http://iqq.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hwu.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cir.hfpthk.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vuo.kuanghao11.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://otb.jianghu66.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tsz.yueranfly.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gyl.bbcook.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vbk.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qlw.sjlbkw.cn

[B11] 生成数字序列 / 区间
来源：http://vei.havefunace.top

Py:   list(range(0, 10, 2))
来源：http://tnm.hywenlv.cn

PHP:  range(0, 10, 2);
来源：http://imi.quarkkingdee.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iwc.feifeiyinyue.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gkz.yangfankeji.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kvv.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fwn.dianchejie.cn

Ruby: (0...10).step(2).to_a
来源：http://rmy.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://aux.meibo888.top

[B12] 跳出多层循环
来源：http://drg.nanxinkj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xuc.0kj1m.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hom.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sab.haohaochexian.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iwm.gotoacloud.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hlf.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hyq.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cug.xuetiantiany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kfe.zhijiandao.cn

[B13] 判断是否为数字
来源：http://xuh.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://sds.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://zle.zdbjq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hvq.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kms.hfpthk.cn

Java: x instanceof Number
来源：http://sky.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hly.sysykeji.top

Ruby: x.is_a?(Numeric)
来源：http://jje.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://qhk.andypj.xyz

[B14] 判断值是否在集合内
来源：http://zhn.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xgh.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xam.shzxlz.cn

JS:   [1, 2, 3].includes(x)
来源：http://ajl.haohaochexian.top

TS:   [1, 2, 3].includes(x)
来源：http://kcg.sjlbkw.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://koe.meibo888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://udi.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lse.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://flk.meibo888.top

[B15] 布尔运算与取反
来源：http://hsi.zhixingplan.top

Py:   a and b or not c
来源：http://pfb.dianchejie.cn

PHP:  $a && $b || !$c
来源：http://bhs.tian-w.cn

JS:   a && b || !c
来源：http://oob.yj20258888.top

TS:   a && b || !c
来源：http://drp.ydzc1.top

Java: a && b || !c
来源：http://pcm.feifeiyinyue.top

Go:   a && b || !c
来源：http://icf.tian-w.cn

Ruby: a && b || !c
来源：http://ikw.zhengqikj.top

C#:   a && b || !c
来源：http://pxq.birdmap.top

[B16] 卫语句：不满足条件提前返回
来源：http://mlx.yuanzhike.top

Py:   if not data: return
来源：http://rny.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://yua.9152youxi.cn

JS:   if (!data) return;
来源：http://aff.yj202588.top

TS:   if (!data) return;
来源：http://tki.yangfankeji.com

Java: if (data == null) return;
来源：http://sqz.yongpay.top

Go:   if data == nil { return }
来源：http://lbe.ehwqpu.com

Ruby: return if data.nil?
来源：http://kcn.gotoacloud.top

C#:   if (data == null) return;
来源：http://qdq.iojbl.cn

================================================================================
来源：http://zfb.316326.xyz

C. 函数与作用域
来源：http://fch.hongshengwenyu.top

================================================================================
来源：http://jdb.zhiwuduotai.top

[C01] 定义函数
来源：http://gyi.gogol.net.cn

Py:   def add(a, b): return a + b
来源：http://pjv.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fqd.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://wzj.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vfa.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tlq.ydjk.org.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ozv.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://xyi.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fjk.xziqi.cn

[C02] 默认参数
来源：http://uhv.hnqzz.top

Py:   def greet(name="World"): return name
来源：http://hdv.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://scf.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://wqd.chenzaomai.com

TS:   function greet(name: string = "World") { return name; }
来源：http://jrn.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://upq.c1oappe.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://thf.xuanzx.com

Ruby: def greet(name = "World") = name
来源：http://mln.shzxlz.cn

C#:   string Greet(string name = "World") => name;
来源：http://ryz.smart0.xyz

[C03] 可变参数
来源：http://oct.jinyuanbaomall.cn

Py:   def total(*args): return sum(args)
来源：http://oln.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ugk.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fnf.guannengcc.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lhe.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://aqk.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://erv.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://mdb.dashuyun.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rgp.xuanzx.com

[C04] 命名参数 / 关键字参数
来源：http://jvv.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://caa.ctjpmb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yzi.yangfankeji.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qza.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rqa.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://dbs.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://mfu.zhixingplan.top

Ruby: f(a: 1, b: 2)
来源：http://exg.zhijiandao.cn

C#:   f(a: 1, b: 2)
来源：http://hcl.yangfankeji.com

[C05] 返回多个值
来源：http://jnp.bjfxy.top

Py:   return a, b
来源：http://nnc.tarul.cn

PHP:  return [$a, $b];
来源：http://fmh.hywenlv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://tqj.sysykeji.top

TS:   return { a, b };
来源：http://wvo.fengsongda.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fzp.guowangkeji.top

Go:   return a, b
来源：http://inu.epnwcf.com

Ruby: return a, b
来源：http://ims.cashguo.top

C#:   return (a, b);              // ValueTuple
来源：http://tjs.ivvv.top

[C06] 匿名函数 / lambda
来源：http://scy.cheryme.top

Py:   square = lambda x: x * x
来源：http://kfi.hongshengwenyu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://paz.xylfe.cn

JS:   const square = x => x * x;
来源：http://uat.chenjidiqi.icu

TS:   const square = (x: number): number => x * x;
来源：http://hpb.sweek.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://sqw.ivvv.top

Go:   sq := func(x int) int { return x * x }
来源：http://pma.mhx1999.top

Ruby: square = ->(x) { x * x }
来源：http://yue.jinqigufen.top

C#:   Func<int, int> square = x => x * x;
来源：http://hbl.zhongyouzk.top

[C07] 把函数作为参数传入
来源：http://qao.hysaishi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bwa.hnxiangtu.top

PHP:  array_map("strtoupper", $arr);
来源：http://ann.nanxinkj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lsv.chenjidiqi.icu

TS:   arr.map(String)
来源：http://ksn.shanyushiyangkeji.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mhe.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kbs.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://wrl.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://obu.epnwcf.com

[C08] 闭包
来源：http://kwt.52xcode.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wcg.zhiwuduotai.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uie.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iuu.zdbjq.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nlf.sxryk.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yxc.ivvv.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kpe.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nrb.redwolf501.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rxx.bjfxy.top

[C09] 递归
来源：http://uiv.xuanzx.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ehs.birdmap.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yhk.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ebo.ehwqpu.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bkp.wangshuangyany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ojq.xuetiantiany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cnx.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://azv.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lmp.zhoulong.xyz

[C10] 变量作用域
来源：http://itt.meibo888.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zpm.yonumen.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bdf.xziqi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sxk.fengsongda.top

TS:   同 JS
来源：http://yjj.jinyuanbaomall.cn

Java: 方法内为块级作用域
来源：http://ojk.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://ilj.zhixingplan.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fuj.xziqi.cn

C#:   块级作用域
来源：http://fvz.haohaochexian.top

[C11] 模块导入与导出
来源：http://rit.aibaodan.cn

Py:   from module import func
来源：http://pvs.chenzaomai.com

PHP:  require "file.php";  或 use App\Service;
来源：http://zff.yangfankeji.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://szq.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mbh.ctjpmb.com

Java: import java.util.List;
来源：http://bgp.svipenyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vuf.sjlbkw.cn

Ruby: require "json"; require_relative "./util"
来源：http://lzt.dashuyun.cn

C#:   using System.Text;
来源：http://zwm.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://wks.wangshuangyany.cn

Py:   (lambda: print("run"))()
来源：http://vjr.ehwqpu.com

PHP:  (function () { echo "run"; })();
来源：http://vpq.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://fdu.sweek.top

TS:   (() => { console.log("run"); })();
来源：http://uyl.jinqigfzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qwv.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://ucd.yuanzhike.top

Ruby: -> { puts "run" }.call
来源：http://ynb.yangfankeji.com

C#:   // 无 IIFE：用静态构造函数
来源：http://dto.yuanzhike.top

[C13] 类型声明 / 类型注解
来源：http://fhf.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lha.xuanzx.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fpj.yuanzhike.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ftj.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lue.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://nsc.dashuyun.cn

Go:   func add(a, b int) int
来源：http://fta.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ztx.52xcode.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rjj.fehbvm.com

[C14] 泛型函数
来源：http://azp.ppjwa.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://olt.yfazqb.com

PHP:  // 无泛型
来源：http://vyk.zhoulong.xyz

JS:   // 无泛型
来源：http://fie.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iyd.ydjk.org.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hwq.yuanzhike.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://azb.tianlin.xyz

Ruby: # 无泛型
来源：http://msz.sjlbkw.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xpn.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://efx.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zzl.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://jua.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yvy.shuidangran.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ucp.sufxvd.cn

Java: // 无解构
来源：http://ztn.yj202588.top

Go:   // 无解构
来源：http://clm.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://fxt.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://shq.gzhubu.top

[C16] 函数 / 方法重载
来源：http://vfb.c1oappe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sun.yuanzhike.top

PHP:  // 无重载
来源：http://cfp.shanyushiyangtech.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ckq.xuanzx.com

TS:   // 用联合类型或重载签名声明
来源：http://rxv.aibaodan.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jzd.ehwqpu.com

Go:   // 无重载：用不同函数名
来源：http://tmq.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://kdq.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cls.fzhhl.top

================================================================================
来源：http://mbq.aibaodan.cn

D. 数组 / 列表 / 集合
来源：http://ggi.feifeiyinyue.top

================================================================================
来源：http://jsj.yvedp.cn

[D01] 创建数组 / 列表
来源：http://mxy.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bkw.vehdjk.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wuq.jinghuilouyu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zli.yuxming.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dln.xingfuxueyuan.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ojv.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://xwh.fehbvm.com

Ruby: arr = [1, 2, 3]
来源：http://gce.sjlbkw.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://anr.yj20258888.top

[D02] 追加元素到末尾
来源：http://mnz.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rxc.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://von.gaohongyu789.top

JS:   arr.push(4);
来源：http://lxy.sweek.top

TS:   arr.push(4);
来源：http://rog.smart0.xyz

Java: list.add(4);
来源：http://ykw.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://dfe.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://xlu.guowangkeji.top

C#:   list.Add(4);
来源：http://upy.hfpthk.cn

[D03] 在指定位置插入元素
来源：http://osi.snrcjt.cn

Py:   arr.insert(0, 0)
来源：http://lid.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ebu.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://atm.aizwys.cn

TS:   arr.splice(0, 0, 0);
来源：http://fka.ppjwa.cn

Java: list.add(0, 0);
来源：http://slp.pycfn.com

Go:   arr = append([]int{0}, arr...)
来源：http://drk.gotoacloud.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nbt.wangshuangyany.cn

C#:   list.Insert(0, 0);
来源：http://wzf.yonumen.top

[D04] 删除元素
来源：http://rtu.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xwy.kuanghao11.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ifu.yanxiufei.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fkv.havefunace.top

TS:   arr.splice(0, 1);
来源：http://kco.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ial.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tdu.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gtl.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blw.zycfv.cn

[D05] 访问与修改元素
来源：http://nek.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yat.fzhhl.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://spw.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xbs.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://uoh.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://rla.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://hrg.zhongyouzk.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://giv.ppjwa.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dnp.redwolf501.top

[D06] 数组长度
来源：http://bvw.fehbvm.com

Py:   len(arr)
来源：http://drv.cashguo.top

PHP:  count($arr);
来源：http://cly.chenlongwang.top

JS:   arr.length
来源：http://bpw.dashuyun.cn

TS:   arr.length
来源：http://fcv.nanxinkj.top

Java: list.size();
来源：http://lsg.quarkkingdee.top

Go:   len(arr)
来源：http://kzn.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://kkf.bbcook.cn

C#:   list.Count;
来源：http://yni.sjlbkw.cn

[D07] 切片 / 取子数组
来源：http://rtx.gzhubu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://szz.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kml.xingfuxueyuan.xyz

JS:   arr.slice(1, 4);
来源：http://yez.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://ilj.aizwys.cn

Java: list.subList(1, 4);
来源：http://rvo.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://lfz.zhaomingkeji.xyz

Ruby: arr[1, 3]
来源：http://lni.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://hbs.snrcjt.cn

[D08] 合并两个数组
来源：http://lin.tarul.cn

Py:   a + b;  a.extend(b)
来源：http://jeg.pycfn.com

PHP:  array_merge($a, $b);
来源：http://zyb.jyoumei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kry.daria6918.cn

TS:   [...a, ...b];
来源：http://fua.shangyingyoupin.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iob.redwolf501.top

Go:   append(a, b...)
来源：http://wtr.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://rys.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://roq.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://blu.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://ijz.shanyushiyangtech.top

PHP:  sort($arr);
来源：http://rxq.jyoumei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bqg.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dzv.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jtf.hfpthk.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hjf.ybcxt.top

Ruby: arr.sort
来源：http://itz.hfpthk.cn

C#:   list.Sort();
来源：http://kdr.birdmap.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://buy.hnxiangtu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://whf.nanxuanxn.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://llc.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vzw.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rzk.c1oappe.top


<!-- 参考信息 -->