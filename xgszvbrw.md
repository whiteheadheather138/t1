代发 wailian999

Py:   def add(a, b): return a + b
来源：http://ybo.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kta.yj20258.top

JS:   function add(a, b) { return a + b; }
来源：http://wdg.yuxming.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gox.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ivo.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://nnt.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://qkv.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bqr.ehwqpu.com

[C02] 默认参数
来源：http://iof.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://ehp.havefunace.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bzk.havefunace.top

JS:   function greet(name = "World") { return name; }
来源：http://mxk.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ajp.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://wuw.yj20258888.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cwb.epnwcf.com

Ruby: def greet(name = "World") = name
来源：http://qwc.nanxuanxn.top

C#:   string Greet(string name = "World") => name;
来源：http://mvs.xuanzx.com

[C03] 可变参数
来源：http://twj.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://wki.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mmf.uphjek.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://skd.meibo888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://svt.gotoacloud.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kry.wangshuangyany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://khw.yj20258888.top

Ruby: def total(*nums); nums.sum; end
来源：http://yam.bbcook.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ngf.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://ble.yj202588.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hzs.daria6918.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ois.yfazqb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qkl.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fxd.ydjk.org.cn

Java: // 无：用 Builder 模式或 record
来源：http://dil.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://rzh.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://tmp.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://fsy.pengpengdd.cyou

[C05] 返回多个值
来源：http://rdr.chenlongwang.top

Py:   return a, b
来源：http://dgs.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://zzr.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ijg.shangyingyoupin.top

TS:   return { a, b };
来源：http://imi.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bdg.svipenyu.cn

Go:   return a, b
来源：http://sad.xziqi.cn

Ruby: return a, b
来源：http://kci.hammf.cn

C#:   return (a, b);              // ValueTuple
来源：http://xks.chenjidiqi.icu

[C06] 匿名函数 / lambda
来源：http://byz.sxryk.cn

Py:   square = lambda x: x * x
来源：http://aal.fktsv.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fal.aibaodan.cn

JS:   const square = x => x * x;
来源：http://whl.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://msm.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tbk.tianlin.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://ifq.sysykeji.top

Ruby: square = ->(x) { x * x }
来源：http://gmr.vehdjk.com

C#:   Func<int, int> square = x => x * x;
来源：http://jot.xuanzx.com

[C07] 把函数作为参数传入
来源：http://qzg.fktsv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bmt.sjlbkw.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tzb.vqdsnc.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nry.cdnleiting.top

TS:   arr.map(String)
来源：http://yvz.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wbm.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xzo.tianlin.xyz

Ruby: arr.map(&:upcase)
来源：http://mii.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://xvl.hnqzz.top

[C08] 闭包
来源：http://hkf.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nbs.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gyv.xinyue.icu

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zif.zhixingplan.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dqk.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gct.jyoumei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ubc.kuanghao11.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://uzu.ywan-chungtsiang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://upc.ybcxt.top

[C09] 递归
来源：http://xie.yj20258.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kxa.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uve.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zil.daxiang520.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://orz.cqqwz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ndn.mhx1999.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://skl.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://urx.yangfankeji.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zyi.ybcxt.top

[C10] 变量作用域
来源：http://xpy.dianchejie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hvu.yuxming.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zks.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fky.havefunace.top

TS:   同 JS
来源：http://qip.gzhubu.top

Java: 方法内为块级作用域
来源：http://vgf.hcnkem.com

Go:   花括号块级作用域
来源：http://srv.sjlbkw.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ngo.pengpengdd.cyou

C#:   块级作用域
来源：http://mlc.guannengcc.top

[C11] 模块导入与导出
来源：http://yul.zhaomingkeji.xyz

Py:   from module import func
来源：http://dse.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tgn.jinghuilouyu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://gms.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vql.jiagoushi.top

Java: import java.util.List;
来源：http://gon.316326.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://skp.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://mtb.52xcode.cn

C#:   using System.Text;
来源：http://ljv.sysykeji.top

[C12] 立即执行函数 IIFE
来源：http://oak.gogol.net.cn

Py:   (lambda: print("run"))()
来源：http://aef.sysykeji.top

PHP:  (function () { echo "run"; })();
来源：http://lql.316326.xyz

JS:   (() => { console.log("run"); })();
来源：http://aft.zhaomingkeji.xyz

TS:   (() => { console.log("run"); })();
来源：http://rfw.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xip.wangshuangyany.cn

Go:   func() { fmt.Println("run") }()
来源：http://edw.sjlbkw.cn

Ruby: -> { puts "run" }.call
来源：http://sun.cdnleiting.top

C#:   // 无 IIFE：用静态构造函数
来源：http://vxp.fanxiaobao.xyz

[C13] 类型声明 / 类型注解
来源：http://jok.yanxiufei.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://quk.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rqs.cashguo.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wbk.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xri.yangfankeji.com

Java: int add(int a, int b) { return a + b; }
来源：http://twt.fktsv.cn

Go:   func add(a, b int) int
来源：http://zag.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://keb.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://hbw.feifeiyinyue.top

[C14] 泛型函数
来源：http://pzm.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qxx.tanke756.top

PHP:  // 无泛型
来源：http://ome.feifeiyinyue.top

JS:   // 无泛型
来源：http://jgh.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ffx.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ymh.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aas.zhixingplan.top

Ruby: # 无泛型
来源：http://ogv.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ipl.fanxiaobao.xyz

[C15] 解构 / 展开参数
来源：http://zdf.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tfc.jyoumei.cn

PHP:  [$a, $b] = $pair;
来源：http://upm.shuidangran.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wph.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xor.epnwcf.com

Java: // 无解构
来源：http://weo.gzhubu.top

Go:   // 无解构
来源：http://ktn.dianchejie.cn

Ruby: a, b = pair
来源：http://kjv.c1oappe.top

C#:   var (a, b) = pair;
来源：http://wta.uphjek.com

[C16] 函数 / 方法重载
来源：http://lzo.nwbrower.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ivm.ivvv.top

PHP:  // 无重载
来源：http://qfj.fktsv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sjj.sysykeji.top

TS:   // 用联合类型或重载签名声明
来源：http://vjy.chenjidiqi.icu

Java: void f(int a) {}  void f(String a) {}
来源：http://yxu.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://faq.ybcxt.top

Ruby: # 无重载：靠动态参数
来源：http://rwp.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bse.yvedp.cn

================================================================================
来源：http://kij.xinyue.icu

D. 数组 / 列表 / 集合
来源：http://rfb.hongshengwenyu.top

================================================================================
来源：http://prt.fehbvm.com

[D01] 创建数组 / 列表
来源：http://rvo.xinyue.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://lxj.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jnn.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lru.uphjek.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://kzl.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wag.iojbl.cn

Go:   arr := []int{1, 2, 3}
来源：http://geg.pengpengdd.cyou

Ruby: arr = [1, 2, 3]
来源：http://vqg.redwolf501.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bie.yfazqb.com

[D02] 追加元素到末尾
来源：http://pls.hfpthk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://boj.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rsj.zhengqikj.top

JS:   arr.push(4);
来源：http://iia.fktsv.cn

TS:   arr.push(4);
来源：http://xpo.gaohongyu789.top

Java: list.add(4);
来源：http://bnx.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://zjo.hcnkem.com

Ruby: arr << 4; arr.push(5)
来源：http://xnf.jyoumei.cn

C#:   list.Add(4);
来源：http://jqh.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://fdt.jinyuanbaomall.cn

Py:   arr.insert(0, 0)
来源：http://pkg.birdmap.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ydy.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wvh.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://bzi.yfazqb.com

Java: list.add(0, 0);
来源：http://yrb.quarkkingdee.top

Go:   arr = append([]int{0}, arr...)
来源：http://lsr.tarul.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vek.shanyushiyangtech.top

C#:   list.Insert(0, 0);
来源：http://qsu.zhongyouzk.top

[D04] 删除元素
来源：http://llt.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zeq.wangshuangyany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cao.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xvp.tanke756.top

TS:   arr.splice(0, 1);
来源：http://pav.yuxming.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dhr.gogol.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://leg.jqgufenzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wks.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aqa.hammf.cn

[D05] 访问与修改元素
来源：http://axj.cdnleiting.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://snh.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kdj.yueranfly.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ygz.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://ddf.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://ryz.cheryme.top

Go:   arr[0]; arr[0] = 9
来源：http://xgb.yangfankeji.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rcx.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zka.chenlongwang.top

[D06] 数组长度
来源：http://opa.zhiwuduotai.top

Py:   len(arr)
来源：http://egq.wangdashe.top

PHP:  count($arr);
来源：http://rwb.hcnkem.com

JS:   arr.length
来源：http://cix.jinghuilouyu.cn

TS:   arr.length
来源：http://vig.ivvv.top

Java: list.size();
来源：http://rri.chenzaomai.com

Go:   len(arr)
来源：http://zyb.yj202588.top

Ruby: arr.length; arr.size
来源：http://wuw.fktsv.cn

C#:   list.Count;
来源：http://trn.zhixingplan.top

[D07] 切片 / 取子数组
来源：http://mji.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nid.jqgfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://thu.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://hdy.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://xql.dianchejie.cn

Java: list.subList(1, 4);
来源：http://ncr.wangshuangyany.cn

Go:   arr[1:4]
来源：http://cbl.chenlongwang.top

Ruby: arr[1, 3]
来源：http://ahe.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://hap.hesvh.cn

[D08] 合并两个数组
来源：http://ejp.52xcode.cn

Py:   a + b;  a.extend(b)
来源：http://tgr.jinghuilouyu.cn

PHP:  array_merge($a, $b);
来源：http://atn.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rci.ybcxt.top

TS:   [...a, ...b];
来源：http://ola.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mvl.jqgufenzy.top

Go:   append(a, b...)
来源：http://dad.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://lvh.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://aqt.fengsongda.top

[D09] 排序（升序）
来源：http://vcr.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://ssf.0kj1m.cn

PHP:  sort($arr);
来源：http://gpp.meibo888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qff.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://evq.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gul.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hyg.fengsongda.top

Ruby: arr.sort
来源：http://ueq.aizwys.cn

C#:   list.Sort();
来源：http://nkj.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lxi.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pud.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://axk.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zcz.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ugh.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qeq.nwbrower.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tqo.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sta.cqqwz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://llt.vehdjk.com

[D11] 反转数组
来源：http://hlk.cqqwz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qhi.jlsjyb.cn

PHP:  array_reverse($arr);
来源：http://bek.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ybr.ybcxt.top

TS:   [...arr].reverse();
来源：http://psp.gogol.net.cn

Java: Collections.reverse(list);
来源：http://pis.zycfv.cn

Go:   slices.Reverse(arr)
来源：http://wqt.guowangkeji.top

Ruby: arr.reverse
来源：http://fzq.0kj1m.cn

C#:   list.Reverse();
来源：http://zts.sufxvd.cn

[D12] 查找元素下标
来源：http://oil.cheryme.top

Py:   arr.index(x);  x in arr
来源：http://fmh.vehdjk.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kuz.tian-w.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pur.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wzd.svipenyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dej.birdmap.top

Go:   slices.Index(arr, x)
来源：http://bas.fzhhl.top

Ruby: arr.index(x)
来源：http://tss.ctjpmb.com

C#:   list.IndexOf(x);
来源：http://pop.zhongyouzk.top

[D13] 过滤（保留满足条件的）
来源：http://ers.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jsw.yangfankeji.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wvu.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://ynk.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://anm.yfazqb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qns.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mhe.xziqi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fad.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rzn.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://uxm.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cix.jinghuilouyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uik.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://ega.52xcode.cn

TS:   arr.map(x => x * 2)
来源：http://gdp.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jip.bbcook.cn

Go:   // 手写循环
来源：http://rvo.jinghuilouyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://juq.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xxk.jlsjyb.cn

[D15] 去重
来源：http://ghj.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://btz.cheryme.top

PHP:  array_unique($arr);
来源：http://fye.yongpay.top

JS:   [...new Set(arr)]
来源：http://deo.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://ymp.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kef.jiagoushi.top

Go:   // 用 map[T]struct{} 手写
来源：http://zrz.ehwqpu.com

Ruby: arr.uniq
来源：http://rie.hammf.cn

C#:   list.Distinct().ToList()
来源：http://byl.feifeiyinyue.top

[D16] 求和与平均值
来源：http://vpk.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bij.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jdy.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://scs.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fge.nanxinkj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sbk.9152youxi.cn

Go:   // 手写循环累加
来源：http://kzg.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hze.fktsv.cn

C#:   list.Sum();  list.Average()
来源：http://tns.ppjwa.cn

[D17] 最大值与最小值
来源：http://iiw.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://zxo.chenjidiqi.icu

PHP:  max($arr);  min($arr);
来源：http://qeo.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qjp.svipenyu.cn

TS:   Math.max(...arr);
来源：http://ile.shzxlz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://huj.jinqigfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vxa.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://han.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://npt.jinghuilouyu.cn

[D18] 扁平化嵌套数组
来源：http://qyi.ywan-chungtsiang.top


<!-- 参考信息 -->