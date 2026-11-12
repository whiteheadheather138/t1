代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kqs.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ugt.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vjs.tianlin.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mdp.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vne.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yjb.zhiwuduotai.top

[B11] 生成数字序列 / 区间
来源：http://zsf.316326.xyz

Py:   list(range(0, 10, 2))
来源：http://ozc.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://xxh.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://adn.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bjn.yongpay.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nhh.epnwcf.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kjx.mhx1999.top

Ruby: (0...10).step(2).to_a
来源：http://lsh.zhiwuduotai.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://stg.cashguo.top

[B12] 跳出多层循环
来源：http://dyt.xylfe.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vbo.cashguo.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://roo.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ytj.nwbrower.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zpv.zhiwuduotai.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://itc.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vip.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ylx.shzxlz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yzg.yj202588.top

[B13] 判断是否为数字
来源：http://okc.hammf.cn

Py:   isinstance(x, (int, float))
来源：http://qsp.ivvv.top

PHP:  is_numeric($x)
来源：http://qnc.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://poe.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://put.iojbl.cn

Java: x instanceof Number
来源：http://iaq.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://enf.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://gfl.chenzaomai.com

C#:   x is int or double or decimal
来源：http://svc.fanxiaobao.xyz

[B14] 判断值是否在集合内
来源：http://okp.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eye.gzhubu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zez.hcnkem.com

JS:   [1, 2, 3].includes(x)
来源：http://pnf.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://dcf.ydjk.org.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://naw.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sjp.zhengqikj.top

Ruby: [1, 2, 3].include?(x)
来源：http://jng.c1oappe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://scx.bbcook.cn

[B15] 布尔运算与取反
来源：http://lus.pengpengdd.cyou

Py:   a and b or not c
来源：http://cds.yj202588.top

PHP:  $a && $b || !$c
来源：http://dmb.yfazqb.com

JS:   a && b || !c
来源：http://ewr.andypj.xyz

TS:   a && b || !c
来源：http://mbb.redwolf501.top

Java: a && b || !c
来源：http://ulo.vehdjk.com

Go:   a && b || !c
来源：http://bpg.zhiwuduotai.top

Ruby: a && b || !c
来源：http://ltn.hywenlv.cn

C#:   a && b || !c
来源：http://ihu.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://dvc.tianlin.xyz

Py:   if not data: return
来源：http://msb.yongpay.top

PHP:  if (!$data) { return; }
来源：http://dmy.guowangkeji.top

JS:   if (!data) return;
来源：http://pin.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://hsp.jinqigfzy.top

Java: if (data == null) return;
来源：http://qev.jyoumei.cn

Go:   if data == nil { return }
来源：http://ncx.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://ann.vehdjk.com

C#:   if (data == null) return;
来源：http://raq.9152youxi.cn

================================================================================
来源：http://lab.quarkkingdee.top

C. 函数与作用域
来源：http://olb.aizwys.cn

================================================================================
来源：http://pql.andypj.xyz

[C01] 定义函数
来源：http://bsp.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://vwh.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qkk.havefunace.top

JS:   function add(a, b) { return a + b; }
来源：http://kjv.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pyk.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ktt.shzxlz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fxk.aibaodan.cn

Ruby: def add(a, b); a + b; end
来源：http://dto.gogol.net.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gcj.meibo888.top

[C02] 默认参数
来源：http://iex.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://wxm.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zsy.jlsjyb.cn

JS:   function greet(name = "World") { return name; }
来源：http://tpu.gogol.net.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ftj.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nzr.shanyushiyangkeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bus.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://dmw.zdbjq.cn

C#:   string Greet(string name = "World") => name;
来源：http://rmn.316326.xyz

[C03] 可变参数
来源：http://ajf.yfazqb.com

Py:   def total(*args): return sum(args)
来源：http://kfu.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cmm.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://sha.shangyingyoupin.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iqe.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qup.hysaishi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jqt.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://cuk.shuidangran.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hpa.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://tub.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fdq.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yba.316326.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pyv.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dim.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://dpl.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://abr.yj20258888.top

Ruby: f(a: 1, b: 2)
来源：http://zxq.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://gos.jlsjyb.cn

[C05] 返回多个值
来源：http://wgy.cheryme.top

Py:   return a, b
来源：http://had.0kj1m.cn

PHP:  return [$a, $b];
来源：http://qql.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://otz.gotoacloud.top

TS:   return { a, b };
来源：http://ijp.ehwqpu.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ngs.yuanzhike.top

Go:   return a, b
来源：http://kpo.yueranfly.top

Ruby: return a, b
来源：http://mef.xinyue.icu

C#:   return (a, b);              // ValueTuple
来源：http://wxo.shanyushiyangkeji.top

[C06] 匿名函数 / lambda
来源：http://nrd.ywan-chungtsiang.top

Py:   square = lambda x: x * x
来源：http://kgq.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hun.jinqigufen.top

JS:   const square = x => x * x;
来源：http://fxc.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://rsp.ppjwa.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qmz.feifeiyinyue.top

Go:   sq := func(x int) int { return x * x }
来源：http://yap.xuanzx.com

Ruby: square = ->(x) { x * x }
来源：http://kfr.fengsongda.top

C#:   Func<int, int> square = x => x * x;
来源：http://fbm.pengpengdd.cyou

[C07] 把函数作为参数传入
来源：http://nrd.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://chh.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://duh.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pjy.nanxinkj.top

TS:   arr.map(String)
来源：http://inh.feifeiyinyue.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://seq.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ugp.zhiwuduotai.top

Ruby: arr.map(&:upcase)
来源：http://wev.jinghuilouyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://xia.zhixingplan.top

[C08] 闭包
来源：http://yik.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fuf.hfpthk.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ltj.quarkkingdee.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mik.dashuyun.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xnj.xuanzx.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nqf.xziqi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gph.zycfv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xrq.dashuyun.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sjd.tianlin.xyz

[C09] 递归
来源：http://ygc.52xcode.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mur.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kqj.vqdsnc.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rkk.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nnv.feifeiyinyue.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wjq.gzhubu.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oop.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gwh.jinqigfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lqv.haohaochexian.top

[C10] 变量作用域
来源：http://mzk.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ytn.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://nag.andypj.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ooq.shzxlz.cn

TS:   同 JS
来源：http://cwp.jyoumei.cn

Java: 方法内为块级作用域
来源：http://ayd.cqqwz.cn

Go:   花括号块级作用域
来源：http://apo.haohaochexian.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qyw.zhaomingkeji.xyz

C#:   块级作用域
来源：http://bft.vqdsnc.cn

[C11] 模块导入与导出
来源：http://tfh.chenzaomai.com

Py:   from module import func
来源：http://mhw.bjfxy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yah.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vvo.jinqigfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://onb.andypj.xyz

Java: import java.util.List;
来源：http://pob.ivvv.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wse.52xcode.cn

Ruby: require "json"; require_relative "./util"
来源：http://kar.jinyuanbaomall.cn

C#:   using System.Text;
来源：http://nge.hnqzz.top

[C12] 立即执行函数 IIFE
来源：http://tdj.gzhubu.top

Py:   (lambda: print("run"))()
来源：http://xxy.gaohongyu789.top

PHP:  (function () { echo "run"; })();
来源：http://bas.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://chn.cdnleiting.top

TS:   (() => { console.log("run"); })();
来源：http://knb.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://abj.smart0.xyz

Go:   func() { fmt.Println("run") }()
来源：http://aqu.yj202588.top

Ruby: -> { puts "run" }.call
来源：http://lkp.zhoulong.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://shv.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://exv.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rpo.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://evb.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ccw.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ffy.tarul.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tyo.daria6918.cn

Go:   func add(a, b int) int
来源：http://dlm.cqqwz.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jry.ybcxt.top

C#:   int Add(int a, int b) => a + b;
来源：http://nod.wangshuangyany.cn

[C14] 泛型函数
来源：http://ayi.daxiang520.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nti.pycfn.com

PHP:  // 无泛型
来源：http://yfg.ctjpmb.com

JS:   // 无泛型
来源：http://qpz.cashguo.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rsw.havefunace.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jiv.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ggc.sysykeji.top

Ruby: # 无泛型
来源：http://itd.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wef.shanyushiyangkeji.top

[C15] 解构 / 展开参数
来源：http://nop.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rrs.zycfv.cn

PHP:  [$a, $b] = $pair;
来源：http://gpb.aizwys.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mnr.hnxiangtu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ubc.jqgfzy.top

Java: // 无解构
来源：http://mvj.daria6918.cn

Go:   // 无解构
来源：http://sjt.yonumen.top

Ruby: a, b = pair
来源：http://fbh.shangyingyoupin.top

C#:   var (a, b) = pair;
来源：http://nql.sweek.top

[C16] 函数 / 方法重载
来源：http://kht.jinyuanbaomall.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://geh.zycfv.cn

PHP:  // 无重载
来源：http://csx.guowangkeji.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://bgv.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://sjw.yanxiufei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xtz.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://rkg.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://bdj.bjfxy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uyn.ywan-chungtsiang.top

================================================================================
来源：http://jyc.yj20258.top

D. 数组 / 列表 / 集合
来源：http://zen.tarul.cn

================================================================================
来源：http://hrk.kuanghao11.cn

[D01] 创建数组 / 列表
来源：http://otu.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hue.ywan-chungtsiang.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ybd.zycfv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xsn.ybcxt.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nro.havefunace.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qlt.xylfe.cn

Go:   arr := []int{1, 2, 3}
来源：http://ipc.haohaochexian.top

Ruby: arr = [1, 2, 3]
来源：http://njb.kuanghao11.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dkz.xinyue.icu

[D02] 追加元素到末尾
来源：http://rds.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jpo.zycfv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yti.ehwqpu.com

JS:   arr.push(4);
来源：http://fjb.52xcode.cn

TS:   arr.push(4);
来源：http://sgo.cqqwz.cn

Java: list.add(4);
来源：http://osx.cdnleiting.top

Go:   arr = append(arr, 4)
来源：http://enr.shangyingyoupin.top

Ruby: arr << 4; arr.push(5)
来源：http://unx.gzhubu.top

C#:   list.Add(4);
来源：http://eqa.ivvv.top

[D03] 在指定位置插入元素
来源：http://thp.iojbl.cn

Py:   arr.insert(0, 0)
来源：http://wel.hysaishi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dhl.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xur.daria6918.cn

TS:   arr.splice(0, 0, 0);
来源：http://rna.hesvh.cn

Java: list.add(0, 0);
来源：http://gos.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://hmi.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iyb.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://tmq.xinyue.icu

[D04] 删除元素
来源：http://hse.vehdjk.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vuk.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://usb.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sxo.c1oappe.top

TS:   arr.splice(0, 1);
来源：http://zmv.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gck.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pae.yueranfly.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dsl.guannengcc.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yuw.fzhhl.top

[D05] 访问与修改元素
来源：http://cme.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mzt.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zso.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rsq.yanxiufei.cn

TS:   arr[0]; arr.at(-1);
来源：http://jwt.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://iuv.daxiang520.top

Go:   arr[0]; arr[0] = 9
来源：http://pyi.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cym.zhongyouzk.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vif.hywenlv.cn

[D06] 数组长度
来源：http://uop.yj20258888.top

Py:   len(arr)
来源：http://quh.sxryk.cn

PHP:  count($arr);
来源：http://rtz.sxryk.cn

JS:   arr.length
来源：http://sli.jianghu66.top

TS:   arr.length
来源：http://uxg.xuetiantiany.cn

Java: list.size();
来源：http://okr.andypj.xyz

Go:   len(arr)
来源：http://kha.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://mzk.cqqwz.cn

C#:   list.Count;
来源：http://zjy.jinqigfzy.top

[D07] 切片 / 取子数组
来源：http://tbo.ybcxt.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jdz.jinghuilouyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://liz.hongshengwenyu.top

JS:   arr.slice(1, 4);
来源：http://pnb.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://jgf.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://mmj.xziqi.cn

Go:   arr[1:4]
来源：http://vcd.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://xoc.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://fym.shzxlz.cn

[D08] 合并两个数组
来源：http://fga.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://sup.zhengqikj.top

PHP:  array_merge($a, $b);
来源：http://khp.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://aoa.jqgufenzy.top

TS:   [...a, ...b];
来源：http://shl.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lrd.redwolf501.top

Go:   append(a, b...)
来源：http://jox.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://gvl.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://oph.guannengcc.top

[D09] 排序（升序）
来源：http://oeq.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://mmm.dashuyun.cn

PHP:  sort($arr);
来源：http://smv.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yiv.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wzl.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dpb.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vzj.hesvh.cn

Ruby: arr.sort
来源：http://loh.birdmap.top

C#:   list.Sort();
来源：http://qql.dashuyun.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://urn.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lrx.meibo888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fsp.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bgv.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tpb.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vog.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iix.tian-w.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hab.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dmt.zdbjq.cn


<!-- 参考信息 -->