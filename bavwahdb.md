代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sed.andypj.xyz

[B10] 遍历同时拿索引
来源：http://rsn.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kcq.xziqi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ncj.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://udm.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jrn.nanxuanxn.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ren.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ujk.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dby.chenjidiqi.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jxw.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://xlz.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://cgn.zhijiandao.cn

PHP:  range(0, 10, 2);
来源：http://oiw.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wpe.pycfn.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rls.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gzk.zhongyouzk.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ogv.yanxiufei.cn

Ruby: (0...10).step(2).to_a
来源：http://skz.jyoumei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://szm.chenlongwang.top

[B12] 跳出多层循环
来源：http://crd.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tkv.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gwi.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://aug.tianlin.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lax.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xoq.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ryf.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sac.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wba.hcnkem.com

[B13] 判断是否为数字
来源：http://hpn.hywenlv.cn

Py:   isinstance(x, (int, float))
来源：http://oem.zhengqikj.top

PHP:  is_numeric($x)
来源：http://oge.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xyc.aibaodan.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nmx.jinghuilouyu.cn

Java: x instanceof Number
来源：http://pxo.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://byt.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://onl.wangshuangyany.cn

C#:   x is int or double or decimal
来源：http://ezs.xziqi.cn

[B14] 判断值是否在集合内
来源：http://rtu.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kni.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bwk.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://fmh.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://uan.yvedp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dud.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lqo.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://idi.xinyue.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ddx.hesvh.cn

[B15] 布尔运算与取反
来源：http://nle.chenzaomai.com

Py:   a and b or not c
来源：http://gam.ivvv.top

PHP:  $a && $b || !$c
来源：http://vkb.haohaochexian.top

JS:   a && b || !c
来源：http://izd.yueranfly.top

TS:   a && b || !c
来源：http://bmt.hongshengwenyu.top

Java: a && b || !c
来源：http://zhy.ydzc1.top

Go:   a && b || !c
来源：http://efu.ydjk.org.cn

Ruby: a && b || !c
来源：http://qub.jinqigfzy.top

C#:   a && b || !c
来源：http://fao.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://rke.shuidangran.top

Py:   if not data: return
来源：http://nzl.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://fiv.yuanzhike.top

JS:   if (!data) return;
来源：http://qwk.nanxinkj.top

TS:   if (!data) return;
来源：http://xqc.daria6918.cn

Java: if (data == null) return;
来源：http://ege.shangyingyoupin.top

Go:   if data == nil { return }
来源：http://ppg.yfazqb.com

Ruby: return if data.nil?
来源：http://xsr.xuetiantiany.cn

C#:   if (data == null) return;
来源：http://trh.sweek.top

================================================================================
来源：http://twl.fehbvm.com

C. 函数与作用域
来源：http://jqi.jqgfzy.top

================================================================================
来源：http://bxy.yvedp.cn

[C01] 定义函数
来源：http://swf.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://ygi.daxiang520.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://low.jinqigufen.top

JS:   function add(a, b) { return a + b; }
来源：http://nwd.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ayr.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sbi.ppjwa.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lwo.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://jjd.quarkkingdee.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mim.zhixingplan.top

[C02] 默认参数
来源：http://dbl.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://sco.cucudq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fgm.birdmap.top

JS:   function greet(name = "World") { return name; }
来源：http://hzr.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vsg.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://zxz.hnqzz.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eaw.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://fwk.fzhhl.top

C#:   string Greet(string name = "World") => name;
来源：http://kbu.andypj.xyz

[C03] 可变参数
来源：http://qjf.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://tik.hesvh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ays.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://yqi.xylfe.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jyc.jiagoushi.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xwy.jlsjyb.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pzy.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://qcq.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xxd.ivvv.top

[C04] 命名参数 / 关键字参数
来源：http://omh.yangfankeji.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tnd.hnxiangtu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gik.hesvh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mby.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rpu.gzhubu.top

Java: // 无：用 Builder 模式或 record
来源：http://rfy.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://bsc.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://wzm.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://itu.vqdsnc.cn

[C05] 返回多个值
来源：http://hhh.zdqjudy.top

Py:   return a, b
来源：http://hfw.ydjk.org.cn

PHP:  return [$a, $b];
来源：http://uyn.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hbx.shanyushiyangtech.top

TS:   return { a, b };
来源：http://cag.uphjek.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ptl.yonumen.top

Go:   return a, b
来源：http://zic.havefunace.top

Ruby: return a, b
来源：http://gns.shanyushiyangtech.top

C#:   return (a, b);              // ValueTuple
来源：http://ghn.xziqi.cn

[C06] 匿名函数 / lambda
来源：http://ste.cucudq.cn

Py:   square = lambda x: x * x
来源：http://tdp.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hsc.xinyue.icu

JS:   const square = x => x * x;
来源：http://aas.jinghuilouyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://ulk.yj20258888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yfs.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://fmw.cdnleiting.top

Ruby: square = ->(x) { x * x }
来源：http://ejg.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://qwv.0kj1m.cn

[C07] 把函数作为参数传入
来源：http://iiu.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hpv.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://eqx.hongshengwenyu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ehy.tanke756.top

TS:   arr.map(String)
来源：http://kpj.chenjidiqi.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ztf.ppjwa.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://czz.guannengcc.top

Ruby: arr.map(&:upcase)
来源：http://hlb.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://zwo.yfazqb.com

[C08] 闭包
来源：http://qsl.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dnn.wangshuangyany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://nei.chenzaomai.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cxd.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ssw.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nat.hammf.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jzf.cheryme.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uxi.sufxvd.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ocb.hcnkem.com

[C09] 递归
来源：http://auf.xylfe.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jiz.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://frv.iojbl.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uzz.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rms.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mct.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iht.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pek.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tgu.iojbl.cn

[C10] 变量作用域
来源：http://jpw.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bvj.daria6918.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lht.ydzc1.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tnx.aizwys.cn

TS:   同 JS
来源：http://ewn.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://itm.shzxlz.cn

Go:   花括号块级作用域
来源：http://vqa.jinyuanbaomall.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mdo.xuanzx.com

C#:   块级作用域
来源：http://qye.0kj1m.cn

[C11] 模块导入与导出
来源：http://rbf.hysaishi.cn

Py:   from module import func
来源：http://dpk.yuanzhike.top

PHP:  require "file.php";  或 use App\Service;
来源：http://cyv.hnxiangtu.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mrt.shanyushiyangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sms.dianchejie.cn

Java: import java.util.List;
来源：http://gjt.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xbg.gzhubu.top

Ruby: require "json"; require_relative "./util"
来源：http://crt.cashguo.top

C#:   using System.Text;
来源：http://djk.cucudq.cn

[C12] 立即执行函数 IIFE
来源：http://ygr.0kj1m.cn

Py:   (lambda: print("run"))()
来源：http://opf.jinqigfzy.top

PHP:  (function () { echo "run"; })();
来源：http://kvh.jyoumei.cn

JS:   (() => { console.log("run"); })();
来源：http://akt.uphjek.com

TS:   (() => { console.log("run"); })();
来源：http://lqh.zhengqikj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jbs.yangfankeji.com

Go:   func() { fmt.Println("run") }()
来源：http://pkh.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://lck.smart0.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://sqa.guowangkeji.top

[C13] 类型声明 / 类型注解
来源：http://abp.shzxlz.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jkl.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jbd.redwolf501.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://upo.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mat.gogol.net.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vgc.andypj.xyz

Go:   func add(a, b int) int
来源：http://gxc.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cpe.aibaodan.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cfy.shuidangran.top

[C14] 泛型函数
来源：http://cql.52xcode.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jms.ppjwa.cn

PHP:  // 无泛型
来源：http://sve.zhengqikj.top

JS:   // 无泛型
来源：http://gjw.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yuy.yfazqb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cen.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zbv.0kj1m.cn

Ruby: # 无泛型
来源：http://iqu.jinyuanbaomall.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zuo.pycfn.com

[C15] 解构 / 展开参数
来源：http://wbf.xylfe.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rij.svipenyu.cn

PHP:  [$a, $b] = $pair;
来源：http://bro.shuidangran.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rfi.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bdi.guowangkeji.top

Java: // 无解构
来源：http://nti.xinyue.icu

Go:   // 无解构
来源：http://nka.zhongyouzk.top

Ruby: a, b = pair
来源：http://rae.nanxuanxn.top

C#:   var (a, b) = pair;
来源：http://uzf.kuanghao11.cn

[C16] 函数 / 方法重载
来源：http://ghs.yongpay.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zji.shanyushiyangtech.top

PHP:  // 无重载
来源：http://igx.yueranfly.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bym.redwolf501.top

TS:   // 用联合类型或重载签名声明
来源：http://bja.yonumen.top

Java: void f(int a) {}  void f(String a) {}
来源：http://bdi.aizwys.cn

Go:   // 无重载：用不同函数名
来源：http://zxu.ctjpmb.com

Ruby: # 无重载：靠动态参数
来源：http://ylw.fanxiaobao.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://mhy.sysykeji.top

================================================================================
来源：http://qft.hywenlv.cn

D. 数组 / 列表 / 集合
来源：http://vrh.shangyingyoupin.top

================================================================================
来源：http://dqc.zhongyouzk.top

[D01] 创建数组 / 列表
来源：http://yuu.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://htm.uphjek.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vjn.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qeh.hysaishi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yfa.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xrx.quarkkingdee.top

Go:   arr := []int{1, 2, 3}
来源：http://kwt.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://xvy.nanxuanxn.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://owv.zdqjudy.top

[D02] 追加元素到末尾
来源：http://bhm.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hbz.jlsjyb.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xgu.daria6918.cn

JS:   arr.push(4);
来源：http://ctj.vehdjk.com

TS:   arr.push(4);
来源：http://ggc.shanyushiyangkeji.top

Java: list.add(4);
来源：http://xmt.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://cpr.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://xwy.kuanghao11.cn

C#:   list.Add(4);
来源：http://kjq.ctjpmb.com

[D03] 在指定位置插入元素
来源：http://ggj.ywan-chungtsiang.top

Py:   arr.insert(0, 0)
来源：http://obn.yangfankeji.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://npf.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ktt.haohaochexian.top

TS:   arr.splice(0, 0, 0);
来源：http://kzr.zdbjq.cn

Java: list.add(0, 0);
来源：http://rhl.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://ytn.xuanzx.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dtg.shanyushiyangkeji.top

C#:   list.Insert(0, 0);
来源：http://gve.yuxming.cn

[D04] 删除元素
来源：http://bok.daxiang520.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qei.haohaochexian.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://njo.xinyue.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zdl.jiagoushi.top

TS:   arr.splice(0, 1);
来源：http://nrf.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://chr.zhengqikj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zgx.ydzc1.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://agr.yvedp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qot.sweek.top

[D05] 访问与修改元素
来源：http://vrj.yj20258.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jqj.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uxr.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pug.chenjidiqi.icu

TS:   arr[0]; arr.at(-1);
来源：http://sgs.zhiwuduotai.top

Java: list.get(0); list.set(0, 9);
来源：http://gmq.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://dmm.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aae.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cas.mhx1999.top

[D06] 数组长度
来源：http://jte.sufxvd.cn

Py:   len(arr)
来源：http://rvy.zhoulong.xyz

PHP:  count($arr);
来源：http://paa.chenjidiqi.icu

JS:   arr.length
来源：http://kzb.fengsongda.top

TS:   arr.length
来源：http://sqo.pycfn.com

Java: list.size();
来源：http://jmc.xziqi.cn

Go:   len(arr)
来源：http://wxo.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://apv.hysaishi.cn

C#:   list.Count;
来源：http://rna.havefunace.top

[D07] 切片 / 取子数组
来源：http://fue.aizwys.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mpf.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://qcr.zhaomingkeji.xyz

JS:   arr.slice(1, 4);
来源：http://lcr.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://ihy.fktsv.cn

Java: list.subList(1, 4);
来源：http://rck.sufxvd.cn

Go:   arr[1:4]
来源：http://grr.andypj.xyz

Ruby: arr[1, 3]
来源：http://muz.zhengqikj.top

C#:   list.GetRange(1, 3);
来源：http://glf.mhx1999.top

[D08] 合并两个数组
来源：http://fgp.birdmap.top

Py:   a + b;  a.extend(b)
来源：http://iaq.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://owy.cheryme.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jpf.hesvh.cn

TS:   [...a, ...b];
来源：http://jtv.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://brc.jinqigfzy.top

Go:   append(a, b...)
来源：http://ogz.cheryme.top

Ruby: a + b;  a.concat(b)
来源：http://nau.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://feu.kuanghao11.cn

[D09] 排序（升序）
来源：http://ipt.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://gvo.sweek.top

PHP:  sort($arr);
来源：http://hib.tanke756.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xrc.redwolf501.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jxi.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://acp.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jad.bbcook.cn

Ruby: arr.sort
来源：http://umc.redwolf501.top

C#:   list.Sort();
来源：http://vwd.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://stf.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dlh.yfazqb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xjm.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://etr.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jwm.haohaochexian.top


<!-- 参考信息 -->