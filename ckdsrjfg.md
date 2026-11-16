代发 wailian999

Go:   a && b || !c
来源：http://wch.smart0.xyz

Ruby: a && b || !c
来源：http://egl.aizwys.cn

C#:   a && b || !c
来源：http://gni.andypj.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://lfc.fanxiaobao.xyz

Py:   if not data: return
来源：http://qxm.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://jmp.xuetiantiany.cn

JS:   if (!data) return;
来源：http://onh.nanxinkj.top

TS:   if (!data) return;
来源：http://ete.guowangkeji.top

Java: if (data == null) return;
来源：http://teo.chenzaomai.com

Go:   if data == nil { return }
来源：http://jay.sxryk.cn

Ruby: return if data.nil?
来源：http://wex.jqgufenzy.top

C#:   if (data == null) return;
来源：http://dpa.hesvh.cn

================================================================================
来源：http://akc.xuanzx.com

C. 函数与作用域
来源：http://ppn.hysaishi.cn

================================================================================
来源：http://oka.chenlongwang.top

[C01] 定义函数
来源：http://quk.feifeiyinyue.top

Py:   def add(a, b): return a + b
来源：http://ghu.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nrf.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://sqy.ctjpmb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gdt.ydjk.org.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mfh.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kfo.nanxuanxn.top

Ruby: def add(a, b); a + b; end
来源：http://pfy.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://njq.dianchejie.cn

[C02] 默认参数
来源：http://ezv.hywenlv.cn

Py:   def greet(name="World"): return name
来源：http://xdm.hysaishi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xfl.xylfe.cn

JS:   function greet(name = "World") { return name; }
来源：http://fru.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://wmp.hcnkem.com

Java: // 无默认参数：方法重载或 Optional
来源：http://zap.ydzc1.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jfu.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://pig.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://weh.yonumen.top

[C03] 可变参数
来源：http://wnw.sysykeji.top

Py:   def total(*args): return sum(args)
来源：http://qof.gotoacloud.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kek.yuxming.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vil.zhiwuduotai.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ges.shuidangran.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rim.daria6918.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vnv.mhx1999.top

Ruby: def total(*nums); nums.sum; end
来源：http://knm.gogol.net.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kff.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://ijm.zhengqikj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xdm.zhijiandao.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://guv.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dbu.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zuh.xuanzx.com

Java: // 无：用 Builder 模式或 record
来源：http://aci.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://kcz.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://ypw.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://hrs.yuanzhike.top

[C05] 返回多个值
来源：http://hyy.shangyingyoupin.top

Py:   return a, b
来源：http://nev.tian-w.cn

PHP:  return [$a, $b];
来源：http://vug.quarkkingdee.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gqu.havefunace.top

TS:   return { a, b };
来源：http://mve.zhaomingkeji.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nye.redwolf501.top

Go:   return a, b
来源：http://mxw.chenjidiqi.icu

Ruby: return a, b
来源：http://fgz.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://rfg.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://pvv.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://cgt.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jly.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://ywf.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://jth.gzhubu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yja.zdqjudy.top

Go:   sq := func(x int) int { return x * x }
来源：http://loo.nanxinkj.top

Ruby: square = ->(x) { x * x }
来源：http://bmf.ydjk.org.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kcc.iojbl.cn

[C07] 把函数作为参数传入
来源：http://bmj.vehdjk.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://etk.hywenlv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://kmv.0kj1m.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yos.dianchejie.cn

TS:   arr.map(String)
来源：http://cno.xuanzx.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://eec.jianghu66.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://btd.ybcxt.top

Ruby: arr.map(&:upcase)
来源：http://eja.ywan-chungtsiang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zlc.ydzc1.top

[C08] 闭包
来源：http://gtr.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zfb.jqgufenzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lpk.chenlongwang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hcm.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xev.yanxiufei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jsu.daxiang520.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ase.tianlin.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fdo.shanyushiyangtech.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jcq.jqgfzy.top

[C09] 递归
来源：http://bji.hesvh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fui.shanyushiyangtech.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wns.nanxuanxn.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kzc.pengpengdd.cyou

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vtc.ivvv.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zuu.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gcj.yvedp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oqh.ydzc1.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vkc.c1oappe.top

[C10] 变量作用域
来源：http://nij.jinqigufen.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wul.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fth.jiagoushi.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ilp.zdqjudy.top

TS:   同 JS
来源：http://yad.0kj1m.cn

Java: 方法内为块级作用域
来源：http://vvx.zhiwuduotai.top

Go:   花括号块级作用域
来源：http://lkf.tian-w.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://xya.smart0.xyz

C#:   块级作用域
来源：http://xjc.fanxiaobao.xyz

[C11] 模块导入与导出
来源：http://bhg.shanyushiyangkeji.top

Py:   from module import func
来源：http://nga.52xcode.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qum.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ldo.zhijiandao.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kbz.gaohongyu789.top

Java: import java.util.List;
来源：http://xrp.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lca.52xcode.cn

Ruby: require "json"; require_relative "./util"
来源：http://omg.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://rqs.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://rrm.yfazqb.com

Py:   (lambda: print("run"))()
来源：http://fsx.52xcode.cn

PHP:  (function () { echo "run"; })();
来源：http://ckp.cheryme.top

JS:   (() => { console.log("run"); })();
来源：http://sdk.shanyushiyangkeji.top

TS:   (() => { console.log("run"); })();
来源：http://cmk.ywan-chungtsiang.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://znm.gotoacloud.top

Go:   func() { fmt.Println("run") }()
来源：http://cgr.gogol.net.cn

Ruby: -> { puts "run" }.call
来源：http://tbo.jinyuanbaomall.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qgd.tarul.cn

[C13] 类型声明 / 类型注解
来源：http://tci.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hjq.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://stx.yfazqb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hqj.smart0.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vqk.jqgfzy.top

Java: int add(int a, int b) { return a + b; }
来源：http://gch.zdbjq.cn

Go:   func add(a, b int) int
来源：http://sbi.redwolf501.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sae.dashuyun.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tvw.shanyushiyangkeji.top

[C14] 泛型函数
来源：http://izl.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bwq.xingfuxueyuan.xyz

PHP:  // 无泛型
来源：http://ctk.zhijiandao.cn

JS:   // 无泛型
来源：http://kgc.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vbv.bjfxy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://brf.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pjq.hfpthk.cn

Ruby: # 无泛型
来源：http://zjp.ppjwa.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tse.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://bsi.nanxinkj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tmk.yongpay.top

PHP:  [$a, $b] = $pair;
来源：http://gvl.yj20258.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iok.hysaishi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wqw.yuanzhike.top

Java: // 无解构
来源：http://hta.jlsjyb.cn

Go:   // 无解构
来源：http://cwh.hnxiangtu.top

Ruby: a, b = pair
来源：http://lio.c1oappe.top

C#:   var (a, b) = pair;
来源：http://eqy.yonumen.top

[C16] 函数 / 方法重载
来源：http://cdf.ppjwa.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ayy.yj20258888.top

PHP:  // 无重载
来源：http://vlz.iojbl.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xsd.52xcode.cn

TS:   // 用联合类型或重载签名声明
来源：http://axe.aizwys.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qaz.uphjek.com

Go:   // 无重载：用不同函数名
来源：http://gmh.c1oappe.top

Ruby: # 无重载：靠动态参数
来源：http://doj.nanxinkj.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xdu.xuetiantiany.cn

================================================================================
来源：http://zfz.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://dmp.vehdjk.com

================================================================================
来源：http://afm.yueranfly.top

[D01] 创建数组 / 列表
来源：http://qud.gogol.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dlt.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nkn.jianghu66.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lvx.vqdsnc.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://hvl.zdbjq.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cpi.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://lrm.gogol.net.cn

Ruby: arr = [1, 2, 3]
来源：http://hew.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bss.zycfv.cn

[D02] 追加元素到末尾
来源：http://map.cqqwz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qtn.hesvh.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lbh.daria6918.cn

JS:   arr.push(4);
来源：http://rvv.fanxiaobao.xyz

TS:   arr.push(4);
来源：http://ynj.daria6918.cn

Java: list.add(4);
来源：http://ijd.sxryk.cn

Go:   arr = append(arr, 4)
来源：http://njg.yuxming.cn

Ruby: arr << 4; arr.push(5)
来源：http://rne.jiagoushi.top

C#:   list.Add(4);
来源：http://juc.sufxvd.cn

[D03] 在指定位置插入元素
来源：http://srb.vehdjk.com

Py:   arr.insert(0, 0)
来源：http://hlx.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xjt.yongpay.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ovm.hywenlv.cn

TS:   arr.splice(0, 0, 0);
来源：http://xtq.yvedp.cn

Java: list.add(0, 0);
来源：http://qpx.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lcq.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iij.sxryk.cn

C#:   list.Insert(0, 0);
来源：http://jib.chenlongwang.top

[D04] 删除元素
来源：http://lyy.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lwg.yj202588.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zpv.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://trh.ehwqpu.com

TS:   arr.splice(0, 1);
来源：http://evq.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iof.wangshuangyany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pqi.yj202588.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jza.jqgufenzy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ems.zdbjq.cn

[D05] 访问与修改元素
来源：http://kck.iojbl.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://luk.vqdsnc.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vmz.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wsf.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://xmg.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://pqv.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://kry.gaohongyu789.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yvg.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://igi.ydjk.org.cn

[D06] 数组长度
来源：http://gfr.zhongyouzk.top

Py:   len(arr)
来源：http://cvi.mhx1999.top

PHP:  count($arr);
来源：http://tak.sufxvd.cn

JS:   arr.length
来源：http://nyi.zhongyouzk.top

TS:   arr.length
来源：http://qlj.zhoulong.xyz

Java: list.size();
来源：http://kia.316326.xyz

Go:   len(arr)
来源：http://hro.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://ddz.yj20258888.top

C#:   list.Count;
来源：http://qus.aizwys.cn

[D07] 切片 / 取子数组
来源：http://ssa.gzhubu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qzg.ybcxt.top

PHP:  array_slice($arr, 1, 3);
来源：http://jft.yfazqb.com

JS:   arr.slice(1, 4);
来源：http://znz.chenzaomai.com

TS:   arr.slice(1, 4);
来源：http://mpi.hywenlv.cn

Java: list.subList(1, 4);
来源：http://pbr.hnqzz.top

Go:   arr[1:4]
来源：http://lbj.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://vku.xingfuxueyuan.xyz

C#:   list.GetRange(1, 3);
来源：http://mog.aibaodan.cn

[D08] 合并两个数组
来源：http://ohk.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://van.ctjpmb.com

PHP:  array_merge($a, $b);
来源：http://uee.shzxlz.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://erw.yj20258.top

TS:   [...a, ...b];
来源：http://ehn.andypj.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://caw.xylfe.cn

Go:   append(a, b...)
来源：http://udc.guannengcc.top

Ruby: a + b;  a.concat(b)
来源：http://rfs.pengpengdd.cyou

C#:   a.Concat(b).ToList()
来源：http://deo.xuanzx.com

[D09] 排序（升序）
来源：http://wqa.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://wyb.sufxvd.cn

PHP:  sort($arr);
来源：http://kje.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nfh.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yom.smart0.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://rcb.jyoumei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sik.cqqwz.cn

Ruby: arr.sort
来源：http://wcw.tanke756.top

C#:   list.Sort();
来源：http://qve.jinyuanbaomall.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://obs.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cit.shzxlz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ore.ydzc1.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hjx.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qmi.guowangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://egu.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qxv.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qdt.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qen.zhengqikj.top

[D11] 反转数组
来源：http://tdx.xuanzx.com

Py:   arr[::-1];  arr.reverse()
来源：http://sqg.hongshengwenyu.top

PHP:  array_reverse($arr);
来源：http://otu.0kj1m.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eco.bjfxy.top

TS:   [...arr].reverse();
来源：http://rul.bbcook.cn

Java: Collections.reverse(list);
来源：http://bpp.meibo888.top

Go:   slices.Reverse(arr)
来源：http://zig.yonumen.top

Ruby: arr.reverse
来源：http://llh.ppjwa.cn

C#:   list.Reverse();
来源：http://tgn.yangfankeji.com

[D12] 查找元素下标
来源：http://qlb.xylfe.cn

Py:   arr.index(x);  x in arr
来源：http://grg.vehdjk.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xot.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gll.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mcj.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tdi.zhoulong.xyz

Go:   slices.Index(arr, x)
来源：http://phq.hongshengwenyu.top

Ruby: arr.index(x)
来源：http://myo.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://bhf.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://qlc.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ckb.sweek.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rdc.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://ogv.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://xek.fengsongda.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://izg.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ysn.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://jhc.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qex.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://oaa.cheryme.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xsq.aizwys.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vcx.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://euy.yonumen.top

TS:   arr.map(x => x * 2)
来源：http://roa.tanke756.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zxm.zhixingplan.top

Go:   // 手写循环
来源：http://zzt.dashuyun.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xhb.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://toq.jqgufenzy.top

[D15] 去重
来源：http://nnb.fanxiaobao.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xuj.zhixingplan.top

PHP:  array_unique($arr);
来源：http://xho.yanxiufei.cn

JS:   [...new Set(arr)]
来源：http://mwm.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://jbg.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://acp.0kj1m.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rhp.guannengcc.top

Ruby: arr.uniq
来源：http://qgl.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://rsz.ydzc1.top

[D16] 求和与平均值
来源：http://wob.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://brr.meibo888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fyt.ctjpmb.com


<!-- 参考信息 -->