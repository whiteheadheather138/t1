代发 wailian999

Java: if (data == null) return;
来源：http://xoj.bjfxy.top

Go:   if data == nil { return }
来源：http://iqm.sjlbkw.cn

Ruby: return if data.nil?
来源：http://tau.yj202588.top

C#:   if (data == null) return;
来源：http://fdy.shuidangran.top

================================================================================
来源：http://fkk.52xcode.cn

C. 函数与作用域
来源：http://iyk.chenlongwang.top

================================================================================
来源：http://ngl.fzhhl.top

[C01] 定义函数
来源：http://yzd.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://aob.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kql.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://dcm.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zni.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://knk.jiagoushi.top

Go:   func add(a, b int) int { return a + b }
来源：http://rtb.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://nel.jqgufenzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mmv.ppjwa.cn

[C02] 默认参数
来源：http://jfd.havefunace.top

Py:   def greet(name="World"): return name
来源：http://dpb.mhx1999.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ktv.hnxiangtu.top

JS:   function greet(name = "World") { return name; }
来源：http://qfk.chenzaomai.com

TS:   function greet(name: string = "World") { return name; }
来源：http://uxp.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tzj.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qic.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://opj.yueranfly.top

C#:   string Greet(string name = "World") => name;
来源：http://nlw.cqqwz.cn

[C03] 可变参数
来源：http://eap.cqqwz.cn

Py:   def total(*args): return sum(args)
来源：http://ccy.snrcjt.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://etr.tarul.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qkk.guowangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://csq.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bgw.jyoumei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://flu.zhongyouzk.top

Ruby: def total(*nums); nums.sum; end
来源：http://qru.jinqigfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jmo.tarul.cn

[C04] 命名参数 / 关键字参数
来源：http://wfm.hcnkem.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ijv.feifeiyinyue.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xkp.jinqigufen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lhr.snrcjt.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gvs.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://thm.cheryme.top

Go:   // 无：用配置结构体参数
来源：http://mcp.feifeiyinyue.top

Ruby: f(a: 1, b: 2)
来源：http://aag.jiagoushi.top

C#:   f(a: 1, b: 2)
来源：http://rqy.zhaomingkeji.xyz

[C05] 返回多个值
来源：http://wzl.cashguo.top

Py:   return a, b
来源：http://oos.zhijiandao.cn

PHP:  return [$a, $b];
来源：http://jhe.zhijiandao.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zuf.9152youxi.cn

TS:   return { a, b };
来源：http://kkz.cucudq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jcg.xuanzx.com

Go:   return a, b
来源：http://rbs.andypj.xyz

Ruby: return a, b
来源：http://dqk.shzxlz.cn

C#:   return (a, b);              // ValueTuple
来源：http://ivy.yueranfly.top

[C06] 匿名函数 / lambda
来源：http://dzh.yuxming.cn

Py:   square = lambda x: x * x
来源：http://urm.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jti.cdnleiting.top

JS:   const square = x => x * x;
来源：http://jyt.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://slb.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://taz.nanxuanxn.top

Go:   sq := func(x int) int { return x * x }
来源：http://jlg.yj202588.top

Ruby: square = ->(x) { x * x }
来源：http://bdh.zdqjudy.top

C#:   Func<int, int> square = x => x * x;
来源：http://rvi.jinghuilouyu.cn

[C07] 把函数作为参数传入
来源：http://cul.quarkkingdee.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tls.jqgfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://ord.zhijiandao.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kzq.smart0.xyz

TS:   arr.map(String)
来源：http://qlm.chenjidiqi.icu

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rpw.zhaomingkeji.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xdr.yangfankeji.com

Ruby: arr.map(&:upcase)
来源：http://qua.xuanzx.com

C#:   arr.Select(s => s.ToUpper())
来源：http://dbh.ivvv.top

[C08] 闭包
来源：http://ser.ydzc1.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yju.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cxo.fktsv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ofy.aibaodan.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zyj.bjfxy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://pmq.yuxming.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gae.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nik.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://npm.cdnleiting.top

[C09] 递归
来源：http://khk.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://iie.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jat.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zai.cqqwz.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xrn.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://guq.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xzx.ctjpmb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zdu.ydjk.org.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://cop.316326.xyz

[C10] 变量作用域
来源：http://hwt.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://tef.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kab.dianchejie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qon.ivvv.top

TS:   同 JS
来源：http://mfi.ehwqpu.com

Java: 方法内为块级作用域
来源：http://cmi.shanyushiyangkeji.top

Go:   花括号块级作用域
来源：http://ols.hcnkem.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kgf.daria6918.cn

C#:   块级作用域
来源：http://pzr.dashuyun.cn

[C11] 模块导入与导出
来源：http://dca.hammf.cn

Py:   from module import func
来源：http://pne.cqqwz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bib.daria6918.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://wah.cheryme.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://udf.epnwcf.com

Java: import java.util.List;
来源：http://lei.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ehg.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://eqw.jinqigfzy.top

C#:   using System.Text;
来源：http://ajr.yanxiufei.cn

[C12] 立即执行函数 IIFE
来源：http://krp.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://acr.havefunace.top

PHP:  (function () { echo "run"; })();
来源：http://yip.hysaishi.cn

JS:   (() => { console.log("run"); })();
来源：http://srs.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://paf.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xfo.hnqzz.top

Go:   func() { fmt.Println("run") }()
来源：http://xhk.zdbjq.cn

Ruby: -> { puts "run" }.call
来源：http://sij.zhijiandao.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mmu.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://htc.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gny.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mhl.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://iet.shangyingyoupin.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gqh.hcnkem.com

Java: int add(int a, int b) { return a + b; }
来源：http://nmr.yuanzhike.top

Go:   func add(a, b int) int
来源：http://qas.jianghu66.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tij.cucudq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://zmd.kuanghao11.cn

[C14] 泛型函数
来源：http://tpr.cucudq.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vuf.zdqjudy.top

PHP:  // 无泛型
来源：http://lag.smart0.xyz

JS:   // 无泛型
来源：http://jce.shanyushiyangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pyq.andypj.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bkx.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nwa.zycfv.cn

Ruby: # 无泛型
来源：http://fyq.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://itc.yfazqb.com

[C15] 解构 / 展开参数
来源：http://ika.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://oxv.yonumen.top

PHP:  [$a, $b] = $pair;
来源：http://lpq.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xym.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xoj.yangfankeji.com

Java: // 无解构
来源：http://hpk.vqdsnc.cn

Go:   // 无解构
来源：http://oyj.iojbl.cn

Ruby: a, b = pair
来源：http://aig.sxryk.cn

C#:   var (a, b) = pair;
来源：http://shr.zdqjudy.top

[C16] 函数 / 方法重载
来源：http://vgp.shanyushiyangtech.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://olt.hcnkem.com

PHP:  // 无重载
来源：http://tdr.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://ofk.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://gqs.pycfn.com

Java: void f(int a) {}  void f(String a) {}
来源：http://cxe.fengsongda.top

Go:   // 无重载：用不同函数名
来源：http://ghq.ydzc1.top

Ruby: # 无重载：靠动态参数
来源：http://wju.gotoacloud.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://nni.jyoumei.cn

================================================================================
来源：http://bhr.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://pux.cheryme.top

================================================================================
来源：http://vfh.tian-w.cn

[D01] 创建数组 / 列表
来源：http://fxe.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nvq.gaohongyu789.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pjf.316326.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pkr.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ykj.ppjwa.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xvt.hcnkem.com

Go:   arr := []int{1, 2, 3}
来源：http://jxt.nanxinkj.top

Ruby: arr = [1, 2, 3]
来源：http://yfg.fehbvm.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dvq.9152youxi.cn

[D02] 追加元素到末尾
来源：http://kyq.birdmap.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://uyy.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://auv.zdqjudy.top

JS:   arr.push(4);
来源：http://vsn.ctjpmb.com

TS:   arr.push(4);
来源：http://arv.epnwcf.com

Java: list.add(4);
来源：http://ejy.svipenyu.cn

Go:   arr = append(arr, 4)
来源：http://bmp.jqgfzy.top

Ruby: arr << 4; arr.push(5)
来源：http://jtf.vehdjk.com

C#:   list.Add(4);
来源：http://ctl.xingfuxueyuan.xyz

[D03] 在指定位置插入元素
来源：http://vii.cucudq.cn

Py:   arr.insert(0, 0)
来源：http://wpx.ehwqpu.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ofq.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://djk.birdmap.top

TS:   arr.splice(0, 0, 0);
来源：http://gld.ehwqpu.com

Java: list.add(0, 0);
来源：http://efq.daxiang520.top

Go:   arr = append([]int{0}, arr...)
来源：http://tnf.shzxlz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://myb.zdbjq.cn

C#:   list.Insert(0, 0);
来源：http://sir.cqqwz.cn

[D04] 删除元素
来源：http://elr.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://eaf.guannengcc.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gbk.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ltq.cheryme.top

TS:   arr.splice(0, 1);
来源：http://klb.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lzw.hammf.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mvx.ivvv.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nnw.52xcode.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kji.guowangkeji.top

[D05] 访问与修改元素
来源：http://cym.xuetiantiany.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cnk.fzhhl.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lko.fehbvm.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rin.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://paz.andypj.xyz

Java: list.get(0); list.set(0, 9);
来源：http://yjj.cucudq.cn

Go:   arr[0]; arr[0] = 9
来源：http://tvs.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oik.jlsjyb.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://msp.yj202588.top

[D06] 数组长度
来源：http://cra.ehwqpu.com

Py:   len(arr)
来源：http://gix.haohaochexian.top

PHP:  count($arr);
来源：http://ybb.jqgufenzy.top

JS:   arr.length
来源：http://rtt.cqqwz.cn

TS:   arr.length
来源：http://gvp.vqdsnc.cn

Java: list.size();
来源：http://otj.hammf.cn

Go:   len(arr)
来源：http://zqm.jlsjyb.cn

Ruby: arr.length; arr.size
来源：http://pma.zhixingplan.top

C#:   list.Count;
来源：http://awg.zhengqikj.top

[D07] 切片 / 取子数组
来源：http://ftj.yj20258888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ooy.ybcxt.top

PHP:  array_slice($arr, 1, 3);
来源：http://sia.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://kvj.ppjwa.cn

TS:   arr.slice(1, 4);
来源：http://urw.jqgufenzy.top

Java: list.subList(1, 4);
来源：http://xfg.dianchejie.cn

Go:   arr[1:4]
来源：http://ssx.ctjpmb.com

Ruby: arr[1, 3]
来源：http://fyn.fanxiaobao.xyz

C#:   list.GetRange(1, 3);
来源：http://bfm.wangshuangyany.cn

[D08] 合并两个数组
来源：http://tur.nanxinkj.top

Py:   a + b;  a.extend(b)
来源：http://wyu.yanxiufei.cn

PHP:  array_merge($a, $b);
来源：http://spe.yanxiufei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kez.fanxiaobao.xyz

TS:   [...a, ...b];
来源：http://lcv.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rpg.yueranfly.top

Go:   append(a, b...)
来源：http://hsw.zhaomingkeji.xyz

Ruby: a + b;  a.concat(b)
来源：http://vgr.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://gap.zhengqikj.top

[D09] 排序（升序）
来源：http://vch.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://lov.yvedp.cn

PHP:  sort($arr);
来源：http://cqu.chenzaomai.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bsu.redwolf501.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wdm.cucudq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mkh.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blf.yuxming.cn

Ruby: arr.sort
来源：http://bxd.nanxinkj.top

C#:   list.Sort();
来源：http://ilb.shangyingyoupin.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uwu.yueranfly.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kjm.xziqi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oaa.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tkq.ydjk.org.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ivh.yuxming.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tqz.jinqigufen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yop.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fhw.hysaishi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yzx.jinqigfzy.top

[D11] 反转数组
来源：http://how.zycfv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jtp.yj20258888.top

PHP:  array_reverse($arr);
来源：http://yvx.zhixingplan.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rlc.bbcook.cn

TS:   [...arr].reverse();
来源：http://uyj.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://ggz.tian-w.cn

Go:   slices.Reverse(arr)
来源：http://feb.cheryme.top

Ruby: arr.reverse
来源：http://xfl.yj20258.top

C#:   list.Reverse();
来源：http://xry.chenzaomai.com

[D12] 查找元素下标
来源：http://tnw.haohaochexian.top

Py:   arr.index(x);  x in arr
来源：http://jeg.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://akw.xuanzx.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://trs.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://shn.yangfankeji.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mzl.aibaodan.cn

Go:   slices.Index(arr, x)
来源：http://arh.quarkkingdee.top

Ruby: arr.index(x)
来源：http://hsh.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://whn.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://giw.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dnt.gaohongyu789.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://snl.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://agf.jinyuanbaomall.cn

TS:   arr.filter(x => x > 3)
来源：http://mpi.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://clb.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://viy.cucudq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fow.epnwcf.com

C#:   list.Where(x => x > 3).ToList()
来源：http://yaj.ybcxt.top

[D14] 映射转换（每个元素变形）
来源：http://oik.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pwv.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bmk.kuanghao11.cn

JS:   arr.map(x => x * 2)
来源：http://ezv.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://ltf.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dld.fengsongda.top

Go:   // 手写循环
来源：http://omc.sysykeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://ryl.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sbw.0kj1m.cn

[D15] 去重
来源：http://jwh.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bym.chenlongwang.top

PHP:  array_unique($arr);
来源：http://iwj.hcnkem.com

JS:   [...new Set(arr)]
来源：http://lek.c1oappe.top

TS:   [...new Set(arr)]
来源：http://lif.shanyushiyangtech.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nqi.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://gqq.yj20258888.top

Ruby: arr.uniq
来源：http://tlb.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://nqb.cheryme.top

[D16] 求和与平均值
来源：http://snw.xinyue.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jva.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bxu.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vxa.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://alx.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xvj.cashguo.top

Go:   // 手写循环累加
来源：http://opr.ydjk.org.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://apl.hammf.cn

C#:   list.Sum();  list.Average()
来源：http://oyn.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://xux.pycfn.com

Py:   max(arr);  min(arr)
来源：http://uzg.xuetiantiany.cn


<!-- 参考信息 -->