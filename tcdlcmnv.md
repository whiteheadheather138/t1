代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pci.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hkr.hammf.cn

[B11] 生成数字序列 / 区间
来源：http://uzu.shzxlz.cn

Py:   list(range(0, 10, 2))
来源：http://kgh.zhijiandao.cn

PHP:  range(0, 10, 2);
来源：http://jjj.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bvq.shzxlz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gna.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aqq.cucudq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ofz.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://xsr.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ehv.jyoumei.cn

[B12] 跳出多层循环
来源：http://bnu.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kvg.nanxuanxn.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://avt.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zeg.gzhubu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vun.fengsongda.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uqv.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ekz.meibo888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zjh.sysykeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rsu.jyoumei.cn

[B13] 判断是否为数字
来源：http://fps.ppjwa.cn

Py:   isinstance(x, (int, float))
来源：http://slq.sweek.top

PHP:  is_numeric($x)
来源：http://por.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yiy.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ohk.sweek.top

Java: x instanceof Number
来源：http://leo.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fvv.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://ukk.hysaishi.cn

C#:   x is int or double or decimal
来源：http://fgz.xinyue.icu

[B14] 判断值是否在集合内
来源：http://poh.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cta.yonumen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pup.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://oyw.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://fjk.zhixingplan.top

Java: List.of(1, 2, 3).contains(x)
来源：http://haz.smart0.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rgc.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://rna.sjlbkw.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://twx.ybcxt.top

[B15] 布尔运算与取反
来源：http://bdv.dianchejie.cn

Py:   a and b or not c
来源：http://yrq.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://kpq.zhengqikj.top

JS:   a && b || !c
来源：http://udh.zhengqikj.top

TS:   a && b || !c
来源：http://xku.haohaochexian.top

Java: a && b || !c
来源：http://vld.fktsv.cn

Go:   a && b || !c
来源：http://mgi.fanxiaobao.xyz

Ruby: a && b || !c
来源：http://syf.yfazqb.com

C#:   a && b || !c
来源：http://ypb.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://dzm.gaohongyu789.top

Py:   if not data: return
来源：http://mpv.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://lay.xziqi.cn

JS:   if (!data) return;
来源：http://snt.snrcjt.cn

TS:   if (!data) return;
来源：http://yld.gogol.net.cn

Java: if (data == null) return;
来源：http://uyo.hnxiangtu.top

Go:   if data == nil { return }
来源：http://tcp.nanxinkj.top

Ruby: return if data.nil?
来源：http://koo.jiagoushi.top

C#:   if (data == null) return;
来源：http://vlf.cdnleiting.top

================================================================================
来源：http://ppo.bbcook.cn

C. 函数与作用域
来源：http://kku.hesvh.cn

================================================================================
来源：http://biw.yfazqb.com

[C01] 定义函数
来源：http://vrv.shangyingyoupin.top

Py:   def add(a, b): return a + b
来源：http://iuv.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rxl.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://xak.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ctz.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lpi.316326.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://oas.cdnleiting.top

Ruby: def add(a, b); a + b; end
来源：http://qbe.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sgf.9152youxi.cn

[C02] 默认参数
来源：http://cun.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://xkj.ydjk.org.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cfp.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://qth.zhengqikj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://cbj.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gyf.tanke756.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uvp.epnwcf.com

Ruby: def greet(name = "World") = name
来源：http://ovj.feifeiyinyue.top

C#:   string Greet(string name = "World") => name;
来源：http://suu.yanxiufei.cn

[C03] 可变参数
来源：http://xem.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://bgm.c1oappe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jan.cucudq.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tdq.zhengqikj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vmx.yonumen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jvc.nanxuanxn.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dct.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ksf.hywenlv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jbd.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://lwd.snrcjt.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yow.yueranfly.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ank.yj202588.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lpy.cucudq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zgr.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://wce.fktsv.cn

Go:   // 无：用配置结构体参数
来源：http://fos.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://inx.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://bjy.zhijiandao.cn

[C05] 返回多个值
来源：http://bkd.jinghuilouyu.cn

Py:   return a, b
来源：http://toj.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://tfu.tanke756.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dax.hammf.cn

TS:   return { a, b };
来源：http://bdt.zdqjudy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tze.316326.xyz

Go:   return a, b
来源：http://pnf.meibo888.top

Ruby: return a, b
来源：http://kjr.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://ftw.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://jeo.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://fuj.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://edk.bjfxy.top

JS:   const square = x => x * x;
来源：http://mqb.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://jgh.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nkl.aizwys.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fyb.wangdashe.top

Ruby: square = ->(x) { x * x }
来源：http://ejs.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://vtq.hesvh.cn

[C07] 把函数作为参数传入
来源：http://pqz.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gmz.yfazqb.com

PHP:  array_map("strtoupper", $arr);
来源：http://ruw.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jvr.cdnleiting.top

TS:   arr.map(String)
来源：http://are.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fee.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mxg.aizwys.cn

Ruby: arr.map(&:upcase)
来源：http://upw.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fzq.zhoulong.xyz

[C08] 闭包
来源：http://rai.xinyue.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yga.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://seh.jiagoushi.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zom.shzxlz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bjk.fehbvm.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ied.yueranfly.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jma.jqgfzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xvi.c1oappe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fpt.jinqigufen.top

[C09] 递归
来源：http://ibu.jinqigufen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yyp.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vrj.smart0.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gxo.tanke756.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nfp.yanxiufei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://psy.haohaochexian.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tnt.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ryw.52xcode.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mnt.chenzaomai.com

[C10] 变量作用域
来源：http://phi.yj20258.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qxf.snrcjt.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jgm.mhx1999.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wkq.chenjidiqi.icu

TS:   同 JS
来源：http://lff.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://xze.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://ibq.gzhubu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://opf.jinqigufen.top

C#:   块级作用域
来源：http://prj.vqdsnc.cn

[C11] 模块导入与导出
来源：http://kwo.meibo888.top

Py:   from module import func
来源：http://kbo.pengpengdd.cyou

PHP:  require "file.php";  或 use App\Service;
来源：http://ijg.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dpm.yongpay.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zcx.jinqigfzy.top

Java: import java.util.List;
来源：http://xmr.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ymb.zhongyouzk.top

Ruby: require "json"; require_relative "./util"
来源：http://zfe.zhongyouzk.top

C#:   using System.Text;
来源：http://jop.yueranfly.top

[C12] 立即执行函数 IIFE
来源：http://mav.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://bgx.dianchejie.cn

PHP:  (function () { echo "run"; })();
来源：http://fxc.daria6918.cn

JS:   (() => { console.log("run"); })();
来源：http://adz.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://olg.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cri.cdnleiting.top

Go:   func() { fmt.Println("run") }()
来源：http://qic.nanxinkj.top

Ruby: -> { puts "run" }.call
来源：http://tnz.shzxlz.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kln.shuidangran.top

[C13] 类型声明 / 类型注解
来源：http://lvk.fzhhl.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hnz.wangshuangyany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://clk.kuanghao11.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mhg.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sxx.fanxiaobao.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://wkb.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://skl.gaohongyu789.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wbd.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://uae.tanke756.top

[C14] 泛型函数
来源：http://vkl.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dsc.bbcook.cn

PHP:  // 无泛型
来源：http://jaq.hnqzz.top

JS:   // 无泛型
来源：http://eqr.yonumen.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://olk.ppjwa.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mpz.tian-w.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ccg.gogol.net.cn

Ruby: # 无泛型
来源：http://wqr.birdmap.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://sup.fzhhl.top

[C15] 解构 / 展开参数
来源：http://okd.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hfk.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://kue.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kei.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gcw.52xcode.cn

Java: // 无解构
来源：http://eeu.hywenlv.cn

Go:   // 无解构
来源：http://hjv.tian-w.cn

Ruby: a, b = pair
来源：http://rbe.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://zrr.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://nea.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://uwa.hongshengwenyu.top

PHP:  // 无重载
来源：http://fxx.cheryme.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wnu.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://kny.aibaodan.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yzd.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://rwe.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://kmg.ybcxt.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://sff.fanxiaobao.xyz

================================================================================
来源：http://qmv.pycfn.com

D. 数组 / 列表 / 集合
来源：http://jnn.wangshuangyany.cn

================================================================================
来源：http://atm.yueranfly.top

[D01] 创建数组 / 列表
来源：http://gdt.quarkkingdee.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xjj.yj20258888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://czd.dianchejie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eoi.cashguo.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cql.wangshuangyany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ore.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://kem.sysykeji.top

Ruby: arr = [1, 2, 3]
来源：http://lie.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hbe.pycfn.com

[D02] 追加元素到末尾
来源：http://hsw.fanxiaobao.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://veu.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lcr.jinyuanbaomall.cn

JS:   arr.push(4);
来源：http://tus.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://nfs.ctjpmb.com

Java: list.add(4);
来源：http://fsp.hesvh.cn

Go:   arr = append(arr, 4)
来源：http://atb.ivvv.top

Ruby: arr << 4; arr.push(5)
来源：http://lev.jiagoushi.top

C#:   list.Add(4);
来源：http://mpe.andypj.xyz

[D03] 在指定位置插入元素
来源：http://yum.birdmap.top

Py:   arr.insert(0, 0)
来源：http://gxl.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qqs.316326.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mfc.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://mai.ehwqpu.com

Java: list.add(0, 0);
来源：http://rui.jinghuilouyu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xwn.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rfo.hfpthk.cn

C#:   list.Insert(0, 0);
来源：http://iyv.aibaodan.cn

[D04] 删除元素
来源：http://exe.cashguo.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lam.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://saw.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uyk.zdbjq.cn

TS:   arr.splice(0, 1);
来源：http://oih.smart0.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pnf.aizwys.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://szo.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cyf.yuxming.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kfl.jinqigfzy.top

[D05] 访问与修改元素
来源：http://zkx.shangyingyoupin.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kar.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fhj.fktsv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://otx.jqgfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://pgm.ppjwa.cn

Java: list.get(0); list.set(0, 9);
来源：http://bsm.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://skr.havefunace.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ncf.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cns.yj20258.top

[D06] 数组长度
来源：http://atv.yangfankeji.com

Py:   len(arr)
来源：http://sla.fehbvm.com

PHP:  count($arr);
来源：http://bhg.cqqwz.cn

JS:   arr.length
来源：http://enf.tian-w.cn

TS:   arr.length
来源：http://jgw.hammf.cn

Java: list.size();
来源：http://wkh.zhijiandao.cn

Go:   len(arr)
来源：http://dpx.bjfxy.top

Ruby: arr.length; arr.size
来源：http://lmd.sjlbkw.cn

C#:   list.Count;
来源：http://cpi.sysykeji.top

[D07] 切片 / 取子数组
来源：http://abv.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kvb.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://mty.yanxiufei.cn

JS:   arr.slice(1, 4);
来源：http://wnj.hfpthk.cn

TS:   arr.slice(1, 4);
来源：http://xdy.ehwqpu.com

Java: list.subList(1, 4);
来源：http://fek.smart0.xyz

Go:   arr[1:4]
来源：http://ybs.guannengcc.top

Ruby: arr[1, 3]
来源：http://axg.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://dzz.hcnkem.com

[D08] 合并两个数组
来源：http://wfq.fktsv.cn

Py:   a + b;  a.extend(b)
来源：http://anq.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://yjz.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rcm.cheryme.top

TS:   [...a, ...b];
来源：http://rwo.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cic.nwbrower.top

Go:   append(a, b...)
来源：http://whe.dianchejie.cn

Ruby: a + b;  a.concat(b)
来源：http://blo.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://mkn.nanxuanxn.top

[D09] 排序（升序）
来源：http://zdy.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://cfn.dashuyun.cn

PHP:  sort($arr);
来源：http://llc.zhengqikj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://luo.yongpay.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qyd.wangdashe.top

Java: Collections.sort(list);  list.sort(null);
来源：http://niw.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vbu.sufxvd.cn

Ruby: arr.sort
来源：http://wvl.hammf.cn

C#:   list.Sort();
来源：http://lcy.yueranfly.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cme.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jcw.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zqk.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eqk.yueranfly.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yty.xziqi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vjp.ydzc1.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pzw.fzhhl.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hpx.daria6918.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://amh.ydjk.org.cn

[D11] 反转数组
来源：http://mfl.sysykeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://gro.ivvv.top

PHP:  array_reverse($arr);
来源：http://qfn.hysaishi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xjz.dashuyun.cn


<!-- 参考信息 -->