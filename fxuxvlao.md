代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://lut.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://wcc.9152youxi.cn

Ruby: def add(a, b); a + b; end
来源：http://iql.sxryk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vax.nanxinkj.top

[C02] 默认参数
来源：http://nny.chenjidiqi.icu

Py:   def greet(name="World"): return name
来源：http://ttd.daria6918.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://inr.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://bzn.iojbl.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://rkt.yfazqb.com

Java: // 无默认参数：方法重载或 Optional
来源：http://yvo.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ugg.yangfankeji.com

Ruby: def greet(name = "World") = name
来源：http://uzg.mhx1999.top

C#:   string Greet(string name = "World") => name;
来源：http://ojm.tian-w.cn

[C03] 可变参数
来源：http://dgq.yj20258.top

Py:   def total(*args): return sum(args)
来源：http://gnx.sweek.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ccq.9152youxi.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://czg.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yof.yongpay.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rik.pycfn.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gek.fehbvm.com

Ruby: def total(*nums); nums.sum; end
来源：http://iha.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fao.zdqjudy.top

[C04] 命名参数 / 关键字参数
来源：http://uaa.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xmp.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jxr.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rvv.gzhubu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rmm.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://zwi.chenzaomai.com

Go:   // 无：用配置结构体参数
来源：http://khu.gogol.net.cn

Ruby: f(a: 1, b: 2)
来源：http://cju.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://giu.wangshuangyany.cn

[C05] 返回多个值
来源：http://etb.hnxiangtu.top

Py:   return a, b
来源：http://mxf.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://zga.tanke756.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wgp.smart0.xyz

TS:   return { a, b };
来源：http://wiw.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hpx.zdqjudy.top

Go:   return a, b
来源：http://fne.hysaishi.cn

Ruby: return a, b
来源：http://zlh.yonumen.top

C#:   return (a, b);              // ValueTuple
来源：http://ahz.yuxming.cn

[C06] 匿名函数 / lambda
来源：http://ngt.svipenyu.cn

Py:   square = lambda x: x * x
来源：http://kpb.hcnkem.com

PHP:  $square = fn($x) => $x * $x;
来源：http://dcg.xingfuxueyuan.xyz

JS:   const square = x => x * x;
来源：http://hhu.yj20258888.top

TS:   const square = (x: number): number => x * x;
来源：http://oet.wangdashe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hxk.yuxming.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pqn.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://koq.zhaomingkeji.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ihi.nwbrower.top

[C07] 把函数作为参数传入
来源：http://gbj.guannengcc.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gnc.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://dxp.zhongyouzk.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://upx.birdmap.top

TS:   arr.map(String)
来源：http://jtm.yanxiufei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kyt.fanxiaobao.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xzy.zhaomingkeji.xyz

Ruby: arr.map(&:upcase)
来源：http://cgz.hysaishi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nbv.fengsongda.top

[C08] 闭包
来源：http://bsg.hysaishi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cyl.uphjek.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://atb.yangfankeji.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sqi.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hpw.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zaa.snrcjt.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bkb.9152youxi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://szp.andypj.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ftm.pengpengdd.cyou

[C09] 递归
来源：http://ern.tianlin.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fqa.aibaodan.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kpb.hnqzz.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gqb.jinghuilouyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zha.yj20258.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hin.zhoulong.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jhy.tarul.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dlk.c1oappe.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iqw.zhengqikj.top

[C10] 变量作用域
来源：http://pos.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yud.chenzaomai.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cox.52xcode.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ymj.zhixingplan.top

TS:   同 JS
来源：http://efo.bjfxy.top

Java: 方法内为块级作用域
来源：http://bjt.shzxlz.cn

Go:   花括号块级作用域
来源：http://sbi.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gxa.jlsjyb.cn

C#:   块级作用域
来源：http://nly.cashguo.top

[C11] 模块导入与导出
来源：http://qch.ivvv.top

Py:   from module import func
来源：http://bgs.hnqzz.top

PHP:  require "file.php";  或 use App\Service;
来源：http://paz.yuanzhike.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cea.yj20258888.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://had.cashguo.top

Java: import java.util.List;
来源：http://kog.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fdr.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://chi.dianchejie.cn

C#:   using System.Text;
来源：http://hyx.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://jpr.pycfn.com

Py:   (lambda: print("run"))()
来源：http://skb.snrcjt.cn

PHP:  (function () { echo "run"; })();
来源：http://pta.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://zek.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://mlc.vqdsnc.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://odf.yuxming.cn

Go:   func() { fmt.Println("run") }()
来源：http://hyg.vqdsnc.cn

Ruby: -> { puts "run" }.call
来源：http://mkx.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://bjm.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://skf.pengpengdd.cyou

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://abu.dianchejie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xvd.yj20258.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yxo.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uci.xuanzx.com

Java: int add(int a, int b) { return a + b; }
来源：http://aws.birdmap.top

Go:   func add(a, b int) int
来源：http://ytt.ppjwa.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dea.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://agf.ivvv.top

[C14] 泛型函数
来源：http://xex.jianghu66.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xli.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://fvk.xuanzx.com

JS:   // 无泛型
来源：http://ulq.xylfe.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yzv.hnxiangtu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vxo.9152youxi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://owk.xinyue.icu

Ruby: # 无泛型
来源：http://kfs.nwbrower.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://exx.pycfn.com

[C15] 解构 / 展开参数
来源：http://orj.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qoe.xingfuxueyuan.xyz

PHP:  [$a, $b] = $pair;
来源：http://bie.cucudq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wub.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tkx.cqqwz.cn

Java: // 无解构
来源：http://xmq.9152youxi.cn

Go:   // 无解构
来源：http://xzi.uphjek.com

Ruby: a, b = pair
来源：http://svh.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://xfl.316326.xyz

[C16] 函数 / 方法重载
来源：http://zvf.bbcook.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zon.chenjidiqi.icu

PHP:  // 无重载
来源：http://cou.birdmap.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://kfr.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://nlo.ybcxt.top

Java: void f(int a) {}  void f(String a) {}
来源：http://hkx.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://nfm.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://kza.hysaishi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dgv.nanxinkj.top

================================================================================
来源：http://chh.jqgfzy.top

D. 数组 / 列表 / 集合
来源：http://eup.0kj1m.cn

================================================================================
来源：http://ruh.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://ngw.jqgfzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rdn.xingfuxueyuan.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vxy.316326.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kaf.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://hrh.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dit.cheryme.top

Go:   arr := []int{1, 2, 3}
来源：http://gqt.hnqzz.top

Ruby: arr = [1, 2, 3]
来源：http://bse.fzhhl.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ewe.hesvh.cn

[D02] 追加元素到末尾
来源：http://xgg.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://huy.zhengqikj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jts.hammf.cn

JS:   arr.push(4);
来源：http://vcd.guannengcc.top

TS:   arr.push(4);
来源：http://fzi.nanxinkj.top

Java: list.add(4);
来源：http://ubo.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://qgo.ydzc1.top

Ruby: arr << 4; arr.push(5)
来源：http://stq.yj20258888.top

C#:   list.Add(4);
来源：http://esr.guannengcc.top

[D03] 在指定位置插入元素
来源：http://kme.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://lve.0kj1m.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dhf.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wcu.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://myd.xziqi.cn

Java: list.add(0, 0);
来源：http://mpl.chenlongwang.top

Go:   arr = append([]int{0}, arr...)
来源：http://byy.yj20258888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uce.epnwcf.com

C#:   list.Insert(0, 0);
来源：http://hzo.jinghuilouyu.cn

[D04] 删除元素
来源：http://uql.haohaochexian.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ear.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nmd.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nuo.hammf.cn

TS:   arr.splice(0, 1);
来源：http://otg.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dpw.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fod.hongshengwenyu.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mli.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cvb.yongpay.top

[D05] 访问与修改元素
来源：http://jlo.gzhubu.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nez.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pep.yj20258.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kwo.ywan-chungtsiang.top

TS:   arr[0]; arr.at(-1);
来源：http://cdt.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://knq.shzxlz.cn

Go:   arr[0]; arr[0] = 9
来源：http://gwe.dianchejie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wvs.chenjidiqi.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ept.yueranfly.top

[D06] 数组长度
来源：http://vww.hongshengwenyu.top

Py:   len(arr)
来源：http://ycp.zycfv.cn

PHP:  count($arr);
来源：http://wfn.zdqjudy.top

JS:   arr.length
来源：http://sia.ydjk.org.cn

TS:   arr.length
来源：http://uka.ywan-chungtsiang.top

Java: list.size();
来源：http://zbq.havefunace.top

Go:   len(arr)
来源：http://irv.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://dbr.cqqwz.cn

C#:   list.Count;
来源：http://qou.birdmap.top

[D07] 切片 / 取子数组
来源：http://yib.zhixingplan.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wqt.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://vaa.snrcjt.cn

JS:   arr.slice(1, 4);
来源：http://zwf.jinqigfzy.top

TS:   arr.slice(1, 4);
来源：http://tub.tarul.cn

Java: list.subList(1, 4);
来源：http://riq.daxiang520.top

Go:   arr[1:4]
来源：http://ipx.chenlongwang.top

Ruby: arr[1, 3]
来源：http://zvr.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://vsm.guannengcc.top

[D08] 合并两个数组
来源：http://mfl.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://fcz.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://wlw.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ybj.yj202588.top

TS:   [...a, ...b];
来源：http://mpl.hesvh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mcn.tianlin.xyz

Go:   append(a, b...)
来源：http://euw.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://rgl.jiagoushi.top

C#:   a.Concat(b).ToList()
来源：http://ggi.hongshengwenyu.top

[D09] 排序（升序）
来源：http://mbu.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://nxx.bjfxy.top

PHP:  sort($arr);
来源：http://kek.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jpi.chenzaomai.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://get.birdmap.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ztq.zhengqikj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cgv.9152youxi.cn

Ruby: arr.sort
来源：http://wpr.fengsongda.top

C#:   list.Sort();
来源：http://xae.yanxiufei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oal.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vcm.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wgi.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lbk.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rcz.hfpthk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://izm.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yhv.zhixingplan.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vzd.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bmj.jiagoushi.top

[D11] 反转数组
来源：http://glg.zhaomingkeji.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://vhu.ybcxt.top

PHP:  array_reverse($arr);
来源：http://abi.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pyx.jqgfzy.top

TS:   [...arr].reverse();
来源：http://nyz.cheryme.top

Java: Collections.reverse(list);
来源：http://bqw.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://sjb.bjfxy.top

Ruby: arr.reverse
来源：http://sfn.wangshuangyany.cn

C#:   list.Reverse();
来源：http://ful.zdqjudy.top

[D12] 查找元素下标
来源：http://sbd.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://aap.ydzc1.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ood.tarul.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ice.gzhubu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vam.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uxm.havefunace.top

Go:   slices.Index(arr, x)
来源：http://rod.9152youxi.cn

Ruby: arr.index(x)
来源：http://kvy.ywan-chungtsiang.top

C#:   list.IndexOf(x);
来源：http://fpq.dianchejie.cn

[D13] 过滤（保留满足条件的）
来源：http://dfl.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tut.haohaochexian.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oqh.wangdashe.top

JS:   arr.filter(x => x > 3)
来源：http://rne.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://ngz.9152youxi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yyj.xylfe.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qde.gzhubu.top

Ruby: arr.select { |x| x > 3 }
来源：http://tof.yangfankeji.com

C#:   list.Where(x => x > 3).ToList()
来源：http://vhu.iojbl.cn

[D14] 映射转换（每个元素变形）
来源：http://eym.sxryk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fbj.hesvh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://amk.sweek.top

JS:   arr.map(x => x * 2)
来源：http://ekj.tianlin.xyz

TS:   arr.map(x => x * 2)
来源：http://zna.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://aom.cashguo.top

Go:   // 手写循环
来源：http://mub.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://jwb.jqgufenzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jfq.hongshengwenyu.top

[D15] 去重
来源：http://ezd.bbcook.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vfi.epnwcf.com

PHP:  array_unique($arr);
来源：http://ktf.guannengcc.top

JS:   [...new Set(arr)]
来源：http://imf.ydzc1.top

TS:   [...new Set(arr)]
来源：http://fqa.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vgv.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://cni.hesvh.cn

Ruby: arr.uniq
来源：http://ozd.fehbvm.com

C#:   list.Distinct().ToList()
来源：http://oxd.yuxming.cn

[D16] 求和与平均值
来源：http://rgt.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pok.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://puc.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mgk.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://omo.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zsb.xuanzx.com

Go:   // 手写循环累加
来源：http://ogs.jlsjyb.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lux.sweek.top

C#:   list.Sum();  list.Average()
来源：http://fel.ivvv.top

[D17] 最大值与最小值
来源：http://wwo.meibo888.top

Py:   max(arr);  min(arr)
来源：http://skq.hesvh.cn

PHP:  max($arr);  min($arr);
来源：http://syt.hysaishi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qjp.yangfankeji.com

TS:   Math.max(...arr);
来源：http://xyt.wangdashe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xxi.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gff.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://gjd.tanke756.top

C#:   list.Max();  list.Min()
来源：http://uyj.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://hqu.jyoumei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eng.52xcode.cn

PHP:  array_merge(...$nested);
来源：http://npd.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ovz.zhiwuduotai.top

TS:   nested.flat();
来源：http://icr.xinyue.icu


<!-- 参考信息 -->