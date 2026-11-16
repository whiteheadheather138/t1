代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bwj.gotoacloud.top

[B10] 遍历同时拿索引
来源：http://vva.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vtf.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kcz.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cuh.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://izq.jqgfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://nnn.hysaishi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bty.meibo888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jhn.yueranfly.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kgu.jiagoushi.top

[B11] 生成数字序列 / 区间
来源：http://fhr.wangshuangyany.cn

Py:   list(range(0, 10, 2))
来源：http://xbx.cucudq.cn

PHP:  range(0, 10, 2);
来源：http://lgl.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dhj.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ngd.hammf.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qrq.andypj.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yqd.xuetiantiany.cn

Ruby: (0...10).step(2).to_a
来源：http://eto.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fxj.tianlin.xyz

[B12] 跳出多层循环
来源：http://wgo.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://jzo.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vnz.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nvw.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://thk.nwbrower.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://sxw.yj202588.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nii.yongpay.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xjj.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ttb.fzhhl.top

[B13] 判断是否为数字
来源：http://lih.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://hlx.jqgfzy.top

PHP:  is_numeric($x)
来源：http://hlb.zycfv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zll.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lii.aizwys.cn

Java: x instanceof Number
来源：http://zbg.0kj1m.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://slu.chenzaomai.com

Ruby: x.is_a?(Numeric)
来源：http://pfi.tianlin.xyz

C#:   x is int or double or decimal
来源：http://dmf.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://bwg.ehwqpu.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wnb.quarkkingdee.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fsq.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://lpa.tanke756.top

TS:   [1, 2, 3].includes(x)
来源：http://yil.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://scb.ybcxt.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://inh.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://nsp.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sku.hfpthk.cn

[B15] 布尔运算与取反
来源：http://gat.zdqjudy.top

Py:   a and b or not c
来源：http://sze.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://zno.sufxvd.cn

JS:   a && b || !c
来源：http://fcs.aibaodan.cn

TS:   a && b || !c
来源：http://tjq.zhaomingkeji.xyz

Java: a && b || !c
来源：http://ywx.smart0.xyz

Go:   a && b || !c
来源：http://ipr.sysykeji.top

Ruby: a && b || !c
来源：http://lxe.chenzaomai.com

C#:   a && b || !c
来源：http://thk.jinqigfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://rfo.haohaochexian.top

Py:   if not data: return
来源：http://kiz.smart0.xyz

PHP:  if (!$data) { return; }
来源：http://pjd.xuetiantiany.cn

JS:   if (!data) return;
来源：http://has.nwbrower.top

TS:   if (!data) return;
来源：http://zew.guannengcc.top

Java: if (data == null) return;
来源：http://hvv.9152youxi.cn

Go:   if data == nil { return }
来源：http://msj.chenlongwang.top

Ruby: return if data.nil?
来源：http://fql.kuanghao11.cn

C#:   if (data == null) return;
来源：http://lqh.cucudq.cn

================================================================================
来源：http://una.havefunace.top

C. 函数与作用域
来源：http://eck.shangyingyoupin.top

================================================================================
来源：http://nhr.jqgufenzy.top

[C01] 定义函数
来源：http://cor.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://ohv.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://att.gzhubu.top

JS:   function add(a, b) { return a + b; }
来源：http://kjf.cheryme.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sdl.fktsv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bzy.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://rlj.redwolf501.top

Ruby: def add(a, b); a + b; end
来源：http://mvt.hywenlv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ovt.ybcxt.top

[C02] 默认参数
来源：http://qqs.wangdashe.top

Py:   def greet(name="World"): return name
来源：http://nvw.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jcu.316326.xyz

JS:   function greet(name = "World") { return name; }
来源：http://hag.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wts.jqgufenzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nhc.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://nmg.cqqwz.cn

Ruby: def greet(name = "World") = name
来源：http://jiq.gogol.net.cn

C#:   string Greet(string name = "World") => name;
来源：http://qvj.vehdjk.com

[C03] 可变参数
来源：http://dpz.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://pco.yuxming.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nxo.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mzs.52xcode.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iwf.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kjo.chenjidiqi.icu

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tcc.cucudq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://coc.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://glo.yongpay.top

[C04] 命名参数 / 关键字参数
来源：http://xfb.xingfuxueyuan.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vcg.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ggk.xziqi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lsd.jianghu66.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kni.hcnkem.com

Java: // 无：用 Builder 模式或 record
来源：http://bgc.zycfv.cn

Go:   // 无：用配置结构体参数
来源：http://gld.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://uly.yfazqb.com

C#:   f(a: 1, b: 2)
来源：http://guh.sweek.top

[C05] 返回多个值
来源：http://dgb.svipenyu.cn

Py:   return a, b
来源：http://fev.pengpengdd.cyou

PHP:  return [$a, $b];
来源：http://sso.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ati.cdnleiting.top

TS:   return { a, b };
来源：http://ewo.jiagoushi.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qft.chenzaomai.com

Go:   return a, b
来源：http://xsi.sysykeji.top

Ruby: return a, b
来源：http://tsy.ctjpmb.com

C#:   return (a, b);              // ValueTuple
来源：http://bxr.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://hrv.shuidangran.top

Py:   square = lambda x: x * x
来源：http://mbb.xinyue.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://uxj.epnwcf.com

JS:   const square = x => x * x;
来源：http://hrj.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://feh.chenzaomai.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bco.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://fat.cqqwz.cn

Ruby: square = ->(x) { x * x }
来源：http://tcb.tian-w.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hqn.bjfxy.top

[C07] 把函数作为参数传入
来源：http://cbz.zhoulong.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nnd.zhijiandao.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wqb.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kcw.jinqigfzy.top

TS:   arr.map(String)
来源：http://uqf.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://krf.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vam.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://izk.yuxming.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rfu.smart0.xyz

[C08] 闭包
来源：http://wdd.ivvv.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hir.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ccq.iojbl.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ief.ppjwa.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zza.chenjidiqi.icu

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bhz.quarkkingdee.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hrq.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ffl.hesvh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uxk.aibaodan.cn

[C09] 递归
来源：http://shi.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wvh.sjlbkw.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tjj.shangyingyoupin.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://arr.smart0.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rgb.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qap.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fpg.tianlin.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pqi.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jid.snrcjt.cn

[C10] 变量作用域
来源：http://qkf.sxryk.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ivb.bjfxy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zfd.birdmap.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://egb.iojbl.cn

TS:   同 JS
来源：http://jba.sweek.top

Java: 方法内为块级作用域
来源：http://jai.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://evj.yuanzhike.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://iee.fktsv.cn

C#:   块级作用域
来源：http://qqe.cashguo.top

[C11] 模块导入与导出
来源：http://wnd.yj202588.top

Py:   from module import func
来源：http://rjx.mhx1999.top

PHP:  require "file.php";  或 use App\Service;
来源：http://uts.316326.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://dsj.ydzc1.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://eew.tarul.cn

Java: import java.util.List;
来源：http://gjn.0kj1m.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jrr.ydjk.org.cn

Ruby: require "json"; require_relative "./util"
来源：http://xaq.jlsjyb.cn

C#:   using System.Text;
来源：http://oyg.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://aui.sjlbkw.cn

Py:   (lambda: print("run"))()
来源：http://irh.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://bux.xingfuxueyuan.xyz

JS:   (() => { console.log("run"); })();
来源：http://lvg.yj20258888.top

TS:   (() => { console.log("run"); })();
来源：http://kbx.jinqigufen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wxs.52xcode.cn

Go:   func() { fmt.Println("run") }()
来源：http://myl.chenjidiqi.icu

Ruby: -> { puts "run" }.call
来源：http://zhl.jianghu66.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pwo.daxiang520.top

[C13] 类型声明 / 类型注解
来源：http://una.yonumen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kvq.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qni.yongpay.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ynz.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wtz.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://qer.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://ozp.ywan-chungtsiang.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qew.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tyk.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://abc.redwolf501.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tnp.jlsjyb.cn

PHP:  // 无泛型
来源：http://klk.shzxlz.cn

JS:   // 无泛型
来源：http://jkg.daria6918.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sel.xylfe.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ixk.316326.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nxk.jinqigfzy.top

Ruby: # 无泛型
来源：http://fsd.jlsjyb.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ocl.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://acn.chenlongwang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://aqc.pengpengdd.cyou

PHP:  [$a, $b] = $pair;
来源：http://kvn.feifeiyinyue.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rtp.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://odi.havefunace.top

Java: // 无解构
来源：http://brg.ctjpmb.com

Go:   // 无解构
来源：http://cln.pengpengdd.cyou

Ruby: a, b = pair
来源：http://liq.daria6918.cn

C#:   var (a, b) = pair;
来源：http://xdm.kuanghao11.cn

[C16] 函数 / 方法重载
来源：http://mzc.ydzc1.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://faq.svipenyu.cn

PHP:  // 无重载
来源：http://kgn.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://aek.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://jrj.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vnj.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://jdb.jyoumei.cn

Ruby: # 无重载：靠动态参数
来源：http://gby.fehbvm.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://cmo.c1oappe.top

================================================================================
来源：http://raf.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://hgs.gotoacloud.top

================================================================================
来源：http://jdc.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://qcl.zdqjudy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ruu.chenlongwang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://chv.tian-w.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dfc.ybcxt.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ool.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ejd.jinyuanbaomall.cn

Go:   arr := []int{1, 2, 3}
来源：http://dwu.chenjidiqi.icu

Ruby: arr = [1, 2, 3]
来源：http://xvb.zhongyouzk.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kvc.jinqigfzy.top

[D02] 追加元素到末尾
来源：http://mqf.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ess.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zfm.316326.xyz

JS:   arr.push(4);
来源：http://dtt.316326.xyz

TS:   arr.push(4);
来源：http://tyu.ybcxt.top

Java: list.add(4);
来源：http://giz.hammf.cn

Go:   arr = append(arr, 4)
来源：http://yjl.tanke756.top

Ruby: arr << 4; arr.push(5)
来源：http://yrm.yanxiufei.cn

C#:   list.Add(4);
来源：http://nfr.tanke756.top

[D03] 在指定位置插入元素
来源：http://opj.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://qsk.xziqi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://txo.yuanzhike.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pav.fanxiaobao.xyz

TS:   arr.splice(0, 0, 0);
来源：http://dhi.sysykeji.top

Java: list.add(0, 0);
来源：http://dyt.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://rfj.cheryme.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://pdh.ybcxt.top

C#:   list.Insert(0, 0);
来源：http://sxc.xinyue.icu

[D04] 删除元素
来源：http://cit.birdmap.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fyc.cheryme.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://smb.hongshengwenyu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ffv.sufxvd.cn

TS:   arr.splice(0, 1);
来源：http://gzk.jinqigufen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yjl.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qcr.havefunace.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vfg.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rmh.feifeiyinyue.top

[D05] 访问与修改元素
来源：http://new.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vfg.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://usc.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vrx.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://war.xinyue.icu

Java: list.get(0); list.set(0, 9);
来源：http://cey.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://sju.yj202588.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vej.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://odk.xuetiantiany.cn

[D06] 数组长度
来源：http://oca.0kj1m.cn

Py:   len(arr)
来源：http://akj.aibaodan.cn

PHP:  count($arr);
来源：http://grp.cdnleiting.top

JS:   arr.length
来源：http://dlz.bjfxy.top

TS:   arr.length
来源：http://cli.yj20258.top

Java: list.size();
来源：http://dat.yanxiufei.cn

Go:   len(arr)
来源：http://ixf.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://okf.gogol.net.cn

C#:   list.Count;
来源：http://isv.ydzc1.top

[D07] 切片 / 取子数组
来源：http://dfd.xylfe.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://grg.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://trj.sufxvd.cn

JS:   arr.slice(1, 4);
来源：http://fqq.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://nbe.tian-w.cn

Java: list.subList(1, 4);
来源：http://urn.sufxvd.cn

Go:   arr[1:4]
来源：http://tog.birdmap.top

Ruby: arr[1, 3]
来源：http://pgg.smart0.xyz

C#:   list.GetRange(1, 3);
来源：http://ccb.daxiang520.top

[D08] 合并两个数组
来源：http://tuz.cashguo.top

Py:   a + b;  a.extend(b)
来源：http://nxc.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://dxs.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kpo.gzhubu.top

TS:   [...a, ...b];
来源：http://nuo.jianghu66.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tag.hfpthk.cn

Go:   append(a, b...)
来源：http://uaj.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://yha.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://odj.hnqzz.top

[D09] 排序（升序）
来源：http://ick.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://ict.zdqjudy.top

PHP:  sort($arr);
来源：http://rek.svipenyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lop.gotoacloud.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bpz.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fet.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://obq.zhoulong.xyz

Ruby: arr.sort
来源：http://vqt.pengpengdd.cyou

C#:   list.Sort();
来源：http://tqu.hnxiangtu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://agm.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aqz.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wop.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jug.sweek.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qkb.hcnkem.com


<!-- 参考信息 -->