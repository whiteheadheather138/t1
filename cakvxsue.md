代发 wailian999

[C02] 默认参数
来源：http://aww.jqgufenzy.top

Py:   def greet(name="World"): return name
来源：http://heu.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jya.tian-w.cn

JS:   function greet(name = "World") { return name; }
来源：http://ltq.zhongyouzk.top

TS:   function greet(name: string = "World") { return name; }
来源：http://agv.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qdf.yonumen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gnl.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://jfk.fktsv.cn

C#:   string Greet(string name = "World") => name;
来源：http://vcc.fehbvm.com

[C03] 可变参数
来源：http://eif.jinqigufen.top

Py:   def total(*args): return sum(args)
来源：http://kre.ydzc1.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://twe.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://shy.bjfxy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hqz.xylfe.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xcv.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gkk.cashguo.top

Ruby: def total(*nums); nums.sum; end
来源：http://fyh.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bvy.yvedp.cn

[C04] 命名参数 / 关键字参数
来源：http://tpm.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ehh.pycfn.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dsm.jqgfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xal.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ehs.bjfxy.top

Java: // 无：用 Builder 模式或 record
来源：http://pza.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://tfo.vqdsnc.cn

Ruby: f(a: 1, b: 2)
来源：http://oiu.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://tze.52xcode.cn

[C05] 返回多个值
来源：http://nqo.dashuyun.cn

Py:   return a, b
来源：http://zcz.hywenlv.cn

PHP:  return [$a, $b];
来源：http://vpw.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://fkt.yongpay.top

TS:   return { a, b };
来源：http://zao.jqgufenzy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yle.mhx1999.top

Go:   return a, b
来源：http://prd.daria6918.cn

Ruby: return a, b
来源：http://exy.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://rjf.hnqzz.top

[C06] 匿名函数 / lambda
来源：http://zjq.yuxming.cn

Py:   square = lambda x: x * x
来源：http://vyq.ivvv.top

PHP:  $square = fn($x) => $x * $x;
来源：http://nec.hesvh.cn

JS:   const square = x => x * x;
来源：http://kbr.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://qld.xuetiantiany.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hvo.jyoumei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bmy.xziqi.cn

Ruby: square = ->(x) { x * x }
来源：http://fiu.wangshuangyany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vis.epnwcf.com

[C07] 把函数作为参数传入
来源：http://hwn.hnqzz.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vbo.jyoumei.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wum.gogol.net.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kxv.jqgufenzy.top

TS:   arr.map(String)
来源：http://hka.andypj.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://piq.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://eof.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://ixr.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mwe.quarkkingdee.top

[C08] 闭包
来源：http://dxj.zdbjq.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yrj.316326.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hkd.yangfankeji.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://skj.hongshengwenyu.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bhl.yueranfly.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://eba.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dcp.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qqb.zdqjudy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://bhz.xziqi.cn

[C09] 递归
来源：http://apm.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hpa.tianlin.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ivl.shzxlz.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://swv.c1oappe.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rsg.zhaomingkeji.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zwd.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://miw.fzhhl.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yao.shuidangran.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://awo.ydjk.org.cn

[C10] 变量作用域
来源：http://udl.cheryme.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mba.tian-w.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://opw.hysaishi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wvj.gzhubu.top

TS:   同 JS
来源：http://lmn.hysaishi.cn

Java: 方法内为块级作用域
来源：http://dyv.xinyue.icu

Go:   花括号块级作用域
来源：http://arf.pycfn.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zrx.guannengcc.top

C#:   块级作用域
来源：http://hxe.ybcxt.top

[C11] 模块导入与导出
来源：http://lvq.hcnkem.com

Py:   from module import func
来源：http://pxe.hcnkem.com

PHP:  require "file.php";  或 use App\Service;
来源：http://vnl.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://cod.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ltg.dashuyun.cn

Java: import java.util.List;
来源：http://wvb.quarkkingdee.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yws.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://dyv.cashguo.top

C#:   using System.Text;
来源：http://mun.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://haa.jinyuanbaomall.cn

Py:   (lambda: print("run"))()
来源：http://bco.jqgfzy.top

PHP:  (function () { echo "run"; })();
来源：http://hwc.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://ijr.cucudq.cn

TS:   (() => { console.log("run"); })();
来源：http://bdj.havefunace.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ayr.xingfuxueyuan.xyz

Go:   func() { fmt.Println("run") }()
来源：http://dyz.ywan-chungtsiang.top

Ruby: -> { puts "run" }.call
来源：http://ovm.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://pdj.gzhubu.top

[C13] 类型声明 / 类型注解
来源：http://ccz.tanke756.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bnx.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nqe.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zti.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xfo.316326.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://cml.gzhubu.top

Go:   func add(a, b int) int
来源：http://lcv.ehwqpu.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lmp.yfazqb.com

C#:   int Add(int a, int b) => a + b;
来源：http://arq.yuxming.cn

[C14] 泛型函数
来源：http://qxp.jqgufenzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://evg.sysykeji.top

PHP:  // 无泛型
来源：http://omf.fanxiaobao.xyz

JS:   // 无泛型
来源：http://isw.pycfn.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://svt.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://arv.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qaq.sufxvd.cn

Ruby: # 无泛型
来源：http://qgq.sysykeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hhm.pengpengdd.cyou

[C15] 解构 / 展开参数
来源：http://ajl.pycfn.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ojc.zycfv.cn

PHP:  [$a, $b] = $pair;
来源：http://kjk.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zch.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://csd.yvedp.cn

Java: // 无解构
来源：http://eja.xziqi.cn

Go:   // 无解构
来源：http://qbv.gogol.net.cn

Ruby: a, b = pair
来源：http://vqo.yfazqb.com

C#:   var (a, b) = pair;
来源：http://aau.fehbvm.com

[C16] 函数 / 方法重载
来源：http://mdv.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://amx.meibo888.top

PHP:  // 无重载
来源：http://gpq.chenjidiqi.icu

JS:   // 无重载：靠 arguments.length 分支
来源：http://vjy.yanxiufei.cn

TS:   // 用联合类型或重载签名声明
来源：http://efc.yanxiufei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://els.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://kjz.snrcjt.cn

Ruby: # 无重载：靠动态参数
来源：http://pjl.snrcjt.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://myy.52xcode.cn

================================================================================
来源：http://hcn.yuanzhike.top

D. 数组 / 列表 / 集合
来源：http://dvl.haohaochexian.top

================================================================================
来源：http://ajx.fengsongda.top

[D01] 创建数组 / 列表
来源：http://nmx.ehwqpu.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://gnr.hcnkem.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fpb.cashguo.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lwk.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://unp.cheryme.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ouh.316326.xyz

Go:   arr := []int{1, 2, 3}
来源：http://iyd.hfpthk.cn

Ruby: arr = [1, 2, 3]
来源：http://aex.wangdashe.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://civ.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://lyg.xingfuxueyuan.xyz

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wcf.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wvd.zhaomingkeji.xyz

JS:   arr.push(4);
来源：http://mhh.shanyushiyangkeji.top

TS:   arr.push(4);
来源：http://yek.gotoacloud.top

Java: list.add(4);
来源：http://rrl.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://vdt.sysykeji.top

Ruby: arr << 4; arr.push(5)
来源：http://ccn.tianlin.xyz

C#:   list.Add(4);
来源：http://yzt.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://ski.tarul.cn

Py:   arr.insert(0, 0)
来源：http://xlo.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://muv.c1oappe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dba.jinghuilouyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://gto.jinqigfzy.top

Java: list.add(0, 0);
来源：http://oas.snrcjt.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ada.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fxu.daria6918.cn

C#:   list.Insert(0, 0);
来源：http://fgx.wangshuangyany.cn

[D04] 删除元素
来源：http://elr.daxiang520.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hgx.quarkkingdee.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hhk.fehbvm.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rig.feifeiyinyue.top

TS:   arr.splice(0, 1);
来源：http://jld.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vsb.fktsv.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pec.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pjn.zhijiandao.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tta.sjlbkw.cn

[D05] 访问与修改元素
来源：http://wlu.jinghuilouyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rtc.andypj.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hun.snrcjt.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uzz.zdbjq.cn

TS:   arr[0]; arr.at(-1);
来源：http://web.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://epp.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://lci.yuanzhike.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hkj.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sgp.tanke756.top

[D06] 数组长度
来源：http://qtg.xinyue.icu

Py:   len(arr)
来源：http://vzr.zdqjudy.top

PHP:  count($arr);
来源：http://thk.svipenyu.cn

JS:   arr.length
来源：http://yvh.daria6918.cn

TS:   arr.length
来源：http://yjq.tanke756.top

Java: list.size();
来源：http://lys.dianchejie.cn

Go:   len(arr)
来源：http://byp.birdmap.top

Ruby: arr.length; arr.size
来源：http://xjj.birdmap.top

C#:   list.Count;
来源：http://iuw.sweek.top

[D07] 切片 / 取子数组
来源：http://fai.xylfe.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bzw.daxiang520.top

PHP:  array_slice($arr, 1, 3);
来源：http://xke.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://hsp.aizwys.cn

TS:   arr.slice(1, 4);
来源：http://jux.pycfn.com

Java: list.subList(1, 4);
来源：http://jvs.cashguo.top

Go:   arr[1:4]
来源：http://irt.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://whq.haohaochexian.top

C#:   list.GetRange(1, 3);
来源：http://aom.sufxvd.cn

[D08] 合并两个数组
来源：http://lle.daria6918.cn

Py:   a + b;  a.extend(b)
来源：http://ykw.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://zji.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://eun.iojbl.cn

TS:   [...a, ...b];
来源：http://adh.nwbrower.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://drz.hammf.cn

Go:   append(a, b...)
来源：http://rfg.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://hqv.yj20258888.top

C#:   a.Concat(b).ToList()
来源：http://oab.ivvv.top

[D09] 排序（升序）
来源：http://twi.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://ego.0kj1m.cn

PHP:  sort($arr);
来源：http://hqu.sxryk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wfx.zycfv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mct.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yuk.shzxlz.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dzw.aizwys.cn

Ruby: arr.sort
来源：http://cqv.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://qyg.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hdo.xziqi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://usa.jinqigufen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fje.hesvh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://klq.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yxd.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://egv.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zyd.gaohongyu789.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jrb.quarkkingdee.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://inq.epnwcf.com

[D11] 反转数组
来源：http://qsv.yj20258.top

Py:   arr[::-1];  arr.reverse()
来源：http://xct.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://kre.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zlx.316326.xyz

TS:   [...arr].reverse();
来源：http://yxw.cashguo.top

Java: Collections.reverse(list);
来源：http://aey.xinyue.icu

Go:   slices.Reverse(arr)
来源：http://nig.redwolf501.top

Ruby: arr.reverse
来源：http://rim.9152youxi.cn

C#:   list.Reverse();
来源：http://lap.mhx1999.top

[D12] 查找元素下标
来源：http://wiq.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://zye.sysykeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hin.sysykeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lgh.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fhq.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qyh.ydzc1.top

Go:   slices.Index(arr, x)
来源：http://aij.sxryk.cn

Ruby: arr.index(x)
来源：http://qed.hongshengwenyu.top

C#:   list.IndexOf(x);
来源：http://pjj.feifeiyinyue.top

[D13] 过滤（保留满足条件的）
来源：http://ytc.hnqzz.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dub.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mia.daxiang520.top

JS:   arr.filter(x => x > 3)
来源：http://viy.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://rfl.vehdjk.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hio.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mez.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://flc.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xxx.chenjidiqi.icu

[D14] 映射转换（每个元素变形）
来源：http://wfo.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pdw.gogol.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tkn.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://nxl.hysaishi.cn

TS:   arr.map(x => x * 2)
来源：http://idm.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xxd.cashguo.top

Go:   // 手写循环
来源：http://zye.sysykeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://dqq.ppjwa.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bra.yuxming.cn

[D15] 去重
来源：http://rxa.vehdjk.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cah.yueranfly.top

PHP:  array_unique($arr);
来源：http://wuh.yvedp.cn

JS:   [...new Set(arr)]
来源：http://upb.guannengcc.top

TS:   [...new Set(arr)]
来源：http://rks.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lkn.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://crh.0kj1m.cn

Ruby: arr.uniq
来源：http://xmo.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://hlb.zhixingplan.top

[D16] 求和与平均值
来源：http://hgg.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fna.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mbv.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gdf.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yyk.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ndd.nanxinkj.top

Go:   // 手写循环累加
来源：http://lmj.sjlbkw.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lji.yueranfly.top

C#:   list.Sum();  list.Average()
来源：http://jzz.jinqigufen.top

[D17] 最大值与最小值
来源：http://xzh.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://sdm.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://qej.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ekb.bbcook.cn

TS:   Math.max(...arr);
来源：http://cib.xziqi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://noj.aibaodan.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uxd.316326.xyz

Ruby: arr.max;  arr.min
来源：http://tyk.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://jbb.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://ywd.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://glj.feifeiyinyue.top

PHP:  array_merge(...$nested);
来源：http://lou.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gts.aibaodan.cn

TS:   nested.flat();
来源：http://bvj.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://szo.fktsv.cn

Go:   // 手写双层循环
来源：http://ryi.sjlbkw.cn

Ruby: nested.flatten
来源：http://ccj.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ifo.birdmap.top


<!-- 参考信息 -->