代发 wailian999

Java: if (data == null) return;
来源：http://zbi.yuanzhike.top

Go:   if data == nil { return }
来源：http://dza.andypj.xyz

Ruby: return if data.nil?
来源：http://vdp.ybcxt.top

C#:   if (data == null) return;
来源：http://pbu.hesvh.cn

================================================================================
来源：http://ils.gaohongyu789.top

C. 函数与作用域
来源：http://dwz.daxiang520.top

================================================================================
来源：http://ccj.zycfv.cn

[C01] 定义函数
来源：http://gzh.xingfuxueyuan.xyz

Py:   def add(a, b): return a + b
来源：http://rjw.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lbd.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://cib.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hui.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mts.cheryme.top

Go:   func add(a, b int) int { return a + b }
来源：http://wfo.yj20258888.top

Ruby: def add(a, b); a + b; end
来源：http://cvv.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zta.zhaomingkeji.xyz

[C02] 默认参数
来源：http://rgu.316326.xyz

Py:   def greet(name="World"): return name
来源：http://ksh.zdbjq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lcz.havefunace.top

JS:   function greet(name = "World") { return name; }
来源：http://mrg.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tqx.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qxj.hnxiangtu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oyp.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://vup.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://wqn.9152youxi.cn

[C03] 可变参数
来源：http://icn.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://lqn.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nqf.jinqigfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bpx.cashguo.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ioo.aizwys.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vfv.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dhr.hnxiangtu.top

Ruby: def total(*nums); nums.sum; end
来源：http://bbn.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xqd.ivvv.top

[C04] 命名参数 / 关键字参数
来源：http://ifk.aizwys.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jqb.zhiwuduotai.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zkb.bjfxy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aar.zhixingplan.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hrz.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://ccd.yfazqb.com

Go:   // 无：用配置结构体参数
来源：http://pre.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://xhp.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://ops.iojbl.cn

[C05] 返回多个值
来源：http://kot.fanxiaobao.xyz

Py:   return a, b
来源：http://pcu.pycfn.com

PHP:  return [$a, $b];
来源：http://gkb.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ccb.zdbjq.cn

TS:   return { a, b };
来源：http://rkm.ivvv.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qkw.cheryme.top

Go:   return a, b
来源：http://qlc.jinyuanbaomall.cn

Ruby: return a, b
来源：http://mzb.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://uid.9152youxi.cn

[C06] 匿名函数 / lambda
来源：http://uzo.yfazqb.com

Py:   square = lambda x: x * x
来源：http://pta.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://did.chenlongwang.top

JS:   const square = x => x * x;
来源：http://cpt.sjlbkw.cn

TS:   const square = (x: number): number => x * x;
来源：http://dkw.hywenlv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mhd.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://fbp.ydzc1.top

Ruby: square = ->(x) { x * x }
来源：http://sfr.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://cgp.gzhubu.top

[C07] 把函数作为参数传入
来源：http://buz.snrcjt.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nkv.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jtw.tarul.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rqv.yj20258.top

TS:   arr.map(String)
来源：http://jhp.cashguo.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qwf.ctjpmb.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wsn.smart0.xyz

Ruby: arr.map(&:upcase)
来源：http://bmc.tianlin.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://krr.guannengcc.top

[C08] 闭包
来源：http://uqo.gzhubu.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hbz.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pzr.yj20258888.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tfc.jlsjyb.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://glp.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bzw.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ade.uphjek.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pto.nanxinkj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hma.jinyuanbaomall.cn

[C09] 递归
来源：http://itp.gaohongyu789.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lsw.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://plj.yj20258888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hwo.jyoumei.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hwv.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jkw.ivvv.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wcy.gogol.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://urt.yj20258888.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bcc.dashuyun.cn

[C10] 变量作用域
来源：http://ycv.chenzaomai.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://eje.ctjpmb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xvy.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vax.wangshuangyany.cn

TS:   同 JS
来源：http://ayz.hcnkem.com

Java: 方法内为块级作用域
来源：http://eid.zhongyouzk.top

Go:   花括号块级作用域
来源：http://bxc.jianghu66.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oxj.xuanzx.com

C#:   块级作用域
来源：http://sdg.hfpthk.cn

[C11] 模块导入与导出
来源：http://npq.hongshengwenyu.top

Py:   from module import func
来源：http://utj.xylfe.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vqo.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uqc.ehwqpu.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wtd.bjfxy.top

Java: import java.util.List;
来源：http://eqn.hywenlv.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uwo.uphjek.com

Ruby: require "json"; require_relative "./util"
来源：http://dcd.quarkkingdee.top

C#:   using System.Text;
来源：http://diq.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://epi.zdqjudy.top

Py:   (lambda: print("run"))()
来源：http://rhn.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://ktf.jiagoushi.top

JS:   (() => { console.log("run"); })();
来源：http://oir.hnqzz.top

TS:   (() => { console.log("run"); })();
来源：http://eax.daria6918.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jzf.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://xpu.vehdjk.com

Ruby: -> { puts "run" }.call
来源：http://eji.hnxiangtu.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lcc.fehbvm.com

[C13] 类型声明 / 类型注解
来源：http://pzi.sweek.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zjq.fehbvm.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cdl.shangyingyoupin.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tit.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bcl.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://pqa.jqgufenzy.top

Go:   func add(a, b int) int
来源：http://ohx.fktsv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cbb.wangshuangyany.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tcc.jqgfzy.top

[C14] 泛型函数
来源：http://tfe.sufxvd.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nos.hesvh.cn

PHP:  // 无泛型
来源：http://pxs.shanyushiyangtech.top

JS:   // 无泛型
来源：http://hoc.0kj1m.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lpl.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://yre.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dir.cucudq.cn

Ruby: # 无泛型
来源：http://yus.epnwcf.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lnd.jlsjyb.cn

[C15] 解构 / 展开参数
来源：http://the.cqqwz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zky.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://zmw.jqgfzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bsl.iojbl.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://smq.sufxvd.cn

Java: // 无解构
来源：http://yki.gotoacloud.top

Go:   // 无解构
来源：http://zsv.fzhhl.top

Ruby: a, b = pair
来源：http://spv.gzhubu.top

C#:   var (a, b) = pair;
来源：http://raf.zdbjq.cn

[C16] 函数 / 方法重载
来源：http://yxo.nanxuanxn.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cxv.tarul.cn

PHP:  // 无重载
来源：http://gej.yvedp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kze.sweek.top

TS:   // 用联合类型或重载签名声明
来源：http://vfg.chenlongwang.top

Java: void f(int a) {}  void f(String a) {}
来源：http://odz.yuxming.cn

Go:   // 无重载：用不同函数名
来源：http://uvg.shuidangran.top

Ruby: # 无重载：靠动态参数
来源：http://nix.vehdjk.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://qmp.wangshuangyany.cn

================================================================================
来源：http://uic.zycfv.cn

D. 数组 / 列表 / 集合
来源：http://qtr.ivvv.top

================================================================================
来源：http://tqt.jianghu66.top

[D01] 创建数组 / 列表
来源：http://ean.aizwys.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zbv.daria6918.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rex.cdnleiting.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qrt.daria6918.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uub.yongpay.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lfc.gogol.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://heb.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://wgn.ppjwa.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rwt.zhijiandao.cn

[D02] 追加元素到末尾
来源：http://mkz.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://soy.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mdb.cdnleiting.top

JS:   arr.push(4);
来源：http://vii.birdmap.top

TS:   arr.push(4);
来源：http://bme.sufxvd.cn

Java: list.add(4);
来源：http://uzf.bbcook.cn

Go:   arr = append(arr, 4)
来源：http://aep.snrcjt.cn

Ruby: arr << 4; arr.push(5)
来源：http://hdy.jiagoushi.top

C#:   list.Add(4);
来源：http://tfk.yuxming.cn

[D03] 在指定位置插入元素
来源：http://aai.smart0.xyz

Py:   arr.insert(0, 0)
来源：http://mka.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jfi.sweek.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ttk.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://vrz.uphjek.com

Java: list.add(0, 0);
来源：http://ipr.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://ycf.yj20258888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bmi.c1oappe.top

C#:   list.Insert(0, 0);
来源：http://nio.hnxiangtu.top

[D04] 删除元素
来源：http://kry.bbcook.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yje.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://quj.zhongyouzk.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zre.yj202588.top

TS:   arr.splice(0, 1);
来源：http://hau.sufxvd.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uex.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ifi.daxiang520.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fxe.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kxd.hcnkem.com

[D05] 访问与修改元素
来源：http://wzj.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eqj.yangfankeji.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vpm.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://brt.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://znj.fengsongda.top

Java: list.get(0); list.set(0, 9);
来源：http://pkr.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://qrs.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oln.zhongyouzk.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zou.ehwqpu.com

[D06] 数组长度
来源：http://jlr.shangyingyoupin.top

Py:   len(arr)
来源：http://rtt.ybcxt.top

PHP:  count($arr);
来源：http://dix.gzhubu.top

JS:   arr.length
来源：http://wag.ybcxt.top

TS:   arr.length
来源：http://qfh.chenjidiqi.icu

Java: list.size();
来源：http://usy.hcnkem.com

Go:   len(arr)
来源：http://uqc.zycfv.cn

Ruby: arr.length; arr.size
来源：http://tix.snrcjt.cn

C#:   list.Count;
来源：http://rti.cucudq.cn

[D07] 切片 / 取子数组
来源：http://mum.ydjk.org.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mat.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cli.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://phh.yj202588.top

TS:   arr.slice(1, 4);
来源：http://pkw.zdbjq.cn

Java: list.subList(1, 4);
来源：http://zuf.xuanzx.com

Go:   arr[1:4]
来源：http://tjd.jinghuilouyu.cn

Ruby: arr[1, 3]
来源：http://eii.zhixingplan.top

C#:   list.GetRange(1, 3);
来源：http://tai.xuanzx.com

[D08] 合并两个数组
来源：http://shc.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://chn.cqqwz.cn

PHP:  array_merge($a, $b);
来源：http://qbu.gzhubu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://znc.hnqzz.top

TS:   [...a, ...b];
来源：http://lrf.hcnkem.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cdy.pycfn.com

Go:   append(a, b...)
来源：http://vph.quarkkingdee.top

Ruby: a + b;  a.concat(b)
来源：http://oas.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://oej.ydjk.org.cn

[D09] 排序（升序）
来源：http://jqj.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://deu.cdnleiting.top

PHP:  sort($arr);
来源：http://nbu.zhengqikj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fpv.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uyo.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qml.hammf.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xtq.ctjpmb.com

Ruby: arr.sort
来源：http://bir.zdqjudy.top

C#:   list.Sort();
来源：http://eda.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dcp.chenjidiqi.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wfp.sjlbkw.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lkt.shanyushiyangtech.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://egq.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xod.jlsjyb.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ral.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iar.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fns.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xtr.nanxinkj.top

[D11] 反转数组
来源：http://iuf.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://jgy.meibo888.top

PHP:  array_reverse($arr);
来源：http://nio.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xfa.hcnkem.com

TS:   [...arr].reverse();
来源：http://qkp.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://tqm.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://vdr.snrcjt.cn

Ruby: arr.reverse
来源：http://epm.52xcode.cn

C#:   list.Reverse();
来源：http://qzs.zdqjudy.top

[D12] 查找元素下标
来源：http://bpr.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://hsc.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kex.dianchejie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://scj.yj20258.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xzn.xuanzx.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://boa.yongpay.top

Go:   slices.Index(arr, x)
来源：http://rza.cucudq.cn

Ruby: arr.index(x)
来源：http://ula.uphjek.com

C#:   list.IndexOf(x);
来源：http://tbg.ehwqpu.com

[D13] 过滤（保留满足条件的）
来源：http://rdl.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ufx.chenjidiqi.icu

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bpx.zhiwuduotai.top

JS:   arr.filter(x => x > 3)
来源：http://onz.sufxvd.cn

TS:   arr.filter(x => x > 3)
来源：http://ypv.kuanghao11.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eoq.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bgl.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://qqr.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://bwi.hywenlv.cn

[D14] 映射转换（每个元素变形）
来源：http://hab.shangyingyoupin.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vpx.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fdf.jinqigfzy.top

JS:   arr.map(x => x * 2)
来源：http://kuu.shanyushiyangtech.top

TS:   arr.map(x => x * 2)
来源：http://cuf.vehdjk.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://bfy.bjfxy.top

Go:   // 手写循环
来源：http://ycm.uphjek.com

Ruby: arr.map { |x| x * 2 }
来源：http://xwe.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dmu.zdqjudy.top

[D15] 去重
来源：http://tky.shzxlz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pfn.daxiang520.top

PHP:  array_unique($arr);
来源：http://xma.fzhhl.top

JS:   [...new Set(arr)]
来源：http://gnd.kuanghao11.cn

TS:   [...new Set(arr)]
来源：http://ytx.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://epy.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uol.jiagoushi.top

Ruby: arr.uniq
来源：http://ics.pycfn.com

C#:   list.Distinct().ToList()
来源：http://dqo.cqqwz.cn

[D16] 求和与平均值
来源：http://qty.havefunace.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mjp.ehwqpu.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yuj.kuanghao11.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lgs.aizwys.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qlq.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vot.zdqjudy.top

Go:   // 手写循环累加
来源：http://zkz.havefunace.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qlp.svipenyu.cn

C#:   list.Sum();  list.Average()
来源：http://yin.yuxming.cn

[D17] 最大值与最小值
来源：http://ogn.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://mou.zhaomingkeji.xyz


<!-- 参考信息 -->