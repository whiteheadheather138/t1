代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://smz.shanyushiyangtech.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qjm.yueranfly.top

[B11] 生成数字序列 / 区间
来源：http://trn.zhijiandao.cn

Py:   list(range(0, 10, 2))
来源：http://clb.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://jcg.zhijiandao.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nzh.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zak.chenzaomai.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gvy.guannengcc.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tse.jinqigfzy.top

Ruby: (0...10).step(2).to_a
来源：http://qfs.shanyushiyangtech.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://urc.gaohongyu789.top

[B12] 跳出多层循环
来源：http://ypb.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bem.cdnleiting.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://aqs.ivvv.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ata.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cak.0kj1m.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yaa.jqgufenzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lnw.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xtm.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://axg.cdnleiting.top

[B13] 判断是否为数字
来源：http://qxl.hongshengwenyu.top

Py:   isinstance(x, (int, float))
来源：http://cjt.yvedp.cn

PHP:  is_numeric($x)
来源：http://dxc.xinyue.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dky.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rlc.hysaishi.cn

Java: x instanceof Number
来源：http://eic.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nyh.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://lfa.pengpengdd.cyou

C#:   x is int or double or decimal
来源：http://vqq.shuidangran.top

[B14] 判断值是否在集合内
来源：http://mia.ybcxt.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://enl.havefunace.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vus.jinghuilouyu.cn

JS:   [1, 2, 3].includes(x)
来源：http://eul.vehdjk.com

TS:   [1, 2, 3].includes(x)
来源：http://sjp.nanxinkj.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ncc.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jat.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://pyx.yvedp.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jay.tanke756.top

[B15] 布尔运算与取反
来源：http://rne.ybcxt.top

Py:   a and b or not c
来源：http://upw.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://ctj.feifeiyinyue.top

JS:   a && b || !c
来源：http://fgr.yangfankeji.com

TS:   a && b || !c
来源：http://aks.tianlin.xyz

Java: a && b || !c
来源：http://quc.gzhubu.top

Go:   a && b || !c
来源：http://tfj.quarkkingdee.top

Ruby: a && b || !c
来源：http://wtl.jqgfzy.top

C#:   a && b || !c
来源：http://bqy.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://xsz.xuanzx.com

Py:   if not data: return
来源：http://fcn.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://nct.chenlongwang.top

JS:   if (!data) return;
来源：http://dby.zdbjq.cn

TS:   if (!data) return;
来源：http://mec.daxiang520.top

Java: if (data == null) return;
来源：http://bya.hfpthk.cn

Go:   if data == nil { return }
来源：http://zxs.cdnleiting.top

Ruby: return if data.nil?
来源：http://ajs.yfazqb.com

C#:   if (data == null) return;
来源：http://mfm.jqgufenzy.top

================================================================================
来源：http://wml.aizwys.cn

C. 函数与作用域
来源：http://sfh.cucudq.cn

================================================================================
来源：http://tjb.ivvv.top

[C01] 定义函数
来源：http://djs.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://cgj.jianghu66.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mdl.wangdashe.top

JS:   function add(a, b) { return a + b; }
来源：http://zqh.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tfg.ybcxt.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jlv.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fcs.dashuyun.cn

Ruby: def add(a, b); a + b; end
来源：http://euz.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hro.hfpthk.cn

[C02] 默认参数
来源：http://mnx.tian-w.cn

Py:   def greet(name="World"): return name
来源：http://ede.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://eqy.gaohongyu789.top

JS:   function greet(name = "World") { return name; }
来源：http://wlv.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ixa.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bjr.zhoulong.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zol.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://fos.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://yan.nwbrower.top

[C03] 可变参数
来源：http://twm.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://how.guowangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vez.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dhe.cheryme.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hew.jinghuilouyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vre.c1oappe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rtp.9152youxi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://irw.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qcf.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://ddp.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aiu.havefunace.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tod.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gsk.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hsl.shanyushiyangtech.top

Java: // 无：用 Builder 模式或 record
来源：http://zct.gogol.net.cn

Go:   // 无：用配置结构体参数
来源：http://uws.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://lzc.yueranfly.top

C#:   f(a: 1, b: 2)
来源：http://cuo.daxiang520.top

[C05] 返回多个值
来源：http://era.ywan-chungtsiang.top

Py:   return a, b
来源：http://cal.xingfuxueyuan.xyz

PHP:  return [$a, $b];
来源：http://wyx.xziqi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://smc.hnqzz.top

TS:   return { a, b };
来源：http://phj.xuanzx.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ton.dianchejie.cn

Go:   return a, b
来源：http://jzr.xinyue.icu

Ruby: return a, b
来源：http://kha.sweek.top

C#:   return (a, b);              // ValueTuple
来源：http://nbe.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://vig.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://gpe.yongpay.top

PHP:  $square = fn($x) => $x * $x;
来源：http://myz.yuxming.cn

JS:   const square = x => x * x;
来源：http://dlp.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://sxg.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yug.havefunace.top

Go:   sq := func(x int) int { return x * x }
来源：http://wsl.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://rdd.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://gdi.316326.xyz

[C07] 把函数作为参数传入
来源：http://adb.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xqt.cucudq.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xiy.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wmj.tian-w.cn

TS:   arr.map(String)
来源：http://puz.ctjpmb.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jsw.hysaishi.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tiu.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://xtb.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qlw.fengsongda.top

[C08] 闭包
来源：http://fia.yongpay.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mmi.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jit.ybcxt.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fuj.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xcf.cqqwz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mfd.chenjidiqi.icu

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://apv.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jqt.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://odj.yangfankeji.com

[C09] 递归
来源：http://dwi.guannengcc.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sla.fzhhl.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://igq.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tum.shanyushiyangtech.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vuv.vqdsnc.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://uob.uphjek.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://toe.hesvh.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fta.wangdashe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iob.epnwcf.com

[C10] 变量作用域
来源：http://lkq.shanyushiyangkeji.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kwh.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nvp.yj20258.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wkn.gotoacloud.top

TS:   同 JS
来源：http://gfl.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://jrn.gotoacloud.top

Go:   花括号块级作用域
来源：http://inx.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bqz.iojbl.cn

C#:   块级作用域
来源：http://vlc.316326.xyz

[C11] 模块导入与导出
来源：http://npj.pycfn.com

Py:   from module import func
来源：http://asv.meibo888.top

PHP:  require "file.php";  或 use App\Service;
来源：http://poz.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hcg.cashguo.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://egk.iojbl.cn

Java: import java.util.List;
来源：http://kit.jiagoushi.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://stg.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://hfg.ehwqpu.com

C#:   using System.Text;
来源：http://ako.fzhhl.top

[C12] 立即执行函数 IIFE
来源：http://dya.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://jwp.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://idn.jinyuanbaomall.cn

JS:   (() => { console.log("run"); })();
来源：http://soo.hammf.cn

TS:   (() => { console.log("run"); })();
来源：http://pox.chenlongwang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://trt.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://htz.yvedp.cn

Ruby: -> { puts "run" }.call
来源：http://fam.sweek.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lvi.wangshuangyany.cn

[C13] 类型声明 / 类型注解
来源：http://snr.kuanghao11.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ugl.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://von.zhoulong.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bcd.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://axd.haohaochexian.top

Java: int add(int a, int b) { return a + b; }
来源：http://jbw.ybcxt.top

Go:   func add(a, b int) int
来源：http://iyg.hongshengwenyu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://dnh.fengsongda.top

[C14] 泛型函数
来源：http://noy.yueranfly.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tmd.jiagoushi.top

PHP:  // 无泛型
来源：http://csy.nanxinkj.top

JS:   // 无泛型
来源：http://ria.guowangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lib.zhengqikj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nvl.ydjk.org.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://uwx.52xcode.cn

Ruby: # 无泛型
来源：http://bmf.xuetiantiany.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://req.cqqwz.cn

[C15] 解构 / 展开参数
来源：http://lag.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://spd.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://shu.fengsongda.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://unp.dashuyun.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lwr.hcnkem.com

Java: // 无解构
来源：http://bkk.zhongyouzk.top

Go:   // 无解构
来源：http://byo.hongshengwenyu.top

Ruby: a, b = pair
来源：http://tpl.guannengcc.top

C#:   var (a, b) = pair;
来源：http://kbw.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://nrw.wangdashe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rva.yj202588.top

PHP:  // 无重载
来源：http://qwd.nanxinkj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://taw.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://ssg.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dxk.sjlbkw.cn

Go:   // 无重载：用不同函数名
来源：http://puk.chenjidiqi.icu

Ruby: # 无重载：靠动态参数
来源：http://rcp.sweek.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fzk.yueranfly.top

================================================================================
来源：http://rki.nanxuanxn.top

D. 数组 / 列表 / 集合
来源：http://zkh.ywan-chungtsiang.top

================================================================================
来源：http://hxr.yj20258888.top

[D01] 创建数组 / 列表
来源：http://dxl.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://vxj.c1oappe.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://raz.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://trd.xuetiantiany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mka.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gjm.xuanzx.com

Go:   arr := []int{1, 2, 3}
来源：http://wkj.sxryk.cn

Ruby: arr = [1, 2, 3]
来源：http://asu.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wfi.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://cux.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ezx.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://twy.jinqigfzy.top

JS:   arr.push(4);
来源：http://tpp.ehwqpu.com

TS:   arr.push(4);
来源：http://szh.epnwcf.com

Java: list.add(4);
来源：http://cpk.yj202588.top

Go:   arr = append(arr, 4)
来源：http://dwr.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://jrq.chenzaomai.com

C#:   list.Add(4);
来源：http://fxj.fehbvm.com

[D03] 在指定位置插入元素
来源：http://zyv.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://ybo.yj20258.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mtk.yonumen.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://aku.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://jbh.tanke756.top

Java: list.add(0, 0);
来源：http://ytg.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hxw.yueranfly.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vet.yj202588.top

C#:   list.Insert(0, 0);
来源：http://cwy.52xcode.cn

[D04] 删除元素
来源：http://vlw.shuidangran.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qfz.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://juy.xylfe.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uod.sweek.top

TS:   arr.splice(0, 1);
来源：http://mqm.sysykeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hxl.tanke756.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://irp.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pyz.wangshuangyany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dfh.cucudq.cn

[D05] 访问与修改元素
来源：http://cfw.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vln.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qtx.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ryg.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://suy.quarkkingdee.top

Java: list.get(0); list.set(0, 9);
来源：http://zsa.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://ihi.tian-w.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qgm.jyoumei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ffp.hongshengwenyu.top

[D06] 数组长度
来源：http://mtb.hnqzz.top

Py:   len(arr)
来源：http://vqh.hongshengwenyu.top

PHP:  count($arr);
来源：http://kao.xinyue.icu

JS:   arr.length
来源：http://rgd.andypj.xyz

TS:   arr.length
来源：http://xdq.kuanghao11.cn

Java: list.size();
来源：http://bud.9152youxi.cn

Go:   len(arr)
来源：http://fnj.aibaodan.cn

Ruby: arr.length; arr.size
来源：http://qly.epnwcf.com

C#:   list.Count;
来源：http://jni.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://hxz.xingfuxueyuan.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nof.fehbvm.com

PHP:  array_slice($arr, 1, 3);
来源：http://zja.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://fou.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://qln.ivvv.top

Java: list.subList(1, 4);
来源：http://say.epnwcf.com

Go:   arr[1:4]
来源：http://vko.sufxvd.cn

Ruby: arr[1, 3]
来源：http://muf.gaohongyu789.top

C#:   list.GetRange(1, 3);
来源：http://utw.cucudq.cn

[D08] 合并两个数组
来源：http://vlw.cqqwz.cn

Py:   a + b;  a.extend(b)
来源：http://ayx.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://oen.cqqwz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sql.zhoulong.xyz

TS:   [...a, ...b];
来源：http://vhx.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ezf.tanke756.top

Go:   append(a, b...)
来源：http://gjl.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://geh.ppjwa.cn

C#:   a.Concat(b).ToList()
来源：http://oin.zhengqikj.top

[D09] 排序（升序）
来源：http://jvj.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://zfa.wangdashe.top

PHP:  sort($arr);
来源：http://obc.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wlk.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://waz.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ubd.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nsi.hnxiangtu.top

Ruby: arr.sort
来源：http://gin.yuanzhike.top

C#:   list.Sort();
来源：http://tub.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://msc.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://byb.yuxming.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iec.sxryk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tak.meibo888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ahh.xuetiantiany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ssx.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tav.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bgu.birdmap.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zsy.haohaochexian.top

[D11] 反转数组
来源：http://lkz.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://mga.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://rrm.yj20258.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bww.daxiang520.top


<!-- 参考信息 -->