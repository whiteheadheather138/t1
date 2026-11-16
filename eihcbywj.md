代发 wailian999

================================================================================
来源：http://tvb.chenzaomai.com

C. 函数与作用域
来源：http://gzo.hywenlv.cn

================================================================================
来源：http://lkc.sysykeji.top

[C01] 定义函数
来源：http://tvz.hywenlv.cn

Py:   def add(a, b): return a + b
来源：http://xpy.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://com.guannengcc.top

JS:   function add(a, b) { return a + b; }
来源：http://vih.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sua.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wvp.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sfd.quarkkingdee.top

Ruby: def add(a, b); a + b; end
来源：http://tuo.jianghu66.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://suw.fengsongda.top

[C02] 默认参数
来源：http://qsu.zhongyouzk.top

Py:   def greet(name="World"): return name
来源：http://pii.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dek.andypj.xyz

JS:   function greet(name = "World") { return name; }
来源：http://xxv.hcnkem.com

TS:   function greet(name: string = "World") { return name; }
来源：http://qsa.sjlbkw.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://bwk.birdmap.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ryc.jinyuanbaomall.cn

Ruby: def greet(name = "World") = name
来源：http://cym.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://nmm.yongpay.top

[C03] 可变参数
来源：http://fxi.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://bqc.fengsongda.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bif.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fid.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ais.uphjek.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://acq.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qyh.uphjek.com

Ruby: def total(*nums); nums.sum; end
来源：http://xdn.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fer.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://uti.jqgfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nbl.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rsb.52xcode.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://riq.daria6918.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://did.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://vvp.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://zlr.fengsongda.top

Ruby: f(a: 1, b: 2)
来源：http://zfl.haohaochexian.top

C#:   f(a: 1, b: 2)
来源：http://kkg.sxryk.cn

[C05] 返回多个值
来源：http://beu.kuanghao11.cn

Py:   return a, b
来源：http://uer.uphjek.com

PHP:  return [$a, $b];
来源：http://tzb.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ywy.ehwqpu.com

TS:   return { a, b };
来源：http://ndi.chenzaomai.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qgl.redwolf501.top

Go:   return a, b
来源：http://cgh.kuanghao11.cn

Ruby: return a, b
来源：http://qop.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://dib.jinqigfzy.top

[C06] 匿名函数 / lambda
来源：http://uph.nanxinkj.top

Py:   square = lambda x: x * x
来源：http://oap.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zqu.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://qbu.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://dat.fehbvm.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fnt.yfazqb.com

Go:   sq := func(x int) int { return x * x }
来源：http://cje.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://xak.uphjek.com

C#:   Func<int, int> square = x => x * x;
来源：http://umr.hnqzz.top

[C07] 把函数作为参数传入
来源：http://xhw.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ulv.yuanzhike.top

PHP:  array_map("strtoupper", $arr);
来源：http://xse.uphjek.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lzy.iojbl.cn

TS:   arr.map(String)
来源：http://tce.zhengqikj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://paa.fzhhl.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://adr.xuetiantiany.cn

Ruby: arr.map(&:upcase)
来源：http://ckx.zhaomingkeji.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://bri.ydjk.org.cn

[C08] 闭包
来源：http://awe.9152youxi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vev.yonumen.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uie.yj202588.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mgk.yonumen.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hix.pycfn.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xrn.zhoulong.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ofi.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rrk.sysykeji.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://snw.zycfv.cn

[C09] 递归
来源：http://jrz.yuxming.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eng.chenzaomai.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ayo.gotoacloud.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eoq.fzhhl.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://srk.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pro.0kj1m.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ozb.bjfxy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://iyu.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://una.chenlongwang.top

[C10] 变量作用域
来源：http://gxk.fanxiaobao.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://efi.shanyushiyangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ywd.yfazqb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://upw.pengpengdd.cyou

TS:   同 JS
来源：http://npr.xuetiantiany.cn

Java: 方法内为块级作用域
来源：http://dti.9152youxi.cn

Go:   花括号块级作用域
来源：http://jnt.wangdashe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gdi.ehwqpu.com

C#:   块级作用域
来源：http://dso.jqgfzy.top

[C11] 模块导入与导出
来源：http://gly.bjfxy.top

Py:   from module import func
来源：http://fso.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://xsk.jinyuanbaomall.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://aas.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dyl.fzhhl.top

Java: import java.util.List;
来源：http://lft.shanyushiyangtech.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://egv.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://dow.xingfuxueyuan.xyz

C#:   using System.Text;
来源：http://hjg.quarkkingdee.top

[C12] 立即执行函数 IIFE
来源：http://myn.ivvv.top

Py:   (lambda: print("run"))()
来源：http://bal.hfpthk.cn

PHP:  (function () { echo "run"; })();
来源：http://dnq.fzhhl.top

JS:   (() => { console.log("run"); })();
来源：http://vem.smart0.xyz

TS:   (() => { console.log("run"); })();
来源：http://uuo.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://pda.zhiwuduotai.top

Go:   func() { fmt.Println("run") }()
来源：http://mkg.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://isl.feifeiyinyue.top

C#:   // 无 IIFE：用静态构造函数
来源：http://txz.hongshengwenyu.top

[C13] 类型声明 / 类型注解
来源：http://oxx.birdmap.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gxv.jqgfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jca.zycfv.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yvn.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hmw.sysykeji.top

Java: int add(int a, int b) { return a + b; }
来源：http://jkl.jyoumei.cn

Go:   func add(a, b int) int
来源：http://cic.birdmap.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xqb.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://zbq.smart0.xyz

[C14] 泛型函数
来源：http://bov.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://otq.zdqjudy.top

PHP:  // 无泛型
来源：http://qiv.yonumen.top

JS:   // 无泛型
来源：http://odf.guowangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zgx.daria6918.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://irt.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://aoo.zycfv.cn

Ruby: # 无泛型
来源：http://fwv.iojbl.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dya.haohaochexian.top

[C15] 解构 / 展开参数
来源：http://rxl.zhoulong.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mdr.wangshuangyany.cn

PHP:  [$a, $b] = $pair;
来源：http://nsu.hnqzz.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ebq.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pch.gotoacloud.top

Java: // 无解构
来源：http://egn.sweek.top

Go:   // 无解构
来源：http://iuu.ppjwa.cn

Ruby: a, b = pair
来源：http://dvp.zhiwuduotai.top

C#:   var (a, b) = pair;
来源：http://und.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://vdw.yj202588.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xeg.iojbl.cn

PHP:  // 无重载
来源：http://kyk.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mdy.gogol.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://hho.9152youxi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://eru.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://per.epnwcf.com

Ruby: # 无重载：靠动态参数
来源：http://eba.gogol.net.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://lex.zhengqikj.top

================================================================================
来源：http://yfn.xylfe.cn

D. 数组 / 列表 / 集合
来源：http://lbz.gaohongyu789.top

================================================================================
来源：http://lef.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://jdm.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fwt.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ecz.yongpay.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cmg.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://mnq.hysaishi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lcj.yvedp.cn

Go:   arr := []int{1, 2, 3}
来源：http://stl.havefunace.top

Ruby: arr = [1, 2, 3]
来源：http://jol.zhaomingkeji.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://njz.iojbl.cn

[D02] 追加元素到末尾
来源：http://tai.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hel.zhongyouzk.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wpr.iojbl.cn

JS:   arr.push(4);
来源：http://aue.chenlongwang.top

TS:   arr.push(4);
来源：http://rxa.yvedp.cn

Java: list.add(4);
来源：http://cdt.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://edc.zdbjq.cn

Ruby: arr << 4; arr.push(5)
来源：http://fre.pengpengdd.cyou

C#:   list.Add(4);
来源：http://tit.havefunace.top

[D03] 在指定位置插入元素
来源：http://keb.fktsv.cn

Py:   arr.insert(0, 0)
来源：http://jrs.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nbl.52xcode.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yqy.zhongyouzk.top

TS:   arr.splice(0, 0, 0);
来源：http://nao.yonumen.top

Java: list.add(0, 0);
来源：http://ijo.guowangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://sdn.feifeiyinyue.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yny.ehwqpu.com

C#:   list.Insert(0, 0);
来源：http://bom.yj202588.top

[D04] 删除元素
来源：http://knm.jianghu66.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tfc.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tyg.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ygp.tarul.cn

TS:   arr.splice(0, 1);
来源：http://ijk.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vzb.fzhhl.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gfo.guannengcc.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fzl.chenlongwang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kmt.yj202588.top

[D05] 访问与修改元素
来源：http://tsz.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sjs.0kj1m.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fdx.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ldn.daxiang520.top

TS:   arr[0]; arr.at(-1);
来源：http://vjr.ppjwa.cn

Java: list.get(0); list.set(0, 9);
来源：http://wzc.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://tkx.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hpo.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wmj.c1oappe.top

[D06] 数组长度
来源：http://vyd.fanxiaobao.xyz

Py:   len(arr)
来源：http://saz.yanxiufei.cn

PHP:  count($arr);
来源：http://rjw.aibaodan.cn

JS:   arr.length
来源：http://jhe.ivvv.top

TS:   arr.length
来源：http://jqa.zycfv.cn

Java: list.size();
来源：http://ohj.chenlongwang.top

Go:   len(arr)
来源：http://nec.xingfuxueyuan.xyz

Ruby: arr.length; arr.size
来源：http://drh.hongshengwenyu.top

C#:   list.Count;
来源：http://nxc.tian-w.cn

[D07] 切片 / 取子数组
来源：http://xrb.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yox.kuanghao11.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lfh.shuidangran.top

JS:   arr.slice(1, 4);
来源：http://rjc.jinghuilouyu.cn

TS:   arr.slice(1, 4);
来源：http://gam.aizwys.cn

Java: list.subList(1, 4);
来源：http://dyg.ivvv.top

Go:   arr[1:4]
来源：http://czk.hfpthk.cn

Ruby: arr[1, 3]
来源：http://ncv.shanyushiyangkeji.top

C#:   list.GetRange(1, 3);
来源：http://vpm.xingfuxueyuan.xyz

[D08] 合并两个数组
来源：http://beq.sweek.top

Py:   a + b;  a.extend(b)
来源：http://qbs.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://fpz.52xcode.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hnx.cashguo.top

TS:   [...a, ...b];
来源：http://osf.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xua.0kj1m.cn

Go:   append(a, b...)
来源：http://ujt.wangdashe.top

Ruby: a + b;  a.concat(b)
来源：http://qiy.yanxiufei.cn

C#:   a.Concat(b).ToList()
来源：http://lgv.haohaochexian.top

[D09] 排序（升序）
来源：http://rnx.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://ftg.yongpay.top

PHP:  sort($arr);
来源：http://wmc.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://odo.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yoq.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://haz.epnwcf.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xby.cdnleiting.top

Ruby: arr.sort
来源：http://awc.nanxuanxn.top

C#:   list.Sort();
来源：http://lem.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hgs.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://idl.cashguo.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iul.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dfu.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zei.bbcook.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fqn.chenjidiqi.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://puv.aibaodan.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pqz.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jhb.ppjwa.cn

[D11] 反转数组
来源：http://gnr.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://ukz.shzxlz.cn

PHP:  array_reverse($arr);
来源：http://kwo.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bce.hnqzz.top

TS:   [...arr].reverse();
来源：http://qie.tianlin.xyz

Java: Collections.reverse(list);
来源：http://lxj.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://hwr.cdnleiting.top

Ruby: arr.reverse
来源：http://brt.gzhubu.top

C#:   list.Reverse();
来源：http://str.cheryme.top

[D12] 查找元素下标
来源：http://xwa.ydjk.org.cn

Py:   arr.index(x);  x in arr
来源：http://gck.jinghuilouyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hhw.gogol.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bvj.jinghuilouyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mjj.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://esl.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://ogo.ppjwa.cn

Ruby: arr.index(x)
来源：http://ghg.fanxiaobao.xyz

C#:   list.IndexOf(x);
来源：http://rgk.redwolf501.top

[D13] 过滤（保留满足条件的）
来源：http://ssq.svipenyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uhi.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qzt.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://hut.gogol.net.cn

TS:   arr.filter(x => x > 3)
来源：http://mwe.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ypx.daria6918.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://irh.tianlin.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://hln.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kdh.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://jof.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bab.ydzc1.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mtl.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://ics.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://hbo.yvedp.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://edb.andypj.xyz

Go:   // 手写循环
来源：http://krt.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ggz.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sof.jqgufenzy.top

[D15] 去重
来源：http://ubu.zdqjudy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://due.zhijiandao.cn

PHP:  array_unique($arr);
来源：http://vit.xinyue.icu

JS:   [...new Set(arr)]
来源：http://zwp.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://phn.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xwy.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rdx.uphjek.com

Ruby: arr.uniq
来源：http://ooy.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://hqq.tanke756.top

[D16] 求和与平均值
来源：http://mlq.dianchejie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tic.daxiang520.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ork.kuanghao11.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wmd.316326.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://edg.nanxinkj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://chv.yuanzhike.top

Go:   // 手写循环累加
来源：http://aqp.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jfo.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://fxi.fengsongda.top

[D17] 最大值与最小值
来源：http://vpm.yanxiufei.cn

Py:   max(arr);  min(arr)
来源：http://ybv.hammf.cn

PHP:  max($arr);  min($arr);
来源：http://szn.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nez.havefunace.top

TS:   Math.max(...arr);
来源：http://qra.52xcode.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fym.xuetiantiany.cn


<!-- 参考信息 -->