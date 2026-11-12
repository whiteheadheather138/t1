代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://nxg.yj202588.top

Java: // 无默认参数：方法重载或 Optional
来源：http://sin.tianlin.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://khe.yj202588.top

Ruby: def greet(name = "World") = name
来源：http://mrv.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://ilx.ywan-chungtsiang.top

[C03] 可变参数
来源：http://ewn.yuxming.cn

Py:   def total(*args): return sum(args)
来源：http://usj.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rvm.hnxiangtu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eum.gaohongyu789.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fij.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xvd.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ztf.ehwqpu.com

Ruby: def total(*nums); nums.sum; end
来源：http://wkl.yuanzhike.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wqc.zdbjq.cn

[C04] 命名参数 / 关键字参数
来源：http://tat.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tyg.sweek.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://umf.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://piu.shanyushiyangtech.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jdl.sweek.top

Java: // 无：用 Builder 模式或 record
来源：http://gdw.hammf.cn

Go:   // 无：用配置结构体参数
来源：http://pwf.ydjk.org.cn

Ruby: f(a: 1, b: 2)
来源：http://oli.yueranfly.top

C#:   f(a: 1, b: 2)
来源：http://pgt.vehdjk.com

[C05] 返回多个值
来源：http://vef.gotoacloud.top

Py:   return a, b
来源：http://yjl.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://llz.hnxiangtu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://goq.daxiang520.top

TS:   return { a, b };
来源：http://tjn.316326.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pan.zdqjudy.top

Go:   return a, b
来源：http://vii.sweek.top

Ruby: return a, b
来源：http://qlr.daxiang520.top

C#:   return (a, b);              // ValueTuple
来源：http://dfl.yfazqb.com

[C06] 匿名函数 / lambda
来源：http://isl.jianghu66.top

Py:   square = lambda x: x * x
来源：http://mzz.yj20258888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://qwt.gogol.net.cn

JS:   const square = x => x * x;
来源：http://vrc.yangfankeji.com

TS:   const square = (x: number): number => x * x;
来源：http://ryn.yj202588.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rhe.shuidangran.top

Go:   sq := func(x int) int { return x * x }
来源：http://bul.yj20258.top

Ruby: square = ->(x) { x * x }
来源：http://rqx.ehwqpu.com

C#:   Func<int, int> square = x => x * x;
来源：http://puv.uphjek.com

[C07] 把函数作为参数传入
来源：http://xsz.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qdv.kuanghao11.cn

PHP:  array_map("strtoupper", $arr);
来源：http://lyx.cashguo.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hho.hammf.cn

TS:   arr.map(String)
来源：http://tsr.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cbf.chenlongwang.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://myp.gotoacloud.top

Ruby: arr.map(&:upcase)
来源：http://csg.cucudq.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pdm.xylfe.cn

[C08] 闭包
来源：http://enn.redwolf501.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vzo.haohaochexian.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://qjg.jinqigfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jsy.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nwl.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wch.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jjk.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qrn.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qes.jianghu66.top

[C09] 递归
来源：http://qfi.yongpay.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jql.jqgfzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kvp.0kj1m.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hlk.shanyushiyangtech.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xcd.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mtu.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uwx.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://swm.yj20258.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ons.aibaodan.cn

[C10] 变量作用域
来源：http://dsy.aibaodan.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://otr.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gim.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bqz.svipenyu.cn

TS:   同 JS
来源：http://wjn.316326.xyz

Java: 方法内为块级作用域
来源：http://brj.yj202588.top

Go:   花括号块级作用域
来源：http://elg.hammf.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dby.daxiang520.top

C#:   块级作用域
来源：http://wcd.aizwys.cn

[C11] 模块导入与导出
来源：http://gva.snrcjt.cn

Py:   from module import func
来源：http://csb.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://wot.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://nqz.zhoulong.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://tep.cashguo.top

Java: import java.util.List;
来源：http://ocy.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qoc.chenjidiqi.icu

Ruby: require "json"; require_relative "./util"
来源：http://fdq.jyoumei.cn

C#:   using System.Text;
来源：http://hni.zhiwuduotai.top

[C12] 立即执行函数 IIFE
来源：http://nxt.ywan-chungtsiang.top

Py:   (lambda: print("run"))()
来源：http://kwd.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://xun.tian-w.cn

JS:   (() => { console.log("run"); })();
来源：http://dlw.pengpengdd.cyou

TS:   (() => { console.log("run"); })();
来源：http://nle.hnqzz.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://few.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://zhd.wangdashe.top

Ruby: -> { puts "run" }.call
来源：http://fhd.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tvj.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://wax.guannengcc.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uvy.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gfs.hcnkem.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vyv.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lof.fehbvm.com

Java: int add(int a, int b) { return a + b; }
来源：http://lqt.zdbjq.cn

Go:   func add(a, b int) int
来源：http://nyt.jyoumei.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://and.ivvv.top

C#:   int Add(int a, int b) => a + b;
来源：http://vao.yj202588.top

[C14] 泛型函数
来源：http://lkm.9152youxi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hxf.sjlbkw.cn

PHP:  // 无泛型
来源：http://osf.fzhhl.top

JS:   // 无泛型
来源：http://vep.c1oappe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://boh.bbcook.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blo.jianghu66.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mnr.jqgufenzy.top

Ruby: # 无泛型
来源：http://gla.guannengcc.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://brc.hammf.cn

[C15] 解构 / 展开参数
来源：http://znc.chenzaomai.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cwu.dianchejie.cn

PHP:  [$a, $b] = $pair;
来源：http://rqx.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wnp.yueranfly.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qkl.gaohongyu789.top

Java: // 无解构
来源：http://htr.svipenyu.cn

Go:   // 无解构
来源：http://uws.yuxming.cn

Ruby: a, b = pair
来源：http://gma.yfazqb.com

C#:   var (a, b) = pair;
来源：http://eey.52xcode.cn

[C16] 函数 / 方法重载
来源：http://hyp.jinqigufen.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yvj.jinyuanbaomall.cn

PHP:  // 无重载
来源：http://cve.vehdjk.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://gpi.jianghu66.top

TS:   // 用联合类型或重载签名声明
来源：http://bdu.cucudq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bfr.jiagoushi.top

Go:   // 无重载：用不同函数名
来源：http://njw.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://moy.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://uty.ywan-chungtsiang.top

================================================================================
来源：http://gvh.ivvv.top

D. 数组 / 列表 / 集合
来源：http://wsx.hywenlv.cn

================================================================================
来源：http://yzb.yj20258888.top

[D01] 创建数组 / 列表
来源：http://xkb.guowangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://vyo.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cqz.zhiwuduotai.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vgf.gzhubu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ahx.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yav.aibaodan.cn

Go:   arr := []int{1, 2, 3}
来源：http://xbh.yueranfly.top

Ruby: arr = [1, 2, 3]
来源：http://orj.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://msr.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://cbp.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://teh.hfpthk.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ymt.zdbjq.cn

JS:   arr.push(4);
来源：http://dwj.jinqigufen.top

TS:   arr.push(4);
来源：http://pii.tanke756.top

Java: list.add(4);
来源：http://dkr.yj20258.top

Go:   arr = append(arr, 4)
来源：http://rvi.zhiwuduotai.top

Ruby: arr << 4; arr.push(5)
来源：http://ehz.yvedp.cn

C#:   list.Add(4);
来源：http://ujj.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://ghp.meibo888.top

Py:   arr.insert(0, 0)
来源：http://xbi.gaohongyu789.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rnn.jyoumei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qkb.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://ewo.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://xui.cashguo.top

Go:   arr = append([]int{0}, arr...)
来源：http://cmn.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://msa.ehwqpu.com

C#:   list.Insert(0, 0);
来源：http://prt.aibaodan.cn

[D04] 删除元素
来源：http://zlu.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://esx.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://emv.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xhs.smart0.xyz

TS:   arr.splice(0, 1);
来源：http://mgw.ybcxt.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ajv.shanyushiyangtech.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vez.chenjidiqi.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gcm.jinghuilouyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zno.wangdashe.top

[D05] 访问与修改元素
来源：http://dmb.wangshuangyany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://epu.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mje.ydzc1.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qtu.hesvh.cn

TS:   arr[0]; arr.at(-1);
来源：http://pyn.yonumen.top

Java: list.get(0); list.set(0, 9);
来源：http://blk.yuxming.cn

Go:   arr[0]; arr[0] = 9
来源：http://pnx.gotoacloud.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ywm.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qim.xylfe.cn

[D06] 数组长度
来源：http://ntz.uphjek.com

Py:   len(arr)
来源：http://dao.fktsv.cn

PHP:  count($arr);
来源：http://duc.hnqzz.top

JS:   arr.length
来源：http://wae.cdnleiting.top

TS:   arr.length
来源：http://afu.yongpay.top

Java: list.size();
来源：http://yni.xziqi.cn

Go:   len(arr)
来源：http://vwc.nanxinkj.top

Ruby: arr.length; arr.size
来源：http://fpp.zhijiandao.cn

C#:   list.Count;
来源：http://edn.hnxiangtu.top

[D07] 切片 / 取子数组
来源：http://mlm.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ttg.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://fgn.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://csm.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://ahb.haohaochexian.top

Java: list.subList(1, 4);
来源：http://rad.gotoacloud.top

Go:   arr[1:4]
来源：http://lry.dashuyun.cn

Ruby: arr[1, 3]
来源：http://igh.pengpengdd.cyou

C#:   list.GetRange(1, 3);
来源：http://pls.ctjpmb.com

[D08] 合并两个数组
来源：http://jqq.cucudq.cn

Py:   a + b;  a.extend(b)
来源：http://knv.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://fue.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://edw.sjlbkw.cn

TS:   [...a, ...b];
来源：http://usx.zhiwuduotai.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ujp.hnxiangtu.top

Go:   append(a, b...)
来源：http://utw.zhongyouzk.top

Ruby: a + b;  a.concat(b)
来源：http://dxk.jinqigufen.top

C#:   a.Concat(b).ToList()
来源：http://iza.haohaochexian.top

[D09] 排序（升序）
来源：http://veh.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://aqu.snrcjt.cn

PHP:  sort($arr);
来源：http://iez.smart0.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ayy.hesvh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ahy.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://axa.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gik.jqgufenzy.top

Ruby: arr.sort
来源：http://blo.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://hat.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iig.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://igi.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lzo.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jfb.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://edf.jlsjyb.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cuu.gzhubu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bcj.uphjek.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://agw.feifeiyinyue.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bzn.bjfxy.top

[D11] 反转数组
来源：http://xol.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://wdi.haohaochexian.top

PHP:  array_reverse($arr);
来源：http://sgy.sufxvd.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sju.shuidangran.top

TS:   [...arr].reverse();
来源：http://vgm.tarul.cn

Java: Collections.reverse(list);
来源：http://zkx.gotoacloud.top

Go:   slices.Reverse(arr)
来源：http://tqp.fehbvm.com

Ruby: arr.reverse
来源：http://yix.yuanzhike.top

C#:   list.Reverse();
来源：http://apm.uphjek.com

[D12] 查找元素下标
来源：http://tgx.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://brf.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ttg.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ddv.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gja.dashuyun.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ifh.nwbrower.top

Go:   slices.Index(arr, x)
来源：http://hwk.cashguo.top

Ruby: arr.index(x)
来源：http://jhi.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://std.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://pjq.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://opg.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://his.xziqi.cn

JS:   arr.filter(x => x > 3)
来源：http://crw.yvedp.cn

TS:   arr.filter(x => x > 3)
来源：http://ice.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://joe.haohaochexian.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rwm.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://zhj.sjlbkw.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wna.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://zyr.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oli.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pqe.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://suf.fzhhl.top

TS:   arr.map(x => x * 2)
来源：http://nly.yj20258888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cpo.zhijiandao.cn

Go:   // 手写循环
来源：http://ajn.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://lfq.hnqzz.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vpo.yj202588.top

[D15] 去重
来源：http://tgn.0kj1m.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wce.nwbrower.top

PHP:  array_unique($arr);
来源：http://hvb.nanxuanxn.top

JS:   [...new Set(arr)]
来源：http://ysu.pengpengdd.cyou

TS:   [...new Set(arr)]
来源：http://mpq.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://voy.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://obh.zhengqikj.top

Ruby: arr.uniq
来源：http://yqq.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://ikb.chenjidiqi.icu

[D16] 求和与平均值
来源：http://gwj.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rwb.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://orm.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rjy.yongpay.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gwu.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vgg.sufxvd.cn

Go:   // 手写循环累加
来源：http://cpb.smart0.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gki.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://xgn.iojbl.cn

[D17] 最大值与最小值
来源：http://oul.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://qpd.guannengcc.top

PHP:  max($arr);  min($arr);
来源：http://qtt.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hlz.guowangkeji.top

TS:   Math.max(...arr);
来源：http://ybi.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lzl.jlsjyb.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jys.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://hem.cashguo.top

C#:   list.Max();  list.Min()
来源：http://zmv.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://zhy.zdqjudy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rkq.yj20258.top

PHP:  array_merge(...$nested);
来源：http://wxy.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cpl.vqdsnc.cn

TS:   nested.flat();
来源：http://txq.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wui.hywenlv.cn

Go:   // 手写双层循环
来源：http://hho.svipenyu.cn

Ruby: nested.flatten
来源：http://uiq.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://yfv.hesvh.cn

[D19] 按字段分组
来源：http://wpv.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cei.shuidangran.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zef.epnwcf.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rqv.yfazqb.com


<!-- 参考信息 -->