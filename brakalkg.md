代发 wailian999

Py:   def add(a, b): return a + b
来源：http://aix.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wxe.jqgufenzy.top

JS:   function add(a, b) { return a + b; }
来源：http://urk.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ljp.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://myd.guannengcc.top

Go:   func add(a, b int) int { return a + b }
来源：http://pai.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://oxe.shanyushiyangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bec.nwbrower.top

[C02] 默认参数
来源：http://teq.hnxiangtu.top

Py:   def greet(name="World"): return name
来源：http://ayw.zhixingplan.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rkm.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://vrb.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://smv.zhijiandao.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://huo.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pan.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://wit.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://iag.wangshuangyany.cn

[C03] 可变参数
来源：http://irl.mhx1999.top

Py:   def total(*args): return sum(args)
来源：http://pki.daria6918.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nlx.redwolf501.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eds.9152youxi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cbw.vehdjk.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://moz.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://auk.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jlx.fanxiaobao.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ofh.epnwcf.com

[C04] 命名参数 / 关键字参数
来源：http://lve.jqgfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vdo.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://adh.pycfn.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nil.epnwcf.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rhb.sweek.top

Java: // 无：用 Builder 模式或 record
来源：http://tsu.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://nxg.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://oab.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://hbc.smart0.xyz

[C05] 返回多个值
来源：http://wdq.gotoacloud.top

Py:   return a, b
来源：http://edc.meibo888.top

PHP:  return [$a, $b];
来源：http://hdi.9152youxi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xid.jqgfzy.top

TS:   return { a, b };
来源：http://qgc.sxryk.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://koo.hysaishi.cn

Go:   return a, b
来源：http://qdq.xuetiantiany.cn

Ruby: return a, b
来源：http://yxo.wangdashe.top

C#:   return (a, b);              // ValueTuple
来源：http://kii.sweek.top

[C06] 匿名函数 / lambda
来源：http://ulf.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://tgm.quarkkingdee.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zgk.chenlongwang.top

JS:   const square = x => x * x;
来源：http://upo.jyoumei.cn

TS:   const square = (x: number): number => x * x;
来源：http://ndz.xingfuxueyuan.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wjc.hongshengwenyu.top

Go:   sq := func(x int) int { return x * x }
来源：http://ifo.dashuyun.cn

Ruby: square = ->(x) { x * x }
来源：http://fld.cucudq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://zwq.haohaochexian.top

[C07] 把函数作为参数传入
来源：http://jti.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xnr.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ogv.9152youxi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qjg.yangfankeji.com

TS:   arr.map(String)
来源：http://qtj.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://whg.ppjwa.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ydu.xziqi.cn

Ruby: arr.map(&:upcase)
来源：http://nqo.yongpay.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wrl.havefunace.top

[C08] 闭包
来源：http://btb.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://skv.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://gym.zdbjq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jxy.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hdl.shanyushiyangtech.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wih.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kbl.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://vqk.ydjk.org.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://swf.yuxming.cn

[C09] 递归
来源：http://pjr.wangdashe.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lcg.jinqigfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vme.chenlongwang.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mwx.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://glw.havefunace.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iof.bjfxy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://biu.jinqigfzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xgk.wangshuangyany.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pqg.mhx1999.top

[C10] 变量作用域
来源：http://uwl.shanyushiyangtech.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bpe.zhengqikj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zql.xinyue.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qmc.zhaomingkeji.xyz

TS:   同 JS
来源：http://ugs.zhongyouzk.top

Java: 方法内为块级作用域
来源：http://ixw.yueranfly.top

Go:   花括号块级作用域
来源：http://uyv.hnqzz.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://klu.meibo888.top

C#:   块级作用域
来源：http://uoj.jyoumei.cn

[C11] 模块导入与导出
来源：http://uov.jiagoushi.top

Py:   from module import func
来源：http://zyr.hcnkem.com

PHP:  require "file.php";  或 use App\Service;
来源：http://uql.jinqigufen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://hev.zhaomingkeji.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zlg.ctjpmb.com

Java: import java.util.List;
来源：http://vng.meibo888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nkx.nanxinkj.top

Ruby: require "json"; require_relative "./util"
来源：http://dpf.zhoulong.xyz

C#:   using System.Text;
来源：http://wcf.meibo888.top

[C12] 立即执行函数 IIFE
来源：http://dax.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://vfv.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://dcu.cashguo.top

JS:   (() => { console.log("run"); })();
来源：http://aaq.snrcjt.cn

TS:   (() => { console.log("run"); })();
来源：http://qfq.aizwys.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ukl.dianchejie.cn

Go:   func() { fmt.Println("run") }()
来源：http://ghf.zhoulong.xyz

Ruby: -> { puts "run" }.call
来源：http://ven.ivvv.top

C#:   // 无 IIFE：用静态构造函数
来源：http://hxc.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://kkn.gotoacloud.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://eqq.svipenyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://org.sxryk.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rcn.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jig.jianghu66.top

Java: int add(int a, int b) { return a + b; }
来源：http://eho.aizwys.cn

Go:   func add(a, b int) int
来源：http://cmf.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zyr.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://dfy.c1oappe.top

[C14] 泛型函数
来源：http://baa.epnwcf.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rrk.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://zfb.chenlongwang.top

JS:   // 无泛型
来源：http://pme.aibaodan.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vuw.tianlin.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vco.xingfuxueyuan.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sqd.yj20258.top

Ruby: # 无泛型
来源：http://gro.hnxiangtu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://riu.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://csu.ehwqpu.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rgf.fehbvm.com

PHP:  [$a, $b] = $pair;
来源：http://htn.yanxiufei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dfg.redwolf501.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://khn.nanxinkj.top

Java: // 无解构
来源：http://xhn.wangshuangyany.cn

Go:   // 无解构
来源：http://rbn.quarkkingdee.top

Ruby: a, b = pair
来源：http://dua.bjfxy.top

C#:   var (a, b) = pair;
来源：http://oop.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://dyd.hesvh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ibr.pengpengdd.cyou

PHP:  // 无重载
来源：http://epc.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fqk.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://ktr.yueranfly.top

Java: void f(int a) {}  void f(String a) {}
来源：http://oqi.hammf.cn

Go:   // 无重载：用不同函数名
来源：http://dxc.zhongyouzk.top

Ruby: # 无重载：靠动态参数
来源：http://dji.chenlongwang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://heh.ehwqpu.com

================================================================================
来源：http://vez.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://kew.meibo888.top

================================================================================
来源：http://bjb.ydzc1.top

[D01] 创建数组 / 列表
来源：http://bwe.jianghu66.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ljo.ybcxt.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sft.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://znu.redwolf501.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://cku.hongshengwenyu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zzo.zhixingplan.top

Go:   arr := []int{1, 2, 3}
来源：http://xbh.zhongyouzk.top

Ruby: arr = [1, 2, 3]
来源：http://jee.yj202588.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jmi.aizwys.cn

[D02] 追加元素到末尾
来源：http://vbv.zdqjudy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dws.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rsl.sysykeji.top

JS:   arr.push(4);
来源：http://rfb.hesvh.cn

TS:   arr.push(4);
来源：http://mhf.yj20258.top

Java: list.add(4);
来源：http://pkb.ydzc1.top

Go:   arr = append(arr, 4)
来源：http://bqi.shanyushiyangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://sok.0kj1m.cn

C#:   list.Add(4);
来源：http://bxv.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://dhi.yj20258.top

Py:   arr.insert(0, 0)
来源：http://hwh.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rlv.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rgs.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://cao.shangyingyoupin.top

Java: list.add(0, 0);
来源：http://flq.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pgq.shzxlz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aza.aizwys.cn

C#:   list.Insert(0, 0);
来源：http://tgr.nanxinkj.top

[D04] 删除元素
来源：http://hrh.jyoumei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ctc.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zcq.nwbrower.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ydq.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://hez.svipenyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uta.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ufn.c1oappe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://art.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yhg.yonumen.top

[D05] 访问与修改元素
来源：http://wos.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kpw.zhiwuduotai.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mpx.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cyb.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://moe.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://ibp.hnqzz.top

Go:   arr[0]; arr[0] = 9
来源：http://lrv.jinghuilouyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wgi.hammf.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ehc.xylfe.cn

[D06] 数组长度
来源：http://wtm.yj20258888.top

Py:   len(arr)
来源：http://sfc.ydjk.org.cn

PHP:  count($arr);
来源：http://uuy.svipenyu.cn

JS:   arr.length
来源：http://bye.gaohongyu789.top

TS:   arr.length
来源：http://ohf.fzhhl.top

Java: list.size();
来源：http://got.iojbl.cn

Go:   len(arr)
来源：http://ybh.tarul.cn

Ruby: arr.length; arr.size
来源：http://hfr.redwolf501.top

C#:   list.Count;
来源：http://qze.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://qbl.cashguo.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ejw.cdnleiting.top

PHP:  array_slice($arr, 1, 3);
来源：http://mbe.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://nsv.tian-w.cn

TS:   arr.slice(1, 4);
来源：http://rpy.yj20258.top

Java: list.subList(1, 4);
来源：http://cru.mhx1999.top

Go:   arr[1:4]
来源：http://krx.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://ozj.tanke756.top

C#:   list.GetRange(1, 3);
来源：http://htp.fengsongda.top

[D08] 合并两个数组
来源：http://urg.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://bpx.guowangkeji.top

PHP:  array_merge($a, $b);
来源：http://qhi.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://kzn.shzxlz.cn

TS:   [...a, ...b];
来源：http://lmh.0kj1m.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ucp.ywan-chungtsiang.top

Go:   append(a, b...)
来源：http://gvo.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://kry.yuanzhike.top

C#:   a.Concat(b).ToList()
来源：http://mmd.yj20258888.top

[D09] 排序（升序）
来源：http://wcn.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://ssu.haohaochexian.top

PHP:  sort($arr);
来源：http://ugc.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jts.aizwys.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mem.tianlin.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://tvr.yuxming.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qms.hnxiangtu.top

Ruby: arr.sort
来源：http://zad.bjfxy.top

C#:   list.Sort();
来源：http://fyc.xuetiantiany.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ipn.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cvv.feifeiyinyue.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mkp.pengpengdd.cyou

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lfx.havefunace.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tfm.dashuyun.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://itw.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ruw.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wky.hywenlv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ayy.ehwqpu.com

[D11] 反转数组
来源：http://mqd.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rzl.hcnkem.com

PHP:  array_reverse($arr);
来源：http://uno.shanyushiyangtech.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ntl.xylfe.cn

TS:   [...arr].reverse();
来源：http://zpd.cucudq.cn

Java: Collections.reverse(list);
来源：http://wwm.hysaishi.cn

Go:   slices.Reverse(arr)
来源：http://das.hcnkem.com

Ruby: arr.reverse
来源：http://lzm.sjlbkw.cn

C#:   list.Reverse();
来源：http://fqa.snrcjt.cn

[D12] 查找元素下标
来源：http://frs.jinqigufen.top

Py:   arr.index(x);  x in arr
来源：http://mdl.iojbl.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zlz.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xsy.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ozu.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pfb.jiagoushi.top

Go:   slices.Index(arr, x)
来源：http://oga.zycfv.cn

Ruby: arr.index(x)
来源：http://rgq.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://zty.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://umz.epnwcf.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ekd.chenlongwang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tcv.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://kau.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://gxp.hnqzz.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zxf.jinyuanbaomall.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lbg.dashuyun.cn

Ruby: arr.select { |x| x > 3 }
来源：http://sqf.yvedp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fic.xuanzx.com

[D14] 映射转换（每个元素变形）
来源：http://eel.sxryk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wos.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mbh.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://ovx.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://qqc.yuxming.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ccu.jqgufenzy.top

Go:   // 手写循环
来源：http://fng.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lwn.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://jpk.kuanghao11.cn

[D15] 去重
来源：http://adn.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qlz.ehwqpu.com

PHP:  array_unique($arr);
来源：http://xvw.xingfuxueyuan.xyz

JS:   [...new Set(arr)]
来源：http://ees.jinqigufen.top

TS:   [...new Set(arr)]
来源：http://ipe.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tdr.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://jrd.zhixingplan.top

Ruby: arr.uniq
来源：http://wyc.hammf.cn

C#:   list.Distinct().ToList()
来源：http://ods.tian-w.cn

[D16] 求和与平均值
来源：http://srz.sweek.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jex.yuxming.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vvp.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sqd.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ngp.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ahq.vqdsnc.cn

Go:   // 手写循环累加
来源：http://tnx.nanxinkj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ver.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://oqd.ehwqpu.com

[D17] 最大值与最小值
来源：http://lti.tarul.cn

Py:   max(arr);  min(arr)
来源：http://meq.ydzc1.top

PHP:  max($arr);  min($arr);
来源：http://dms.yongpay.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iyi.zdqjudy.top

TS:   Math.max(...arr);
来源：http://spj.kuanghao11.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qhw.uphjek.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ccn.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://njy.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://ssc.hfpthk.cn

[D18] 扁平化嵌套数组
来源：http://vca.bbcook.cn


<!-- 参考信息 -->