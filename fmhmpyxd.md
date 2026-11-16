代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://ixf.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://lnj.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://rgg.wangdashe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rhh.nwbrower.top

[C02] 默认参数
来源：http://vfs.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://juc.shanyushiyangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rnd.cucudq.cn

JS:   function greet(name = "World") { return name; }
来源：http://loq.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cus.bbcook.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://wli.ywan-chungtsiang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yrx.uphjek.com

Ruby: def greet(name = "World") = name
来源：http://xzm.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://eit.zhoulong.xyz

[C03] 可变参数
来源：http://bhg.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://vfo.hfpthk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pgu.xingfuxueyuan.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://knb.hcnkem.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://twc.jinyuanbaomall.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xqe.hywenlv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dqv.shanyushiyangtech.top

Ruby: def total(*nums); nums.sum; end
来源：http://khq.jqgufenzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ezu.epnwcf.com

[C04] 命名参数 / 关键字参数
来源：http://mjh.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cub.fehbvm.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vyr.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bis.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kzl.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://vlm.hcnkem.com

Go:   // 无：用配置结构体参数
来源：http://zgx.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://pzi.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://urp.jinyuanbaomall.cn

[C05] 返回多个值
来源：http://ael.jlsjyb.cn

Py:   return a, b
来源：http://rlr.wangdashe.top

PHP:  return [$a, $b];
来源：http://izo.hammf.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://glp.shzxlz.cn

TS:   return { a, b };
来源：http://oik.quarkkingdee.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xvs.aizwys.cn

Go:   return a, b
来源：http://ldj.pycfn.com

Ruby: return a, b
来源：http://nku.316326.xyz

C#:   return (a, b);              // ValueTuple
来源：http://ywl.svipenyu.cn

[C06] 匿名函数 / lambda
来源：http://cxc.zhiwuduotai.top

Py:   square = lambda x: x * x
来源：http://ayq.guowangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://syv.iojbl.cn

JS:   const square = x => x * x;
来源：http://bgs.jinqigfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://dde.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://phc.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zue.kuanghao11.cn

Ruby: square = ->(x) { x * x }
来源：http://dwc.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://upq.pycfn.com

[C07] 把函数作为参数传入
来源：http://xnp.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fxq.aibaodan.cn

PHP:  array_map("strtoupper", $arr);
来源：http://koc.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rvs.hnxiangtu.top

TS:   arr.map(String)
来源：http://vwj.zdbjq.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iuy.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fvg.daria6918.cn

Ruby: arr.map(&:upcase)
来源：http://nmd.xinyue.icu

C#:   arr.Select(s => s.ToUpper())
来源：http://rqx.cdnleiting.top

[C08] 闭包
来源：http://yaz.hnxiangtu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mly.quarkkingdee.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ctr.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hpf.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://frp.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cfu.hesvh.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lwl.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bgh.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mva.nanxuanxn.top

[C09] 递归
来源：http://svz.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xny.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rzg.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gxp.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bph.meibo888.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://boy.meibo888.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uof.jinghuilouyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qyi.xinyue.icu

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ovj.aibaodan.cn

[C10] 变量作用域
来源：http://osk.xuanzx.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ufk.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xny.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://huw.vehdjk.com

TS:   同 JS
来源：http://mha.xziqi.cn

Java: 方法内为块级作用域
来源：http://qtj.wangshuangyany.cn

Go:   花括号块级作用域
来源：http://cah.zycfv.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://beu.shuidangran.top

C#:   块级作用域
来源：http://alb.aizwys.cn

[C11] 模块导入与导出
来源：http://evx.c1oappe.top

Py:   from module import func
来源：http://dsd.hongshengwenyu.top

PHP:  require "file.php";  或 use App\Service;
来源：http://yrf.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wez.hfpthk.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qmc.tianlin.xyz

Java: import java.util.List;
来源：http://kbw.52xcode.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eag.gogol.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://mxq.jinghuilouyu.cn

C#:   using System.Text;
来源：http://zch.xingfuxueyuan.xyz

[C12] 立即执行函数 IIFE
来源：http://ymi.pycfn.com

Py:   (lambda: print("run"))()
来源：http://jsz.vehdjk.com

PHP:  (function () { echo "run"; })();
来源：http://ips.sweek.top

JS:   (() => { console.log("run"); })();
来源：http://igj.aizwys.cn

TS:   (() => { console.log("run"); })();
来源：http://tqx.chenjidiqi.icu

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ipo.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://onb.jinqigufen.top

Ruby: -> { puts "run" }.call
来源：http://afc.tarul.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ooi.dianchejie.cn

[C13] 类型声明 / 类型注解
来源：http://zkn.epnwcf.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qlm.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://unq.nanxuanxn.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wll.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bpq.ywan-chungtsiang.top

Java: int add(int a, int b) { return a + b; }
来源：http://ocm.sxryk.cn

Go:   func add(a, b int) int
来源：http://iua.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://piq.hongshengwenyu.top

C#:   int Add(int a, int b) => a + b;
来源：http://scv.aibaodan.cn

[C14] 泛型函数
来源：http://qzv.jqgfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uno.ppjwa.cn

PHP:  // 无泛型
来源：http://aoh.gaohongyu789.top

JS:   // 无泛型
来源：http://baj.fengsongda.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pwf.jyoumei.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://irj.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lnp.0kj1m.cn

Ruby: # 无泛型
来源：http://hzh.cucudq.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nil.yanxiufei.cn

[C15] 解构 / 展开参数
来源：http://qeq.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://pym.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://ikc.yongpay.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ehl.0kj1m.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bgy.jinqigufen.top

Java: // 无解构
来源：http://nno.zdqjudy.top

Go:   // 无解构
来源：http://kae.zhengqikj.top

Ruby: a, b = pair
来源：http://wrs.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://sxi.haohaochexian.top

[C16] 函数 / 方法重载
来源：http://hrd.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hgs.hywenlv.cn

PHP:  // 无重载
来源：http://gmq.kuanghao11.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bro.tianlin.xyz

TS:   // 用联合类型或重载签名声明
来源：http://oyz.yvedp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://btf.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://tap.9152youxi.cn

Ruby: # 无重载：靠动态参数
来源：http://ghw.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yqr.guowangkeji.top

================================================================================
来源：http://nug.tarul.cn

D. 数组 / 列表 / 集合
来源：http://vbp.yongpay.top

================================================================================
来源：http://tpb.zdqjudy.top

[D01] 创建数组 / 列表
来源：http://nhd.jinghuilouyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://saf.ehwqpu.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eiy.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pwc.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xpk.xziqi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://quh.cqqwz.cn

Go:   arr := []int{1, 2, 3}
来源：http://ewz.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://uwe.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gnd.sweek.top

[D02] 追加元素到末尾
来源：http://jss.hongshengwenyu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dsl.ivvv.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dur.chenjidiqi.icu

JS:   arr.push(4);
来源：http://dff.zhiwuduotai.top

TS:   arr.push(4);
来源：http://jyl.ydjk.org.cn

Java: list.add(4);
来源：http://ewz.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://wbp.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://csw.yfazqb.com

C#:   list.Add(4);
来源：http://xqa.havefunace.top

[D03] 在指定位置插入元素
来源：http://xpp.uphjek.com

Py:   arr.insert(0, 0)
来源：http://dqn.guowangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xic.hesvh.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wya.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://exk.smart0.xyz

Java: list.add(0, 0);
来源：http://pnw.ywan-chungtsiang.top

Go:   arr = append([]int{0}, arr...)
来源：http://qag.hywenlv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://why.yvedp.cn

C#:   list.Insert(0, 0);
来源：http://oxv.guowangkeji.top

[D04] 删除元素
来源：http://lcx.jianghu66.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nhf.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ugr.ywan-chungtsiang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jyz.birdmap.top

TS:   arr.splice(0, 1);
来源：http://vnl.yj202588.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nfh.ywan-chungtsiang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mqx.zhiwuduotai.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zye.jinyuanbaomall.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qga.zhengqikj.top

[D05] 访问与修改元素
来源：http://jkm.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ktv.jlsjyb.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gpk.iojbl.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://obs.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://ohh.cheryme.top

Java: list.get(0); list.set(0, 9);
来源：http://jvz.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://zcg.xuetiantiany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rjp.yangfankeji.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vrx.zycfv.cn

[D06] 数组长度
来源：http://her.zdqjudy.top

Py:   len(arr)
来源：http://bvx.jinqigufen.top

PHP:  count($arr);
来源：http://wdr.chenlongwang.top

JS:   arr.length
来源：http://ovb.hnxiangtu.top

TS:   arr.length
来源：http://rre.andypj.xyz

Java: list.size();
来源：http://dyq.xylfe.cn

Go:   len(arr)
来源：http://xqy.wangshuangyany.cn

Ruby: arr.length; arr.size
来源：http://ndq.bjfxy.top

C#:   list.Count;
来源：http://bai.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://huf.aibaodan.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qkd.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://ttp.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://ksq.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://fzn.hysaishi.cn

Java: list.subList(1, 4);
来源：http://ylu.havefunace.top

Go:   arr[1:4]
来源：http://vug.hysaishi.cn

Ruby: arr[1, 3]
来源：http://bzf.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://gbx.pycfn.com

[D08] 合并两个数组
来源：http://wgb.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://jrj.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://voa.sjlbkw.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jrv.epnwcf.com

TS:   [...a, ...b];
来源：http://umb.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qbn.epnwcf.com

Go:   append(a, b...)
来源：http://uks.ehwqpu.com

Ruby: a + b;  a.concat(b)
来源：http://vua.yangfankeji.com

C#:   a.Concat(b).ToList()
来源：http://ysb.jianghu66.top

[D09] 排序（升序）
来源：http://hmx.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://lqc.bbcook.cn

PHP:  sort($arr);
来源：http://tvo.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pnh.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://erb.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://vtj.zdbjq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gcx.zdbjq.cn

Ruby: arr.sort
来源：http://rsw.chenlongwang.top

C#:   list.Sort();
来源：http://bsi.jlsjyb.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qfv.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qjq.fktsv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://egd.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nnx.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ipw.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zvz.bbcook.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bff.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pjb.c1oappe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zqs.yanxiufei.cn

[D11] 反转数组
来源：http://xky.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://jfz.tian-w.cn

PHP:  array_reverse($arr);
来源：http://ogd.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gxx.shzxlz.cn

TS:   [...arr].reverse();
来源：http://ybk.feifeiyinyue.top

Java: Collections.reverse(list);
来源：http://zlr.yj20258.top

Go:   slices.Reverse(arr)
来源：http://xzn.meibo888.top

Ruby: arr.reverse
来源：http://jcu.smart0.xyz

C#:   list.Reverse();
来源：http://qrw.shanyushiyangtech.top

[D12] 查找元素下标
来源：http://fkq.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://osw.dianchejie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xck.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fob.zhengqikj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://liz.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://alz.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://une.jinqigufen.top

Ruby: arr.index(x)
来源：http://rzm.uphjek.com

C#:   list.IndexOf(x);
来源：http://ark.shanyushiyangtech.top

[D13] 过滤（保留满足条件的）
来源：http://mje.wangdashe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dhs.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tcn.sjlbkw.cn

JS:   arr.filter(x => x > 3)
来源：http://exa.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://hrn.yfazqb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hoh.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://abi.zdbjq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://pwj.vqdsnc.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bec.yangfankeji.com

[D14] 映射转换（每个元素变形）
来源：http://urn.hammf.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://siw.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://olt.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://lrk.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://fxu.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pmj.chenjidiqi.icu

Go:   // 手写循环
来源：http://xkw.fzhhl.top

Ruby: arr.map { |x| x * 2 }
来源：http://goc.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iwz.feifeiyinyue.top

[D15] 去重
来源：http://yto.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gvp.ivvv.top

PHP:  array_unique($arr);
来源：http://iag.yj20258.top

JS:   [...new Set(arr)]
来源：http://bou.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://nqp.cdnleiting.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ejm.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lgs.hnxiangtu.top

Ruby: arr.uniq
来源：http://amx.xziqi.cn

C#:   list.Distinct().ToList()
来源：http://kpg.guannengcc.top

[D16] 求和与平均值
来源：http://pxr.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lrh.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ufe.hcnkem.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dvu.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lcz.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gcm.jqgufenzy.top

Go:   // 手写循环累加
来源：http://npc.nanxuanxn.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://seh.tianlin.xyz

C#:   list.Sum();  list.Average()
来源：http://vlj.c1oappe.top

[D17] 最大值与最小值
来源：http://qcb.fengsongda.top

Py:   max(arr);  min(arr)
来源：http://stb.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://fbg.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://scm.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://iub.ywan-chungtsiang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://blh.jlsjyb.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fbd.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://log.ywan-chungtsiang.top

C#:   list.Max();  list.Min()
来源：http://wvp.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://rlj.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wyc.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://ozv.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gxx.52xcode.cn

TS:   nested.flat();
来源：http://vcc.fehbvm.com


<!-- 参考信息 -->