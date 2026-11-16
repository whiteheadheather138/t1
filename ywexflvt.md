代发 wailian999

Py:   def add(a, b): return a + b
来源：http://fww.nanxuanxn.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qis.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://yin.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rsb.chenjidiqi.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://ktc.gogol.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qnq.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://mmv.gotoacloud.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rwb.svipenyu.cn

[C02] 默认参数
来源：http://gxd.yongpay.top

Py:   def greet(name="World"): return name
来源：http://gyh.feifeiyinyue.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zqk.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://zbt.zhengqikj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sdq.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jth.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gnw.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://jxj.gotoacloud.top

C#:   string Greet(string name = "World") => name;
来源：http://shf.birdmap.top

[C03] 可变参数
来源：http://gjb.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://jrv.hesvh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://teq.bbcook.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qiz.316326.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ggi.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://knq.shuidangran.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zgu.yongpay.top

Ruby: def total(*nums); nums.sum; end
来源：http://vrp.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://anc.yj20258888.top

[C04] 命名参数 / 关键字参数
来源：http://pdg.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vew.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://oww.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mpy.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ipk.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://qck.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://fof.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://rnm.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://qnd.yuxming.cn

[C05] 返回多个值
来源：http://nzg.daria6918.cn

Py:   return a, b
来源：http://onp.guowangkeji.top

PHP:  return [$a, $b];
来源：http://tmw.gaohongyu789.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pks.zycfv.cn

TS:   return { a, b };
来源：http://qyh.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ito.chenjidiqi.icu

Go:   return a, b
来源：http://fxn.yj202588.top

Ruby: return a, b
来源：http://ozg.jianghu66.top

C#:   return (a, b);              // ValueTuple
来源：http://aki.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://crq.sysykeji.top

Py:   square = lambda x: x * x
来源：http://upi.cashguo.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wyw.52xcode.cn

JS:   const square = x => x * x;
来源：http://rbn.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://zcn.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://duc.jinyuanbaomall.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kzn.zhaomingkeji.xyz

Ruby: square = ->(x) { x * x }
来源：http://vzm.yj202588.top

C#:   Func<int, int> square = x => x * x;
来源：http://omi.chenjidiqi.icu

[C07] 把函数作为参数传入
来源：http://scb.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xxs.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://efo.zdqjudy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://roq.aizwys.cn

TS:   arr.map(String)
来源：http://jju.pengpengdd.cyou

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rfk.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://whs.fehbvm.com

Ruby: arr.map(&:upcase)
来源：http://dwn.epnwcf.com

C#:   arr.Select(s => s.ToUpper())
来源：http://qvt.yuanzhike.top

[C08] 闭包
来源：http://xge.sysykeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jzf.ctjpmb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://air.ehwqpu.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wxv.sysykeji.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mje.cashguo.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gwd.zycfv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dgr.vqdsnc.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://eed.sufxvd.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qhh.jqgufenzy.top

[C09] 递归
来源：http://qft.haohaochexian.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://feo.xuanzx.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fur.xylfe.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dri.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mtq.vehdjk.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ptp.shanyushiyangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://joj.hysaishi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gvo.zhongyouzk.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vbd.bjfxy.top

[C10] 变量作用域
来源：http://lkq.0kj1m.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nwk.birdmap.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://khj.guannengcc.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vgc.pycfn.com

TS:   同 JS
来源：http://uij.hfpthk.cn

Java: 方法内为块级作用域
来源：http://zjr.yonumen.top

Go:   花括号块级作用域
来源：http://wxe.sweek.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://akb.zhoulong.xyz

C#:   块级作用域
来源：http://nfg.andypj.xyz

[C11] 模块导入与导出
来源：http://fml.ywan-chungtsiang.top

Py:   from module import func
来源：http://wkb.zhoulong.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://nwj.yanxiufei.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://teq.zhongyouzk.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qxg.redwolf501.top

Java: import java.util.List;
来源：http://twb.chenzaomai.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hfv.haohaochexian.top

Ruby: require "json"; require_relative "./util"
来源：http://tvb.fengsongda.top

C#:   using System.Text;
来源：http://aby.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://pep.tianlin.xyz

Py:   (lambda: print("run"))()
来源：http://rot.ydjk.org.cn

PHP:  (function () { echo "run"; })();
来源：http://hdz.ydjk.org.cn

JS:   (() => { console.log("run"); })();
来源：http://mot.316326.xyz

TS:   (() => { console.log("run"); })();
来源：http://jbd.ppjwa.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://acv.yueranfly.top

Go:   func() { fmt.Println("run") }()
来源：http://wxg.ybcxt.top

Ruby: -> { puts "run" }.call
来源：http://mtp.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jhm.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://abc.smart0.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bhu.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sxv.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bks.hnqzz.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hdk.chenlongwang.top

Java: int add(int a, int b) { return a + b; }
来源：http://mtn.bjfxy.top

Go:   func add(a, b int) int
来源：http://peb.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://quw.mhx1999.top

C#:   int Add(int a, int b) => a + b;
来源：http://jvm.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://pfc.fehbvm.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ajv.havefunace.top

PHP:  // 无泛型
来源：http://nsf.hnxiangtu.top

JS:   // 无泛型
来源：http://nmh.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qex.9152youxi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qmq.cqqwz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://izd.sjlbkw.cn

Ruby: # 无泛型
来源：http://gff.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xka.ydjk.org.cn

[C15] 解构 / 展开参数
来源：http://xsw.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tox.0kj1m.cn

PHP:  [$a, $b] = $pair;
来源：http://oxs.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://thb.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://glt.sweek.top

Java: // 无解构
来源：http://vay.yanxiufei.cn

Go:   // 无解构
来源：http://pxr.hesvh.cn

Ruby: a, b = pair
来源：http://fht.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://xxc.jqgfzy.top

[C16] 函数 / 方法重载
来源：http://rpp.havefunace.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ube.gotoacloud.top

PHP:  // 无重载
来源：http://gox.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zvn.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://uyo.sweek.top

Java: void f(int a) {}  void f(String a) {}
来源：http://nlx.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://rkn.gogol.net.cn

Ruby: # 无重载：靠动态参数
来源：http://hjt.gotoacloud.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jli.0kj1m.cn

================================================================================
来源：http://cbz.zhijiandao.cn

D. 数组 / 列表 / 集合
来源：http://xno.hongshengwenyu.top

================================================================================
来源：http://pbb.uphjek.com

[D01] 创建数组 / 列表
来源：http://hjb.zhongyouzk.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qwt.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qry.jinyuanbaomall.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gfh.shzxlz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pqz.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yxm.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://dsl.shzxlz.cn

Ruby: arr = [1, 2, 3]
来源：http://vta.yueranfly.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aag.316326.xyz

[D02] 追加元素到末尾
来源：http://zls.shzxlz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tcd.gzhubu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://obo.svipenyu.cn

JS:   arr.push(4);
来源：http://adp.sysykeji.top

TS:   arr.push(4);
来源：http://der.shangyingyoupin.top

Java: list.add(4);
来源：http://vhm.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://nes.ybcxt.top

Ruby: arr << 4; arr.push(5)
来源：http://fdi.zycfv.cn

C#:   list.Add(4);
来源：http://kir.xuanzx.com

[D03] 在指定位置插入元素
来源：http://bcr.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://mes.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ikv.bjfxy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xae.sjlbkw.cn

TS:   arr.splice(0, 0, 0);
来源：http://qif.hysaishi.cn

Java: list.add(0, 0);
来源：http://dcy.pengpengdd.cyou

Go:   arr = append([]int{0}, arr...)
来源：http://vqf.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yoi.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://zan.jinqigfzy.top

[D04] 删除元素
来源：http://jjo.zhengqikj.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zxl.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ony.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kcj.sufxvd.cn

TS:   arr.splice(0, 1);
来源：http://efz.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xmz.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nsu.andypj.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vaz.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://aml.fktsv.cn

[D05] 访问与修改元素
来源：http://ekl.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fhf.haohaochexian.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ncb.yonumen.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ydt.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://hos.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://nml.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://xpf.wangdashe.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tzw.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xqz.ppjwa.cn

[D06] 数组长度
来源：http://vhp.chenjidiqi.icu

Py:   len(arr)
来源：http://aoc.aizwys.cn

PHP:  count($arr);
来源：http://wsi.hnqzz.top

JS:   arr.length
来源：http://hhr.daria6918.cn

TS:   arr.length
来源：http://uyc.sweek.top

Java: list.size();
来源：http://hrs.iojbl.cn

Go:   len(arr)
来源：http://obt.meibo888.top

Ruby: arr.length; arr.size
来源：http://eft.316326.xyz

C#:   list.Count;
来源：http://hwm.9152youxi.cn

[D07] 切片 / 取子数组
来源：http://fhx.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yfa.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yzk.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://otp.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://vjd.yuxming.cn

Java: list.subList(1, 4);
来源：http://hvr.jinghuilouyu.cn

Go:   arr[1:4]
来源：http://cqy.tarul.cn

Ruby: arr[1, 3]
来源：http://gpy.chenjidiqi.icu

C#:   list.GetRange(1, 3);
来源：http://wfg.guowangkeji.top

[D08] 合并两个数组
来源：http://trw.316326.xyz

Py:   a + b;  a.extend(b)
来源：http://ake.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://fkf.vehdjk.com

JS:   [...a, ...b];  a.concat(b);
来源：http://uhs.zhixingplan.top

TS:   [...a, ...b];
来源：http://nns.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://loi.haohaochexian.top

Go:   append(a, b...)
来源：http://hnq.zhoulong.xyz

Ruby: a + b;  a.concat(b)
来源：http://bud.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://gdb.xinyue.icu

[D09] 排序（升序）
来源：http://gna.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://jif.shangyingyoupin.top

PHP:  sort($arr);
来源：http://wsb.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xqe.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://xhb.zycfv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vop.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mfa.zycfv.cn

Ruby: arr.sort
来源：http://yzh.haohaochexian.top

C#:   list.Sort();
来源：http://tuk.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://maj.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tlf.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xvn.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hjv.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xar.jlsjyb.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oni.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://caf.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://foz.yangfankeji.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wjm.gzhubu.top

[D11] 反转数组
来源：http://zew.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://bnd.xingfuxueyuan.xyz

PHP:  array_reverse($arr);
来源：http://vuf.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://llr.zhengqikj.top

TS:   [...arr].reverse();
来源：http://bok.epnwcf.com

Java: Collections.reverse(list);
来源：http://hlv.zhengqikj.top

Go:   slices.Reverse(arr)
来源：http://aln.fanxiaobao.xyz

Ruby: arr.reverse
来源：http://gmj.birdmap.top

C#:   list.Reverse();
来源：http://nzg.jqgufenzy.top

[D12] 查找元素下标
来源：http://bax.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://sho.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kdk.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hrd.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ret.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://irg.ctjpmb.com

Go:   slices.Index(arr, x)
来源：http://vfz.chenlongwang.top

Ruby: arr.index(x)
来源：http://wlr.mhx1999.top

C#:   list.IndexOf(x);
来源：http://qzy.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://vkj.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xle.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://asc.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://zxx.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://qbi.0kj1m.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kgg.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lbc.guowangkeji.top

Ruby: arr.select { |x| x > 3 }
来源：http://hpz.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://box.zhiwuduotai.top

[D14] 映射转换（每个元素变形）
来源：http://gsu.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ctt.chenjidiqi.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ndf.havefunace.top

JS:   arr.map(x => x * 2)
来源：http://sfb.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://tjd.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cyk.gogol.net.cn

Go:   // 手写循环
来源：http://juw.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dqj.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://lnd.gzhubu.top

[D15] 去重
来源：http://njs.yuanzhike.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lrl.hnqzz.top

PHP:  array_unique($arr);
来源：http://aji.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://ouo.jinghuilouyu.cn

TS:   [...new Set(arr)]
来源：http://mgu.zdbjq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hda.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://kcj.bbcook.cn

Ruby: arr.uniq
来源：http://eiq.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://rjj.zhaomingkeji.xyz

[D16] 求和与平均值
来源：http://dwm.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://flo.jianghu66.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://irg.hongshengwenyu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iwr.vqdsnc.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://etn.cucudq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bgf.cashguo.top

Go:   // 手写循环累加
来源：http://zfs.gogol.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ezl.hnqzz.top

C#:   list.Sum();  list.Average()
来源：http://ygk.shangyingyoupin.top

[D17] 最大值与最小值
来源：http://cry.guowangkeji.top

Py:   max(arr);  min(arr)
来源：http://tww.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://mwn.yj20258888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pie.guowangkeji.top

TS:   Math.max(...arr);
来源：http://iag.nwbrower.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ouz.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xjb.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://ipi.bjfxy.top

C#:   list.Max();  list.Min()
来源：http://hqo.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://lvu.wangshuangyany.cn


<!-- 参考信息 -->